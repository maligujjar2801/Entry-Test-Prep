# Mathematics Session 4 — Complete Conceptual Notes

> **Admission-test track:** NUST NET + FAST/NUCES  
> **Session theme:** Functions and their properties  
> **Teaching sequence:** Concept → Formal model → Reasoning → Worked examples → Entry-test recognition → Practice

## How to use these notes

Do not memorize a rule before understanding what it is protecting you from. In function questions, always identify the domain and codomain first. Then decide whether the question is asking about the function property, injectivity, surjectivity, bijectivity, or an inverse.

---

# Phase I — Function Fundamentals

## 1. What is a function?

A function is a rule that assigns **exactly one output** to every input in its domain.

If a function maps a set \(A\) to a set \(B\), we write:

$$
f:A\to B
$$

The defining condition is:

$$
\boxed{\forall x\in A,\ \exists! y\in B\text{ such that }y=f(x)}
$$

The symbol \(\exists!\) means “there exists exactly one.”

### The conceptual model

Imagine the domain as a collection of input values and the codomain as the permitted output collection. Every valid input must be assigned one output. An input cannot be left without an output, and it cannot be assigned two different outputs.

However, **two different inputs are allowed to share the same output**. That situation is still a function; it simply may not be injective.

Example:

$$
f(1)=5,\qquad f(2)=5
$$

This is a valid function assignment. The inputs 1 and 2 both map to 5.

By contrast:

$$
R=\{(1,2),(2,3),(1,4),(3,5)\}
$$

is not a function because input 1 has two different outputs, 2 and 4.

## 2. Relation versus function

A relation is any set of ordered pairs. A function is a special kind of relation in which each input occurs with exactly one output.

- A repeated first coordinate paired with two different second coordinates violates the function rule.
- A repeated second coordinate is allowed.
- An input that never appears in the relation is a problem if it belongs to the declared domain, because every domain element must receive an output.

## 3. Function notation

In \(y=f(x)\):

- \(x\) is the input or independent variable.
- \(f(x)\) is the output corresponding to input \(x\).
- The expression \(f(3)\) means evaluate the function at \(x=3\).

The notation \(f:A\to B\) also states the declared domain and codomain. These are part of the function's definition, not optional labels.

## 4. Vertical-line test

A graph represents a function of \(x\) only if every vertical line intersects the graph at most once.

Why? A vertical line fixes one input \(x\). If it intersects the graph twice at different heights, that one input has two different outputs.

Example: the full circle

$$
x^2+y^2=16
$$

is not a function of \(x\), because for many \(x\)-values it has both a positive and a negative \(y\)-value. The upper semicircle

$$
y=\sqrt{16-x^2},\qquad -4\le x\le4
$$

does define a function of \(x\).

**Do not confuse the tests:** the vertical-line test checks whether a graph is a function; the horizontal-line test checks whether a function is injective.

## 5. Domain, codomain, and range

For \(f:A\to B\):

- **Domain \(A\):** all permitted inputs.
- **Codomain \(B\):** the declared set in which outputs are required to lie.
- **Range:** the outputs the function actually produces.

Always:

$$
\boxed{\operatorname{Range}(f)\subseteq\operatorname{Codomain}(f)}
$$

The range can equal the codomain, but it cannot contain values outside it.

This distinction becomes crucial when deciding whether a function is surjective. Surjectivity depends on the declared codomain.

---

# Phase II — Domain and Range

## 6. Domain: what inputs are allowed?

The domain is the set of every input for which the rule is mathematically defined within the specified number system, usually the real numbers in this session.

### 6.1 Polynomial functions

Every real number can be substituted into a polynomial.

$$
f(x)=x^3-4x^2+7x-1
\quad\Longrightarrow\quad
D_f=\mathbb R
$$

### 6.2 Rational functions

A denominator cannot equal zero.

$$
f(x)=\frac{1}{x^2-9}
$$

Require:

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

### 6.3 Real square-root functions

The expression inside a real square root must be non-negative.

$$
f(x)=\sqrt{2x-6}
$$

Require:

$$
2x-6\ge0
\Rightarrow x\ge3
$$

Therefore:

$$
\boxed{D_f=[3,\infty)}
$$

The endpoint 3 is included because the square root of zero exists.

### 6.4 Logarithmic functions

For a real logarithm:

$$
\log_a(g(x))
$$

the argument must be strictly positive:

$$
g(x)>0
$$

The base must also satisfy:

$$
a>0,\qquad a\ne1
$$

The argument cannot equal zero. Unlike a square-root radicand, a logarithm's argument does not allow zero.

## 7. Interval notation

- \((a,b)\): endpoints excluded.
- \([a,b]\): endpoints included.
- \([a,b)\): include \(a\), exclude \(b\).
- \((a,b]\): exclude \(a\), include \(b\).
- \([a,\infty)\): include \(a\), extend without an upper bound.

Infinity is never an included endpoint, so it always uses a parenthesis.

## 8. Range: what outputs can actually occur?

The range is determined by the outputs the function can produce from its domain.

### 8.1 Quadratic functions

The parent quadratic:

$$
f(x)=x^2
$$

has minimum value 0, so:

$$
\boxed{R_f=[0,\infty)}
$$

A translated quadratic:

$$
f(x)=(x-2)^2+3
$$

has minimum value 3, attained at \(x=2\):

$$
\boxed{R_f=[3,\infty)}
$$

The vertex tells us the boundary value for a parabola opening upward or downward.

### 8.2 Rational range using algebra

Consider:

$$
f(x)=\frac{x+1}{x-2}
$$

Set the output equal to an arbitrary real value \(y\):

$$
y=\frac{x+1}{x-2}
$$

Solve for \(x\):

$$
y(x-2)=x+1
$$

$$
yx-2y=x+1
$$

$$
x(y-1)=2y+1
$$

$$
x=\frac{2y+1}{y-1}
$$

This expression gives a real \(x\) for every real \(y\) except \(y=1\), where the denominator becomes zero. At \(y=1\), the original equation would require \(x+1=x-2\), which is impossible.

Therefore:

$$
\boxed{R_f=\mathbb R\setminus\{1\}}
$$

**Why this method works:** a number belongs to the range exactly when there is an allowed input that produces it. Solving for \(x\) tests whether such an input exists.

### 8.3 Exponential and logarithmic ranges

For the real exponential function:

$$
f(x)=2^x
$$

the output is always positive and can approach zero without reaching it:

$$
\boxed{R_f=(0,\infty)}
$$

For:

$$
f(x)=\log_2x
$$

the domain is \((0,\infty)\), and the range is all real numbers:

$$
\boxed{R_f=\mathbb R}
$$

### 8.4 Absolute-value functions

The parent function:

$$
f(x)=|x|
$$

has minimum output zero:

$$
R_f=[0,\infty)
$$

A vertical shift:

$$
f(x)=|x|+k
$$

has range \([k,\infty)\). A downward reflection such as \(-|x|\) has range \((-\infty,0]\).

### 8.5 Piecewise functions

For a piecewise function, determine the range of each branch under that branch's own domain restriction, then take the union.

For example:

$$
f(x)=
\begin{cases}
x+2,&x<0,\\
x^2,&x\ge0.
\end{cases}
$$

First branch: as \(x<0\), \(x+2\) produces \((-\infty,2)\).

Second branch: as \(x\ge0\), \(x^2\) produces \([0,\infty)\).

Therefore:

$$
R_f=(-\infty,2)\cup[0,\infty)=\mathbb R
$$

The union notation is useful because it shows the output set of each branch. Here the intervals overlap, so together they cover every real number.

---

# Phase III — Function Transformations

## 9. Parent functions and transformed graphs

A parent function is a basic graph used as the starting point. A transformation changes its position, orientation, or scale.

The session taught horizontal and vertical translations and reflections. Scaling was identified as a remaining revision topic; it is not counted as completed theory here.

## 10. Horizontal translations

For a positive shift amount \(a\):

$$
\boxed{g(x)=f(x-a)\ \Rightarrow\ \text{shift right by }a}
$$

$$
\boxed{g(x)=f(x+a)\ \Rightarrow\ \text{shift left by }a}
$$

The sign inside the input appears opposite to the direction of the horizontal movement.

Example:

$$
f(x)=x^2,\qquad g(x)=(x-5)^2
$$

The minimum of \(g\) occurs when \(x-5=0\), so the vertex moves from \((0,0)\) to \((5,0)\): five units right.

## 11. Vertical translations

A change outside the function shifts the output:

$$
\boxed{g(x)=f(x)+a\ \Rightarrow\ \text{shift up by }a}
$$

$$
\boxed{g(x)=f(x)-a\ \Rightarrow\ \text{shift down by }a}
$$

For \(g(x)=x^2+3\), every output is three greater than the corresponding output of \(x^2\), so the graph moves up three units.

## 12. Reflections

A negative sign inside the input changes the horizontal coordinate:

$$
\boxed{g(x)=f(-x)\ \Rightarrow\ \text{reflection across the }y\text{-axis}}
$$

A negative sign outside changes the output:

$$
\boxed{g(x)=-f(x)\ \Rightarrow\ \text{reflection across the }x\text{-axis}}
$$

Point interpretation:

- \(f(-x)\): \((x,y)\) is reflected to \((-x,y)\).
- \(-f(x)\): \((x,y)\) is reflected to \((x,-y)\).

For \(f(x)=x^2\), the graph \(g(x)=-x^2\) opens downward instead of upward.

## 13. Scaling — explicitly marked for revision

Scaling requires a separate conceptual lesson and graph practice:

- \(g(x)=a f(x)\) changes vertical output scale.
- \(g(x)=f(ax)\) changes horizontal input scale.

The factors do not act in the same direction in the same way. These expressions are included as a revision signpost, not as a claim that scaling was fully taught or assessed during this session.

---

# Phase IV — Injectivity

## 14. What does injective mean?

A function is injective (one-to-one) if different inputs always produce different outputs.

Equivalent formal statement:

$$
\boxed{f(a)=f(b)\Rightarrow a=b}
$$

Or:

$$
a\ne b\Rightarrow f(a)\ne f(b)
$$

Think of injectivity as a limit on how many inputs may share one output: **at most one**.

A normal function already has exactly one output for each input. Injectivity adds the condition that two different inputs cannot share that output.

## 15. Horizontal-line test

A function is injective if every horizontal line intersects its graph at most once.

A horizontal line represents one fixed output value. If it crosses the graph at two different input values, those inputs produce the same output, so the function is not injective.

## 16. Algebraic proof of injectivity

For a proof:

1. Let \(a\) and \(b\) be arbitrary elements of the domain.
2. Assume \(f(a)=f(b)\).
3. Substitute the function rule.
4. Simplify using valid algebra.
5. Show that \(a=b\).
6. Conclude that the function is injective.

To disprove injectivity, one counterexample is enough: find \(a\ne b\) such that \(f(a)=f(b)\).

## 17. Domain restrictions matter

For:

$$
f(x)=x^2
$$

on \(\mathbb R\):

$$
f(2)=4=f(-2)
$$

Since \(2\ne-2\), the function is not injective on all real numbers.

But on \([0,\infty)\), the function is strictly increasing and injective. It is also injective on \((-\infty,0]\), where it is strictly decreasing.

Therefore injectivity is a property of the function together with its domain.

Adding a constant to the output does not change this collision pattern: \(x^2+7\) is not injective on \(\mathbb R\), but it is injective on either half-line.

## 18. Strict monotonicity and injectivity

If a function is strictly increasing on its entire domain, then:

$$
a<b\Rightarrow f(a)<f(b)
$$

No two different inputs can have equal outputs.

If a function is strictly decreasing:

$$
a<b\Rightarrow f(a)>f(b)
$$

again, no two different inputs can have equal outputs.

Thus either strict monotonicity condition guarantees injectivity. Merely non-decreasing is not enough, because a function could be constant over an interval.

An optional calculus observation covered in the session: if a differentiable function has \(f'(x)>0\) throughout an interval, it is strictly increasing there; if \(f'(x)<0\) throughout, it is strictly decreasing. Use this only when calculus and the interval conditions are within the question's scope.

## 19. Composition of injective functions

If \(f\) and \(g\) are injective and the composition \(g\circ f\) is defined, then \(g\circ f\) is injective.

Reason: if:

$$
g(f(a))=g(f(b))
$$

injectivity of \(g\) gives \(f(a)=f(b)\). Injectivity of \(f\) then gives \(a=b\).

## 20. Common injectivity traps

- The fact that every input has one output does not prove injectivity.
- A quadratic is not automatically non-injective on every possible domain; a suitable domain restriction may make it injective.
- The horizontal-line test is for injectivity, not for checking whether a graph is a function.
- A single collision disproves injectivity.
- Strictly increasing or strictly decreasing means injective; non-decreasing alone does not guarantee it.

---

# Phase V — Surjectivity

## 21. What does surjective mean?

A function \(f:A\to B\) is surjective (onto) if every element of the codomain is reached by at least one input.

Formal definition:

$$
\boxed{\forall y\in B,\ \exists x\in A\text{ such that }f(x)=y}
$$

Equivalent condition:

$$
\boxed{\operatorname{Range}(f)=\operatorname{Codomain}(f)}
$$

Think of surjectivity as: **at least one preimage for every codomain element**.

Contrast:

- Injective: each output has at most one input.
- Surjective: each codomain element has at least one input.
- Bijective: each codomain element has exactly one input.

## 22. How to prove surjectivity

For \(f:A\to B\):

1. Take an arbitrary \(y\in B\).
2. Solve \(y=f(x)\) for \(x\).
3. Verify that the resulting \(x\) belongs to the declared domain \(A\).
4. Conclude that every \(y\in B\) has a preimage.

The domain-membership check matters. Solving an equation is not enough if the resulting input is not allowed.

## 23. How to disprove surjectivity

Find one element of the codomain with no preimage.

For example, \(f:\mathbb R\to\mathbb R\), \(f(x)=x^2\), is not onto because a negative codomain value such as \(-1\) cannot equal \(x^2\) for any real \(x\).

One missing codomain value is sufficient to disprove surjectivity.

## 24. The codomain can change the answer

Consider the same rule \(f(x)=x^2\):

$$
f:\mathbb R\to\mathbb R
$$

is not surjective because its range is \([0,\infty)\), not all of \(\mathbb R\).

But:

$$
f:\mathbb R\to[0,\infty)
$$

is surjective because its range equals the codomain. It is still not injective.

And:

$$
f:[0,\infty)\to[0,\infty)
$$

is both injective and surjective, so it is bijective.

The expression alone does not decide surjectivity; the domain and codomain matter.

## 25. Surjectivity examples covered

| Function and declared mapping | Result | Reason |
|---|---|---|
| \(x^2:\mathbb R\to\mathbb R\) | Not onto | Negative codomain values are missed |
| \(x^2:\mathbb R\to[0,\infty)\) | Onto | Every non-negative value has a real square root |
| \(x^2+3:\mathbb R\to[3,\infty)\) | Onto | Every \(y\ge3\) has \(x=\pm\sqrt{y-3}\) |
| \(1/x:\mathbb R\setminus\{0\}\to\mathbb R\setminus\{0\}\) | Onto | Choose \(x=1/y\) |
| \(2^x:\mathbb R\to(0,\infty)\) | Onto | For \(y>0\), choose \(x=\log_2y\) |
| \(\log_2x:(0,\infty)\to\mathbb R\) | Onto | For any real \(y\), choose \(x=2^y\) |
| \(3x-7:\mathbb R\to\mathbb R\) | Onto | Choose \(x=(y+7)/3\) |
| \(x^2+1:\mathbb R\to[1,\infty)\) | Onto | Choose \(x=\pm\sqrt{y-1}\) |
| \(x^2+1:\mathbb R\to\mathbb R\) | Not onto | \(y=0\) has no real preimage |
| \(x^3+4:\mathbb R\to\mathbb R\) | Onto | Choose \(x=\sqrt[3]{y-4}\) |
| \(e^x:\mathbb R\to\mathbb R\) | Not onto | Negative values and zero are missed |
| \(\ln x:(0,\infty)\to\mathbb R\) | Onto | Choose \(x=e^y\) |
| \(x^2-9:\mathbb R\to\mathbb R\) | Not onto | Range is \([-9,\infty)\) |
| \(1/(x+2):\mathbb R\setminus\{-2\}\to\mathbb R\setminus\{0\}\) | Onto | For \(y\ne0\), choose \(x=1/y-2\) |

---

# Phase VI — Bijectivity

## 26. What does bijective mean?

A function is bijective if it is both injective and surjective:

$$
\boxed{\text{Bijective}=\text{Injective}+\text{Surjective}}
$$

A bijection pairs every element of the codomain with exactly one element of the domain.

Why exactly one?

- Surjectivity guarantees at least one preimage.
- Injectivity guarantees at most one preimage.
- Together, they guarantee exactly one preimage.

## 27. Classification examples

### Injective but not surjective

$$
f:\mathbb R\to\mathbb R,\qquad f(x)=e^x
$$

The exponential function is strictly increasing, so it is injective. Its range is \((0,\infty)\), so it misses zero and all negative real values. It is not surjective and therefore not bijective.

### Surjective but not injective

$$
f:\mathbb R\to[0,\infty),\qquad f(x)=x^2
$$

Every non-negative number is reached, so the function is onto. But \(f(2)=f(-2)\), so it is not injective.

### Bijective

$$
f:[0,\infty)\to[0,\infty),\qquad f(x)=x^2
$$

On this restricted domain, the function is strictly increasing and reaches every non-negative output. It is both injective and surjective.

### Neither

$$
f:\mathbb R\to\mathbb R,\qquad f(x)=x^2+1
$$

It is not injective because opposite inputs can produce the same output, and it is not onto \(\mathbb R\) because values below 1 are missed.

---

# Phase VII — Inverse Functions

## 28. What is an inverse function?

An inverse function reverses the input-output relationship of the original function.

If:

$$
f:A\to B
$$

is bijective, then:

$$
\boxed{f^{-1}:B\to A}
$$

The inverse accepts an original output and returns the unique original input that produced it.

The inverse exists as a function from the original codomain to the original domain exactly when the original function is bijective.

## 29. Why both injectivity and surjectivity are necessary

If the original function is not injective, one output may come from two different inputs. Reversing that relationship would give one input two possible outputs, so the inverse would not be a function.

Example: \(f(x)=x^2\) on \(\mathbb R\). The output 4 comes from both 2 and -2.

If the original function is not surjective onto its declared codomain, some codomain elements have no original input. The inverse cannot assign an output to those inputs in its declared domain.

Example: \(e^x:\mathbb R\to\mathbb R\) misses negative values and zero. It has an inverse only when the codomain is correctly taken as \((0,\infty)\).

## 30. Finding an inverse algebraically

For a bijection:

1. Write \(y=f(x)\).
2. Exchange \(x\) and \(y\).
3. Solve the resulting equation for \(y\).
4. Write the result as \(f^{-1}(x)\).
5. State the inverse domain and range.
6. Verify the compositions where useful.

The exchange works because the inverse reverses the ordered input-output pairs: \((a,b)\) becomes \((b,a)\).

## 31. Domain and range exchange

For an invertible function:

$$
\boxed{\operatorname{Domain}(f^{-1})=\operatorname{Range}(f)}
$$

$$
\boxed{\operatorname{Range}(f^{-1})=\operatorname{Domain}(f)}
$$

If the original function is bijective from \(A\) onto \(B\), then its inverse maps from \(B\) back to \(A\).

## 32. Linear inverse example

Let:

$$
f(x)=2x+6
$$

Write:

$$
y=2x+6
$$

Exchange:

$$
x=2y+6
$$

Solve:

$$
2y=x-6
$$

$$
\boxed{f^{-1}(x)=\frac{x-6}{2}}
$$

The original function and inverse undo one another.

## 33. Quadratic inverse with a restricted domain

For:

$$
f(x)=x^2,\qquad x\in[0,\infty)
$$

the function is bijective from \([0,\infty)\) to \([0,\infty)\), so:

$$
\boxed{f^{-1}(x)=\sqrt{x}}
$$

If instead the original domain is \((-\infty,0]\), then the inverse is:

$$
\boxed{f^{-1}(x)=-\sqrt{x}}
$$

The inverse is not \(\pm\sqrt{x}\) as a single function, because that would assign two outputs to one input.

## 34. Rational inverse example

Let:

$$
f(x)=\frac{2x+3}{x-4},\qquad x\ne4
$$

The inverse is:

$$
\boxed{f^{-1}(x)=\frac{4x+3}{x-2}}
$$

The original range excludes 2, so the inverse domain excludes 2. The inverse range excludes 4, matching the original domain.

## 35. Exponential and logarithmic inverse pair

For:

$$
f(x)=2^x,\qquad x\in\mathbb R
$$

the range is \((0,\infty)\), and:

$$
\boxed{f^{-1}(x)=\log_2x,\qquad x>0}
$$

Conversely, the inverse of \(\log_2x\) from \((0,\infty)\) to \(\mathbb R\) is \(2^x\).

Similarly:

$$
e^x\longleftrightarrow\ln x
$$

## 36. Verify inverse functions through composition

A correct inverse satisfies both:

$$
\boxed{f(f^{-1}(x))=x}
$$

and:

$$
\boxed{f^{-1}(f(x))=x}
$$

Each identity is used on the appropriate domain. The first checks that applying the inverse and then the original function returns the starting value. The second checks the reverse order.

## 37. Graph of an inverse

The graph of \(f^{-1}\) is the reflection of the graph of \(f\) across the line:

$$
\boxed{y=x}
$$

Every point \((a,b)\) on the original graph corresponds to \((b,a)\) on the inverse graph.

This reflection swaps horizontal and vertical coordinates. It is not a reflection across the x-axis or y-axis.

## 38. Notation trap: inverse versus reciprocal

These are different:

$$
f^{-1}(x)\ne\frac{1}{f(x)}
$$

unless a special relationship happens to make them equal at some input.

- \(f^{-1}\) means the inverse function.
- \(1/f(x)\) means the reciprocal of the output.

---

# Consolidated recognition sheet

| Question asks… | Look for… |
|---|---|
| Is it a function? | Exactly one output for every domain input; vertical-line test |
| Is it injective? | No repeated output from distinct inputs; horizontal-line test |
| Is it surjective? | Range equals declared codomain |
| Is it bijective? | Both injective and surjective |
| Does an inverse exist as a function \(B\to A\)? | Original mapping must be bijective |
| Domain of inverse? | Original range |
| Range of inverse? | Original domain |
| Graph of inverse? | Reflection across \(y=x\) |
| Horizontal shift? | Change inside input, with opposite sign |
| Vertical shift? | Change outside function |
| Reflection across y-axis? | Replace \(x\) by \(-x\) |
| Reflection across x-axis? | Multiply the function output by \(-1\) |

## Entry-test problem-solving checklist

Before selecting an answer:

1. Read the domain and codomain, not just the formula.
2. Decide which property the question tests.
3. For injectivity, look for two distinct inputs with the same output or use a horizontal-line argument.
4. For surjectivity, compare range with codomain or solve for an input for arbitrary \(y\).
5. For bijectivity, establish both properties.
6. For inverses, exchange variables and solve carefully.
7. Check restrictions and excluded values at the end.
8. For transformations, identify whether the change is inside or outside the function.

## Coverage and completion notes

- Function fundamentals: taught and assessed.
- Domain and range: taught, revised, and assessed.
- Horizontal/vertical translations: taught.
- Reflections: taught.
- Scaling: identified as a revision need; not fully taught or assessed.
- Injectivity: taught with introductory, algebraic, and advanced checkpoints.
- Surjectivity: taught; conceptual challenge answered correctly; the offered formal checkpoint was not submitted.
- Bijectivity: taught; offered checkpoint was not submitted.
- Inverse functions: taught through advanced inverse examples; the advanced 6-question checkpoint was completed with 6/6; the written rational-inverse challenge was not submitted.
- Final comprehensive assessment: 22/25 (88%) in approximately 25 minutes.

For the full assessment history and exact final questions, see [MCQs and Assessments](Math-Session-4-MCQs-and-Assessments.md). For the mathematical working, see [Worked Examples](Math-Session-4-Worked-Examples.md).


---

# Supplement — Material from the original comprehensive Session 4 artifact

The initial comprehensive Session 4 artifact was broader than the later seven-phase interactive sequence. It also included parity, composition, advanced range techniques, functional equations, and scaling. The following topics are preserved here so the original scope is not lost.

## Additional function properties: even and odd functions

A function is even when:

$$
f(-x)=f(x)
$$

Its graph is symmetric about the y-axis.

A function is odd when:

$$
f(-x)=-f(x)
$$

Its graph is symmetric about the origin.

Example:

$$
f(x)=x^3-2x
$$

Then:

$$
f(-x)=(-x)^3-2(-x)=-x^3+2x
$$

Factor out the negative:

$$
f(-x)=-(x^3-2x)=-f(x)
$$

Therefore the function is odd. The domain must also be symmetric about zero for the usual even/odd classification.

## Composition and its domain

For functions $f$ and $g$, the composition is:

$$
(f\circ g)(x)=f(g(x))
$$

The output of the inner function $g$ becomes the input of the outer function $f$. The composite is defined only when $x$ belongs to the domain of $g$ and $g(x)$ belongs to the domain of $f$.

Example:

$$
f(x)=\sqrt{x},\qquad g(x)=x^2-4
$$

Then:

$$
(f\circ g)(x)=\sqrt{x^2-4}
$$

A real square root requires:

$$
x^2-4\ge0
$$

Factor:

$$
(x-2)(x+2)\ge0
$$

This holds when:

$$
x\le-2\quad\text{or}\quad x\ge2
$$

Therefore:

$$
D_{f\circ g}=(-\infty,-2]\cup[2,\infty)
$$

The important idea is to apply the domain restrictions of the outer function to the output of the inner function.

## Advanced range example

For:

$$
f(x)=\frac{x^2}{x^2+1}
$$

let $t=x^2$. Since $t\ge0$:

$$
f(x)=\frac{t}{t+1}=1-\frac{1}{t+1}
$$

Because $t+1\ge1$, the expression is at least zero and strictly less than one:

$$
0\le f(x)<1
$$

The value zero is attained at $x=0$. The value one is never attained, because:

$$
\frac{x^2}{x^2+1}=1
\Rightarrow x^2=x^2+1
$$

which is impossible. Hence:

$$
R_f=[0,1)
$$

## Scaling transformations — included in the original comprehensive artifact

The initial comprehensive artifact introduced both vertical and horizontal scaling. The later interactive lessons concentrated mainly on translations and reflections, and the final assessment showed that transformations still needed reinforcement. Therefore, scaling is included in the syllabus record but should not be marked as mastered.

### Vertical scaling

$$
g(x)=a f(x)
$$

Every output is multiplied by $a$.

- If $|a|>1$, the graph is vertically stretched away from the x-axis.
- If $0<|a|<1$, the graph is vertically compressed toward the x-axis.
- If $a<0$, there is also a reflection across the x-axis.

### Horizontal scaling

$$
g(x)=f(ax)
$$

The input is multiplied by $a$, so horizontal scaling acts reciprocally:

- If $|a|>1$, the graph is horizontally compressed by factor $1/|a|$.
- If $0<|a|<1$, the graph is horizontally stretched by factor $1/|a|$.
- If $a<0$, there is also a reflection across the y-axis.

These rules assume $a\ne0$ for a genuine horizontal scaling transformation.

### Original combined transformation example

$$
g(x)=-2(x-3)^2+4
$$

Starting from $y=x^2$:

1. $(x-3)^2$ shifts the graph 3 units right.
2. Multiplication by $-2$ reflects it across the x-axis and vertically stretches it by factor 2.
3. Addition of 4 shifts it 4 units upward.

The vertex is $(3,4)$ and the parabola opens downward.

A second original example was:

$$
g(x)=3|x+2|-5
$$

Starting from $y=|x|$, it shifts 2 units left, stretches vertically by factor 3, and shifts 5 units down. Its vertex is $(-2,-5)$, domain is $\mathbb R$, and range is $[-5,\infty)$.

## Functional equations: using symmetry substitutions

An original advanced example was:

$$
f(x)+2f(-x)=3x+6
$$

Replace $x$ by $-x$:

$$
f(-x)+2f(x)=-3x+6
$$

This creates two equations involving $f(x)$ and $f(-x)$. Solving them simultaneously gives:

$$
\boxed{f(x)=-3x+2}
$$

The method is to use the original equation and its transformed version as a simultaneous linear system. The full algebra is preserved in the Worked Examples companion file.

## Original comprehensive artifact: ten-part structure

The initial artifact organized the wider topic into ten parts: curriculum alignment and objectives; function foundations; domain and range; function properties; composition and inverses; graph transformations; advanced techniques; fourteen worked examples; exam strategy and guided practice; and a 30-MCQ examination with performance analysis and consolidation.

The original practice and examination sections contained planned placeholders rather than a complete submitted set of 15 guided-practice answers or a completed 30-question examination. The later interactive final challenge was a separate 25-question assessment and is documented in the assessment file.

## Coverage clarification

- Scaling was introduced in the original comprehensive artifact with rules and worked transformation examples.
- The later interactive sequence did not provide a full scaling lesson or scaling diagnostic.
- The user subsequently identified graph scaling and transformations as difficult.
- Therefore scaling is documented as introduced in the original material but still requiring focused teaching, practice, and assessment.
