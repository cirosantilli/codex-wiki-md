<h1 id="9c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Group](../../../../../../group-split.md) three consecutive terms. Their block sum is

$$
b_n=-\frac1{2n-1}+\frac1{4n-1}+\frac1{4n}
=-\frac{6n-1}{4n(2n-1)(4n-1)}.
$$

Since $2n-1\ge n$ and $4n-1\ge3n$ for $n\ge1$, we have $|b_n|\le1/(2n^2)$. The [comparison test for series](../../../../../../comparison-test-for-series.md) and the preceding proof of convergence of $\sum n^{-2}$ show that $\sum b_n$ converges absolutely.

This establishes convergence of the original [partial sums](../../../../../../partial-sum.md) at indices $3N$. Each intermediate [partial sum](../../../../../../partial-sum.md) differs from one of these by at most two of the original terms; those terms tend to zero. Thus all [partial sums](../../../../../../partial-sum.md) have the same [limit of a sequence](../../../../../../limit-of-a-sequence.md), which is the mechanism of [convergence from fixed-length series blocks](../../../../../../convergence-from-fixed-length-series-blocks.md). The original [series](../../../../../../series-mathematics.md) is not absolutely convergent, since its absolute-value [series](../../../../../../series-mathematics.md) contains $\sum_n(2n-1)^{-1}\ge\tfrac12\sum_n n^{-1}$. Therefore **the original [series](../../../../../../series-mathematics.md) converges conditionally**.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [9C](../../9c.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ia](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
