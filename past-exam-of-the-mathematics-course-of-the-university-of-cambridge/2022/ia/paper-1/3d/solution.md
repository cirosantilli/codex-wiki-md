<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

The [alternating series test](../../../../../alternating-series-test.md) says that if $a_n\geq0$ decreases to $0$, then

$$
\sum_{n=1}^{\infty}(-1)^na_n
$$

converges. Taking $a_n=n^{-1/2}$ proves convergence of the given series.

It is not [absolute convergence](../../../../../absolute-convergence.md), because the series of absolute values is the [p-series](../../../../../p-series.md)

$$
\sum_{n=1}^{\infty}\frac1{\sqrt n},
$$

which diverges since $p=1/2\leq1$. Thus the original series has [conditional convergence](../../../../../conditional-convergence.md).

For an explicit divergent [rearrangement of a series](../../../../../rearrangement-of-a-series.md), take unused positive terms, which are the even-indexed terms, until the partial sum exceeds $1$, then take the first unused negative term. Next take positive terms until the sum exceeds $2$, then the next unused negative term, and continue. Both the positive and negative subseries have infinite total magnitude, so this procedure uses every term. The negative term inserted at stage $m$ tends to zero, while the preceding partial sum exceeds $m$; consequently these rearranged partial sums tend to $+\infty$. This is a divergent series with exactly the prescribed terms.

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
