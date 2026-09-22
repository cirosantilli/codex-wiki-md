<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Expand the finite [Euler product](../../../../../euler-product.md) into convergent geometric series. Every positive integer $n\le x$ has all its [prime factors](../../../../../prime-factor.md) at most $x$, so

$$
P(x)^{-1}=\prod_{p\le x}\sum_{k\ge0}p^{-k}
=\sum_{\substack{n\ge1\\\text{all prime factors of }n\le x}}\frac1n
\ge\sum_{n\le x}\frac1n.
$$

The [harmonic series](../../../../../harmonic-series.md) diverges, hence **$P(x)\to0$**. If the sum of reciprocal primes were finite, then the inequality $-\log(1-t)\le2t$ for $0\le t\le1/2$ would give

$$
-\log P(x)=\sum_{p\le x}-\log(1-1/p)\le2\sum_p\frac1p<\infty,
$$

uniformly in $x$, contradicting $P(x)\to0$. Thus **the sum of prime reciprocals diverges**. [Unique factorization](../../../../../unique-factorization-in-an-integral-domain.md) justifies the expansion; no estimate for the distribution of primes is required. This is the [Euler proof that the sum of reciprocals of primes diverges](../../../../../euler-proof-that-the-sum-of-reciprocals-of-primes-diverges.md).

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
