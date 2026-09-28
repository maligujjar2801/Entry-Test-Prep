# Math Session 2 — Circle and Conics

> **Admission-test track:** NUST NET + FAST/NUCES  
> **Study method:** Concept → Recognition → Derivation → Worked Examples → MCQ Practice → Timed Test → Error Analysis

## 1. What Are Conic Sections?

A conic section is a curve obtained from the intersection of a plane with a double cone.

The four basic non-degenerate conics are:

1. Circle
2. Parabola
3. Ellipse
4. Hyperbola

For entry tests, the most important skill is recognizing the equation and extracting its geometric information quickly.

---

# Part I — Circle

## 2. Definition of a Circle

A circle is the set of all points whose distance from a fixed point is constant.

- Fixed point = **centre**
- Constant distance = **radius**

Let the centre be

\[
C(h,k)
\]

and an arbitrary point on the circle be

\[
P(x,y).
\]

The radius is

\[
CP=r.
\]

Using the distance formula,

\[
r=\sqrt{(x-h)^2+(y-k)^2}.
\]

Squaring,

\[
\boxed{(x-h)^2+(y-k)^2=r^2}.
\]

This is the standard equation of a circle.

### Fast recognition

\[
(x-h)^2+(y-k)^2=r^2
\]

immediately gives

\[
\boxed{\text{Centre}=(h,k),\quad \text{Radius}=r}.
\]

---

## 3. Circle in Expanded Form

Start with

\[
(x-h)^2+(y-k)^2=r^2.
\]

Expand:

\[
x^2-2hx+h^2+y^2-2ky+k^2=r^2.
\]

Therefore,

\[
x^2+y^2-2hx-2ky+(h^2+k^2-r^2)=0.
\]

A general circle can be written as

\[
\boxed{x^2+y^2+Dx+Ey+F=0}.
\]

Comparing coefficients,

\[
\boxed{h=-\frac D2,\qquad k=-\frac E2}
\]

and

\[
\boxed{r=\sqrt{\frac{D^2+E^2}{4}-F}}.
\]

---

## 4. Completing the Square

Example:

\[
x^2+y^2-6x+4y-3=0.
\]

Group terms:

\[
(x^2-6x)+(y^2+4y)=3.
\]

Complete squares:

\[
(x-3)^2-9+(y+2)^2-4=3.
\]

Hence,

\[
(x-3)^2+(y+2)^2=16.
\]

Therefore,

\[
\boxed{C=(3,-2),\quad r=4}.
\]

---

# Part II — Parabola

## 5. Definition

A parabola is the set of points that are equally distant from:

- a fixed point called the **focus**, and
- a fixed line called the **directrix**.

This definition is extremely important because it explains the standard equation.

---

## 6. Derivation of \(y^2=4ax\)

Take the focus as

\[
F(a,0)
\]

and the directrix as

\[
x=-a.
\]

Let

\[
P(x,y)
\]

be any point on the parabola.

### Distance from \(P\) to the focus

\[
PF=\sqrt{(x-a)^2+y^2}.
\]

### Distance from \(P\) to the directrix

The directrix is \(x=-a\), so

\[
PD=x+a.
\]

By the definition of a parabola,

\[
PF=PD.
\]

Therefore,

\[
\sqrt{(x-a)^2+y^2}=x+a.
\]

Square both sides:

\[
(x-a)^2+y^2=(x+a)^2.
\]

Expand:

\[
x^2-2ax+a^2+y^2=x^2+2ax+a^2.
\]

Cancel common terms:

\[
y^2=4ax.
\]

Thus,

\[
\boxed{y^2=4ax}.
\]

---

## 7. Parts of \(y^2=4ax\)

For

\[
y^2=4ax,
\]

we have:

- Vertex: \(\boxed{(0,0)}\)
- Focus: \(\boxed{(a,0)}\)
- Directrix: \(\boxed{x=-a}\)
- Axis: \(x\)-axis
- Opens right if \(a>0\)
- Opens left if \(a<0\)

The length of the latus rectum is

\[
\boxed{4|a|}.
\]

---

## 8. Other Standard Parabola Forms

### Opens left/right

\[
\boxed{(y-k)^2=4a(x-h)}
\]

Vertex:

\[
\boxed{(h,k)}
\]

Focus:

\[
\boxed{(h+a,k)}
\]

Directrix:

\[
\boxed{x=h-a}.
\]

### Opens up/down

\[
\boxed{(x-h)^2=4a(y-k)}
\]

Vertex:

\[
\boxed{(h,k)}
\]

Focus:

\[
\boxed{(h,k+a)}
\]

Directrix:

\[
\boxed{y=k-a}.
\]

**Recognition:** the squared variable tells you the direction.

- \(y^2\) → opens horizontally.
- \(x^2\) → opens vertically.

---

# Part III — Ellipse

## 9. Definition

An ellipse is the set of points for which the **sum of the distances from two fixed points** is constant.

The two fixed points are the **foci**.

---

## 10. Standard Horizontal Ellipse

The standard equation is

\[
\boxed{
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
}
\]

with the conventional notation

\[
\boxed{a>b>0}.
\]

For a horizontal major axis:

- Centre: \((0,0)\)
- Vertices: \((\pm a,0)\)
- Co-vertices: \((0,\pm b)\)
- Foci: \((\pm c,0)\)

The relationship is

\[
\boxed{c^2=a^2-b^2}.
\]

---

## 11. Why \(c^2=a^2-b^2\)?

For an ellipse, the semi-major axis, semi-minor axis, and focal distance satisfy

\[
a^2=b^2+c^2.
\]

Rearranging gives

\[
\boxed{c^2=a^2-b^2}.
\]

The eccentricity is

\[
\boxed{e=\frac ca}.
\]

For an ellipse,

\[
\boxed{0<e<1}.
\]

---

## 12. Vertical Ellipse

If

\[
\boxed{
\frac{x^2}{b^2}+\frac{y^2}{a^2}=1
}
\]

then the major axis is vertical.

The foci are

\[
(0,\pm c)
\]

where

\[
c^2=a^2-b^2.
\]

### Shifted ellipse

Horizontal:

\[
\boxed{
\frac{(x-h)^2}{a^2}+
\frac{(y-k)^2}{b^2}=1
}
\]

Centre:

\[
\boxed{(h,k)}.
\]

---

## 13. Latus Rectum of an Ellipse

The length of the latus rectum is

\[
\boxed{\frac{2b^2}{a}}.
\]

This is a useful formula for direct MCQs.

---

# Part IV — Hyperbola

## 14. Definition

A hyperbola is the set of points for which the **absolute difference of the distances from two fixed points** is constant.

The fixed points are the foci.

The defining difference distinguishes a hyperbola from an ellipse.

---

## 15. Standard Horizontal Hyperbola

The standard equation is

\[
\boxed{
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1
}.
\]

For a horizontal hyperbola:

- Centre: \((0,0)\)
- Vertices: \((\pm a,0)\)
- Foci: \((\pm c,0)\)

The focal relationship is

\[
\boxed{c^2=a^2+b^2}.
\]

The eccentricity is

\[
\boxed{e=\frac ca}.
\]

Since \(c>a\),

\[
\boxed{e>1}.
\]

---

## 16. Vertical Hyperbola

\[
\boxed{
\frac{y^2}{a^2}-\frac{x^2}{b^2}=1
}.
\]

The transverse axis is vertical and the foci are

\[
(0,\pm c).
\]

Again,

\[
\boxed{c^2=a^2+b^2}.
\]

---

## 17. Asymptotes of a Hyperbola

For

\[
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1,
\]

replace the right side by zero to obtain the asymptotic equation:

\[
\frac{x^2}{a^2}-\frac{y^2}{b^2}=0.
\]

Therefore,

\[
\frac{x^2}{a^2}=\frac{y^2}{b^2}.
\]

Taking square roots,

\[
\frac xa=\pm\frac yb.
\]

Hence,

\[
\boxed{y=\pm\frac ba x}.
\]

For a shifted hyperbola,

\[
\boxed{
\frac{(x-h)^2}{a^2}
-\frac{(y-k)^2}{b^2}=1
}
\]

the asymptotes are

\[
\boxed{
y-k=\pm\frac ba(x-h)
}.
\]

---

## 18. Latus Rectum of a Hyperbola

The length is

\[
\boxed{\frac{2b^2}{a}}.
\]

---

# Part V — Conic Recognition

## 19. The Fastest Recognition Table

| Conic | Standard equation | Key relationship |
|---|---|---|
| Circle | \((x-h)^2+(y-k)^2=r^2\) | radius \(r\) |
| Parabola | \(y^2=4ax\) or \(x^2=4ay\) | focus/directrix |
| Ellipse | \(x^2/a^2+y^2/b^2=1\) | \(c^2=a^2-b^2\) |
| Hyperbola | \(x^2/a^2-y^2/b^2=1\) | \(c^2=a^2+b^2\) |

### The sign test

- Both squared terms **positive and equal scale** → often circle.
- Both squared terms **positive but different denominators** → ellipse.
- Squared terms with **opposite signs** → hyperbola.
- Only **one variable squared** → parabola.

---

# 20. The Important \(a>b\) Clarification

A major source of confusion is the statement

\[
a>b.
\]

For an ellipse, \(a\) conventionally denotes the semi-major axis, so

\[
\boxed{a>b}.
\]

For a hyperbola, do **not** blindly apply the ellipse rule.

In

\[
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1,
\]

\(a\) is associated with the transverse direction and \(b\) with the conjugate direction. The key relationship is

\[
\boxed{c^2=a^2+b^2},
\]

not \(a>b\).

Therefore, when solving an entry-test question, use the definitions and formula appropriate to the conic rather than importing the ellipse convention into the hyperbola.

---

# 21. Worked Examples

## Example 1 — Circle

Find the centre and radius:

\[
(x-4)^2+(y+2)^2=25.
\]

Compare with

\[
(x-h)^2+(y-k)^2=r^2.
\]

Thus,

\[
h=4,\qquad k=-2,\qquad r=5.
\]

Answer:

\[
\boxed{C=(4,-2),\quad r=5}.
\]

---

## Example 2 — Parabola

For

\[
y^2=12x,
\]

compare with

\[
y^2=4ax.
\]

Thus,

\[
4a=12
\]

so

\[
a=3.
\]

Therefore:

\[
\boxed{\text{Vertex}=(0,0)}
\]

\[
\boxed{\text{Focus}=(3,0)}
\]

\[
\boxed{\text{Directrix}:x=-3}.
\]

---

## Example 3 — Ellipse

Given

\[
\frac{x^2}{25}+\frac{y^2}{9}=1,
\]

we identify

\[
a^2=25,\qquad b^2=9.
\]

Thus,

\[
a=5,\qquad b=3.
\]

Find \(c\):

\[
c^2=a^2-b^2
\]

\[
=25-9=16.
\]

Hence,

\[
c=4.
\]

The foci are

\[
\boxed{(\pm4,0)}.
\]

Eccentricity:

\[
e=\frac45.
\]

---

## Example 4 — Hyperbola

Given

\[
\frac{x^2}{16}-\frac{y^2}{9}=1,
\]

we have

\[
a=4,\qquad b=3.
\]

Then

\[
c^2=a^2+b^2
\]

\[
=16+9=25.
\]

So

\[
c=5.
\]

Foci:

\[
\boxed{(\pm5,0)}.
\]

Asymptotes:

\[
y=\pm\frac34x.
\]

Eccentricity:

\[
e=\frac54.
\]

---

# 22. Entry-Test Recognition Workflow

When you see a conic equation:

### Step 1 — Look at the squared terms

Are there two squared variables or only one?

### Step 2 — Look at the signs

\[
+\,+ \quad\Rightarrow\quad \text{circle/ellipse}
\]

\[
+\,- \quad\Rightarrow\quad \text{hyperbola}
\]

one squared variable → parabola.

### Step 3 — Match the standard form

Do not start calculating until the equation has been matched.

### Step 4 — Extract only what is asked

For example:

- centre?
- radius?
- focus?
- directrix?
- eccentricity?
- asymptotes?
- vertices?

### Step 5 — Apply the correct relation

Ellipse:

\[
c^2=a^2-b^2.
\]

Hyperbola:

\[
c^2=a^2+b^2.
\]

---

# 23. Common Traps

1. Reading the centre signs incorrectly.
   - \((x-h)^2\) → centre \(x=h\)
   - \((y-k)^2\) → centre \(y=k\)

2. Confusing ellipse and hyperbola focal formulas.

3. Assuming \(a>b\) is a universal rule for every conic.

4. Forgetting that \(y^2=4ax\) opens horizontally.

5. Forgetting that \(x^2=4ay\) opens vertically.

6. Using the wrong sign for the parabola directrix.

7. Forgetting the square root when finding \(c\).

8. For hyperbola asymptotes, forgetting the \(\pm\).

---

# 24. Session 2 Test Record

- MCQs attempted: **25**
- Time: **23 minutes**

### Recorded issues

**Q2 — Circle:** a genuine radius/form extraction error.  
**Correction:** first rewrite the equation in standard circle form before reading \(r\).

**Q3 — Defective question:** the question allowed two valid answers.  
**Lesson:** do not treat a flawed MCQ as evidence of a conceptual weakness.

**Q24 — Hyperbola/ellipse notation:** confusion arose from applying the ellipse convention \(a>b\) too broadly.  
**Correction:** for hyperbolas, prioritize

\[
c^2=a^2+b^2
\]

and the equation's transverse/conjugate directions.

---

# 25. Master Formula Sheet

## Circle

\[
\boxed{(x-h)^2+(y-k)^2=r^2}
\]

\[
\boxed{C=(h,k)}
\]

\[
\boxed{r=r}
\]

## Parabola

\[
\boxed{y^2=4ax}
\]

\[
\boxed{F=(a,0)}
\]

\[
\boxed{x=-a}
\]

\[
\boxed{x^2=4ay}
\]

\[
\boxed{F=(0,a)}
\]

\[
\boxed{y=-a}
\]

## Ellipse

\[
\boxed{\frac{x^2}{a^2}+\frac{y^2}{b^2}=1}
\]

\[
\boxed{c^2=a^2-b^2}
\]

\[
\boxed{e=\frac ca<1}
\]

\[
\boxed{\text{Latus rectum}=\frac{2b^2}{a}}
\]

## Hyperbola

\[
\boxed{\frac{x^2}{a^2}-\frac{y^2}{b^2}=1}
\]

\[
\boxed{c^2=a^2+b^2}
\]

\[
\boxed{e=\frac ca>1}
\]

\[
\boxed{y=\pm\frac ba x}
\]

\[
\boxed{\text{Latus rectum}=\frac{2b^2}{a}}
\]

---

# 26. Final Revision Checklist

Before treating this session as secure, you should be able to:

- derive the circle equation from the distance formula;
- convert an expanded circle into standard form;
- derive \(y^2=4ax\) from the focus/directrix definition;
- identify parabola vertex, focus and directrix;
- distinguish horizontal and vertical parabolas;
- identify ellipse centre, axes and foci;
- use \(c^2=a^2-b^2\);
- identify hyperbola centre, vertices and foci;
- use \(c^2=a^2+b^2\);
- derive hyperbola asymptotes;
- distinguish ellipse notation from hyperbola notation;
- recognize a conic quickly from its equation.

