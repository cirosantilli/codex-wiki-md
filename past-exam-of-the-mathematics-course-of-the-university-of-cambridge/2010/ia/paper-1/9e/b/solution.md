<h1 id="9e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [limit comparison test](../../../../../../limit-comparison-test.md) says that if $u_n,v_n>0$ and $u_n/v_n\to L$ with $0<L<\infty$, then their [series](../../../../../../series-mathematics.md) either both converge or both diverge. This follows because, eventually, $(L/2)v_n\leq u_n\leq(3L/2)v_n$, and the [comparison test for series](../../../../../../comparison-test-for-series.md) applies in both directions.

Here comparison with the [harmonic series](../../../../../../harmonic-series.md) gives

$$
\frac{1/[n+(\log n)^2]}{1/n}
=\frac1{1+(\log n)^2/n}\longrightarrow1.
$$

For completeness, the [natural logarithm](../../../../../../natural-logarithm.md) grows slowly enough because for $x\geq1$,

$$
0\leq\log x=\int_1^x\frac{dt}{t}
\leq\int_1^x t^{-3/4}\,dt
=4(x^{1/4}-1)\leq4x^{1/4},
$$

so $(\log n)^2/n\leq16/\sqrt n\to0$. The [harmonic series](../../../../../../harmonic-series.md) diverges: every block from $n=2^k$ to $2^{k+1}-1$ has $2^k$ terms at least $2^{-k-1}$ and therefore contributes at least $1/2$. Hence

$$
\boxed{\sum_{n\geq1}\frac1{n+(\log n)^2}\text{ diverges to }+\infty.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9E](../../9e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
