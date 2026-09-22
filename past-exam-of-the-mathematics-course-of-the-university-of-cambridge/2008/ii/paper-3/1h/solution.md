<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Put $N=\lfloor x\rfloor$. Comparing the [harmonic number](../../../../../harmonic-number.md) with an [integral](../../../../../integral.md) gives $H_N=\sum_{n=1}^N1/n>\int_1^{N+1}dt/t=\log(N+1)>\log x$. By the [Fundamental theorem of arithmetic](../../../../../fundamental-theorem-of-arithmetic.md), the finite [Euler product](../../../../../euler-product.md) $\prod_{p\leq x}(1-p^{-1})^{-1}$ expands as the sum of $1/n$ over positive integers whose [prime factors](../../../../../prime-factor.md) are at most $x$. It therefore includes every term of $H_N$, and

$$
\log H_N\leq-\sum_{p\leq x}\log(1-p^{-1})
<\sum_{p\leq x}\frac1p+\frac12\sum_{p\leq x}\frac1{p(p-1)}
<\sum_{p\leq x}\frac1p+\frac12.
$$

The first strict inequality is the [geometric-series bound for the logarithmic remainder](../../../../../geometric-series-bound-for-the-logarithmic-remainder.md); the last uses the [telescoping series](../../../../../telescoping-series.md) $\sum_{n=2}^\infty1/[n(n-1)]=1$. Thus the [prime reciprocal lower bound](../../../../../prime-reciprocal-lower-bound.md) is

$$
\boxed{\sum_{p\leq x}\frac1p>\log H_N-\frac12>\log\log x-\frac12.}
$$

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
