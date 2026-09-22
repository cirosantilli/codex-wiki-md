<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Möbius function](../../../../../../mobius-function.md) has $\mu(1)=1$, vanishes on integers divisible by a square of a prime, and equals $(-1)^r$ on a product of $r$ distinct primes. Factoring the divisor sum prime by prime gives

$$
\sum_{m\mid n}\mu(m)=\begin{cases}1,&n=1,\\0,&n>1.\end{cases}
$$

This is the [Möbius divisor-sum identity](../../../../../../mobius-divisor-sum-identity.md).

For $T/2\le t\le T$ and $0<\sigma\le1$, the [Hardy-Littlewood approximation to the Riemann zeta function](../../../../../../hardy-littlewood-approximation-to-the-riemann-zeta-function.md) at cutoff $T$ gives

$$
\zeta(s)=\sum_{d\le T}d^{-s}+O(T^{-\sigma}).
$$

Indeed $T\ge|t|/\pi$, and the omitted integral term has size at most $T^{1-\sigma}/|s-1|\ll T^{-\sigma}$. Multiply by $\sum_{m\le M}\mu(m)m^{-s}$. Its absolute value is at most

$$
\sum_{m\le M}m^{-\sigma}\le M^{1-\sigma}\sum_{m\le M}\frac1m\ll M^{1-\sigma}\log M,
$$

where the elementary inequality follows from $m^{1-\sigma}\le M^{1-\sigma}$. Reindexing the finite double sum yields coefficients $a_n=\sum_{m\mid n,\ m\le M,\ n/m\le T}\mu(m)$, with no terms for $n>MT$. For $n\le\min(M,T)$ all divisors meet both restrictions, so the [Möbius divisor-sum identity](../../../../../../mobius-divisor-sum-identity.md) gives $a_1=1$ and $a_n=0$ for $1<n\le\min(M,T)$. Hence the [truncated Möbius inverse identity for the Riemann zeta function](../../../../../../truncated-mobius-inverse-identity-for-the-riemann-zeta-function.md) is

$$
\boxed{\zeta(\sigma+it)\sum_{m\le M}\frac{\mu(m)}{m^{\sigma+it}}=1+\sum_{\min(M,T)<n\le MT}\frac{a_n}{n^{\sigma+it}}+O\left(\frac{M\log M}{T^\sigma M^\sigma}\right).}
$$

The displayed error is uniform in $0<\sigma\le1$ and the stated height interval.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
