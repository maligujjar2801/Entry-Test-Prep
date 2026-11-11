# Mathematics Session 4 — Worked Examples and Proofs

This companion file collects the detailed calculations and proof patterns used in Session 4. Each example explains what is being found and why the next step is valid.

---

# A. Function fundamentals and domain

## Example 1 — A relation that is not a function

Consider:

$$
R=\{(1,2),(2,3),(1,4),(3,5)\}
$$

The input 1 occurs with two different outputs, 2 and 4. That violates the exactly-one-output requirement.

**Conclusion:** This relation is not a function from its displayed inputs.

By contrast, $\{(1,5),(2,5),(3,7)\}$ is a function: every input has one output. The repeated output 5 does not violate the function definition.

## Example 2 — Full circle versus semicircle

Given:

$$
x^2+y^2=16
$$

Solve for $y$:

$$
y^2=16-x^2
$$

$$
y=\pm\sqrt{16-x^2}
$$

For an interior x-value such as $x=0$, there are two outputs, $y=4$ and $y=-4$. Therefore the full circle fails the vertical-line test.

The upper semicircle is:

$$
y=\sqrt{16-x^2},\qquad -4\le x\le4
$$

It gives exactly one y-value for each allowed x-value, so it is a function.

## Example 3 — Domain of a rational function

Find the domain of:

$$
f(x)=\frac{1}{x^2-9}
$$

The denominator must be nonzero:

$$
x^2-9\ne0
$$

Factor:

$$
(x-3)(x+3)\ne0
$$

Thus $x\ne3$ and $x\ne-3$:

$$
\boxed{D_f=\mathbb R\setminus\{-3,3\}}
$$

## Example 4 — Domain of a square-root function

Find the real domain of:

$$
f(x)=\sqrt{2x-6}
$$

A real square root requires a non-negative radicand:

$$
2x-6\ge0
$$

$$
2x\ge6
$$

$$
x\ge3
$$

Therefore:

$$
\boxed{D_f=[3,\infty)}
$$

The endpoint is included because $f(3)=0$.

## Example 5 — Logarithm domain

For:

$$
f(x)=\log_2(x-4)
$$

require a strictly positive argument:

$$
x-4>0
$$

$$
\boxed{D_f=(4,\infty)}
$$

Unlike a square-root radicand, the logarithm argument cannot be zero.

---

# B. Range calculations

## Example 6 — Range of a shifted quadratic

Find the range of:

$$
f(x)=(x-2)^2+3
$$

A square is never negative:

$$
(x-2)^2\ge0
$$

Therefore:

$$
(x-2)^2+3\ge3
$$

Equality occurs at $x=2$, so 3 is attained, not merely approached.

$$
\boxed{R_f=[3,\infty)}
$$

## Example 7 — Range of a rational function

Find the range of:

$$
f(x)=\frac{x+1}{x-2}
$$

Set:

$$
y=\frac{x+1}{x-2}
$$

We do this because a range question asks which y-values can be produced. We now test an arbitrary target output $y$.

Cross-multiply:

$$
y(x-2)=x+1
$$

Expand:

$$
yx-2y=x+1
$$

Collect the terms containing $x$:

$$
yx-x=2y+1
$$

Factor:

$$
x(y-1)=2y+1
$$

Solve:

$$
x=\frac{2y+1}{y-1}
$$

This input exists as a real number whenever $y\ne1$. For $y=1$, the original equation would imply $x+1=x-2$, which is impossible.

Thus:

$$
\boxed{R_f=\mathbb R\setminus\{1\}}
$$

## Example 8 — Range of a piecewise function

Let:

$$
f(x)=
\begin{cases}
x+2,&x<0,\\
x^2,&x\ge0.
\end{cases}
$$

For the first branch, $x<0$. Then $x+2$ can be any value less than 2:

$$
R_1=(-\infty,2)
$$

For the second branch, $x\ge0$. Squaring gives all non-negative values:

$$
R_2=[0,\infty)
$$

Combine the branches using a union:

$$
R_f=(-\infty,2)\cup[0,\infty)
$$

These intervals overlap and jointly cover the real line:

$$
\boxed{R_f=\mathbb R}
$$

This also explains the ambiguity flagged in final-assessment Q8: option A ($\mathbb R$) and option C ($(-\infty,2)\cup[0,\infty)$) stated the same set.

---

# C. Transformations

## Example 9 — Horizontal shift

Compare:

$$
f(x)=x^2
$$

with:

$$
g(x)=(x-5)^2
$$

The transformed graph reaches its minimum when the squared expression is zero:

$$
x-5=0\Rightarrow x=5
$$

The vertex therefore moves from $(0,0)$ to $(5,0)$.

**Conclusion:** shift right by 5 units.

Recognition rule:

$$
f(x-a)\Rightarrow\text{right by }a
$$

## Example 10 — Vertical shift

Compare:

$$
f(x)=x^2,\qquad g(x)=x^2+3
$$

Every output of $f$ is increased by 3. The vertex moves from $(0,0)$ to $(0,3)$.

**Conclusion:** shift upward by 3 units.

## Example 11 — Reflection across the x-axis

Let:

$$
f(x)=x^2,\qquad g(x)=-f(x)=-x^2
$$

Every output $y$ changes to $-y$. Thus the graph is reflected across the x-axis.

## Example 12 — Reflection across the y-axis

The transformation:

$$
g(x)=f(-x)
$$

replaces every input $x$ by $-x$. The point transformation is $(x,y)\mapsto(-x,y)$, which reflects the graph across the y-axis.

---

# D. Injectivity proofs

## Example 13 — Disprove injectivity of $x^2$ on the real numbers

Let:

$$
f(x)=x^2,\qquad D_f=\mathbb R
$$

Choose distinct inputs 2 and -2:

$$
2\ne-2
$$

But:

$$
f(2)=2^2=4
$$

$$
f(-2)=(-2)^2=4
$$

Two different inputs produce the same output.

$$
\boxed{f\text{ is not injective on }\mathbb R}
$$

One counterexample is enough to disprove injectivity.

## Example 14 — Explain why restricting the domain fixes $x^2$

On $[0,\infty)$, let $f(a)=f(b)$:

$$
a^2=b^2
$$

Factor:

$$
(a-b)(a+b)=0
$$

So either $a=b$ or $a=-b$. But $a,b\ge0$, so $a=-b$ is possible only when both are zero, which also gives $a=b$.

Therefore:

$$
\boxed{x^2\text{ is injective on }[0,\infty)}
$$

The same function is injective on $(-\infty,0]$ because it is strictly decreasing there.

## Example 15 — Injectivity of a rational function

Prove that:

$$
f(x)=\frac{x+2}{x-3},\qquad D_f=\mathbb R\setminus\{3\}
$$

is injective.

Take arbitrary $a,b$ in the domain and assume equal outputs:

$$
\frac{a+2}{a-3}=\frac{b+2}{b-3}
$$

Cross-multiply. This is valid because neither denominator is zero in the domain:

$$
(a+2)(b-3)=(b+2)(a-3)
$$

Expand:

$$
ab-3a+2b-6=ab-3b+2a-6
$$

Cancel $ab$ and $-6$:

$$
-3a+2b=-3b+2a
$$

Collect terms:

$$
5b=5a
$$

$$
a=b
$$

We started with $f(a)=f(b)$ and derived $a=b$. Therefore:

$$
\boxed{f\text{ is injective}}
$$

## Example 16 — Advanced rational injectivity proof

The function used in the advanced injectivity checkpoint was:

$$
f(x)=\frac{3x-2}{x+5},\qquad D_f=\mathbb R\setminus\{-5\}
$$

Assume:

$$
f(a)=f(b)
$$

Then:

$$
\frac{3a-2}{a+5}=\frac{3b-2}{b+5}
$$

Cross-multiply:

$$
(3a-2)(b+5)=(3b-2)(a+5)
$$

Expand both sides:

$$
3ab+15a-2b-10=3ab+15b-2a-10
$$

Cancel the matching terms:

$$
15a-2b=15b-2a
$$

Collect the $a$- and $b$-terms:

$$
17a=17b
$$

$$
\boxed{a=b}
$$

Thus the function is injective on its natural domain. The submitted proof used this complete strategy and was correct.

## Example 17 — Strict monotonicity

If $a<b$ and $f(a)<f(b)$ throughout the domain, the function is strictly increasing. A repeated output would contradict this inequality. Thus the function is injective.

Similarly, a strictly decreasing function is injective because $a<b$ always gives $f(a)>f(b)$.

## Example 18 — Composition of injective functions

Suppose $f$ and $g$ are injective and $g\circ f$ is defined.

Assume:

$$
(g\circ f)(a)=(g\circ f)(b)
$$

Then:

$$
g(f(a))=g(f(b))
$$

Since $g$ is injective:

$$
f(a)=f(b)
$$

Since $f$ is injective:

$$
a=b
$$

Therefore $g\circ f$ is injective.

---

# E. Surjectivity proofs

## Example 19 — $x^2$ is not onto the real numbers

Let:

$$
f:\mathbb R\to\mathbb R,\qquad f(x)=x^2
$$

Every real square is non-negative. Select the codomain element $y=-1$.

The equation:

$$
x^2=-1
$$

has no real solution. Therefore -1 has no preimage in the declared domain.

$$
\boxed{f\text{ is not surjective onto }\mathbb R}
$$

## Example 20 — The same rule is onto a different codomain

Now let:

$$
f:\mathbb R\to[0,\infty),\qquad f(x)=x^2
$$

Take arbitrary $y\in[0,\infty)$. Choose:

$$
x=\sqrt y
$$

This $x$ is real and belongs to $\mathbb R$. Then:

$$
f(x)=(\sqrt y)^2=y
$$

Every codomain value is reached, so this mapping is surjective. It is not injective because positive outputs have two preimages except at zero.

## Example 21 — Prove a linear function is onto

Let:

$$
f:\mathbb R\to\mathbb R,\qquad f(x)=3x-7
$$

Take arbitrary $y\in\mathbb R$ and solve:

$$
y=3x-7
$$

$$
y+7=3x
$$

$$
x=\frac{y+7}{3}
$$

This is real for every real $y$. Substituting it into the function gives $y$. Therefore:

$$
\boxed{f\text{ is surjective}}
$$

## Example 22 — $x^2+1$ and the importance of codomain

For:

$$
f(x)=x^2+1
$$

the minimum is 1, so the range is $[1,\infty)$.

- Mapping to $[1,\infty)$: onto.
- Mapping to $\mathbb R$: not onto, because 0 (and every value below 1) has no real preimage.

For the second mapping, $y=0$ is a sufficient counterexample:

$$
x^2+1=0\Rightarrow x^2=-1
$$

No real solution exists.

## Example 23 — Cubic function is onto

Let:

$$
f:\mathbb R\to\mathbb R,\qquad f(x)=x^3+4
$$

Take arbitrary $y\in\mathbb R$:

$$
y=x^3+4
$$

$$
x^3=y-4
$$

$$
x=\sqrt[3]{y-4}
$$

The cube root is real for every real $y$. Hence every real codomain value has a real preimage:

$$
\boxed{f\text{ is surjective}}
$$

## Example 24 — Reciprocal shifted rational function

Let:

$$
f(x)=\frac{1}{x+2}
$$

with domain $\mathbb R\setminus\{-2\}$ and codomain $\mathbb R\setminus\{0\}$.

Take arbitrary $y\ne0$:

$$
y=\frac{1}{x+2}
$$

$$
x+2=\frac1y
$$

$$
x=\frac1y-2
$$

This is a real input and it is never $-2$ because $1/y\ne0$. Therefore every nonzero codomain value is reached, so the mapping is onto.

---

# F. Inverse-function derivations

## Example 25 — Inverse of a linear function

Find the inverse of:

$$
f(x)=3x-7
$$

Write $y=3x-7$, then swap x and y:

$$
x=3y-7
$$

Solve:

$$
3y=x+7
$$

$$
\boxed{f^{-1}(x)=\frac{x+7}{3}}
$$

Verification:

$$
f(f^{-1}(x))
=3\left(\frac{x+7}{3}\right)-7
=x+7-7=x
$$

The reverse composition is:

$$
f^{-1}(f(x))
=\frac{(3x-7)+7}{3}
=\frac{3x}{3}=x
$$

Both identities hold.

## Example 26 — Inverse of a rational function

Find the inverse of:

$$
f(x)=\frac{2x+3}{x-4}
$$

Start with:

$$
y=\frac{2x+3}{x-4}
$$

Swap x and y:

$$
x=\frac{2y+3}{y-4}
$$

Cross-multiply:

$$
x(y-4)=2y+3
$$

Expand:

$$
xy-4x=2y+3
$$

Collect terms containing $y$:

$$
xy-2y=4x+3
$$

Factor:

$$
y(x-2)=4x+3
$$

Solve:

$$
\boxed{f^{-1}(x)=\frac{4x+3}{x-2}}
$$

The original function's domain excludes 4. Its range excludes 2: solving $f(x)=2$ would give $2x+3=2x-8$, which is impossible. Thus:

$$
D_f=\mathbb R\setminus\{4\}
$$

$$
R_f=\mathbb R\setminus\{2\}
$$

and:

$$
D_{f^{-1}}=\mathbb R\setminus\{2\}
$$

$$
R_{f^{-1}}=\mathbb R\setminus\{4\}
$$

## Example 27 — Reference solution for the unsubmitted written challenge

The advanced inverse lesson offered the challenge:

$$
f(x)=\frac{3x-5}{2x+1},
\qquad
D_f=\mathbb R\setminus\left\{-\frac12\right\}
$$

The written attempt was not submitted, so the following is a verified reference solution, not a recorded student result.

Start:

$$
y=\frac{3x-5}{2x+1}
$$

Exchange x and y:

$$
x=\frac{3y-5}{2y+1}
$$

Cross-multiply:

$$
x(2y+1)=3y-5
$$

Expand:

$$
2xy+x=3y-5
$$

Collect y-terms:

$$
2xy-3y=-x-5
$$

Factor:

$$
y(2x-3)=-(x+5)
$$

Solve:

$$
\boxed{f^{-1}(x)=-\frac{x+5}{2x-3}
=\frac{x+5}{3-2x}}
$$

The original range excludes $3/2$. To see why, setting $f(x)=3/2$ gives:

$$
\frac{3x-5}{2x+1}=\frac32
$$

$$
2(3x-5)=3(2x+1)
$$

$$
6x-10=6x+3
$$

which is impossible. Therefore:

$$
D_{f^{-1}}=\mathbb R\setminus\left\{\frac32\right\}
$$

and the inverse range equals the original domain:

$$
R_{f^{-1}}=\mathbb R\setminus\left\{-\frac12\right\}
$$

## Example 28 — Inverse of a restricted quadratic

For:

$$
f(x)=x^2,\qquad x\in[0,\infty)
$$

write:

$$
y=x^2
$$

Exchange:

$$
x=y^2
$$

Because the inverse output must be non-negative (the original domain), choose the non-negative root:

$$
\boxed{f^{-1}(x)=\sqrt x}
$$

If the original domain were $(-\infty,0]$, the inverse would instead be $-\sqrt{x}$.

## Example 29 — Exponential and logarithmic inverses

For $f(x)=2^x$, set $y=2^x$, swap x and y to get $x=2^y$, then take logarithm base 2:

$$
y=\log_2x
$$

Therefore:

$$
\boxed{f^{-1}(x)=\log_2x,\quad x>0}
$$

The positivity condition is the original range and therefore the inverse domain.

---

# G. Proof and verification checklist

When writing an injectivity proof, explicitly show the assumed equality, every algebraic step, and the final implication $a=b$.

When writing a surjectivity proof, explicitly choose arbitrary $y$ in the codomain, solve for $x$, and verify that $x$ belongs to the domain.

When finding an inverse, do not stop after solving for a formula. State the swapped domain and range and check the composition if requested.

A complete result is not just the final formula: the domain restrictions are part of the mathematical answer.


---

# H. Original comprehensive artifact — fourteen additional worked examples

These examples preserve the original broad Session 4 practice set. They are separate from the later interactive examples above. The initial artifact's practice set was original instructional material, not represented as official NET/FAST past-paper questions.

## Original Example 1 — Function evaluation

Given:

$$
f(x)=2x^2-3x+1
$$

Find $f(-2)$ by substituting $-2$ everywhere the input $x$ appears:

$$
f(-2)=2(-2)^2-3(-2)+1
$$

Evaluate the square first:

$$
=2(4)+6+1
$$

$$
\boxed{f(-2)=15}
$$

## Original Example 2 — Domain and range of a shifted quadratic

For:

$$
f(x)=x^2+6
$$

A polynomial accepts every real input, so:

$$
D_f=\mathbb R
$$

Since $x^2\ge0$:

$$
x^2+6\ge6
$$

The minimum value 6 is attained at $x=0$:

$$
\boxed{R_f=[6,\infty)}
$$

## Original Example 3 — Rational domain

Find the domain of:

$$
f(x)=\frac{x+4}{x^2-9}
$$

The denominator must not be zero:

$$
x^2-9\ne0
$$

$$
(x-3)(x+3)\ne0
$$

Therefore:

$$
\boxed{D_f=\mathbb R\setminus\{-3,3\}}
$$

## Original Example 4 — Radical and rational restrictions together

Find the real domain of:

$$
f(x)=\frac{\sqrt{2x+6}}{x-1}
$$

The radicand must be non-negative:

$$
2x+6\ge0\Rightarrow x\ge-3
$$

The denominator must be nonzero:

$$
x\ne1
$$

Apply both restrictions:

$$
\boxed{D_f=[-3,1)\cup(1,\infty)}
$$

The endpoint $-3$ is included because the square root is defined at zero. The point 1 is excluded because it makes the denominator zero.

## Original Example 5 — Evaluate a piecewise function

Given:

$$
f(x)=
\begin{cases}
2x+1,&x<0,\\
x^2+1,&x\ge0
\end{cases}
$$

For $x=-3$, use the first branch:

$$
f(-3)=2(-3)+1=-5
$$

For $x=0$, use the second branch because its condition includes zero:

$$
f(0)=0^2+1=1
$$

For $x=2$, use the second branch:

$$
f(2)=2^2+1=5
$$

Thus:

$$
\boxed{f(-3)=-5,\quad f(0)=1,\quad f(2)=5}
$$

The key is to choose the branch using the input's condition before substituting.

## Original Example 6 — Test whether a function is odd

Given:

$$
f(x)=x^3-2x
$$

Replace $x$ by $-x$:

$$
f(-x)=(-x)^3-2(-x)
$$

$$
=-x^3+2x
$$

Factor out $-1$:

$$
f(-x)=-(x^3-2x)=-f(x)
$$

Therefore $f$ is odd. Its graph is symmetric about the origin.

## Original Example 7 — Domain of a composite function

Let:

$$
f(x)=\sqrt{x},\qquad g(x)=x^2-4
$$

Then:

$$
(f\circ g)(x)=f(g(x))=\sqrt{x^2-4}
$$

For real outputs, require:

$$
x^2-4\ge0
$$

Factor:

$$
(x-2)(x+2)\ge0
$$

The product is non-negative outside the roots:

$$
x\le-2\quad\text{or}\quad x\ge2
$$

Therefore:

$$
\boxed{D_{f\circ g}=(-\infty,-2]\cup[2,\infty)}
$$

## Original Example 8 — Inverse of a rational function

Given:

$$
f(x)=\frac{3x-2}{x+4}
$$

Set:

$$
y=\frac{3x-2}{x+4}
$$

Exchange $x$ and $y$:

$$
x=\frac{3y-2}{y+4}
$$

Cross-multiply:

$$
x(y+4)=3y-2
$$

Expand and collect the $y$-terms:

$$
xy+4x=3y-2
$$

$$
xy-3y=-4x-2
$$

Factor:

$$
y(x-3)=-4x-2
$$

Solve:

$$
\boxed{f^{-1}(x)=\frac{-4x-2}{x-3}}
$$

The original domain excludes $-4$. The original range excludes 3, since setting the original output equal to 3 leads to an impossible equation. Thus the inverse domain excludes 3 and its range excludes $-4$.

## Original Example 9 — Quadratic range by completing the square

Given:

$$
f(x)=-x^2+8x-10
$$

Complete the square:

$$
f(x)=-(x^2-8x)-10
$$

$$
=-\big((x-4)^2-16\big)-10
$$

$$
=-(x-4)^2+6
$$

Since $(x-4)^2\ge0$:

$$
-(x-4)^2\le0
$$

Therefore the maximum output is 6, attained at $x=4$:

$$
\boxed{R_f=(-\infty,6]}
$$

## Original Example 10 — Absolute-value transformation

Given:

$$
g(x)=3|x+2|-5
$$

Relative to $y=|x|$:

1. $|x+2|$ shifts the graph 2 units left.
2. Multiplication by 3 stretches it vertically by factor 3.
3. Subtracting 5 shifts it 5 units down.

The vertex is:

$$
\boxed{(-2,-5)}
$$

Since $|x+2|\ge0$:

$$
3|x+2|-5\ge-5
$$

Thus:

$$
\boxed{D_g=\mathbb R,\qquad R_g=[-5,\infty)}
$$

## Original Example 11 — Range of a rational expression in $x^2$

Given:

$$
f(x)=\frac{x^2}{x^2+1}
$$

Let $t=x^2$, so $t\ge0$:

$$
f(x)=\frac{t}{t+1}=1-\frac{1}{t+1}
$$

Because $t+1\ge1$:

$$
0\le\frac{t}{t+1}<1
$$

Zero is attained at $x=0$, but 1 is never attained. Therefore:

$$
\boxed{R_f=[0,1)}
$$

## Original Example 12 — Verify an inverse pair by composition

Let:

$$
f(x)=2x+1,\qquad g(x)=\frac{x-1}{2}
$$

Compute the first composition:

$$
f(g(x))=2\left(\frac{x-1}{2}\right)+1
$$

$$
=x-1+1=x
$$

Compute the reverse composition:

$$
g(f(x))=\frac{(2x+1)-1}{2}
$$

$$
=\frac{2x}{2}=x
$$

Both compositions return the original input, so:

$$
\boxed{g=f^{-1}}
$$

## Original Example 13 — Solve a functional equation

Suppose:

$$
f(x)+2f(-x)=3x+6
$$

Replace $x$ by $-x$:

$$
f(-x)+2f(x)=-3x+6
$$

For clarity, write the pair as:

$$
f(x)+2f(-x)=3x+6
$$

$$
2f(x)+f(-x)=-3x+6
$$

Double the first equation:

$$
2f(x)+4f(-x)=6x+12
$$

Subtract the second equation:

$$
3f(-x)=9x+6
$$

Therefore:

$$
f(-x)=3x+2
$$

Replace $x$ by $-x$ in this identity:

$$
f(x)=-3x+2
$$

Hence:

$$
\boxed{f(x)=-3x+2}
$$

## Original Example 14 — Prove $x^2$ is injective on the non-negative domain

Let:

$$
f(x)=x^2,\qquad D_f=[0,\infty)
$$

Take arbitrary $a,b\ge0$ and assume:

$$
f(a)=f(b)
$$

Then:

$$
a^2=b^2
$$

Factor:

$$
(a-b)(a+b)=0
$$

Thus $a=b$ or $a=-b$. Since both inputs are non-negative, the second possibility can hold only when both are zero, which also gives $a=b$.

Therefore:

$$
\boxed{a=b\text{ and }f\text{ is injective on }[0,\infty)}
$$

---
