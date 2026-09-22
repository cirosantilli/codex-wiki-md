<h1 id="4f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

This is a [lacunary power series](../../../../../../lacunary-power-series.md): the coefficient of $z^{n!}$ is $n^n$, while the other coefficients are zero. Along its nonzero coefficients,

$$
(n^n)^{1/n!}=\exp\!\left(\frac{n\log n}{n!}\right)\longrightarrow1.
$$

The factorial dominates $n\log n$; for example $n!\geq n(n-1)(n-2)(n-3)$ for large $n$ already suffices for this limit. Hence the coefficient limsup in the [Cauchy-Hadamard theorem](../../../../../../cauchy-hadamard-theorem.md) is one. **The [radius of convergence](../../../../../../radius-of-convergence.md) is** $\boxed{R=1}$.

Directly, for $|z|<1$ the consecutive term ratio is $(n+1)^{n+1}n^{-n}|z|^{n n!}$, which tends to zero; for $|z|\geq1$ the term magnitudes are at least $n^n$ and fail to tend to zero. The factorial is the exponent of $z$, not part of its coefficient.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4F](../../4f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
