# Physics Session 1 — Electrostatics: Charge, Coulomb's Law, and Electric Field

**Track:** NUST NET + FAST/NUCES  
**Level:** Class 12 foundation → entry-test conceptual reasoning  
**Session type:** Concept lesson, worked examples, and 30-question performance test  
**Suggested duration:** 90–120 minutes  
**Prerequisite:** Basic vectors, scientific notation, inverse-square relationships, and Newton's laws

---

## Session outcomes

By the end of this session, you should be able to:

- Explain charge, conservation of charge, and quantization without memorizing disconnected statements.
- Predict attraction or repulsion from charge signs.
- Apply Coulomb's law and compare forces when charge or separation changes.
- Distinguish electric force, electric field, and the force on a test charge.
- Find the direction and net value of fields due to multiple point charges using superposition.
- Reason about zero-field points and common symmetry cases.
- Avoid common conceptual traps in NET/FAST-style MCQs.

## The conceptual model: three simple questions

Think of electrostatics through three linked questions:

1. **What creates the effect?** Electric charge.
2. **What does a charge create around itself?** An electric field.
3. **What happens to another charge placed there?** It experiences an electric force.

The field is a property of the location created by source charges. The force depends on both the field and the charge placed there.

$

\boxed{\vec F=q\vec E}

$

A positive test charge accelerates in the direction of the electric field; a negative charge experiences force opposite to the field.

---

## 1. Electric charge

There are two kinds of electric charge: positive and negative. Like charges repel; unlike charges attract.

### Essential properties

**Conservation:** In an isolated system, the total charge remains constant. Charge can move between objects, but ordinary charging does not create net charge from nothing.

**Quantization:** Charge on an isolated object is an integer multiple of the elementary charge:

$

q=ne,\qquad n=0,\pm1,\pm2,\ldots

$

where $e=1.602\times10^{-19}\,\text{C}$. The magnitude of the electron's charge is $e$; its charge is $-e$, while a proton carries $+e$.

**Additivity:** Total charge is the algebraic sum of the charges. For example, $+5\,\text{C}$ and $-2\,\text{C}$ together have net charge $+3\,\text{C}$.

### Charging by transfer

In common solid materials, electrons transfer between objects. An object that gains electrons becomes negatively charged; an object that loses electrons becomes positively charged. A positive object is not necessarily made only of protons—it usually has fewer electrons than positive charges in its material.

### Conductors and insulators

- **Conductors** allow charge to move relatively freely through them.
- **Insulators** do not allow charge to move freely through the material.
- Both can become charged. “Insulator” does not mean “cannot carry charge.”

### Induction and polarization

A charged object can cause charges inside a nearby object to redistribute without direct contact. In a conductor, mobile charges can shift over larger distances. In an insulator, bound positive and negative charge distributions can shift slightly; this is polarization. A neutral object can therefore be attracted to a charged object because the nearer induced opposite-charge region can experience a stronger force.

**Trap:** Attraction does not prove that both objects are oppositely charged. A charged object can attract a neutral, polarizable object.

---

## 2. Coulomb's law

For two stationary point charges separated by distance $r$, the magnitude of the electric force is

$

F=k\frac{|q_1q_2|}{r^2}

$

where

$

k\approx8.99\times10^9\,\text{N m}^2/\text{C}^2

$

in vacuum (approximately the same value in air for typical entry-test calculations).

### Read the equation, do not just memorize it

- Doubling either charge doubles the force magnitude.
- Doubling both charge magnitudes multiplies the force by four.
- Doubling the separation reduces the force to one-quarter.
- Tripling the separation reduces the force to one-ninth.
- The force acts along the line joining the charges.
- Like charges repel; unlike charges attract.

The absolute-value bars calculate magnitude. The signs of $q_1$ and $q_2$ determine whether the force is attractive or repulsive.

### Scaling rule

If $|q_1q_2|$ changes by a factor $a$ and separation changes by a factor $b$, then

$

\frac{F'}{F}=\frac{a}{b^2}

$

This ratio is often faster than substituting constants.

### Newton's third law

The force exerted by charge 1 on charge 2 and the force exerted by charge 2 on charge 1 have equal magnitudes and opposite directions:

$

\vec F_{12}=-\vec F_{21}

$

Different charges do not exert unequal mutual forces simply because one charge is larger. Their accelerations can differ because their masses differ.

---

## 3. Electric field

The electric field describes the force per unit positive test charge at a point:

$

\vec E=\frac{\vec F}{q_0}

$

where $q_0$ is a small positive test charge. The unit is $\text{N/C}$ (equivalently $\text{V/m}$, though potential is not the focus of this session).

For a point source charge $Q$, the field magnitude at distance $r$ is

$

E=k\frac{|Q|}{r^2}

$

Its direction is:

- **Away from a positive source charge.**
- **Toward a negative source charge.**

The field direction is defined using a positive test charge. A negative particle placed there feels force in the opposite direction.

### Field versus force

| Electric field $\vec E$ | Electric force $\vec F$ |
|---|---|
| Created by source charges | Acts on a charge placed in the field |
| Does not depend on the test charge used to measure it | Depends on the charge experiencing it |
| Direction is force direction on a positive test charge | Reverses direction for a negative charge |
| Unit: N/C | Unit: N |

If the test charge is doubled, the force doubles, but the field at that location remains the same, provided the test charge is small enough not to disturb the source arrangement.

---

## 4. Superposition: combine fields as vectors

When several source charges are present, each produces its own field. The net field is the **vector sum**:

$

\vec E_{\text{net}}=\vec E_1+\vec E_2+\cdots+\vec E_n

$

Do not add magnitudes blindly. First determine each field's direction.

### One-dimensional sign method

Choose a positive direction, such as right. Assign fields pointing right a positive sign and fields pointing left a negative sign. Then add algebraically.

### Example A — two positive charges

Place two equal positive charges at the ends of a line. At the midpoint, the field due to the left charge points right, while the field due to the right charge points left. Equal magnitudes cancel, so the net field is zero.

This does **not** mean there are no fields there. Two nonzero fields cancel in their vector sum.

### Example B — opposite charges

Place a positive charge on the left and an equal negative charge on the right. At the midpoint, the positive charge's field points away from it (right), and the negative charge's field points toward it (also right). The fields add.

### Zero-field points: a reasoning strategy

1. Sketch source charges and the point of interest.
2. Draw each field direction using “away from +, toward −”.
3. Compare magnitudes using $E\propto |Q|/r^2$.
4. Add vectors and check whether cancellation is possible.

For two like charges, a zero-field point can lie between them, where the fields oppose. For two opposite charges, the fields between them point in the same direction, so they cannot cancel between the charges. In the unequal opposite-charge case, a zero-field point may lie outside the pair, on the side of the smaller-magnitude charge. Equal and opposite charges have no finite zero-field point on the line.

---

## 5. Worked examples

### Example 1 — Coulomb force

Two charges of magnitudes $2\,\mu\text{C}$ and $3\,\mu\text{C}$ are separated by $0.30\,\text{m}$ in air. Find the force magnitude.

Convert microcoulombs first:

$

q_1=2\times10^{-6}\,\text{C},\quad
q_2=3\times10^{-6}\,\text{C}

$

Substitute:

$

F=8.99\times10^9
\frac{(2\times10^{-6})(3\times10^{-6})}{(0.30)^2}
\approx0.60\,\text{N}

$

The force is approximately $0.60\,\text{N}$. Whether it is attractive or repulsive depends on the signs of the charges, not their magnitudes alone.

### Example 2 — distance scaling

If the separation becomes three times larger while the charges remain unchanged:

$

F'=F\left(\frac{1}{3}\right)^2=\frac{F}{9}

$

The new force is one-ninth of the original.

### Example 3 — field due to a point charge

A $+4\,\mu\text{C}$ point charge produces a field at a point $0.20\,\text{m}$ away:

$

E=8.99\times10^9\frac{4\times10^{-6}}{(0.20)^2}
\approx8.99\times10^5\,\text{N/C}

$

The field points away from the positive charge.

### Example 4 — force from a known field

A charge $q=-2\,\mu\text{C}$ is placed in a uniform field of magnitude $300\,\text{N/C}$. The force magnitude is

$

F=|q|E=(2\times10^{-6})(300)
=6.0\times10^{-4}\,\text{N}

$

Its force direction is opposite to the electric field because the charge is negative.

---

## 6. Common conceptual traps

1. **Using centimetres or microcoulombs without conversion.** Convert to metres and coulombs before substitution.
2. **Confusing field direction with force direction.** They match only for positive charges.
3. **Adding field magnitudes rather than vectors.** Opposing fields subtract.
4. **Assuming a zero net field means each field is zero.** Cancellation can produce zero net field.
5. **Assuming a larger charge always experiences a larger force in a pair.** Mutual forces are equal in magnitude.
6. **Thinking a neutral object cannot be attracted by a charged object.** Polarization can cause attraction.
7. **Forgetting the inverse square.** A distance factor of 2 changes force and point-charge field by a factor of 4, not 2.
8. **Mixing source charge with test charge.** The source charge creates the field; the test charge experiences force.
9. **Assuming field lines are physical strings.** They are a visualization; the tangent gives field direction, and line density represents relative field strength.
10. **Using signs in a magnitude formula incorrectly.** Use absolute values for magnitude, then determine direction separately.

---

## 7. Entry-test recognition checklist

When you see an MCQ, identify its type before calculating:

- **Force ratio:** use $F\propto |q_1q_2|/r^2$.
- **Field ratio:** use $E\propto |Q|/r^2$.
- **Direction:** “away from +, toward −”; reverse force for a negative test charge.
- **Multiple charges:** draw arrows and use vector addition.
- **Zero field:** cancellation requires equal magnitudes in opposite directions.
- **Action–reaction:** mutual forces are equal and opposite.
- **Charging:** check conservation, transfer of electrons, and induced polarization.
- **Units:** charge in coulombs, distance in metres, force in newtons, field in N/C.

---

## 8. Performance test — 30 MCQs

**Suggested time:** 30 minutes.  
**Rules:** Attempt all questions before opening the answer key. Choose one best answer per question. Mark each response as **confident**, **unsure**, or **guess** in your rough work. Do not use the answer key during the timed attempt.

### Q1. Two identical conducting spheres carry charges $+6\,\mu\text{C}$ and $-2\,\mu\text{C}$. They are touched together and separated, with no charge escaping. What charge does each sphere carry?

A. $+4\,\mu\text{C}$  
B. $+2\,\mu\text{C}$  
C. $-2\,\mu\text{C}$  
D. $+8\,\mu\text{C}$

### Q2. An object becomes negatively charged by ordinary rubbing. The best explanation is that it:

A. creates extra electrons from energy  
B. gains electrons from another object  
C. gains protons from the air  
D. loses electrons

### Q3. The separation between two point charges is doubled. Their force magnitude becomes:

A. twice as large  
B. half as large  
C. one-quarter as large  
D. four times as large

### Q4. Both charge magnitudes are tripled and their separation is doubled. The new force divided by the original force is:

A. $3/2$  
B. $9/4$  
C. $9/2$  
D. $3/4$

### Q5. Two charges exert an electric force on each other. Which statement is correct?

A. The larger charge exerts the larger force  
B. The positive charge always exerts the larger force  
C. The forces have equal magnitudes and opposite directions  
D. The force on each charge has the same direction

### Q6. The electric field at a point is defined by the force on a:

A. unit negative charge  
B. positive test charge per unit charge  
C. neutral object  
D. source charge only

### Q7. The electric field points east. A proton placed there experiences force:

A. east  
B. west  
C. north  
D. zero

### Q8. The electric field points east. An electron placed there experiences force:

A. east  
B. west  
C. north  
D. zero

### Q9. At a point, the field magnitude is $200\,\text{N/C}$. A $+3\,\text{C}$ charge is placed there. The force magnitude is:

A. $200/3\,\text{N}$  
B. $203\,\text{N}$  
C. $600\,\text{N}$  
D. $600/3\,\text{N}$

### Q10. If the test charge used to measure a field is doubled, while source charges remain unchanged and the test charge does not disturb them, the measured field:

A. doubles  
B. halves  
C. remains unchanged  
D. becomes zero

### Q11. The field due to a positive point charge points:

A. toward the charge  
B. away from the charge  
C. in a circular direction around it  
D. in the direction of any negative test charge's force

### Q12. Two equal positive charges are placed at the left and right ends of a line. At the midpoint, the net electric field is:

A. zero  
B. directed left  
C. directed right  
D. infinite

### Q13. A positive charge is left of an equal-magnitude negative charge. At the midpoint between them, the net electric field points:

A. toward the positive charge  
B. toward the negative charge  
C. perpendicular to the line  
D. zero

### Q14. Two equal positive charges are separated by a fixed distance. At the midpoint, the net field is zero. Which explanation is correct?

A. Neither charge creates a field there  
B. The charges' fields have equal magnitude and opposite directions  
C. Electric fields cannot exist between positive charges  
D. The charges attract each other

### Q15. Two positive charges of unequal magnitudes are fixed on a line. A zero-field point between them is closer to:

A. the larger charge  
B. the smaller charge  
C. neither; it is always the midpoint  
D. whichever charge was placed first

### Q16. Two opposite charges of equal magnitude are separated by a distance. On the line between them, their electric fields:

A. oppose and cancel everywhere  
B. point in the same direction  
C. are both zero at the midpoint  
D. point away from each other

### Q17. If a point charge is moved from distance $r$ to $2r$, the magnitude of its field at the observation point becomes:

A. $E/2$  
B. $E/4$  
C. $2E$  
D. $4E$

### Q18. Which quantity is a vector?

A. Electric charge  
B. Coulomb constant  
C. Electric field  
D. Distance

### Q19. A neutral conducting sphere is brought near a positively charged rod without touching it. The sphere can be attracted because:

A. it immediately gains net positive charge  
B. its mobile charges redistribute  
C. its protons move freely to the far side  
D. the electric force acts only on charged objects with net charge

### Q20. A charged comb attracts small neutral paper pieces. The best explanation is:

A. every paper piece must already be negatively charged  
B. the paper is polarized by the comb's electric field  
C. gravity becomes zero near the comb  
D. charge conservation is violated

### Q21. Two point charges have opposite signs. The force between them is:

A. repulsive  
B. attractive  
C. always zero  
D. dependent only on which charge is larger

### Q22. If one charge is doubled and the separation is reduced to half, the force magnitude changes by a factor of:

A. 2  
B. 4  
C. 8  
D. 1/8

### Q23. A charge experiences a force of $0.12\,\text{N}$ in a field of $4\,\text{N/C}$. The magnitude of its charge is:

A. $0.03\,\text{C}$  
B. $0.48\,\text{C}$  
C. $3\,\text{C}$  
D. $0.33\,\text{C}$

### Q24. Two equal positive charges are at positions $-a$ and $+a$. At the midpoint, the net field is zero. The electric potential there (if considering the usual point-charge potential model) is:

A. necessarily zero  
B. positive, because scalar potentials add  
C. negative, because field is zero  
D. undefined because the field is zero

### Q25. Which statement best distinguishes electric field from electric force?

A. Field is a force that has no direction  
B. Force exists only around negative charges  
C. Field describes force per unit positive test charge; force depends on the charge placed there  
D. Field and force are always numerically equal

### Q26. A source charge is changed from $+Q$ to $-Q$ without changing its magnitude or location. At a fixed observation point, its field:

A. keeps the same direction and magnitude  
B. reverses direction but keeps the same magnitude  
C. becomes zero  
D. doubles in magnitude and reverses direction

### Q27. Three charges contribute fields at a point: $5\,\text{N/C}$ east, $5\,\text{N/C}$ west, and $2\,\text{N/C}$ north. The net field is:

A. zero  
B. $2\,\text{N/C}$ north  
C. $12\,\text{N/C}$ east  
D. $8\,\text{N/C}$ north

### Q28. Which change causes the greatest increase in Coulomb force magnitude?

A. Double one charge, keep distance fixed  
B. Double both charges, keep distance fixed  
C. Double distance, keep charges fixed  
D. Halve one charge, keep distance fixed

### Q29. A point where the net electric field is zero must be a point where:

A. all source charges are zero  
B. each individual field is zero  
C. the vector sum of all individual fields is zero  
D. electric force is infinite

### Q30. A negative test charge is released from rest in a region where the electric field is uniform and points north. Ignoring other forces, its initial acceleration is:

A. north  
B. south  
C. east  
D. zero

---

## 9. Answer key and conceptual explanations

**Finish the timed attempt before reading this section.** Each explanation identifies the central idea, not just the letter.

| Q | Answer | Explanation |
|---:|:---:|---|
| 1 | B | Total charge is $+4\,\mu\text{C}$. Identical conducting spheres share it equally, so each gets $+2\,\mu\text{C}$. |
| 2 | B | Ordinary rubbing transfers electrons; charge is conserved. |
| 3 | C | Coulomb force varies as $1/r^2$; doubling distance gives $1/4$. |
| 4 | B | Charge product scales by 9; distance squared by 4. Ratio $9/4$. |
| 5 | C | Newton's third law: equal and opposite mutual forces. |
| 6 | B | Field is force per unit positive test charge. |
| 7 | A | A proton is positive, so force follows field direction. |
| 8 | B | An electron is negative, so force opposes the field. |
| 9 | C | $F=|q|E=3\times200=600\,\text{N}$. |
| 10 | C | The field is set by source charges, not the measuring test charge. |
| 11 | B | Field direction is defined away from a positive source. |
| 12 | A | Equal fields point in opposite directions and cancel. |
| 13 | B | Between + and −, the field points away from + and toward −; both directions agree. |
| 14 | B | Net zero can result from cancellation of nonzero fields. |
| 15 | B | To balance a stronger charge's field, the point must be farther from the stronger charge and therefore closer to the weaker one. |
| 16 | B | Between opposite charges, the field points from + toward − for both contributions. |
| 17 | B | Inverse-square scaling: $E'=E/2^2=E/4$. |
| 18 | C | Electric field has magnitude and direction; charge, constant, and distance are scalars. |
| 19 | B | Mobile charges redistribute in a conductor, creating induced charge separation and attraction. |
| 20 | B | Polarization shifts bound charge distributions; the nearer opposite-charge region can attract more strongly. |
| 21 | B | Unlike charges attract. |
| 22 | C | Doubling charge gives factor 2; halving distance gives factor 4. Total factor 8. |
| 23 | A | $|q|=F/E=0.12/4=0.03\,\text{C}$. |
| 24 | B | Electric potential is scalar and the two positive contributions add; zero field does not imply zero potential. |
| 25 | C | Field characterizes the location; force depends on the charge placed in it. |
| 26 | B | Same source magnitude and distance mean same field magnitude, but reversing charge sign reverses field direction. |
| 27 | B | East and west contributions cancel; the north contribution remains. |
| 28 | B | Doubling both charges multiplies their product by four. Option A gives only a factor of two; C decreases force; D halves it. |
| 29 | C | Zero net field means the vector sum vanishes, not necessarily each contribution. |
| 30 | B | A negative charge's force and acceleration are opposite the northward field. |

---

## 10. Score interpretation and error analysis

### Score bands

- **27–30 correct:** Strong command. Review any guessed answers and explain why the distractors are wrong.
- **23–26 correct:** Good foundation. Identify whether errors came from vectors, signs, or scaling.
- **18–22 correct:** Developing. Revisit field versus force and superposition, then retry missed questions.
- **Below 18:** Rebuild the conceptual model and worked examples before repeating the timed test.

These are study-guidance bands, not official NUST or FAST cutoffs.

### Error log

For every wrong or guessed answer, record:

| Field | What to write |
|---|---|
| Question | Q number and topic |
| Error type | Concept / direction / formula / unit / arithmetic / rushed reading |
| Why I chose it | Your original reasoning |
| Correct principle | One sentence in your own words |
| Retry | Solve again without looking at the key |

### Diagnosing patterns

- **Sign/direction errors:** Redraw arrows and explicitly state whether the charge is positive or negative.
- **Scaling errors:** Write a ratio before substituting numbers.
- **Superposition errors:** Draw every vector separately before adding.
- **Charge-transfer errors:** Track electrons and conserve total charge.
- **Calculation errors:** Recheck powers of ten, microcoulomb conversion, and squared distance.
- **Lucky correct answers:** Treat guesses as review items even if the selected option is correct.

### Revision loop

1. Take the test in 30 minutes without notes.
2. Mark each answer correct/incorrect and confident/unsure/guess.
3. Review every incorrect and guessed item.
4. Explain the concept aloud in simple language.
5. Retry missed items after a break, without seeing the key.
6. Revisit the full test the next day and compare performance.

## 11. One-page formula recap

$

F=k\frac{|q_1q_2|}{r^2}
\qquad
E=k\frac{|Q|}{r^2}
\qquad
\vec F=q\vec E

$

$

\vec E_{\text{net}}=\sum_i\vec E_i
\qquad
q=ne

$

- Coulomb force: along the line joining the two charges.
- Field of + charge: outward; field of − charge: inward.
- Force on + test charge: along the field.
- Force on − test charge: opposite the field.
- Like charges repel; unlike charges attract.
- Force pair: equal magnitude, opposite directions.
- Distance factor $b$: force/point-charge field scales by $1/b^2$.
- Add fields as vectors; add charge and potential as signed scalars.
- Net field zero means the vector contributions cancel.

## Session completion checklist

- [ ] I can explain the charge–field–force relationship without reading.
- [ ] I can solve inverse-square ratio questions quickly.
- [ ] I can draw field directions for positive and negative charges.
- [ ] I can explain why a neutral object can be attracted.
- [ ] I attempted all 30 MCQs under timed conditions.
- [ ] I recorded every wrong and guessed answer in my error log.
- [ ] I know which subtopic to revise next.

**Next recommended session:** Electric potential and potential energy, followed by conductors, electrostatic equilibrium, and capacitor fundamentals as required by the target test syllabus.
