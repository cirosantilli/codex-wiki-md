<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Split the [power series](../../../../../../../power-series.md) into even and odd indices:

$$
\sum_{n=0}^{\infty}a_nz^n=\sum_{j=0}^{\infty}\left(\frac z2\right)^{2j}+\sum_{j=0}^{\infty}\frac{z^{2j+1}}{(2j+1)^2},
$$

whenever the two [series](../../../../../../../series-mathematics.md) converge absolutely. If $|z|<1$, the even part is a convergent [geometric series](../../../../../../../geometric-series.md), while the odd part is bounded termwise in [absolute value](../../../../../../../absolute-value.md) by $\sum_j|z|^{2j+1}$, also a convergent [geometric series](../../../../../../../geometric-series.md). Hence there is [absolute convergence](../../../../../../../absolute-convergence.md) throughout $|z|<1$.

If $|z|>1$, the odd terms have [absolute values](../../../../../../../absolute-value.md) $|z|^{2j+1}/(2j+1)^2$. Their successive ratio tends to $|z|^2>1$, so these terms grow eventually and do not tend to zero. The [term test for divergence](../../../../../../../term-test-for-divergence.md) therefore forces divergence of the original [power series](../../../../../../../power-series.md). Consequently its [radius of convergence](../../../../../../../radius-of-convergence.md) is

$$
\boxed{R=1.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
