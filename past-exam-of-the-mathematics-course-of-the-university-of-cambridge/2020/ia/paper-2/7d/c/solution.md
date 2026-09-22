<h1 id="7d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [RSA cryptosystem](../../../../../../rsa-cryptosystem.md), choose distinct large primes $p,q$, put $N=pq$, and choose $e$ coprime to

$$
\phi(N)=(p-1)(q-1).
$$

The decryption exponent is the [modular multiplicative inverse](../../../../../../modular-multiplicative-inverse.md)

$$
d\equiv e^{-1}\pmod{\phi(N)}.
$$

Thus $ed=1+k\phi(N)$. For a message with $\gcd(m,N)=1$, the [Fermat-Euler theorem](../../../../../../euler-s-theorem.md) gives

$$
c^d\equiv m^{ed}
=m(m^{\phi(N)})^k\equiv m\pmod N.
$$

For $N=187=11\cdot17$, $\phi(N)=160$. The [extended Euclidean algorithm](../../../../../../extended-euclidean-algorithm.md) gives

$$
1=37\cdot13-3\cdot160,
$$

so

$$
\boxed{d=37}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7D](../../7d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
