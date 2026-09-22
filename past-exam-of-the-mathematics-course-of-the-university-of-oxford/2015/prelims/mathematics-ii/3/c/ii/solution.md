<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [ceiling function](../../../../../../../ceiling-function.md) to choose positive [integer](../../../../../../../integer-split.md) [coefficients](../../../../../../../coefficient.md)

$$
\boxed{a_n=\lceil\alpha^{-n}\rceil\qquad(n\geq0).}
$$

Because $0<\alpha<1$, we have $\alpha^{-n}\geq1$ and

$$
\alpha^{-n}\leq a_n<\alpha^{-n}+1\leq2\alpha^{-n}.
$$

For $|z|<\alpha$, the [comparison test for series](../../../../../../../comparison-test-for-series.md) with the [geometric series](../../../../../../../geometric-series.md) gives

$$
\sum_{n=0}^{\infty}|a_nz^n|\leq2\sum_{n=0}^{\infty}\left(\frac{|z|}{\alpha}\right)^n<\infty.
$$

For $|z|\geq\alpha$, we instead have $|a_nz^n|\geq(|z|/\alpha)^n\geq1$, so the terms do not tend to zero. Thus **the [power series](../../../../../../../power-series.md) has [radius of convergence](../../../../../../../radius-of-convergence.md) exactly $\alpha$.**

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
