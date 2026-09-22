<h1 id="9f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For any fixed $r>0$, $\log y=o(y^{1/r})$ as $y\to\infty$. For example, l'Hôpital's rule applied to $\log y/y^{1/r}$ gives the limit zero. With $y=\log n$, this implies $(\log\log n)^r<\log n$ eventually. Therefore

$$
\frac1{n(\log\log n)^r}>\frac1{n\log n}
$$

for all sufficiently large $n$. The comparison [series](../../../../../../series-mathematics.md) diverges by the [integral test for convergence](../../../../../../integral-test-for-convergence.md), since

$$
\int^M\frac{dx}{x\log x}=\log\log M+\text{constant}\longrightarrow\infty.
$$

The [comparison test for series](../../../../../../comparison-test-for-series.md) gives

$$
\boxed{\sum_{n=3}^\infty\frac1{n(\log\log n)^r}\text{ diverges for every }r>0.}
$$

One may obtain the same growth bound by extending the given logarithmic estimate to real $y$ through $\lceil y\rceil$ and choosing any exponent smaller than $1/r$; no special convergence test for iterated logarithms is needed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
