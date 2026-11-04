# Physics Session 2 — Alternating Current: Signals, Reactance, Resonance, and Power

**Track:** NUST NET + FAST/NUCES  
**Level:** Class 12 foundation → entry-test conceptual reasoning  
**Session type:** Deep concept lesson, worked examples, and 36-question NET-style performance test  
**Suggested duration:** 120–150 minutes  
**Prerequisite:** Ohm’s law, basic trigonometry, electromagnetic induction, and the meaning of frequency

---

## Session outcomes

By the end of this session, you should be able to:

- Read a sinusoidal AC signal and connect its peak value, frequency, period, angular frequency, and phase.
- Explain why RMS values are used and convert between peak and RMS values for a sine wave.
- Predict the phase relationship between voltage and current in a resistor, inductor, and capacitor.
- Calculate inductive reactance, capacitive reactance, impedance, phase angle, and resonant frequency.
- Identify whether a series RLC circuit is inductive, capacitive, or at resonance.
- Calculate average AC power and explain the power factor.
- Apply ideal transformer ratios and reason about power transmission.
- Recognize common NET-style traps before choosing an answer.

## The big picture: what “alternating” means

In a direct-current circuit, current has one direction. In an alternating-current circuit, the current repeatedly changes direction. A generator or AC source makes the terminal voltage rise, fall, reverse, and repeat. The charge carriers in a wire therefore move back and forth; they do not travel all the way from the power station to the appliance during each cycle.

For an ideal sinusoidal source, voltage can be written as

$$
v(t)=V_0\sin(\omega t+\theta_v)
$$

and current as

$$
i(t)=I_0\sin(\omega t+\theta_i).
$$

Here, $V_0$ and $I_0$ are peak values, $t$ is time, $\omega$ is angular frequency, and $\theta_v$ and $\theta_i$ set the starting phase. The phase difference is

$$
\phi=\theta_v-\theta_i.
$$

The sign of $\phi$ tells which signal reaches a corresponding point in its cycle first. Saying “current lags voltage by $30^\circ$” means the current waveform is shifted later by $30^\circ$.

### Frequency, period, and angular frequency

One cycle takes a time $T$, called the period. Frequency $f$ is the number of cycles each second:

$$
f=\frac{1}{T},
\qquad
\omega=2\pi f=\frac{2\pi}{T}.
$$

Frequency is measured in hertz (Hz), period in seconds (s), and angular frequency in radians per second (rad/s). A full cycle is $2\pi$ radians or $360^\circ$.

**Useful recognition:** If a question gives the time for one cycle, use $f=1/T$. If it gives cycles per second, use $\omega=2\pi f$. Do not confuse $f$ with $\omega$; they differ by the factor $2\pi$.

### What happens over one complete cycle?

The signed average of a pure sine-wave current over one full cycle is zero: the positive half-cycle and negative half-cycle cancel. But the wire and appliance can still heat up. Heating depends on current squared, and $i^2(t)$ is positive during both halves of the cycle.

That is why “average current is zero” does **not** mean “AC transfers no energy.” The relevant heating measure is the RMS current.

---

## 1. Peak values and RMS values

A peak value is the maximum magnitude reached by a waveform. RMS means **root mean square**: square the instantaneous values, average over a cycle, and take the square root. For a sinusoid,

$$
V_{\mathrm{rms}}=\frac{V_0}{\sqrt{2}},
\qquad
I_{\mathrm{rms}}=\frac{I_0}{\sqrt{2}}.
$$

Equivalently,

$$
V_0=\sqrt{2}\,V_{\mathrm{rms}},
\qquad
I_0=\sqrt{2}\,I_{\mathrm{rms}}.
$$

The RMS value is the steady DC value that would produce the same average heating in a resistor. For example, a sinusoidal current with $I_{\mathrm{rms}}=2\,\text{A}$ heats a resistor at the same average rate as a steady $2\,\text{A}$ current.

For a resistor,

$$
P_{\mathrm{avg}}=I_{\mathrm{rms}}^2R
=\frac{V_{\mathrm{rms}}^2}{R}.
$$

**Important:** The factor $1/\sqrt{2}$ applies to a sinusoidal waveform. Do not apply it to every possible repeating signal without checking its shape.

---

## 2. Phase: who reaches the peak first?

Voltage and current do not always rise and fall together. Their phase relation depends on the circuit element. Imagine comparing the two waveforms at the same instant and asking which one is ahead in its cycle.

### Pure resistor: voltage and current are in phase

For a resistor, Ohm’s law applies at every instant:

$$
v(t)=Ri(t).
$$

Voltage and current reach zero and peak together, so $\phi=0^\circ$. If the supply voltage is sinusoidal, the resistor current is sinusoidal with the same frequency and phase.

### Pure inductor: current lags voltage

An inductor opposes a change in current. Its voltage is related to how quickly current changes:

$$
v_L=L\frac{di}{dt}.
$$

When the current is changing most rapidly, the inductor voltage is large. When the current is at a maximum or minimum, its rate of change is momentarily zero and the ideal inductor voltage is zero. This produces the rule:

> **In an ideal inductor, current lags voltage by $90^\circ$.**

Another safe wording is: **inductor voltage leads its current by $90^\circ$.** These two statements describe the same relationship. Be careful not to reverse them.

An inductor stores energy in its magnetic field and can return that energy to the circuit. An ideal inductor does not consume average power over a complete cycle.

### Pure capacitor: current leads voltage

A capacitor current depends on how quickly its voltage changes:

$$
i_C=C\frac{dv}{dt}.
$$

When the voltage is changing most rapidly, current is largest. When capacitor voltage is at a maximum or minimum, its rate of change is momentarily zero and the current is zero. Thus:

> **In an ideal capacitor, current leads voltage by $90^\circ$.**

Equivalently, capacitor voltage lags its current by $90^\circ$. A capacitor stores energy in its electric field and can return it to the circuit; an ideal capacitor consumes no average power over a complete cycle.

### A phase memory aid

- **R:** current and voltage are together.
- **L:** current lags.
- **C:** current comes first (leads).

These are phase relationships for ideal components. Real coils and capacitors can also have resistance and other losses.

---

## 3. Reactance: AC opposition from L and C

Resistance opposes current in both DC and AC. Inductors and capacitors also oppose AC, but their opposition depends on frequency. This frequency-dependent opposition is called **reactance** and is measured in ohms ($\Omega$).

### Inductive reactance

For an ideal inductor,

$$
X_L=\omega L=2\pi fL.
$$

- Increasing $L$ increases $X_L$.
- Increasing $f$ increases $X_L$.
- At zero frequency (steady DC after the switching transient), ideal inductive reactance is zero.

Physical meaning: a rapidly changing current requires a larger induced voltage, so a high-frequency current is harder to change through an inductor.

### Capacitive reactance

For an ideal capacitor,

$$
X_C=\frac{1}{\omega C}=\frac{1}{2\pi fC}.
$$

- Increasing $C$ decreases $X_C$.
- Increasing $f$ decreases $X_C$.
- At very low frequency, a capacitor strongly opposes current.
- At high frequency, it offers less reactance.

Physical meaning: at high frequency the capacitor has less time in each half-cycle to build up charge and voltage, so alternating current passes more readily.

**NET comparison trap:** Raising the frequency raises $X_L$ but lowers $X_C$. They change in opposite directions.

---

## 4. Series RLC circuit: combine voltages as phasors

In a series circuit, the same current flows through the resistor, inductor, and capacitor. Their voltage drops do not all peak together, so ordinary arithmetic addition of their peak or RMS magnitudes is generally wrong.

Take current as the phase reference:

- $V_R=IR$ is in phase with current.
- $V_L=IX_L$ is $90^\circ$ ahead of current.
- $V_C=IX_C$ is $90^\circ$ behind current.

The inductor and capacitor voltage directions oppose each other in the phase diagram. Therefore, the net reactive voltage has magnitude $I|X_L-X_C|$. The supply voltage is the perpendicular vector combination of the resistive and net reactive parts:

$$
V=I\sqrt{R^2+(X_L-X_C)^2}.
$$

The **impedance** $Z$ is the total opposition relating RMS supply voltage to RMS current:

$$
Z=\sqrt{R^2+(X_L-X_C)^2},
\qquad
I_{\mathrm{rms}}=\frac{V_{\mathrm{rms}}}{Z}.
$$

Impedance is measured in ohms. It is not found by simply adding $R+X_L+X_C$.

### Phase angle of a series RLC circuit

With $\phi$ defined as the supply-voltage phase minus the current phase,

$$
\tan\phi=\frac{X_L-X_C}{R},
\qquad
\cos\phi=\frac{R}{Z}.
$$

- If $X_L>X_C$, the circuit is net **inductive**: current lags supply voltage.
- If $X_C>X_L$, it is net **capacitive**: current leads supply voltage.
- If $X_L=X_C$, the circuit is at **resonance**: current and supply voltage are in phase.

For a pure inductor or pure capacitor, the phase difference is $90^\circ$ in magnitude. For a series RLC circuit with nonzero $R$, the magnitude of the phase angle is less than $90^\circ$.

---

## 5. Resonance: the inductor and capacitor balance

In a series RLC circuit, resonance occurs when the inductive and capacitive reactances are equal:

$$
X_L=X_C.
$$

Using $X_L=\omega L$ and $X_C=1/(\omega C)$ gives the resonant angular frequency and frequency:

$$
\omega_0=\frac{1}{\sqrt{LC}},
\qquad
f_0=\frac{1}{2\pi\sqrt{LC}}.
$$

At resonance:

- Net reactance is zero: $X_L-X_C=0$.
- Impedance is smallest: $Z=R$.
- Current is largest for a fixed supply voltage: $I_{\mathrm{rms}}=V_{\mathrm{rms}}/R$.
- Supply voltage and current are in phase: $\phi=0^\circ$.
- Power factor is one.

If frequency is **below** resonance, $X_C>X_L$: the circuit is net capacitive. If frequency is **above** resonance, $X_L>X_C$: it is net inductive.

The supply voltage can be much smaller than either individual inductor or capacitor voltage near resonance. Their phasors point in opposite directions and nearly cancel. This does not violate energy conservation; it is a phase cancellation, not a disappearance of voltage across each element.

With resistance present, the resonant current is finite: $I=V/R$. An idealized circuit with exactly zero resistance would predict unbounded current at resonance, but real circuits always have losses.

---

## 6. AC power and power factor

Instantaneous power is the product of instantaneous voltage and current:

$$
p(t)=v(t)i(t).
$$

For sinusoidal voltage and current, the average power over a full cycle is

$$
P_{\mathrm{avg}}=V_{\mathrm{rms}}I_{\mathrm{rms}}\cos\phi.
$$

The factor $\cos\phi$ is the **power factor**. It tells what fraction of the apparent volt-ampere product becomes average real power in the load.

For a series RLC circuit,

$$
\cos\phi=\frac{R}{Z},
\qquad
P_{\mathrm{avg}}=I_{\mathrm{rms}}^2R.
$$

Only the resistance consumes average power in an ideal series RLC model. The inductor and capacitor exchange stored energy with the source; averaged over a whole cycle, their net energy consumption is zero.

Special cases:

- Pure resistor: $\phi=0^\circ$, so $\cos\phi=1$ and $P=V_{\mathrm{rms}}I_{\mathrm{rms}}$.
- Pure inductor or capacitor: $|\phi|=90^\circ$, so $\cos\phi=0$ and ideal average power is zero.
- Mixed RLC load: $0<\cos\phi<1$ in general.

A low power factor means more current is needed to deliver a given real power at a fixed supply voltage. In power systems, that extra current raises resistive line losses, since heating loss is proportional to $I^2R$.

---

## 7. Transformers: changing AC voltage

A transformer uses changing magnetic flux from the primary coil to induce an alternating voltage in the secondary coil. For an ideal transformer,

$$
\frac{V_s}{V_p}=\frac{N_s}{N_p},
\qquad
\frac{I_s}{I_p}=\frac{N_p}{N_s},
\qquad
V_pI_p=V_sI_s.
$$

Here $N_p,N_s$ are the primary and secondary turns; $V_p,V_s$ and $I_p,I_s$ are RMS voltages and currents.

- **Step-up:** $N_s>N_p$, so secondary voltage rises and secondary current falls.
- **Step-down:** $N_s<N_p$, so secondary voltage falls and secondary current rises.
- In an ideal transformer, input and output power are equal. Real transformers lose some power as heat, sound, and magnetic losses.

A transformer needs changing magnetic flux. A steady DC supply gives only a brief change when switched on, then no continuous induced secondary voltage. Applying DC to a real transformer can also cause a dangerously large primary current because the winding resistance is small and there is no continuing inductive opposition from changing flux.

### Why high voltage helps transmit power

For a fixed transmitted power, raising the voltage lowers the current because $P\approx VI$ when the power factor is near one. The line’s resistive heating loss is $P_{\mathrm{loss}}=I^2R$. If current is reduced by a factor of 10, the same line resistance dissipates one-hundredth the heat. Power stations therefore step voltage up for transmission and step it down near consumers.

---

## 8. Worked examples

### Example 1 — Convert peak current to RMS current

A sinusoidal current has peak value $I_0=8.0\,\text{A}$. Its RMS value is

$$
I_{\mathrm{rms}}=\frac{I_0}{\sqrt{2}}
=\frac{8.0}{\sqrt{2}}
\approx5.66\,\text{A}.
$$

Use RMS current when calculating average heating in a resistor.

### Example 2 — Reactances at 50 Hz

A $0.10\,\text{H}$ inductor and a $100\,\mu\text{F}$ capacitor are each connected to a $50\,\text{Hz}$ source. Since $100\,\mu\text{F}=1.00\times10^{-4}\,\text{F}$,

$$
X_L=2\pi fL=2\pi(50)(0.10)=10\pi\approx31.4\,\Omega,
$$

$$
X_C=\frac{1}{2\pi fC}
=\frac{1}{2\pi(50)(1.00\times10^{-4})}
\approx31.8\,\Omega.
$$

At this frequency their reactances are nearly equal, so together in series they are close to resonance.

### Example 3 — Impedance and current in a series RLC circuit

Let $R=30\,\Omega$, $X_L=50\,\Omega$, and $X_C=10\,\Omega$. Then

$$
Z=\sqrt{30^2+(50-10)^2}
=\sqrt{2500}
=50\,\Omega.
$$

With $V_{\mathrm{rms}}=100\,\text{V}$,

$$
I_{\mathrm{rms}}=\frac{100}{50}=2.0\,\text{A}.
$$

Since $X_L>X_C$, it is net inductive and current lags. Also $\cos\phi=R/Z=30/50=0.60$.

### Example 4 — Average power

A load has $V_{\mathrm{rms}}=120\,\text{V}$, $I_{\mathrm{rms}}=5.0\,\text{A}$, and power factor $0.80$. Its average real power is

$$
P_{\mathrm{avg}}=V_{\mathrm{rms}}I_{\mathrm{rms}}\cos\phi
=(120)(5.0)(0.80)=480\,\text{W}.
$$

The apparent product is $600\,\text{VA}$; the real power is $480\,\text{W}$.

### Example 5 — Resonant frequency

A series circuit contains $L=0.20\,\text{H}$ and $C=50\,\mu\text{F}=5.0\times10^{-5}\,\text{F}$. Then

$$
f_0=\frac{1}{2\pi\sqrt{LC}}
=\frac{1}{2\pi\sqrt{(0.20)(5.0\times10^{-5})}}
\approx159\,\text{Hz}.
$$

At that frequency, $X_L=X_C$ and the ideal series circuit’s impedance is just $R$.

### Example 6 — Transformer ratios

An ideal transformer has $N_p=1000$ turns and $N_s=100$ turns. If $V_p=220\,\text{V}$,

$$
V_s=V_p\frac{N_s}{N_p}
=220\left(\frac{100}{1000}\right)=22\,\text{V}.
$$

It is step-down. For ideal power balance, the secondary current is 10 times the primary current.

---

## 9. NET recognition checklist and common traps

Before calculating, classify the question:

- **Peak or RMS?** For a sine wave, divide peak by $\sqrt{2}$ to get RMS.
- **Frequency or angular frequency?** Convert with $\omega=2\pi f$.
- **Phase?** R: together; L: current lags; C: current leads.
- **Frequency change?** $X_L$ rises with $f$; $X_C$ falls with $f$.
- **Series RLC?** Find $X_L-X_C$, then use $Z=\sqrt{R^2+(X_L-X_C)^2}$.
- **Circuit type?** $X_L>X_C$ is inductive; $X_C>X_L$ is capacitive.
- **Resonance?** Set $X_L=X_C$; then $Z=R$ and current is maximum.
- **Power?** Use RMS values and include $\cos\phi$ unless the circuit is purely resistive.
- **Transformer?** Voltage ratio follows turns ratio; current ratio is inverse.
- **DC and transformer?** A transformer requires changing flux for sustained output.

Common mistakes to catch:

1. Treating peak voltage as RMS voltage, or vice versa.
2. Saying an inductor’s current leads its voltage. It is the current that **lags**.
3. Saying a capacitor’s current lags its voltage. Capacitor current **leads**.
4. Adding $R$, $X_L$, and $X_C$ directly instead of using the right-angle impedance relation.
5. Forgetting the subtraction $X_L-X_C$ in a series circuit.
6. Claiming resonance makes the current zero. In a series RLC circuit, resonance makes impedance minimum and current maximum.
7. Treating zero average power in an ideal L or C as zero current. Current can flow while energy is exchanged back and forth.
8. Using $V_{\mathrm{rms}}I_{\mathrm{rms}}$ as real power when the power factor is not 1.
9. Claiming a step-up transformer also steps up current. For an ideal transformer, voltage and current ratios go in opposite directions.
10. Assuming a transformer continuously transforms steady DC.

---

## 10. Timed performance test — 36 NET-style MCQs

**Suggested time:** 36 minutes.  
**Directions:** Choose the single best answer. Attempt every question before reading the key. Mark each answer **confident**, **unsure**, or **guess**; guessed answers count as revision items even when correct. Unless stated otherwise, assume ideal components and sinusoidal steady state.

### Q1. An AC source completes 50 cycles in one second. Its period is:

A. $50\,\text{s}$  
B. $0.50\,\text{s}$  
C. $0.020\,\text{s}$  
D. $100\,\text{s}$

### Q2. The angular frequency of a $60\,\text{Hz}$ source is:

A. $60\,\text{rad/s}$  
B. $120\pi\,\text{rad/s}$  
C. $30\pi\,\text{rad/s}$  
D. $2\pi/60\,\text{rad/s}$

### Q3. A voltage is given by $v(t)=V_0\sin(\omega t)$. At $t=T/4$, where $T$ is its period, its value is:

A. $0$  
B. $-V_0$  
C. $V_0/2$  
D. $+V_0$

### Q4. A sinusoidal current has a peak value of $10\,\text{A}$. Its RMS value is approximately:

A. $14.1\,\text{A}$  
B. $10\,\text{A}$  
C. $7.07\,\text{A}$  
D. $5.00\,\text{A}$

### Q5. The RMS value of a sinusoidal voltage is $100\,\text{V}$. Its peak value is:

A. $50\sqrt{2}\,\text{V}$  
B. $100\sqrt{2}\,\text{V}$  
C. $200\,\text{V}$  
D. $100/\sqrt{2}\,\text{V}$

### Q6. In a pure resistor connected to an AC source, the current and voltage are:

A. $90^\circ$ out of phase  
B. in phase  
C. always opposite in phase  
D. unrelated in frequency

### Q7. In an ideal inductor, the current:

A. leads the voltage by $90^\circ$  
B. lags the voltage by $90^\circ$  
C. is in phase with voltage  
D. is always zero

### Q8. In an ideal capacitor, the current:

A. leads voltage by $90^\circ$  
B. lags voltage by $90^\circ$  
C. is in phase with voltage  
D. has a different frequency from voltage

### Q9. An inductor of $0.20\,\text{H}$ is connected to a $50\,\text{Hz}$ source. Its inductive reactance is:

A. $5\pi\,\Omega$  
B. $10\pi\,\Omega$  
C. $20\pi\,\Omega$  
D. $50\pi\,\Omega$

### Q10. If the frequency through an ideal inductor is doubled while $L$ stays fixed, $X_L$:

A. halves  
B. doubles  
C. becomes four times larger  
D. stays unchanged

### Q11. A $100\,\mu\text{F}$ capacitor is connected to a $50\,\text{Hz}$ source. Its capacitive reactance is approximately:

A. $3.18\,\Omega$  
B. $31.8\,\Omega$  
C. $318\,\Omega$  
D. $0.0318\,\Omega$

### Q12. If the frequency through an ideal capacitor is doubled while $C$ stays fixed, $X_C$:

A. doubles  
B. becomes four times larger  
C. halves  
D. stays unchanged

### Q13. A series circuit has $R=3\,\Omega$, $X_L=4\,\Omega$, and $X_C=0$. Its impedance is:

A. $7\,\Omega$  
B. $5\,\Omega$  
C. $1\,\Omega$  
D. $25\,\Omega$

### Q14. For a series RLC circuit, $R=6\,\Omega$, $X_L=10\,\Omega$, and $X_C=2\,\Omega$. Its impedance is:

A. $18\,\Omega$  
B. $10\,\Omega$  
C. $8\,\Omega$  
D. $6\,\Omega$

### Q15. A series RLC circuit is at resonance when:

A. $R=X_L+X_C$  
B. $X_L=X_C$  
C. $X_L=0$  
D. $X_C=0$

### Q16. An ideal series RLC circuit has $L=0.25\,\text{H}$ and $C=100\,\mu\text{F}$. Its resonant frequency is approximately:

A. $3.18\,\text{Hz}$  
B. $31.8\,\text{Hz}$  
C. $318\,\text{Hz}$  
D. $1000\,\text{Hz}$

### Q17. A series RLC circuit is operated below its resonant frequency. It is net:

A. inductive, because $X_L>X_C$  
B. resistive, because $R$ is present  
C. capacitive, because $X_C>X_L$  
D. at resonance

### Q18. At resonance in a series RLC circuit with fixed supply voltage, the current is:

A. minimum  
B. maximum  
C. zero  
D. independent of resistance

### Q19. At series resonance, which statement about the inductor and capacitor voltages can be true?

A. Each must be zero.  
B. Each may be larger than the supply voltage, while their phasors oppose.  
C. They always add directly to the supply voltage.  
D. Their magnitudes must equal the resistor voltage.

### Q20. In a series RLC circuit, $X_L=30\,\Omega$, $X_C=50\,\Omega$, and $R=40\,\Omega$. The current relative to the supply voltage is:

A. lagging, because the circuit is inductive  
B. leading, because the circuit is capacitive  
C. in phase, because resistance is present  
D. $90^\circ$ lagging

### Q21. An AC load has $V_{\mathrm{rms}}=100\,\text{V}$, $I_{\mathrm{rms}}=2.0\,\text{A}$, and power factor $0.60$. Its average real power is:

A. $33\,\text{W}$  
B. $120\,\text{W}$  
C. $200\,\text{W}$  
D. $333\,\text{W}$

### Q22. The average power consumed by an ideal pure capacitor over a complete cycle is:

A. $V_{\mathrm{rms}}I_{\mathrm{rms}}$  
B. $I_{\mathrm{rms}}^2X_C$  
C. zero  
D. infinite

### Q23. A load has $R=8\,\Omega$ and impedance $Z=10\,\Omega$. Its power factor is:

A. $0.20$  
B. $0.60$  
C. $0.80$  
D. $1.25$

### Q24. A factory load is strongly inductive. A common way to improve its power factor is to connect a suitable:

A. capacitor bank  
B. resistor in series with every appliance  
C. DC source  
D. open switch

### Q25. An ideal transformer has 800 primary turns and 200 secondary turns. If the primary RMS voltage is $240\,\text{V}$, the secondary RMS voltage is:

A. $960\,\text{V}$  
B. $240\,\text{V}$  
C. $60\,\text{V}$  
D. $30\,\text{V}$

### Q26. An ideal transformer reduces voltage to one-fifth of its primary value. If the primary current is $0.40\,\text{A}$, its secondary current is:

A. $0.08\,\text{A}$  
B. $0.40\,\text{A}$  
C. $2.0\,\text{A}$  
D. $10\,\text{A}$

### Q27. In an ideal step-up transformer:

A. both voltage and current rise  
B. voltage rises while current falls  
C. voltage falls while current rises  
D. both voltage and current fall

### Q28. A transformer is connected to a steady DC source. After the switching instant, its secondary voltage is ideally:

A. a steady amplified DC voltage  
B. continuously alternating  
C. zero, because the magnetic flux is no longer changing  
D. equal to the primary voltage for all turns ratios

### Q29. For the same transmitted real power and approximately the same power factor, increasing transmission voltage by a factor of 10 makes line current approximately:

A. 10 times larger  
B. 10 times smaller  
C. 100 times smaller  
D. unchanged

### Q30. A sinusoidal current and a DC current have equal RMS values through the same resistor. Their average heating powers are:

A. equal  
B. greater for AC  
C. greater for DC  
D. both zero

### Q31. The signed average of a pure sinusoidal current over one complete cycle is zero. Which statement is correct?

A. The current is zero throughout the cycle.  
B. No energy can be transferred during the cycle.  
C. Positive and negative current portions cancel in signed average, but resistive heating can remain positive.  
D. The frequency must be zero.

### Q32. A source has angular frequency $\omega=400\pi\,\text{rad/s}$. Its frequency is:

A. $100\,\text{Hz}$  
B. $200\,\text{Hz}$  
C. $400\,\text{Hz}$  
D. $800\pi\,\text{Hz}$

### Q33. Which change makes an ideal capacitor pass AC more readily?

A. Lowering frequency  
B. Increasing frequency  
C. Decreasing frequency and capacitance  
D. Replacing AC with a higher-amplitude source at the same frequency

### Q34. At resonance in an ideal series RLC circuit with nonzero resistance, the power factor is:

A. zero  
B. $1/2$  
C. one  
D. infinite

### Q35. Two loads have the same RMS voltage and RMS current. Load A has power factor $0.9$ and load B has power factor $0.5$. Which has larger average real power?

A. Load A  
B. Load B  
C. They are equal  
D. Cannot be determined even with the power factors

### Q36. If a sinusoidal source voltage is written as $v(t)=V_0\sin(\omega t+\pi/3)$, the phase constant indicates that at $t=0$ the voltage is:

A. zero  
B. $+V_0/2$  
C. $+\sqrt{3}V_0/2$  
D. $-V_0$

---

## 11. Answer key with reasoning

**Read this only after completing the timed attempt.**

| Q | Answer | Reasoning |
|---:|:---:|---|
| 1 | C | $f=50\,\text{Hz}$, so $T=1/f=1/50=0.020\,\text{s}$. |
| 2 | B | $\omega=2\pi f=2\pi(60)=120\pi\,\text{rad/s}$. |
| 3 | D | Since $T=2\pi/\omega$, at $T/4$ the phase is $\pi/2$ and $\sin(\pi/2)=1$. |
| 4 | C | $I_{\mathrm{rms}}=I_0/\sqrt{2}=10/\sqrt{2}\approx7.07\,\text{A}$. |
| 5 | B | Peak is $\sqrt{2}$ times RMS: $V_0=100\sqrt{2}\,\text{V}$. |
| 6 | B | A resistor obeys $v=Ri$ at every instant, so the waveforms are in phase. |
| 7 | B | Inductor current lags its voltage by $90^\circ$. |
| 8 | A | Capacitor current leads its voltage by $90^\circ$. |
| 9 | C | $X_L=2\pi fL=2\pi(50)(0.20)=20\pi\,\Omega$. |
| 10 | B | $X_L=2\pi fL$, so doubling $f$ doubles the reactance. |
| 11 | B | $X_C=1/[2\pi(50)(100\times10^{-6})]\approx31.8\,\Omega$. |
| 12 | C | $X_C$ varies as $1/f$, so doubling $f$ halves it. |
| 13 | B | $Z=\sqrt{R^2+X_L^2}=\sqrt{3^2+4^2}=5\,\Omega$. |
| 14 | B | Net reactance is $10-2=8\,\Omega$; $Z=\sqrt{6^2+8^2}=10\,\Omega$. |
| 15 | B | Resonance is the balance condition $X_L=X_C$. |
| 16 | B | $f_0=1/[2\pi\sqrt{(0.25)(100\times10^{-6})}]\approx31.8\,\text{Hz}$. |
| 17 | C | Below resonance, $X_C>X_L$, so the circuit is net capacitive. |
| 18 | B | At resonance, $Z=R$, the minimum series impedance; fixed voltage gives maximum current. |
| 19 | B | $V_L$ and $V_C$ are opposite in phase. Their individual magnitudes can exceed supply voltage while their difference contributes to the supply phasor. |
| 20 | B | Since $X_C>X_L$, the net circuit is capacitive and current leads supply voltage. |
| 21 | B | $P=V_{\mathrm{rms}}I_{\mathrm{rms}}\cos\phi=(100)(2.0)(0.60)=120\,\text{W}$. |
| 22 | C | An ideal capacitor returns the energy it stores; its average power over a full cycle is zero. |
| 23 | C | For a series impedance, $\cos\phi=R/Z=8/10=0.80$. |
| 24 | A | A capacitor offsets part of an inductive load’s reactive effect and can raise power factor. |
| 25 | C | $V_s/V_p=N_s/N_p=200/800=1/4$, so $V_s=240/4=60\,\text{V}$. |
| 26 | C | Voltage is reduced by 5, so ideal current rises by 5: $I_s=5(0.40)=2.0\,\text{A}$. |
| 27 | B | Ideal power is conserved, so increasing voltage requires current to decrease. |
| 28 | C | After the switching transient, steady DC produces constant flux, so there is no continuing induced secondary voltage. |
| 29 | B | At fixed power, a tenfold increase in voltage gives roughly one-tenth the current. |
| 30 | A | Equal RMS current produces equal $I_{\mathrm{rms}}^2R$ average heating in the same resistor. |
| 31 | C | Signed current cancels over a cycle, but $i^2R$ is nonnegative and generally has a positive average. |
| 32 | B | $f=\omega/(2\pi)=400\pi/(2\pi)=200\,\text{Hz}$. |
| 33 | B | Increasing frequency lowers $X_C=1/(2\pi fC)$, making the capacitor’s opposition smaller. |
| 34 | C | At resonance, $\phi=0$, so $\cos\phi=1$. |
| 35 | A | $P=V_{\mathrm{rms}}I_{\mathrm{rms}}\times\text{power factor}$; with the same RMS values, 0.9 gives more real power than 0.5. |
| 36 | C | At $t=0$, $v=V_0\sin(\pi/3)=\sqrt{3}V_0/2$. |

---

## 12. Score interpretation and error analysis

### Score bands

- **33–36 correct:** Strong command. Explain why each distractor is wrong, especially for any guessed answer.
- **28–32 correct:** Good foundation. Review the exact types of errors: phase, RMS, RLC arithmetic, power, or transformer ratios.
- **22–27 correct:** Developing. Rework the examples, then retry missed questions without the key.
- **Below 22:** Rebuild the signal and phase model first, then study reactance and resonance in a second pass.

These bands are study guidance, not official NUST or FAST cutoffs.

### Error log

| Field | What to record |
|---|---|
| Question | Number and subtopic |
| Error type | Concept / phase / formula / units / arithmetic / rushed reading |
| My reasoning | Why the selected option seemed right |
| Correct principle | State the idea in one sentence |
| Retry | Solve again later without the answer key |

### Diagnose the pattern

- **Peak/RMS misses:** Write the conversion beside the question before substituting.
- **Lead/lag misses:** Draw one cycle and label which waveform reaches its peak first.
- **Reactance misses:** Record separately that $X_L$ rises with $f$ and $X_C$ falls with $f$.
- **Impedance misses:** Calculate $X_L-X_C$ first; then use the right-angle relation.
- **Power misses:** Use RMS values and include the power factor.
- **Transformer misses:** Write the turns ratio for voltage, then invert it for current.
- **Lucky correct answers:** Revisit them as unsure answers; recognition without explanation is not mastery.

## 13. One-page formula recap

$$
f=\frac{1}{T},
\qquad
\omega=2\pi f,
\qquad
V_{\mathrm{rms}}=\frac{V_0}{\sqrt{2}},
\qquad
I_{\mathrm{rms}}=\frac{I_0}{\sqrt{2}}
$$

$$
X_L=\omega L,
\qquad
X_C=\frac{1}{\omega C},
\qquad
Z=\sqrt{R^2+(X_L-X_C)^2},
\qquad
I_{\mathrm{rms}}=\frac{V_{\mathrm{rms}}}{Z}
$$

$$
\tan\phi=\frac{X_L-X_C}{R},
\qquad
\cos\phi=\frac{R}{Z},
\qquad
P_{\mathrm{avg}}=V_{\mathrm{rms}}I_{\mathrm{rms}}\cos\phi
$$

$$
\omega_0=\frac{1}{\sqrt{LC}},
\qquad
f_0=\frac{1}{2\pi\sqrt{LC}},
\qquad
\frac{V_s}{V_p}=\frac{N_s}{N_p},
\qquad
\frac{I_s}{I_p}=\frac{N_p}{N_s}
$$

- In a resistor: voltage and current are in phase.
- In an inductor: current lags voltage.
- In a capacitor: current leads voltage.
- At series resonance: $X_L=X_C$, $Z=R$, current is maximum, and power factor is one.
- For an ideal transformer: voltage follows turns; current follows the inverse turns ratio.

## Session completion checklist

- [ ] I can explain RMS as an equivalent heating value.
- [ ] I can state the lead/lag relation for R, L, and C without hesitation.
- [ ] I can predict how each reactance changes when frequency changes.
- [ ] I can calculate series RLC impedance and classify the circuit.
- [ ] I can explain why current is maximum at series resonance.
- [ ] I can calculate real power using RMS values and power factor.
- [ ] I can solve ideal transformer voltage and current ratios.
- [ ] I attempted all 36 questions under timed conditions.
- [ ] I recorded incorrect and guessed answers in my error log.

**Next recommended session:** Electromagnetic induction and transformers in more depth, followed by a mixed electricity and magnetism NET revision set.
