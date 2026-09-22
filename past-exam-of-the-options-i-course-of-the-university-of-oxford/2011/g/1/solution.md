<h1 id="g/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $P=F_{y'}$ and $Q=F_{y''}$. For a smooth [variation](../../../../variation.md) $y+\varepsilon\eta$, the [first variation](../../../../first-variation.md) is

$$
\delta J=\int_a^b(F_y\eta+P\eta'+Q\eta'')\,dx
=\int_a^b(F_y-P'+Q'')\eta\,dx+[(P-Q')\eta+Q\eta']_a^b.
$$

Here the last expression follows by two integrations by parts. Taking variations supported in the interior and applying the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives the [Euler-Lagrange equation for a second-derivative functional](../../../../euler-lagrange-equation-for-a-second-derivative-functional.md):

$$
\boxed{F_y-\frac{d}{dx}F_{y'}+\frac{d^2}{dx^2}F_{y''}=0.}
$$

If both endpoint values and slopes are free, their independent variations force the [natural boundary conditions for second-derivative functionals](../../../../natural-boundary-conditions-for-second-derivative-functionals.md)

$$
\boxed{Q=0,\qquad P-Q'=0\quad\text{at }a,b.}
$$

If an endpoint value or slope is fixed instead, its corresponding variation vanishes and the associated natural condition is not required.

For $H=y''Q-y'(Q'-P)-F$, differentiate using the [chain rule](../../../../chain-rule.md):

$$
H'=y'(P'-Q''-F_y)-F_x.
$$

The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) cancels the first term. Consequently $H'=-F_x$, and if there is no explicit $x$ dependence,

$$
\boxed{H=y''F_{y''}+y'\bigl(F_{y'}-(F_{y''})'\bigr)-F\text{ is constant}.}
$$

This is a [Beltrami identity for a second-derivative functional](../../../../beltrami-identity-for-a-second-derivative-functional.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [G](../../g.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
