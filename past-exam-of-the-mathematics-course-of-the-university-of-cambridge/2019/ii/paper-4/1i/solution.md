<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

For $x\geq2$, expand the finite [Euler product](../../../../../euler-product.md) as a product of [geometric series](../../../../../geometric-series.md):

$$
P(x):=\prod_{p\leq x}\left(1-\frac1p\right)^{-1}
=\sum_{\substack{n\geq1\\p\mid n\Rightarrow p\leq x}}\frac1n.
$$

Every integer $1\leq n\leq x$ has all its prime factors at most $x$, so

$$
P(x)\geq\sum_{n\leq x}\frac1n.
$$

The [harmonic series](../../../../../harmonic-series.md) diverges, and therefore

$$
\boxed{\prod_p\left(1-\frac1p\right)^{-1}=\infty.}
$$

Suppose instead that $\sum_p1/p$ converged. For $0<t\leq1/2$,

$$
0\leq-\log(1-t)-t=\sum_{j\geq2}\frac{t^j}{j}\leq\frac{t^2}{1-t}\leq2t^2.
$$

Since $\sum_p1/p^2$ converges, this would make

$$
\log P(x)=\sum_{p\leq x}-\log\left(1-\frac1p\right)
$$

converge to a finite limit, contradicting the divergence of $P(x)$. Hence the [Euler proof that the sum of reciprocals of primes diverges](../../../../../euler-proof-that-the-sum-of-reciprocals-of-primes-diverges.md) gives

$$
\boxed{\sum_p\frac1p=\infty.}
$$

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
