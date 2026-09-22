<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One general form of the [Erdős-Kac theorem](../../../../../../erdos-kac-theorem.md) is the following. Let $f$ be a real [strongly additive arithmetic function](../../../../../../strongly-additive-arithmetic-function.md), with $|f(p)|\le C$ for all [primes](../../../../../../prime-number.md), and define

$$
A(x)=\sum_{p\le x}\frac{f(p)}p,\qquad B(x)^2=\sum_{p\le x}\frac{f(p)^2}p.
$$

If $B(x)\to\infty$, then under the [discrete uniform distribution](../../../../../../discrete-uniform-distribution.md) on $[N]$,

$$
\boxed{\frac{f(n)-A(N)}{B(N)}\ \xrightarrow{\mathrm d}\ \mathcal N(0,1).}
$$

Here the arrow denotes [convergence in distribution](../../../../../../convergence-in-distribution.md) and $\mathcal N(0,1)$ is the [standard normal distribution](../../../../../../standard-normal-distribution.md). Equivalently, the probability of being at most $z$ tends to the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md) $\Phi(z)$ for every real $z$. Replacing $B(x)^2$ by $\sum_{p\le x}f(p)^2(1-1/p)/p$ is equivalent, because the difference is bounded by $C^2\sum_p p^{-2}$.

This is a general bounded-prime-weight form, not just the special case $f=\omega$. In that case the [Mertens theorem for reciprocal primes](../../../../../../mertens-second-theorem.md) gives $A(N)=\log\log N+O(1)$ and $B(N)^2=\log\log N+O(1)$, so **the classical prime-factor central limit theorem** is

$$
\boxed{\frac{\omega(n)-\log\log N}{\sqrt{\log\log N}}\ \xrightarrow{\mathrm d}\ \mathcal N(0,1).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
