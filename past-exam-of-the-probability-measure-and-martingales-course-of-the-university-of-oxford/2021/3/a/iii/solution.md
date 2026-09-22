<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Consider the [Borel set](../../../../../borel-set.md)

$$
D=\{(x,y):a<x\leq y\leq b\}.
$$

Its [indicator function](../../../../../indicator-function.md) is nonnegative and [measurable](../../../../../measurability.md), so the [Tonelli theorem](../../../../../tonelli-theorem.md) applies to the [product measure](../../../../../product-measure.md), without needing any separate absolute-[integrability](../../../../../integrability.md) argument. At a fixed $y\in(a,b]$, its section in the first coordinate is $(a,y]$; outside $(a,b]$ that section is empty. Therefore

$$
\begin{aligned}
(\mu\otimes\nu)(D)
&=\int_{\mathbb R}\left(\int_{\mathbb R}\mathbf1_D(x,y)\,\mu(dx)\right)\nu(dy)\\
&=\int_{(a,b]}\mu((a,y])\,\nu(dy)\\
&=\int_{(a,b]}\bigl(F_\mu(y)-F_\mu(a)\bigr)\,\nu(dy).
\end{aligned}
$$

The last equality uses the definition of a [cumulative distribution function](../../../../../cumulative-distribution-function.md) on the half-closed [interval](../../../../../interval-mathematics.md). It retains all [point atoms of a measure](../../../../../point-atom-of-a-measure.md) on the diagonal $x=y$, excludes a possible [point atom of a measure](../../../../../point-atom-of-a-measure.md) at $x=a$, and includes $y=b$, exactly as required by the [set](../../../../../set-split.md) $D$. If $a=b$, both sides vanish. This verifies the identity even when the [probability measures](../../../../../probability-measure.md) are not [non-atomic measures](../../../../../non-atomic-measure.md).[§1.7, Theorem 1.7.2, printed pp. 38–40: integration of a nonnegative measurable function on a product space](../../../../../probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
