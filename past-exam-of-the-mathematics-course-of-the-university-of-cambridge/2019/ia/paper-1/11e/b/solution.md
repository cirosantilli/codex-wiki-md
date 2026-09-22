<h1 id="11e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) gives

$$
\sqrt{a_na_{n+1}}\leq\frac{a_n+a_{n+1}}2.
$$

Thus convergence of $\sum_na_n$ implies convergence of $\sum_n\sqrt{a_na_{n+1}}$ by the [comparison test for series](../../../../../../comparison-test-for-series.md).

The converse is false. Define

$$
a_{2n}=\frac1n,
\qquad
a_{2n-1}=\frac1{n^3}.
$$

The even terms make $\sum_na_n$ diverge, while

$$
\sqrt{a_{2n-1}a_{2n}}=\frac1{n^2},
\qquad
\sqrt{a_{2n}a_{2n+1}}=\frac1{\sqrt{n(n+1)^3}}\leq\frac1{n^2},
$$

so the neighboring geometric-mean series converges.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
