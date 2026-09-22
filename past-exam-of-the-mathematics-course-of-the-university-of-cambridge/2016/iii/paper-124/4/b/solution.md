<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D(s)=\sum_{p\le X}p^{-s}$, a [Dirichlet polynomial](../../../../../../dirichlet-polynomial.md) supported on [primes](../../../../../../prime-number.md). The cosine sum is $(D(\sigma+it)+\overline{D(\sigma+it)})/2$, so its $j$th power is a finite linear combination of $D(\sigma+it)^k\overline{D(\sigma+it)^{j-k}}$, $0\le k\le j$.

The [Dirichlet polynomial](../../../../../../dirichlet-polynomial.md) $D(s)^k$ is supported on integers that are products of exactly $k$ [primes](../../../../../../prime-number.md), counted with multiplicity. Each coefficient is at most $k!$ by [unique prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md); for $k=0$ the only coefficient is the one at $1$. As $j$ is odd, $k\ne j-k$, so no integer can appear in both supports. Thus **every diagonal term vanishes** in the [mean value of Dirichlet polynomials](../../../../../../mean-value-of-dirichlet-polynomials.md) from part (a).

Both supports lie in $[1,X^j]$. The first error bound in part (a), with that common length, now gives for each term

$$
\left|\int_T^{2T}D(\sigma+it)^k\overline{D(\sigma+it)^{j-k}}\,dt\right|\ll_j X^j\left(\sum_{n\le X^j}n^{-\sigma}\right)^2.
$$

Summing the finitely many terms proves **the [odd moment of a prime cosine sum](../../../../../../odd-moment-of-a-prime-cosine-sum.md) estimate**:

$$
\boxed{\left|\int_T^{2T}\left(\sum_{p\le X}\frac{\cos(t\log p)}{p^\sigma}\right)^j\,dt\right|\ll_j X^j\left(\sum_{n\le X^j}\frac1{n^\sigma}\right)^2.}
$$

The argument holds for all real $\sigma$ and all $T\ge0$; no cancellation estimate involving $T$ is needed once the diagonal is absent.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
