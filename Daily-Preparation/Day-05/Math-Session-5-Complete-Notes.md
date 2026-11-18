# Mathematics Session 5 — Graph Transformations and Scaling

> **Admission-test track:** NUST NET + FAST/NUCES  
> **Session:** 5  
> **Prerequisite:** Session 4 — Functions, Domain/Range, Injectivity, Surjectivity, and Inverses  
> **Primary goal:** Build reliable graph intuition for translations, reflections, vertical/horizontal scaling, and combined transformations.

## Why this session comes next

Session 4's final assessment was 22/25 (88%). Its two transformation questions were both missed: a horizontal translation was confused with a vertical shift, and a reflection across the x-axis was confused with an upward shift. The progress record also identifies scaling as introduced but not fully reinforced or assessed.

This session therefore concentrates on transformations rather than restarting functions, domain/range, or inverse functions.

## Learning outcomes

By the end, you should be able to:

1. Read a transformed function from its algebraic form.
2. Map a point on the parent graph to its new position.
3. Distinguish horizontal changes (inside the input) from vertical changes (outside the function).
4. Explain why horizontal scaling uses a reciprocal factor.
5. Determine the vertex, domain, range, and opening direction of common transformed graphs.
6. Decode expressions containing multiple transformations in the correct order.
7. Solve entry-test questions without relying on memorized sign rules alone.

---

## Phase 1 — Start with the parent graph

A parent function is the simple base graph before transformations.

| Parent function | Equation | Useful feature |
|---|---|---|
| Linear | \(f(x)=x\) | Straight line through origin |
| Quadratic | \(f(x)=x^2\) | Vertex at \((0,0)\), opens upward |
| Absolute value | \(f(x)=|x|\) | V-shape, vertex at \((0,0)\) |
| Square root | \(f(x)=\sqrt{x}\) | Starts at \((0,0)\), domain \(x\ge0\) |
| Reciprocal | \(f(x)=1/x\) | Asymptotes are the coordinate axes |

A transformation changes the position, orientation, or scale of the graph. It does not randomly change every point: there is a consistent mapping from old coordinates to new coordinates.

### The point-mapping idea

If \((x,y)\) lies on \(y=f(x)\), then:

- \(y=f(x)+k\) maps \((x,y)\) to \((x,y+k)\).
- \(y=f(x-h)\) maps \((x,y)\) to \((x+h,y)\).
- \(y=-f(x)\) maps \((x,y)\) to \((x,-y)\).
- \(y=f(-x)\) maps \((x,y)\) to \((-x,y)\).

This coordinate view is the safest way to understand signs.

---

## Phase 2 — Vertical translations

For:

\[
g(x)=f(x)+k
\]

every output is increased by \(k\). The x-coordinate stays unchanged.

- \(k>0\): shift upward by \(k\).
- \(k<0\): shift downward by \(|k|\).

### Example

Start with \(f(x)=x^2\). Let:

\[
g(x)=x^2+4
\]

The parent vertex \((0,0)\) becomes \((0,4)\). The graph moves up 4 units.

**Recognition:** a number added or subtracted outside the function changes the y-coordinate.

---

## Phase 3 — Horizontal translations

For:

\[
g(x)=f(x-h)
\]

the graph shifts right by \(h\) when \(h>0\). For:

\[
g(x)=f(x+h)
\]

the graph shifts left by \(h\).

The sign feels reversed because the input must reach the old input value. To get the old value \(x=0\), the expression \(x-5\) requires the new coordinate \(x=5\).

### Example

\[
g(x)=(x-3)^2
\]

The minimum occurs when \(x-3=0\), so \(x=3\). The vertex is \((3,0)\): three units right.

### Never rely on sign memorization alone

Set the inner expression equal to zero (or to the old key input) to locate the new horizontal position.

---

## Phase 4 — Reflections

### Reflection across the x-axis

\[
g(x)=-f(x)
\]

Every y-coordinate changes sign:

\[
(x,y)\longrightarrow(x,-y)
\]

Example: \(y=x^2\) becomes \(y=-x^2\), a downward-opening parabola.

### Reflection across the y-axis

\[
g(x)=f(-x)
\]

Every x-coordinate changes sign:

\[
(x,y)\longrightarrow(-x,y)
\]

Example: \(y=(x+2)^2\) is the reflection of \(y=(x-2)^2\) across the y-axis.

### Important distinction

- Negative sign **outside** the function: x-axis reflection.
- Negative sign **inside** the input**:** y-axis reflection.

A reflection is not a translation. It changes orientation or left/right placement, not simply the graph's distance from an axis.

---

## Phase 5 — Vertical scaling

For:

\[
g(x)=a f(x)
\]

the x-coordinate stays the same, while every y-coordinate is multiplied by \(a\):

\[
(x,y)\longrightarrow(x,ay)
\]

- \(|a|>1\): vertical stretch by factor \(|a|\).
- \(0<|a|<1\): vertical compression by factor \(|a|\).
- \(a<0\): also reflect across the x-axis.
- \(a=0\): the graph collapses to \(y=0\), so this is not an ordinary nonzero scaling.

### Example

\[
g(x)=3x^2
\]

A parent point \((2,4)\) becomes \((2,12)\). The graph is three times as tall at each x-coordinate; it is vertically stretched by 3.

### Visual checkpoint

For the parent parabola \(y=x^2\), compare:

\[
y=3x^2,\qquad y=\frac13x^2
\]

The first is narrower/steeper; the second is wider/flatter. The vertex stays at the origin.

---

## Phase 6 — Horizontal scaling (the reciprocal rule)

For:

\[
g(x)=f(ax),\qquad a\ne0
\]

the input is multiplied by \(a\). A parent point \((x,y)\) moves to:

\[
\left(\frac{x}{a},y\right)
\]

Therefore:

- \(|a|>1\): horizontal compression by factor \(1/|a|\).
- \(0<|a|<1\): horizontal stretch by factor \(1/|a|\).
- \(a<0\): also reflect across the y-axis.

### Why is the factor reciprocal?

Suppose the parent graph has a key point at input \(x=4\). In \(g(x)=f(2x)\), the same output occurs when:

\[
2x=4\Rightarrow x=2
\]

The point moves from x-coordinate 4 to x-coordinate 2. The graph is compressed horizontally by \(1/2\), not stretched by 2.

### Example

\[
g(x)=f(3x)
\]

Every old x-coordinate is divided by 3. A point \((6,5)\) becomes \((2,5)\).

---

## Phase 7 — Combined transformations

Consider:

\[
g(x)=-2f(x-3)+4
\]

Starting from a parent point \((x,y)\), the final mapping is:

\[
\boxed{(x,y)\longrightarrow(x+3,-2y+4)}
\]

Interpret each part:

1. \(x-3\): shift right 3.
2. Multiply by \(-2\): reflect across x-axis and vertically stretch by 2.
3. \(+4\): shift up 4.

For \(f(x)=x^2\):

\[
g(x)=-2(x-3)^2+4
\]

The vertex is \((3,4)\), and the parabola opens downward.

### A reliable order for reading an expression

For \(g(x)=a f(b(x-h))+k\):

1. Horizontal shift: \(h\) (right if \(h>0\)).
2. Horizontal scaling/reflection from \(b\): x-coordinates are divided by \(b\) relative to the shifted center.
3. Vertical scaling/reflection from \(a\).
4. Vertical shift by \(k\).

A direct point-mapping formula is often safer than applying transformations mentally in a rushed order. For a parent point \((u,v)\) on \(y=f(x)\), where \(a,b\ne0\):

\[
\boxed{(u,v)\longrightarrow\left(h+\frac{u}{b},\ av+k\right)}
\]

This formula applies to \(g(x)=a f(b(x-h))+k\).

---

## Phase 8 — Domain and range effects

Transformations can change the domain and range.

### Vertical changes

For \(g(x)=af(x)+k\), with \(a\ne0\):

- Domain stays the same.
- Range values \(y\) become \(ay+k\).

### Horizontal changes

For \(g(x)=f(bx)\), with \(b\ne0\):

- Range stays the same.
- Domain values \(x\) are divided by \(b\), with the interval endpoints reordered if \(b<0\).

### Example: square-root graph

Parent:

\[
f(x)=\sqrt{x},\quad D_f=[0,\infty),\quad R_f=[0,\infty)
\]

Transformed:

\[
g(x)=\sqrt{x-2}+3
\]

Require \(x-2\ge0\), so:

\[
D_g=[2,\infty),\qquad R_g=[3,\infty)
\]

The graph starts at \((2,3)\).

---

## Phase 9 — Quadratic vertex form

A quadratic in vertex form is:

\[
y=a(x-h)^2+k
\]

Its vertex is \((h,k)\).

- \(a>0\): opens upward.
- \(a<0\): opens downward.
- \(|a|>1\): vertically stretched.
- \(0<|a|<1\): vertically compressed.

If \(a>0\), the range is \([k,\infty)\). If \(a<0\), the range is \((-\infty,k]\). The domain is all real numbers.

### Example

\[
y=-\frac12(x+4)^2+6
\]

Vertex: \((-4,6)\). It opens downward and is vertically compressed by factor \(1/2\). Domain: \(\mathbb R\). Range: \((-\infty,6]\).

---

## Phase 10 — Entry-test recognition strategy

When a transformation question appears:

1. Identify the parent function.
2. Find the change inside the input.
3. Find the multiplier outside the function.
4. Find the constant outside the function.
5. If signs are confusing, map one or two known points.
6. For quadratics, read the vertex and opening direction.
7. Check domain and range if asked.

### Common traps

| Expression | Correct interpretation |
|---|---|
| \(f(x-5)\) | Right 5 |
| \(f(x+5)\) | Left 5 |
| \(f(x)+5\) | Up 5 |
| \(f(x)-5\) | Down 5 |
| \(-f(x)\) | Reflect across x-axis |
| \(f(-x)\) | Reflect across y-axis |
| \(3f(x)\) | Vertical stretch by 3 |
| \(f(3x)\) | Horizontal compression by \(1/3\) |
| \(\frac12 f(x)\) | Vertical compression by \(1/2\) |
| \(f(x/2)\) | Horizontal stretch by 2 |

---

## Guided worked examples

### Example 1 — Identify a translation

\[
g(x)=|x+4|-2
\]

From \(y=|x|\), shift left 4 and down 2. Vertex: \((-4,-2)\). Range: \([-2,\infty)\).

### Example 2 — Identify reflection and scaling

\[
g(x)=-3\sqrt{x}
\]

Reflect the square-root graph across the x-axis and stretch vertically by 3. Domain: \([0,\infty)\). Range: \((-\infty,0]\).

### Example 3 — Horizontal scaling

\[
g(x)=\sqrt{4x}
\]

Require \(4x\ge0\), so the domain remains \([0,\infty)\). Relative to \(f(x)=\sqrt{x}\), the graph is horizontally compressed by \(1/4\).

### Example 4 — Combined quadratic

\[
g(x)=2(x-1)^2-8
\]

Vertex: \((1,-8)\). Opens upward. Vertical stretch by 2. Domain: \(\mathbb R\). Range: \([-8,\infty)\).

### Example 5 — Point mapping

A point \((4,-2)\) lies on \(y=f(x)\). Find its image on:

\[
y=-2f(x-3)+5
\]

Use \((x,y)\mapsto(x+3,-2y+5)\):

\[
(4,-2)\mapsto(7,9)
\]

---

## Practice before the final test

For each expression, state the transformations and (where possible) the vertex or starting point:

1. \(g(x)=(x-2)^2+3\)
2. \(g(x)=-|x+1|\)
3. \(g(x)=\frac14 f(x)\)
4. \(g(x)=f(2x)\)
5. \(g(x)=3f(x+2)-1\)

Do not look at the answer key in the companion assessment file until after attempting the questions.

## Completion standard

Do not mark scaling as mastered just by memorizing the table. You should be able to explain the point mapping, especially why \(f(2x)\) compresses horizontally by \(1/2\), and correctly decode a combined transformation.

Next: complete the 25-question timed assessment, then submit your answers and reasoning for error analysis.
