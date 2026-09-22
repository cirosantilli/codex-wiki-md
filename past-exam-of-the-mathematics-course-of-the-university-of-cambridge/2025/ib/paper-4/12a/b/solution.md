<h1 id="12a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Split the transform into periods and translate each interval:

$$
\mathcal L\{g\}(s)=\sum_{j=0}^\infty\int_{jT}^{(j+1)T}e^{-st}g(t)dt
=\sum_{j=0}^\infty e^{-sjT}\int_0^T e^{-su}g(u)du.
$$

Summing the [geometric series](../../../../../../geometric-series.md) yields

$$
\boxed{\mathcal L\{g\}(s)=\frac{\mathcal L\{g_T\}(s)}{1-e^{-sT}}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12A](../../12a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
