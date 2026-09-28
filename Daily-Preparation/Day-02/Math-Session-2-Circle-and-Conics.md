# Mathematics Session 2 — Circle and Conic Sections

## 1. Session Objective

This session covers:

1. Circle
2. Parabola
3. Ellipse
4. Hyperbola
5. Focus and directrix
6. Eccentricity
7. Latus rectum
8. Standard equations
9. Graph recognition
10. NET / FAST recognition patterns
11. Common traps

The most important skill is not simply memorizing formulas.

You should be able to look at an equation and immediately identify:

- the conic
- its center or vertex
- orientation
- radius or semi-axes
- focus
- directrix
- eccentricity
- asymptotes where applicable

---

# PART I — CIRCLE

# 2. Definition of a Circle

A circle is the locus of all points that are at a fixed distance from a fixed point.

The fixed point is called the:

$$
\boxed{\text{center}}
$$

The fixed distance is called the:

$$
\boxed{\text{radius}}
$$

---

# 3. Derivation of the Equation of a Circle

Let the center be:

$$
(h,k)
$$

and let any point on the circle be:

$$
(x,y)
$$

The distance between these two points is the radius $$r$$.

Using the distance formula:

$$
r=
\sqrt{(x-h)^2+(y-k)^2}
$$

Square both sides:

$$
r^2=(x-h)^2+(y-k)^2
$$

Therefore:

$$
\boxed{
(x-h)^2+(y-k)^2=r^2
}
$$

This is the **standard equation of a circle**.

---

# 4. Reading the Circle Equation

Given:

$$
(x-h)^2+(y-k)^2=r^2
$$

the center is:

$$
\boxed{(h,k)}
$$

and radius:

$$
\boxed{r}
$$

### Important sign rule

If:

$$
(x-3)^2+(y+4)^2=25
$$

then:

$$
h=3
$$

and:

$$
k=-4
$$

Therefore:

$$
\boxed{\text{center}=(3,-4)}
$$

and:

$$
\boxed{r=5}
$$

The sign inside the bracket is opposite to the coordinate.

---

# 5. Circle With Center at Origin

If:

$$
h=0,\qquad k=0
$$

then:

$$
(x-0)^2+(y-0)^2=r^2
$$

so:

$$
\boxed{x^2+y^2=r^2}
$$

---

# 6. Expanded Form of a Circle

Starting from:

$$
(x-h)^2+(y-k)^2=r^2
$$

Expand:

$$
x^2-2hx+h^2+y^2-2ky+k^2=r^2
$$

Rearrange:

$$
x^2+y^2-2hx-2ky+h^2+k^2-r^2=0
$$

The general form can therefore be written:

$$
\boxed{
x^2+y^2+Dx+Ey+F=0
}
$$

where:

$$
D=-2h
$$

$$
E=-2k
$$

$$
F=h^2+k^2-r^2
$$

Therefore:

$$
\boxed{
h=-\frac D2
}
$$

$$
\boxed{
k=-\frac E2
}
$$

and:

$$
\boxed{
r=\sqrt{h^2+k^2-F}
}
$$

---

# 7. NET Circle Recognition

If you see:

$$
x^2+y^2
$$

with equal coefficients and no $$xy$$ term, immediately investigate a circle.

If the equation is:

$$
(x-h)^2+(y-k)^2=r^2
$$

you should be able to identify the center and radius almost instantly.

---

# PART II — PARABOLA

# 8. Definition of a Parabola

A parabola is the locus of a point whose distance from:

- a fixed point
- and a fixed line

is equal.

The fixed point is:

$$
\boxed{\text{focus}}
$$

The fixed line is:

$$
\boxed{\text{directrix}}
$$

Therefore, for every point $$P$$ on the parabola:

$$
\boxed{PF=PD}
$$

where $$F$$ is the focus and $$D$$ represents the perpendicular distance to the directrix.

---

# 9. Derivation of Standard Parabola

Consider a parabola opening to the right.

Let its vertex be:

$$
(0,0)
$$

Let the focus be:

$$
(a,0)
$$

and directrix:

$$
x=-a
$$

Take a general point:

$$
P(x,y)
$$

Distance from $$P$$ to the focus:

$$
PF=\sqrt{(x-a)^2+y^2}
$$

Distance from $$P$$ to the directrix $$x=-a$$:

$$
PD=x+a
$$

By definition:

$$
PF=PD
$$

Therefore:

$$
\sqrt{(x-a)^2+y^2}=x+a
$$

Square:

$$
(x-a)^2+y^2=(x+a)^2
$$

Expand:

$$
x^2-2ax+a^2+y^2=x^2+2ax+a^2
$$

Cancel:

$$
-2ax+y^2=2ax
$$

Therefore:

$$
\boxed{y^2=4ax}
$$

This is the standard equation of a parabola opening to the right.

---

# 10. Standard Parabola Equations

## Opens right

$$
\boxed{y^2=4ax}
$$

Vertex:

$$
\boxed{(0,0)}
$$

Focus:

$$
\boxed{(a,0)}
$$

Directrix:

$$
\boxed{x=-a}
$$

---

## Opens left

$$
\boxed{y^2=-4ax}
$$

Focus:

$$
\boxed{(-a,0)}
$$

Directrix:

$$
\boxed{x=a}
$$

---

## Opens upward

$$
\boxed{x^2=4ay}
$$

Focus:

$$
\boxed{(0,a)}
$$

Directrix:

$$
\boxed{y=-a}
$$

---

## Opens downward

$$
\boxed{x^2=-4ay}
$$

Focus:

$$
\boxed{(0,-a)}
$$

Directrix:

$$
\boxed{y=a}
$$

---

# 11. Parabola With a Shifted Vertex

If the vertex is:

$$
(h,k)
$$

then:

### Horizontal parabola

$$
\boxed{(y-k)^2=4a(x-h)}
$$

Focus:

$$
\boxed{(h+a,k)}
$$

Directrix:

$$
\boxed{x=h-a}
$$

---

### Vertical parabola

$$
\boxed{(x-h)^2=4a(y-k)}
$$

Focus:

$$
\boxed{(h,k+a)}
$$

Directrix:

$$
\boxed{y=k-a}
$$

---

# 12. Latus Rectum of a Parabola

The latus rectum is the chord passing through the focus and perpendicular to the axis.

For:

$
y^2=4ax
$

the focus is $(a,0)$. At the focus, $x=a$, so:

$
y^2=4a^2
$

$
y=\pm2a
$

Therefore the endpoints are:

$
(a,2a),\qquad(a,-2a)
$

and its length is:

$
2a-(-2a)=4a.
$

For the standard right-opening form, $a>0$, so:

$
\boxed{\text{latus rectum length}=4a}
$

More generally, if a signed parameter is used for the left/down-opening forms, the geometric length is:

$
\boxed{4|a|}
$

The endpoints are:

$$
\boxed{(a,2a)}
$$

and:

$$
\boxed{(a,-2a)}
$$

because at the focus:

$$
x=a
$$

Substitute:

$$
y^2=4a(a)
$$

$$
y^2=4a^2
$$

$$
y=\pm2a
$$

Therefore the length is:

$$
2a-(-2a)=4a
$$

---

# 13. Parabola Recognition Trick

Look at which variable is squared.

### $$y^2$$

If:

$$
y^2=4ax
$$

the parabola opens horizontally.

### $$x^2$$

If:

$$
x^2=4ay
$$

the parabola opens vertically.

The sign tells the direction.

---

# PART III — ELLIPSE

# 14. Definition of an Ellipse

An ellipse is the locus of a point for which the **sum of its distances from two fixed points** is constant.

The two fixed points are called:

$$
\boxed{\text{foci}}
$$

---

# 15. Standard Ellipse Equation

For an ellipse centered at the origin with its major axis along the x-axis:

$$
\boxed{
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
}
$$

For the conventional notation:

$$
\boxed{a>b>0}
$$

Here $$a$$ represents the semi-major axis.

---

# 16. Why Is $$a>b$$?

For:

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$$

the x-intercepts occur when:

$$
y=0
$$

so:

$$
\frac{x^2}{a^2}=1
$$

$$
x=\pm a
$$

The y-intercepts occur when:

$$
x=0
$$

giving:

$$
y=\pm b
$$

Therefore:

- horizontal semi-axis = $$a$$
- vertical semi-axis = $$b$$

If the major axis is horizontal, then:

$$
\boxed{a>b}
$$

---

# 17. Vertical Ellipse

If the major axis is vertical:

$$
\boxed{
\frac{x^2}{b^2}+\frac{y^2}{a^2}=1
}
$$

with:

$$
\boxed{a>b}
$$

Again, $$a$$ is the semi-major axis.

---

# 18. Center and Vertices

For:

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$$

center:

$$
\boxed{(0,0)}
$$

Horizontal vertices:

$$
\boxed{(\pm a,0)}
$$

Co-vertices:

$$
\boxed{(0,\pm b)}
$$

---

# 19. Shifted Ellipse

For a horizontal major axis:

$$
\boxed{
\frac{(x-h)^2}{a^2}
+
\frac{(y-k)^2}{b^2}
=1
}
$$

where:

$$
a>b
$$

Center:

$$
\boxed{(h,k)}
$$

Vertices:

$$
\boxed{(h\pm a,k)}
$$

Co-vertices:

$$
\boxed{(h,k\pm b)}
$$

---

# 20. Focus of an Ellipse

For an ellipse:

$$
\boxed{
c^2=a^2-b^2
}
$$

where $$c$$ is the distance from the center to either focus.

For a horizontal ellipse:

$$
\boxed{\text{foci}=(h\pm c,k)}
$$

For a vertical ellipse:

$$
\boxed{\text{foci}=(h,k\pm c)}
$$

---

# 21. Eccentricity of an Ellipse

Eccentricity is:

$$
\boxed{e=\frac ca}
$$

Since:

$$
c^2=a^2-b^2
$$

and:

$$
c<a
$$

we get:

$$
\boxed{0<e<1}
$$

This is a very important recognition fact.

---

# 22. Deriving the Ellipse Focus Relation

For the horizontal ellipse:

$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$

take the point $P=(0,b)$ and the foci

$
F_1=(-c,0),\\qquad F_2=(c,0).
$

The two distances are equal:

$
PF_1=PF_2=\sqrt{c^2+b^2}.
$

By the defining property of an ellipse, their sum is $2a$:

$
2\sqrt{c^2+b^2}=2a.
$

Therefore:

$
\sqrt{c^2+b^2}=a
$

Squaring:

$
c^2+b^2=a^2.
$

Hence:

$
\boxed{c^2=a^2-b^2}
$

and:

$
\boxed{c=\sqrt{a^2-b^2}}.
$

For a vertical ellipse, the same relation holds; only the foci rotate to the vertical axis.

### Example

Given:

$$
\frac{x^2}{25}+\frac{y^2}{9}=1
$$

we identify:

$$
a^2=25
$$

$$
b^2=9
$$

Therefore:

$$
a=5,\qquad b=3
$$

Now:

$$
c^2=25-9
$$

$$
c^2=16
$$

$$
c=4
$$

So the foci are:

$$
\boxed{(\pm4,0)}
$$

---

# 23. Latus Rectum of an Ellipse

For an ellipse, the length of the latus rectum is:

$$
\boxed{\frac{2b^2}{a}}
$$

This is a common formula-based entry-test question.

---

# PART IV — HYPERBOLA

# 24. Definition of a Hyperbola

A hyperbola is the locus of a point for which the **absolute difference of its distances from two fixed points** is constant.

The fixed points are the foci.

Thus:

$$
\boxed{|PF_1-PF_2|=\text{constant}}
$$

---

# 25. Standard Horizontal Hyperbola

The standard equation is:

$$
\boxed{
\frac{x^2}{a^2}
-
\frac{y^2}{b^2}
=1
}
$$

The positive term is associated with the direction in which the hyperbola opens.

Therefore this hyperbola opens:

$$
\boxed{\text{left and right}}
$$

---

# 26. Center and Vertices

For:

$$
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1
$$

center:

$$
\boxed{(0,0)}
$$

vertices:

$$
\boxed{(\pm a,0)}
$$

---

# 27. Vertical Hyperbola

The equation:

$$
\boxed{
\frac{y^2}{a^2}
-
\frac{x^2}{b^2}
=1
}
$$

opens:

$$
\boxed{\text{upward and downward}}
$$

Vertices:

$$
\boxed{(0,\pm a)}
$$

---

# 28. Focus of a Hyperbola

For a horizontal hyperbola, the foci are:

$
F_1=(-c,0),\\qquad F_2=(c,0).
$

The defining property is that the absolute difference of the distances from the two foci is constant:

$
|PF_1-PF_2|=2a.
$

For the standard hyperbola, this leads to the equation:

$
\frac{x^2}{a^2}-\frac{y^2}{c^2-a^2}=1.
$

Comparing this with:

$
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1,
$

we obtain:

$
b^2=c^2-a^2
$

and therefore:

$
\boxed{c^2=a^2+b^2}.
$

So the foci are:

$
\boxed{(\pm c,0)}
$

for a horizontal hyperbola, and:

$
\boxed{(0,\pm c)}
$

for a vertical hyperbola.

Notice the critical difference:

### Ellipse

$$
\boxed{c^2=a^2-b^2}
$$

### Hyperbola

$$
\boxed{c^2=a^2+b^2}
$$

This is one of the most important conic traps.

---

# 29. Eccentricity of a Hyperbola

$$
\boxed{e=\frac ca}
$$

Since:

$$
c^2=a^2+b^2
$$

we have:

$$
c>a
$$

Therefore:

$$
\boxed{e>1}
$$

---

# 30. Asymptotes of a Hyperbola

For:

$$
\frac{x^2}{a^2}
-
\frac{y^2}{b^2}
=1
$$

the asymptotes are:

$$
\boxed{
y=\pm\frac ba x
}
$$

These lines guide the shape of the hyperbola.

---

# 31. Derivation of Hyperbola Asymptotes

Starting with:

$$
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1
$$

Far from the center, the constant $$1$$ becomes relatively insignificant compared with the large squared terms.

So approximately:

$$
\frac{x^2}{a^2}-\frac{y^2}{b^2}\approx0
$$

Therefore:

$$
\frac{x^2}{a^2}\approx\frac{y^2}{b^2}
$$

Taking square roots:

$$
\frac{x}{a}\approx\pm\frac{y}{b}
$$

Thus:

$$
\boxed{y=\pm\frac ba x}
$$

---

# 32. Shifted Hyperbola

Horizontal:

$$
\boxed{
\frac{(x-h)^2}{a^2}
-
\frac{(y-k)^2}{b^2}
=1
}
$$

Center:

$$
\boxed{(h,k)}
$$

Asymptotes:

$$
\boxed{
y-k=\pm\frac ba(x-h)
}
$$

Vertical:

$$
\boxed{
\frac{(y-k)^2}{a^2}
-
\frac{(x-h)^2}{b^2}
=1
}
$$

Asymptotes:

$$
\boxed{
y-k=\pm\frac ab(x-h)
}
$$

---

# 33. Latus Rectum of a Hyperbola

For the standard horizontal hyperbola, the latus rectum is the chord through a focus perpendicular to the transverse axis.

Its length is:

$
\boxed{\frac{2b^2}{a}}
$

The same length formula applies to the standard vertical hyperbola, with the orientation rotated by $90^\circ$.

Notice that this has the same algebraic form as the ellipse's latus rectum.

---

# 34. The Most Important Conic Comparison

| Property | Parabola | Ellipse | Hyperbola |
|---|---|---|---|
| Definition | Equal distance | Sum of distances | Difference of distances |
| Eccentricity | $$e=1$$ | $$0<e<1$$ | $$e>1$$ |
| Standard relation | — | $$c^2=a^2-b^2$$ | $$c^2=a^2+b^2$$ |
| Asymptotes | No | No | Yes |
| Closed curve? | No | Yes | No |
| Number of branches | 1 | 1 | 2 |

---

# 35. Conic Recognition by Equation

These are **standard-form recognition rules**. For a general second-degree equation, do not classify it from signs alone until you have simplified or transformed it appropriately.

### Circle

$
\boxed{x^2+y^2=r^2}
$

In standard Cartesian form, the $x^2$ and $y^2$ terms have equal positive coefficients and there is no $xy$ term.

---

### Parabola

Only **one variable is squared** in the standard axis-aligned form:

$
\boxed{y^2=4ax}
$

or:

$
\boxed{x^2=4ay}.
$

---

### Ellipse

Both variables are squared and the terms are **added**:

$
\boxed{
\frac{x^2}{a^2}+
\frac{y^2}{b^2}=1
}
$

A circle is the special case where the two squared terms have equal scale.

---

### Hyperbola

Both variables are squared but the terms have **opposite signs**:

$
\boxed{
\frac{x^2}{a^2}-
\frac{y^2}{b^2}=1.
}
$

For rotated or fully general conics, additional analysis may be required.

---

# 36. High-Speed NET Recognition

For the common axis-aligned standard forms:

$
x^2+y^2=\text{constant}>0
\quad\Rightarrow\quad
\boxed{\text{Circle}}
$

If exactly one variable is squared:

$
x^2=\text{linear expression in }y
\quad\text{or}\quad
y^2=\text{linear expression in }x
$

think:

$
\boxed{\text{Parabola}}.
$

If both squared terms are added with positive coefficients, think:

$
\boxed{\text{Ellipse}}
$

(with the circle as the equal-scale special case).

If both squared terms have opposite signs, think:

$
\boxed{\text{Hyperbola}}.
$

---

# 37. Major Axis vs Minor Axis — Critical Clarification

For an ellipse, we conventionally define:

$$
\boxed{a>b}
$$

where $$a$$ is the semi-major axis.

For example:

$$
\frac{x^2}{25}+\frac{y^2}{9}=1
$$

Here:

$$
a=5,\qquad b=3
$$

because:

$$
25>9
$$

However, **do not blindly apply $$a>b$$ to hyperbolas in the same way**.

For:

$$
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1
$$

$$a$$ and $$b$$ have specific roles in the hyperbola formula, and the key relation is:

$$
\boxed{c^2=a^2+b^2}
$$

The earlier confusion between ellipse notation and hyperbola notation is therefore a notation/teaching issue, not a reason to assume the hyperbola behaves like an ellipse.

---

# 38. Worked Example — Circle

Find the center and radius:

$$
(x-4)^2+(y+2)^2=36
$$

Compare with:

$$
(x-h)^2+(y-k)^2=r^2
$$

Therefore:

$$
h=4
$$

$$
k=-2
$$

and:

$$
r^2=36
$$

so:

$$
r=6
$$

Answer:

$$
\boxed{\text{Center}=(4,-2)}
$$

$$
\boxed{r=6}
$$

---

# 39. Worked Example — Parabola

Given:

$$
y^2=12x
$$

Compare with:

$$
y^2=4ax
$$

Therefore:

$$
4a=12
$$

$$
a=3
$$

Focus:

$$
\boxed{(3,0)}
$$

Directrix:

$$
\boxed{x=-3}
$$

Latus rectum:

$$
4a=12
$$

Therefore:

$$
\boxed{\text{Latus rectum}=12}
$$

---

# 40. Worked Example — Ellipse

Given:

$$
\frac{x^2}{36}+\frac{y^2}{16}=1
$$

Therefore:

$$
a^2=36
$$

$$
b^2=16
$$

so:

$$
a=6,\qquad b=4
$$

Find $$c$$:

$$
c^2=a^2-b^2
$$

$$
c^2=36-16
$$

$$
c^2=20
$$

$$
c=2\sqrt5
$$

Therefore foci:

$$
\boxed{(\pm2\sqrt5,0)}
$$

Eccentricity:

$$
e=\frac ca
$$

$$
e=\frac{2\sqrt5}{6}
$$

$$
\boxed{e=\frac{\sqrt5}{3}}
$$

---

# 41. Worked Example — Hyperbola

Given:

$$
\frac{x^2}{25}-\frac{y^2}{9}=1
$$

Therefore:

$$
a=5
$$

$$
b=3
$$

Find $$c$$:

$$
c^2=a^2+b^2
$$

$$
c^2=25+9
$$

$$
c^2=34
$$

$$
c=\sqrt{34}
$$

Foci:

$$
\boxed{(\pm\sqrt{34},0)}
$$

Eccentricity:

$$
\boxed{e=\frac{\sqrt{34}}5}
$$

Asymptotes:

$$
y=\pm\frac ba x
$$

Therefore:

$$
\boxed{
y=\pm\frac35x
}
$$

---

# 42. Conic Formula Master Sheet

## Circle

$$
\boxed{(x-h)^2+(y-k)^2=r^2}
$$

Center:

$$
\boxed{(h,k)}
$$

Radius:

$
\boxed{r}
$

---

## Parabola

$$
\boxed{(y-k)^2=4a(x-h)}
$$

Focus:

$$
\boxed{(h+a,k)}
$$

Directrix:

$$
\boxed{x=h-a}
$$

Latus rectum:

$$
\boxed{4a}
$$

---

$$
\boxed{(x-h)^2=4a(y-k)}
$$

Focus:

$$
\boxed{(h,k+a)}
$$

Directrix:

$$
\boxed{y=k-a}
$$

---

## Ellipse

$$
\boxed{
\frac{(x-h)^2}{a^2}
+
\frac{(y-k)^2}{b^2}=1
}
$$

with conventional:

$$
\boxed{a>b}
$$

Focus relation:

$$
\boxed{c^2=a^2-b^2}
$$

Eccentricity:

$$
\boxed{e=\frac ca<1}
$$

Latus rectum:

$$
\boxed{\frac{2b^2}{a}}
$$

---

## Hyperbola

$$
\boxed{
\frac{(x-h)^2}{a^2}
-
\frac{(y-k)^2}{b^2}=1
}
$$

Focus relation:

$$
\boxed{c^2=a^2+b^2}
$$

Eccentricity:

$$
\boxed{e=\frac ca>1}
$$

Asymptotes:

$$
\boxed{
y-k=\pm\frac ba(x-h)
}
$$

Latus rectum:

$$
\boxed{\frac{2b^2}{a}}
$$

---

# 43. Critical Memory Rules

### Circle

$$
\boxed{\text{radius}^2=\text{RHS}}
$$

---

### Parabola

$$
\boxed{4a\text{ appears in the equation}}
$$

Don't confuse $$a$$ with $$4a$$.

If:

$$
y^2=20x
$$

then:

$$
4a=20
$$

not:

$$
a=20
$$

Therefore:

$$
a=5
$$

---

### Ellipse

$$
\boxed{c^2=a^2-b^2}
$$

---

### Hyperbola

$$
\boxed{c^2=a^2+b^2}
$$

---

### Eccentricity

$$
\boxed{
e=1\text{ parabola}
}
$$

$$
\boxed{
e<1\text{ ellipse}
}
$$

$$
\boxed{
e>1\text{ hyperbola}
}
$$

---

# 44. Session 2 Error Analysis

## Q2 — Circle

The issue was a genuine radius/form extraction mistake.

### Correct approach

Always compare directly with:

$$
(x-h)^2+(y-k)^2=r^2
$$

Then extract:

$$
r=\sqrt{\text{RHS}}
$$

Do not accidentally use $$r^2$$ as $$r$$.

---

## Q3 — Defective MCQ

The question had two valid answers.

Therefore this should **not** be treated as a mathematical weakness.

When a question appears to have multiple mathematically valid choices:

1. substitute each candidate
2. verify the equation
3. check whether the question itself is defective

Never force yourself to choose an answer merely because the test expects one.

---

## Q24 — Ellipse / Hyperbola Notation

The confusion came from applying the ellipse convention:

$$
a>b
$$

too broadly.

For ellipse notation:

$$
\boxed{a>b}
$$

is the conventional definition of the semi-major axis.

For hyperbolas, focus on:

$$
\boxed{c^2=a^2+b^2}
$$

and on which term is positive to determine the opening direction.

---

# 45. Final Session 2 Checklist

You should now be able to answer questions involving:

- Circle center
- Circle radius
- Circle expanded equation
- Completing the square
- Parabola orientation
- Parabola vertex
- Parabola focus
- Parabola directrix
- Parabola latus rectum
- Ellipse center
- Ellipse major/minor axes
- Ellipse vertices
- Ellipse foci
- Ellipse eccentricity
- Ellipse latus rectum
- Hyperbola center
- Hyperbola vertices
- Hyperbola foci
- Hyperbola eccentricity
- Hyperbola asymptotes
- Hyperbola latus rectum
- Conic identification from equations

---

# Session 2 Performance Record

### Timed Test

- Questions: **25**
- Time: **23 minutes**

### Recorded issues

- Q2 — circle radius/form extraction error
- Q3 — defective MCQ with two valid answers
- Q24 — notation/teaching clarification involving ellipse $$a>b$$ versus hyperbola notation

### Revision priority

1. Circle equation → center/radius extraction
2. Parabola $$4a$$ interpretation
3. Ellipse $$c^2=a^2-b^2$$
4. Hyperbola $$c^2=a^2+b^2$$
5. Asymptote recognition
6. Fast conic identification
