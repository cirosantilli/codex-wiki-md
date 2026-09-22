<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For positive integer $n$ and any positive integer $N$, the finite [geometric series](../../../../../../geometric-series.md) identity

$$
\frac1{1-t}=\sum_{j=0}^{N-1}t^j+\frac{t^N}{1-t}
$$

gives an exact decomposition along the indented contour. The polynomial terms have no [pole](../../../../../../pole.md) and may be returned to the positive real axis; their [Gamma function](../../../../../../gamma-function.md) integrals are

$$
I(\lambda,n)=e^\lambda\sum_{r=n}^{n+N-1}\frac{\Gamma(r)}{\lambda^r}+I(\lambda,n+N).
$$

Equivalently, expansion about the endpoint $t=0$ in the [Laplace transform](../../../../../../laplace-transform.md) integral gives the same coefficients. The resulting formal [asymptotic expansion](../../../../../../asymptotic-expansion.md) is

$$
\boxed{I(\lambda,n)\sim e^\lambda\sum_{r=n}^{\infty}\frac{\Gamma(r)}{\lambda^r}}.
$$

The ratio of consecutive terms is $r/\lambda$, so the infinite series is factorially divergent. It should be truncated, not treated as a convergent sum; the [pole](../../../../../../pole.md) prescription controls the contribution beyond its algebraic orders. Although the source initially calls $n$ an integer, the ordinary lower endpoint integral requires $n>0$, as is already implicit in the large-positive-$n$ limit of part (i).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
