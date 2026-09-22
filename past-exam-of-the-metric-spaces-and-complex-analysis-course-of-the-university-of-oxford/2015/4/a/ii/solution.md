<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [generalized binomial theorem](../../../../../binomial-series.md) with exponent $-1/2$, choosing the [analytic branch of a square root](../../../../../analytic-branch-of-a-square-root.md) that equals $1$ at $z=0$. For $|z|<1$,

$$
(1-z)^{-1/2}=\sum_{n=0}^{\infty}\binom{-1/2}{n}(-z)^n.
$$

The signs cancel in each [binomial coefficient](../../../../../binomial-coefficient-split.md). For $n\geq1$,

$$
(-1)^n\binom{-1/2}{n}=\frac{1\cdot3\cdots(2n-1)}{2^n n!}=\frac{(2n)!}{2^{2n}(n!)^2}=\frac1{4^n}\binom{2n}{n}.
$$

The same expression equals $1$ for $n=0$, using the empty-product convention. Consequently the [power series](../../../../../power-series.md) is

$$
\boxed{\frac1{\sqrt{1-z}}=\sum_{n=0}^{\infty}\binom{2n}{n}\left(\frac z4\right)^n,\qquad |z|<1.}
$$

Its coefficients are the [normalized central binomial coefficients](../../../../../normalized-central-binomial-coefficients.md). As a convergence check, the ratio of successive absolute terms tends to $|z|$, so the [ratio test](../../../../../ratio-test.md) gives absolute convergence inside the [unit disc](../../../../../unit-disc.md). Applying the [Cauchy coefficient formula](../../../../../cauchy-coefficient-formula.md) to the [holomorphic function](../../../../../holomorphic-function-split.md) $(1-z)^{-1/2}$ now immediately yields

$$
\boxed{\int_{\gamma(0,r)}\frac{dz}{z^{n+1}\sqrt{1-z}}=\frac{2\pi i}{4^n}\binom{2n}{n},\qquad 0<r<1,\quad n=0,1,2,\ldots.}
$$

This value is independent of the chosen [radius](../../../../../radius.md) because the [contour integral](../../../../../contour-integral.md) extracts the same coefficient on every such [circle](../../../../../circle.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
