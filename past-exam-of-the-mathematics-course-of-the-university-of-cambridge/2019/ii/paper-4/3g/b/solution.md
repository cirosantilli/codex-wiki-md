<h1 id="3g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**No.** The procedure exposes a square-root oracle for the [Rabin cryptosystem](../../../../../../rabin-cryptosystem.md). The verifier chooses $m$, sends $r=m^2\bmod N$, and receives another square root $m_1$. If

$$
m_1\not\equiv\pm m\pmod N,
$$

then the [factorization from distinct square roots modulo a semiprime](../../../../../../factorization-from-distinct-square-roots-modulo-a-semiprime.md) gives

$$
\boxed{\gcd(m-m_1,N)\text{ is a nontrivial factor of }N.}
$$

For a product of two odd primes, a square normally has four roots, and a returned root lies outside the pair $\{\pm m\}$ with probability about $1/2$. Repeating chosen-square challenges therefore factors $N$ with overwhelming probability. The attacker can then compute square roots and impersonate Alice. This is the [chosen-square attack on Rabin authentication](../../../../../../chosen-square-attack-on-rabin-authentication.md), so the proposed protocol is insecure.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3G](../../3g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
