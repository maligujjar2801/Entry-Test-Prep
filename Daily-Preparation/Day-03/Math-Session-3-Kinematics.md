# Math Session 3 — Kinematics of Motion in a Straight Line

> **Admission-test track:** NUST NET + FAST/NUCES  
> **Textbook alignment:** Mathematics 12 (PECTAA), Unit 7 — Kinematics of Motion in a Straight Line  
> **Study sequence:** Quick Recall → Concepts → Formula Recognition → Worked Examples → MCQ Practice → Timed Test → Error Analysis

## 1. Session Objectives

By the end of this session, you should be able to distinguish distance and displacement, speed and velocity; calculate average values; derive velocity and acceleration by differentiation; integrate acceleration using initial conditions; interpret motion graphs; use the three constant-acceleration equations; and solve basic free-fall and vertical-throw problems.

**Method:** identify what is given and what is required, check whether acceleration is constant, then select the formula. Keep units and signs consistent.

## 2. Five-Minute Recall from Sessions 1–2

1. For \((x-2)^2+(y+3)^2=16\), find centre and radius.
2. For \(y^2=24x\), find \(a\) and focus.
3. Which relation belongs to an ellipse: \(c^2=a^2-b^2\) or \(c^2=a^2+b^2\)?
4. What is the difference between average speed and average velocity?

**Key:** (1) centre \((2,-3)\), radius \(4\); (2) \(4a=24\Rightarrow a=6\), focus \((6,0)\); (3) ellipse: \(c^2=a^2-b^2\); (4) speed uses total distance, velocity uses net displacement.

---

# PART I — CORE CONCEPTS

## 3. Kinematics and Rectilinear Motion

Kinematics describes motion without studying its causes. Rectilinear motion is motion along a straight line. Choose one direction as positive; the opposite direction is negative. Displacement, velocity and acceleration can be signed, but distance and speed cannot be negative.

## 4. Scalars and Vectors

| Quantity | Type | Meaning |
|---|---|---|
| Distance | Scalar | Total path length |
| Speed | Scalar | Rate of covering distance |
| Displacement | Vector | Change from initial to final position |
| Velocity | Vector | Rate of change of displacement |
| Acceleration | Vector | Rate of change of velocity |

Negative velocity means motion in the chosen negative direction. It does not automatically mean the object is slowing down. Speed decreases when velocity and acceleration have opposite signs.

## 5. Distance, Displacement, Average Speed and Average Velocity

\[
\boxed{\Delta x=x_f-x_i}
\]

Distance is total path length; displacement is final position minus initial position. Therefore,

\[
\boxed{\text{distance}\geq |\Delta x|}
\]

\[
\boxed{\text{Average speed}=\frac{\text{total distance}}{\text{total time}}}
\qquad
\boxed{\bar v=\frac{\text{net displacement}}{\text{total time}}}
\]

### Worked Example 1 — Out-and-Back Journey

A student walks 180 m east in 30 s, then 80 m west in 20 s. Take east as positive.

- Distance: \(180+80=260\) m.
- Displacement: \(+180-80=+100\) m, or 100 m east.
- Total time: \(30+20=50\) s.
- Average speed: \(260/50=\boxed{5.2\text{ m/s}}\).
- Average velocity: \(100/50=\boxed{2\text{ m/s east}}\).

Use the same total elapsed time for both averages, but different numerators.

## 6. Instantaneous Velocity and Acceleration

If position \(x(t)\) is given as a function of time,

\[
\boxed{v(t)=\frac{dx}{dt}},\qquad
\boxed{\text{instantaneous speed}=|v(t)|}
\]

Acceleration is the rate of change of velocity:

\[
\boxed{a(t)=\frac{dv}{dt}=\frac{d^2x}{dt^2}}
\]

If velocity is expressed as a function of position, the chain rule gives

\[
\boxed{a=v\frac{dv}{dx}}
\]

Units: displacement in metres (m), velocity in m/s and acceleration in m/s².

### Worked Example 2 — Differentiate Position

Let \(x(t)=2t^3-3t^2+4\), with position in metres and time in seconds.

\[
v(t)=\frac{dx}{dt}=6t^2-6t
\]

At \(t=2\), \(v=24-12=\boxed{12\text{ m/s}}\).

\[
a(t)=\frac{dv}{dt}=12t-6
\]

At \(t=2\), \(a=24-6=\boxed{18\text{ m/s}^2}\).

**Recognition:** differentiate once to get velocity, twice to get acceleration.

### Sign of Velocity and Acceleration

| Velocity | Acceleration | Result at that instant |
|---|---|---|
| Positive | Positive | Moving positive; speed increasing |
| Positive | Negative | Moving positive; speed decreasing |
| Negative | Negative | Moving negative; speed increasing |
| Negative | Positive | Moving negative; speed decreasing |

## 7. Integrating Acceleration

If acceleration is given, integrate to obtain velocity; integrate velocity to obtain position. Use initial conditions to determine the integration constants.

\[
a(t)=\frac{dv}{dt}\Rightarrow v(t)=\int a(t)\,dt+C
\]

\[
v(t)=\frac{dx}{dt}\Rightarrow x(t)=\int v(t)\,dt+C_1
\]

### Worked Example 3 — Apply Initial Conditions

Suppose \(a(t)=6t\), \(v(0)=2\text{ m/s}\), and \(x(0)=0\).

\[
v(t)=\int6t\,dt=3t^2+C
\]

Since \(v(0)=2\), \(C=2\), so \(\boxed{v(t)=3t^2+2}\).

\[
x(t)=\int(3t^2+2)\,dt=t^3+2t+C_1
\]

Since \(x(0)=0\), \(C_1=0\), so \(\boxed{x(t)=t^3+2t}\).

Do not discard integration constants before using the initial conditions.

---

# PART II — MOTION GRAPHS

## 8. Displacement-Time Graph

Time is on the horizontal axis and displacement/position on the vertical axis. **Slope gives velocity**:

\[
\boxed{v=\frac{dx}{dt}=\text{slope of the displacement-time graph}}
\]

- Horizontal segment: zero velocity; position is constant.
- Rising straight line: constant positive velocity.
- Falling straight line: constant negative velocity.
- Curved segment: velocity varies; use tangent slope for instantaneous velocity.
- Greater slope magnitude means greater speed.

### Worked Example 4

Position changes from 4 m at \(t=0\) to 28 m at \(t=6\) s along a straight segment:

\[
v=\frac{28-4}{6-0}=\boxed{4\text{ m/s}}
\]

## 9. Velocity-Time Graph

Time is horizontal and velocity is vertical. Two key rules:

\[
\boxed{\text{slope}=\text{acceleration}}
\qquad
\boxed{\text{signed area}=\text{displacement}}
\]

Areas above the time axis contribute positive displacement; areas below contribute negative displacement. For **total distance**, add the magnitudes of the areas.

For uniform acceleration, velocity changes linearly and displacement can be calculated as trapezoid area:

\[
\boxed{s=\frac{u+v}{2}t}
\]

### Worked Example 5

Velocity increases uniformly from 2 m/s to 14 m/s in 4 s.

\[
a=\frac{14-2}{4}=\boxed{3\text{ m/s}^2}
\]

\[
s=\frac{2+14}{2}\times4=\boxed{32\text{ m}}
\]

**Graph traps:** slope of displacement-time means velocity; slope of velocity-time means acceleration; signed area under velocity-time means displacement, not automatically distance.

---

# PART III — CONSTANT ACCELERATION

## 10. The Equations of Motion

Use these only when acceleration is constant throughout the interval.

| Symbol | Meaning |
|---|---|
| \(u\) | Initial velocity |
| \(v\) | Final velocity |
| \(a\) | Constant acceleration |
| \(t\) | Elapsed time |
| \(s\) | Displacement |

\[
\boxed{v=u+at}
\]

\[
\boxed{s=ut+\frac12at^2}
\]

\[
\boxed{v^2=u^2+2as}
\]

A useful companion is \(s=\frac12(u+v)t\), valid for constant acceleration.

### Selecting a Formula

| Given / requested | Usually use |
|---|---|
| \(u,a,t\), find \(v\) | \(v=u+at\) |
| \(u,a,t\), find \(s\) | \(s=ut+\frac12at^2\) |
| \(u,v,a\), find \(s\) without time | \(v^2=u^2+2as\) |
| \(u,v,t\), find \(s\) | \(s=\frac12(u+v)t\) |
| Starts from rest | Set \(u=0\) |
| Comes to rest | Set \(v=0\) |

### Worked Example 6 — Uniform Acceleration

A vehicle begins at 5 m/s and accelerates at 2 m/s² for 4 s.

\[
v=5+2(4)=\boxed{13\text{ m/s}}
\]

\[
s=5(4)+\frac12(2)(4^2)=20+16=\boxed{36\text{ m}}
\]

### Worked Example 7 — Braking

A car travels at 20 m/s and brakes at \(-4\text{ m/s}^2\). At rest, \(v=0\):

\[
0=20-4t\Rightarrow\boxed{t=5\text{ s}}
\]

Without needing time, use \(v^2=u^2+2as\):

\[
0=20^2+2(-4)s\Rightarrow\boxed{s=50\text{ m}}
\]

The displacement is positive because the car still moves forward while braking.

---

# PART IV — VERTICAL MOTION

## 11. Gravity and Sign Convention

Near Earth's surface, \(g\approx9.8\text{ m/s}^2\), unless the question specifies otherwise.

- If upward is positive, \(a=-g\).
- If downward is positive, \(a=+g\).

For upward-positive motion:

\[
\boxed{v=u-gt},\quad
\boxed{s=ut-\frac12gt^2},\quad
\boxed{v^2=u^2-2gs}
\]

At the highest point, velocity is zero but acceleration is still \(-g\).

### Worked Example 8 — Dropped Object

A stone is dropped from 20 m. Neglect air resistance and use \(g=9.8\text{ m/s}^2\).

Since \(u=0\), \(h=\frac12gt^2\):

\[
20=4.9t^2\Rightarrow t=\sqrt{40/9.8}\approx\boxed{2.02\text{ s}}
\]

Impact speed \(v=gt\approx9.8(2.02)=\boxed{19.8\text{ m/s downward}}\).

### Worked Example 9 — Upward Throw

A ball is thrown upward at 19.6 m/s. At maximum height, \(v=0\):

\[
0=19.6-9.8t\Rightarrow\boxed{t=2\text{ s}}
\]

\[
s=19.6(2)-\frac12(9.8)(2^2)=\boxed{19.6\text{ m}}
\]

**Vertical-motion traps:** dropped means \(u=0\); thrown downward may have nonzero \(u\); gravity does not become zero at the top; declare your positive direction before substituting.

---

# PART V — FORMULA MASTER SHEET

| Task | Formula / rule |
|---|---|
| Displacement | \(\Delta x=x_f-x_i\) |
| Average velocity | \(\bar v=\Delta x/\Delta t\) |
| Average speed | Total distance / total time |
| Instantaneous velocity | \(v=dx/dt\) |
| Instantaneous speed | \(|v|\) |
| Acceleration | \(a=dv/dt=d^2x/dt^2\) |
| Acceleration as a function of position | \(a=v\,dv/dx\) |
| Displacement-time graph | Slope = velocity |
| Velocity-time graph | Slope = acceleration |
| Velocity-time graph | Signed area = displacement |
| Constant acceleration | \(v=u+at\) |
| Constant acceleration | \(s=ut+\frac12at^2\) |
| Constant acceleration | \(v^2=u^2+2as\) |
| Constant acceleration | \(s=\frac12(u+v)t\) |
| Free fall from rest | \(h=\frac12gt^2\) |
| Vertical throw, upward positive | \(v=u-gt\) |

## NET / FAST Recognition Patterns

1. Position \(x(t)\) given → differentiate once for \(v\), twice for \(a\).
2. Acceleration \(a(t)\) given → integrate and apply initial conditions.
3. Displacement-time graph → slope is velocity.
4. Velocity-time graph → slope is acceleration; signed area is displacement.
5. Constant acceleration → select the equation from the known variables.
6. No time in the data → consider \(v^2=u^2+2as\).
7. Asked for speed → answer with a non-negative magnitude; asked for velocity → retain sign/direction.
8. Vertical motion → set the sign of gravity consistently.
9. Check units and distinguish distance from displacement before choosing the option.

## Common Traps

- Using displacement instead of total distance to calculate average speed.
- Giving negative speed instead of signed velocity.
- Confusing graph slope and graph area.
- Treating area below a velocity-time axis as negative distance.
- Applying constant-acceleration equations when acceleration varies.
- Forgetting integration constants or initial conditions.
- Mixing signs for braking or gravity.
- Setting both velocity and acceleration to zero at maximum height.
- Mixing metres/kilometres or seconds/hours.

---

# PART VI — PRACTICE MCQs

**Timed attempt:** 25 questions in 23 minutes, matching Session 2's format. Do not consult the key until finished. Use \(g=9.8\text{ m/s}^2\).

### Q1. A particle moves from \(x=3\) m to \(x=-4\) m. Displacement is:
A. \(7\) m  B. \(-7\) m  C. \(1\) m  D. \(-1\) m

### Q2. A person walks 9 m east, then 4 m west. Total distance is:
A. 5 m  B. 13 m  C. 9 m  D. 4 m

### Q3. A runner covers 150 m in 30 s. Average speed is:
A. 3 m/s  B. 4 m/s  C. 5 m/s  D. 6 m/s

### Q4. A person travels 60 m east in 20 s and 20 m west in 10 s. Average velocity is:
A. \(4/3\) m/s east  B. \(8/3\) m/s east  C. \(4/3\) m/s west  D. \(8/3\) m/s west

### Q5. If \(x(t)=2t^2+3t\), velocity at \(t=2\) s is:
A. 7 m/s  B. 8 m/s  C. 11 m/s  D. 14 m/s

### Q6. If \(x(t)=t^3-2t\), velocity at \(t=2\) s is:
A. 4 m/s  B. 8 m/s  C. 10 m/s  D. 12 m/s

### Q7. If \(v(t)=5t^2-2t\), acceleration at \(t=1\) s is:
A. 3 m/s²  B. 6 m/s²  C. 8 m/s²  D. 10 m/s²

### Q8. A horizontal displacement-time segment means the particle is:
A. moving with positive velocity  B. moving with negative velocity  C. at rest  D. speeding up

### Q9. A straight displacement-time graph with negative slope indicates:
A. positive velocity  B. negative velocity  C. zero velocity  D. necessarily increasing speed

### Q10. Velocity changes uniformly from \(-2\) m/s to \(10\) m/s in 3 s. Acceleration is:
A. 2 m/s²  B. 3 m/s²  C. 4 m/s²  D. 6 m/s²

### Q11. Velocity is constant at 7 m/s for 4 s. Displacement is:
A. 11 m  B. 21 m  C. 28 m  D. 49 m

### Q12. Velocity is \(-3\) m/s for 4 s. Distance travelled is:
A. \(-12\) m  B. 3 m  C. 7 m  D. 12 m

### Q13. Velocity rises uniformly from 4 m/s to 12 m/s in 2 s. Displacement is:
A. 8 m  B. 12 m  C. 16 m  D. 24 m

### Q14. \(u=6\) m/s, \(a=3\) m/s², \(t=5\) s. Final velocity is:
A. 9 m/s  B. 15 m/s  C. 21 m/s  D. 30 m/s

### Q15. \(u=4\) m/s, \(a=2\) m/s², \(t=3\) s. Displacement is:
A. 12 m  B. 18 m  C. 21 m  D. 24 m

### Q16. A particle starts from rest, accelerates at 2 m/s² over 25 m. Final speed is:
A. 5 m/s  B. 10 m/s  C. 25 m/s  D. 50 m/s

### Q17. Velocity changes from 30 m/s to 10 m/s at constant acceleration \(-5\) m/s². Elapsed time is:
A. 2 s  B. 4 s  C. 5 s  D. 8 s

### Q18. A car travels at 20 m/s and brakes at \(-4\) m/s². Stopping time is:
A. 4 s  B. 5 s  C. 8 s  D. 10 s

### Q19. For the same car in Q18, stopping displacement is:
A. 20 m  B. 25 m  C. 40 m  D. 50 m

### Q20. An object dropped from rest falls 19.6 m. Fall time is:
A. 1 s  B. 2 s  C. 3 s  D. 4 s

### Q21. A ball is thrown vertically upward at 19.6 m/s. Time to maximum height is:
A. 1 s  B. 2 s  C. 3 s  D. 4 s

### Q22. With upward chosen positive, acceleration at the highest point of a vertical throw is:
A. zero  B. \(+9.8\) m/s²  C. \(-9.8\) m/s²  D. undefined

### Q23. If \(a(t)=6t\) and \(v(0)=2\) m/s, then \(v(2)\) is:
A. 8 m/s  B. 10 m/s  C. 14 m/s  D. 26 m/s

### Q24. Which is a vector quantity?
A. distance  B. speed  C. velocity  D. time

### Q25. If a velocity-time graph has regions both above and below the time axis, net displacement is found by:
A. adding all absolute areas  B. subtracting every area from zero  C. taking the signed sum of areas  D. using only the largest area

---

# PART VII — ANSWER KEY AND QUICK REASONS

| Q | Answer | Reason |
|---:|:---:|---|
| 1 | B | \(\Delta x=-4-3=-7\) m. |
| 2 | B | Total path length: \(9+4=13\) m. |
| 3 | C | \(150/30=5\) m/s. |
| 4 | A | Net displacement \(40\) m east over 30 s: \(40/30=4/3\) m/s east. |
| 5 | C | \(v=4t+3\), so \(v(2)=11\) m/s. |
| 6 | C | \(v=3t^2-2\), so \(v(2)=10\) m/s. |
| 7 | C | \(a=10t-2\), so \(a(1)=8\) m/s². |
| 8 | C | Constant displacement means zero slope and velocity. |
| 9 | B | Displacement-time slope equals velocity. |
| 10 | C | \(a=(10-(-2))/3=4\) m/s². |
| 11 | C | Displacement \(=7(4)=28\) m. |
| 12 | D | Distance \(=|-3|(4)=12\) m. |
| 13 | C | Average velocity \(=(4+12)/2=8\) m/s; \(s=8(2)=16\) m. |
| 14 | C | \(v=6+3(5)=21\) m/s. |
| 15 | C | \(s=4(3)+\frac12(2)(3^2)=21\) m. |
| 16 | B | \(v^2=2as=2(2)(25)=100\), so \(v=10\) m/s. |
| 17 | B | \(t=(10-30)/(-5)=4\) s. |
| 18 | B | \(0=20-4t\Rightarrow t=5\) s. |
| 19 | D | \(0=20^2-8s\Rightarrow s=50\) m. |
| 20 | B | \(19.6=4.9t^2\Rightarrow t=2\) s. |
| 21 | B | At the top \(0=19.6-9.8t\Rightarrow t=2\) s. |
| 22 | C | Gravity remains downward, so \(a=-g\) for upward-positive coordinates. |
| 23 | C | Integrate \(a\): \(v=3t^2+C\); \(v(0)=2\Rightarrow C=2\), so \(v(2)=14\). |
| 24 | C | Velocity has both magnitude and direction. |
| 25 | C | Signed areas give net displacement; absolute areas give total distance. |

## Score Guide

| Score | Next step |
|---|---|
| 22–25 | Rework missed questions and practise for speed. |
| 18–21 | Revise the specific graph or formula rules you missed. |
| 13–17 | Revisit Parts I–IV, then retake the test. |
| 0–12 | Rebuild the core concepts before retrying. |

A score band is a revision guide, not a judgement. Focus on what caused each error.

# PART VIII — TEST RECORD AND ERROR ANALYSIS

Fill this in only after attempting the test without the key.

| Measure | Result |
|---|---|
| Questions attempted | ___ / 25 |
| Correct answers | ___ / 25 |
| Accuracy | ___ % |
| Time taken | ___ min ___ sec |
| Guessed answers | ___ |

\[
\text{Accuracy}=\frac{\text{correct answers}}{25}\times100\%
\]

| Question | Error type | Why it happened | Correct rule | Retry |
|---|---|---|---|---|
| ___ | Concept / Formula / Sign / Algebra / Units / Graph / Guess | ___ | ___ | ___ |
| ___ | Concept / Formula / Sign / Algebra / Units / Graph / Guess | ___ | ___ | ___ |
| ___ | Concept / Formula / Sign / Algebra / Units / Graph / Guess | ___ | ___ | ___ |

Do not label every error “careless.” Identify the actual step: wrong quantity, formula choice, sign, derivative, unit, or graph interpretation.

## Final Checklist

- [ ] Distinguish distance from displacement and speed from velocity.
- [ ] Calculate averages for a multi-stage journey.
- [ ] Differentiate \(x(t)\) for velocity and acceleration.
- [ ] Integrate \(a(t)\) and use initial conditions.
- [ ] Read slope and area correctly on motion graphs.
- [ ] Choose among the constant-acceleration equations.
- [ ] Solve free-fall and upward-throw problems with consistent signs.
- [ ] Explain each missed MCQ in your own words.

## Source Alignment

Prepared against the uploaded *Mathematics 12 (PECTAA)* textbook, Unit 7, *Kinematics of Motion in a Straight Line*, especially rectilinear motion; scalars and vectors; displacement, velocity and acceleration; displacement-time and velocity-time graphs; constant acceleration; and free vertical motion. The practice questions and explanations are original study material aligned to the unit rather than copied textbook exercise questions.
