<h1 id="11g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By the definition of [Fermat pseudoprime](../../../../../../fermat-pseudoprime.md), $M$ is composite as well as odd, and $M\mid2^{M-1}-1$. Put $L=2^M-1$. A proper factorization $M=ab$ makes $2^a-1$ a proper divisor of $L$, so $L$ is composite. Now

$$
L-1=2d,\qquad d=2^{M-1}-1\text{ odd},\qquad M\mid d.
$$

Since $2^M\equiv1\pmod L$, $2^d\equiv1\pmod L$. This is the first passing condition of the [Miller-Rabin primality test](../../../../../../miller-rabin-primality-test.md), with $s=1$. Thus **$2^M-1$ is a base-two [strong pseudoprime](../../../../../../strong-pseudoprime.md)**. If “pseudoprime” were used to include [primes](../../../../../../prime-number.md), the compositeness conclusion would fail, for instance $M=3$ gives $L=7$; the standard composite definition matters.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11G](../../11g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
