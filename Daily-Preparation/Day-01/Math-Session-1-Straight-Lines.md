# Math Session 1 — Straight Lines

> **Admission-test track:** NUST NET + FAST/NUCES  
> **Study method:** Concept → Recognition → Derivation → Worked Examples → MCQ Practice → Timed Test → Error Analysis

## 1. Coordinate Plane

A point is written as \(P(x,y)\).

- \(x\): horizontal coordinate, measured from the \(y\)-axis.
- \(y\): vertical coordinate, measured from the \(x\)-axis.

The axes divide the plane into four quadrants:

| Quadrant | Sign of \(x\) | Sign of \(y\) |
|---|---:|---:|
| I | + | + |
| II | − | + |
| III | − | − |
| IV | + | − |

**Entry-test recognition:** before using a formula, identify whether the question gives coordinates, slopes, intercepts, or an equation.

---

## 2. Distance Between Two Points

Let

\[
P_1(x_1,y_1),\qquad P_2(x_2,y_2).
\]

Draw a right triangle using the horizontal and vertical differences.

The horizontal side is

\[
\Delta x=x_2-x_1
\]

and the vertical side is

\[
\Delta y=y_2-y_1.
\]

By Pythagoras,

\[
d^2=(\Delta x)^2+(\Delta y)^2.
\]

Therefore,

\[
\boxed{d=\sqrt{(x_2-x_1)^2+(y_2-y_1)^2}}.
\]

The order of the points does not matter because the differences are squared.

### Example

Find the distance between \(A(2,3)\) and \(B(8,11)\).

\[
d=\sqrt{(8-2)^2+(11-3)^2}
\]

\[
=\sqrt{6^2+8^2}
=\sqrt{36+64}
=\boxed{10}.
\]

**NET/FAST trap:** do not calculate \(x_2-x_1\) and \(y_2-y_1\) as ordinary positive distances and then forget the square-root step.

---

## 3. Slope of a Straight Line

Slope measures how rapidly \(y\) changes as \(x\) changes.

For two points \(P_1(x_1,y_1)\) and \(P_2(x_2,y_2)\),

\[
\boxed{m=\frac{y_2-y_1}{x_2-x_1}}
\]

provided \(x_2\ne x_1\).

The numerator is the **rise** and the denominator is the **run**:

\[
m=\frac{\text{rise}}{\text{run}}.
\]

### Meaning of the sign

- \(m>0\): line rises from left to right.
- \(m<0\): line falls from left to right.
- \(m=0\): horizontal line.
- Undefined slope: vertical line.

### Example

For \(A(1,2)\) and \(B(5,10)\),

\[
m=\frac{10-2}{5-1}
=\frac84
=\boxed{2}.
\]

---

## 4. Why a Vertical Line Has Undefined Slope

For a vertical line,

\[
x_2=x_1.
\]

Therefore,

\[
m=\frac{y_2-y_1}{x_2-x_1}
=\frac{\text{nonzero}}{0}.
\]

Division by zero is undefined.

So a vertical line has **undefined slope**.

For a horizontal line,

\[
y_2=y_1,
\]

hence

\[
m=\frac0{x_2-x_1}=0.
\]

---

## 5. Equation of a Straight Line

A straight line can be represented in several equivalent forms. Entry tests often give the information in one form and ask you to produce another.

### 5.1 Slope-Intercept Form

\[
\boxed{y=mx+c}
\]

where:

- \(m\) = slope
- \(c\) = \(y\)-intercept

### Derivation

Suppose a line has slope \(m\) and crosses the \(y\)-axis at \((0,c)\).

For an arbitrary point \((x,y)\) on the line,

\[
m=\frac{y-c}{x-0}.
\]

Thus,

\[
m=\frac{y-c}{x}.
\]

Multiply by \(x\):

\[
mx=y-c.
\]

Therefore,

\[
\boxed{y=mx+c}.
\]

### Recognition

If the equation is already

\[
y=3x-7,
\]

then immediately:

\[
m=3,\qquad c=-7.
\]

---

## 6. Point-Slope Form

If you know:

- one point \((x_1,y_1)\), and
- the slope \(m\),

use

\[
\boxed{y-y_1=m(x-x_1)}.
\]

### Derivation

Start with the slope formula between the known point and an arbitrary point:

\[
m=\frac{y-y_1}{x-x_1}.
\]

Multiply by \(x-x_1\):

\[
\boxed{y-y_1=m(x-x_1)}.
\]

### Example

Find the equation of the line with slope \(4\) through \((2,-3)\).

\[
y-(-3)=4(x-2)
\]

\[
y+3=4x-8
\]

\[
\boxed{y=4x-11}.
\]

---

## 7. Two-Point Form

If two points are given, first calculate the slope:

\[
m=\frac{y_2-y_1}{x_2-x_1}.
\]

Then substitute into point-slope form:

\[
\boxed{
y-y_1=
\frac{y_2-y_1}{x_2-x_1}(x-x_1)
}.
\]

### Example

Find the equation through \((1,2)\) and \((5,10)\).

First,

\[
m=\frac{10-2}{5-1}=2.
\]

Using \((1,2)\),

\[
y-2=2(x-1).
\]

Hence,

\[
\boxed{y=2x}.
\]

---

## 8. General Form

The general equation is

\[
\boxed{Ax+By+C=0}.
\]

If \(B\ne0\), solve for \(y\):

\[
By=-Ax-C
\]

\[
y=-\frac ABx-\frac CB.
\]

Comparing with

\[
y=mx+c,
\]

we obtain

\[
\boxed{m=-\frac AB}.
\]

### Example

Find the slope of

\[
3x+2y-8=0.
\]

Here,

\[
A=3,\qquad B=2.
\]

Therefore,

\[
m=-\frac32.
\]

---

## 9. Horizontal and Vertical Lines

### Horizontal line

A horizontal line has constant \(y\):

\[
\boxed{y=k}.
\]

Its slope is

\[
\boxed{m=0}.
\]

### Vertical line

A vertical line has constant \(x\):

\[
\boxed{x=k}.
\]

Its slope is undefined.

**Fast recognition:**

- \(x=5\) → vertical
- \(y=-2\) → horizontal

---

## 10. Parallel Lines

Two non-vertical lines are parallel when their slopes are equal:

\[
\boxed{m_1=m_2}.
\]

Example:

\[
y=2x+5,\qquad y=2x-9
\]

have the same slope \(2\), so they are parallel.

---

## 11. Perpendicular Lines

For non-vertical lines,

\[
\boxed{m_1m_2=-1}.
\]

Therefore,

\[
m_2=-\frac1{m_1}.
\]

### Example

If

\[
m_1=3,
\]

the perpendicular slope is

\[
m_2=-\frac13.
\]

**Trap:** perpendicular does not mean the slopes simply have opposite signs. They must be negative reciprocals.

---

## 12. Intercepts

### \(x\)-intercept

At the \(x\)-axis,

\[
y=0.
\]

### \(y\)-intercept

At the \(y\)-axis,

\[
x=0.
\]

### Example

For

\[
2x+3y=6,
\]

the \(x\)-intercept is found from \(y=0\):

\[
2x=6\Rightarrow x=3.
\]

So the point is

\[
(3,0).
\]

The \(y\)-intercept is found from \(x=0\):

\[
3y=6\Rightarrow y=2.
\]

So the point is

\[
(0,2).
\]

---

## 13. Intercept Form

If a line has:

- \(x\)-intercept \(a\)
- \(y\)-intercept \(b\)

then

\[
\boxed{\frac xa+\frac yb=1}.
\]

### Derivation

The line passes through

\[
(a,0),\qquad(0,b).
\]

Using the two-point form,

\[
y=
\frac{b-0}{0-a}(x-a).
\]

Thus,

\[
y=-\frac ba(x-a)
\]

\[
ay=-bx+ab.
\]

Therefore,

\[
\boxed{bx+ay=ab}.
\]

Divide by \(ab\):

\[
\boxed{\frac xa+\frac yb=1}.
\]

---

## 14. NET/FAST Recognition Patterns

| Given information | First tool to use |
|---|---|
| Two points | Distance or slope formula |
| One point + slope | Point-slope form |
| Two points + line equation | Two-point form |
| \(y=mx+c\) | Read slope/intercept directly |
| \(Ax+By+C=0\) | \(m=-A/B\) |
| Parallel line | Same slope |
| Perpendicular line | Negative reciprocal |
| \(x=k\) | Vertical |
| \(y=k\) | Horizontal |
| Intercepts | Put \(x=0\) or \(y=0\) |

---

## 15. Worked Entry-Test Examples

### Example 1 — Distance

Find the distance between \((-2,1)\) and \((4,9)\).

\[
d=\sqrt{(4+2)^2+(9-1)^2}
\]

\[
=\sqrt{36+64}
=\boxed{10}.
\]

### Example 2 — Perpendicular line

Find the line through \((2,1)\) perpendicular to

\[
y=2x+5.
\]

Original slope:

\[
m_1=2.
\]

Perpendicular slope:

\[
m_2=-\frac12.
\]

Point-slope form:

\[
y-1=-\frac12(x-2).
\]

So

\[
\boxed{y=-\frac12x+2}.
\]

### Example 3 — General form

Find the slope and intercepts of

\[
4x-2y+8=0.
\]

Rearrange:

\[
-2y=-4x-8
\]

\[
y=2x+4.
\]

Therefore,

\[
\boxed{m=2,\quad y\text{-intercept}=4}.
\]

For the \(x\)-intercept:

\[
0=2x+4
\]

\[
\boxed{x=-2}.
\]

---

## 16. Common Traps

1. Forgetting the square root in the distance formula.
2. Reversing only one difference in the slope formula.
3. Calling a vertical slope zero. It is **undefined**.
4. Using \(m_1=m_2\) for perpendicular lines. That is the parallel condition.
5. Forgetting that \(x=constant\) is vertical.
6. Confusing the \(x\)-intercept with the \(y\)-intercept.
7. Reading \(m=-A/B\) incorrectly from \(Ax+By+C=0\).

---

## 17. Session Performance Record

### Practice

- Straight Lines MCQ practice: **11/12**
- Time: **5:33**
- Accuracy: **91.7%**

### Timed Mini-Test

- Score: **10/10**
- Time: **4:43**
- Accuracy: **100%**

### Interpretation

The timed performance showed strong command of the core straight-line techniques. Continue emphasizing recognition speed and careful algebra rather than simply increasing difficulty without purpose.

---

## 18. Revision Checklist

Before moving on, you should be able to:

- derive the distance formula;
- calculate slope from two points;
- identify horizontal/vertical lines;
- convert between line forms;
- find parallel and perpendicular slopes;
- calculate intercepts;
- derive and use intercept form;
- recognize the shortest method for a NET/FAST question.

