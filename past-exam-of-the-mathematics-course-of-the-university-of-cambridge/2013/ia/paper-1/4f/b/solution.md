<h1 id="4f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The summand is positive, so it suffices to show that its [partial sums](../../../../../../partial-sum.md) are unbounded. On the block $2^k\leq n<2^{k+1}$, for $k\geq1$,

$$
\frac1{n\log n}\geq\frac1{2^{k+1}(k+1)\log2}.
$$

There are $2^k$ terms in that block, so its sum is at least $1/[2(k+1)\log2]$. Adding blocks gives a constant multiple of the divergent [harmonic series](../../../../../../harmonic-series.md). Hence

$$
\boxed{\sum_{n=2}^\infty\frac1{n\log n}=+\infty.}
$$

Equivalently the [integral test for convergence](../../../../../../integral-test-for-convergence.md) gives $\int_2^R dx/(x\log x)=\log\log R-\log\log2\to\infty$. The block proof supplies the divergence without assuming the integral test.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4F](../../4f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
