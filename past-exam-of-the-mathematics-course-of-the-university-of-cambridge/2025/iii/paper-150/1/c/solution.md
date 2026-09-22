<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
F(n)=(2n+1)(3n+1)(5n+1).
$$

For every prime $p>5$, the congruence $F(n)\equiv0\pmod p$ excludes the three distinct residue classes

$$
n\equiv-2^{-1},-3^{-1},-5^{-1}\pmod p.
$$

The finitely many smaller primes only alter the implied constant. The [dimension-three upper-bound sieve](../../../../../../dimension-three-upper-bound-sieve.md), used with $z=x^{1/2}$, therefore gives

$$
|\{n\leq x:\gcd(F(n),P(z))=1\}|
\ll x\prod_{5<p\leq z}\left(1-\frac3p\right)
\ll\frac{x}{(\log z)^3}
\ll\frac{x}{(\log x)^3},
$$

where the middle estimate follows from [Mertens theorem](../../../../../../mertens-theorems.md).

If all three linear forms are prime, then either $F(n)$ has no prime divisor at most $z$, or one of the three forms itself equals such a prime. The latter possibility contributes only $O(\pi(z))=O(x^{1/2})$, which is absorbed by $x/(\log x)^3$. Hence the required number of $n$ is $\ll x/(\log x)^3$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
