<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For distinct [prime numbers](../../../../../../prime-number-split.md) $p,q$, compute the [Euler totient function](../../../../../../euler-totient-function.md)

$$
\varphi(n)=(p-1)(q-1).
$$

The [RSA cryptosystem](../../../../../../rsa-cryptosystem.md) private exponent is a [modular multiplicative inverse](../../../../../../modular-multiplicative-inverse.md) of the public exponent:

$$
\boxed{d\equiv 3^{-1}\pmod{\varphi(n)},\qquad 3d\equiv1\pmod{\varphi(n)}.}
$$

Use the [extended Euclidean algorithm](../../../../../../extended-euclidean-algorithm.md) on $3$ and $\varphi(n)$. It produces [integers](../../../../../../integer-split.md) $u,v$ with $3u+\varphi(n)v=1$, and reducing $u$ modulo $\varphi(n)$ gives a suitable positive $d$. Searching through possible exponents is unnecessary.

To see correctness even for a [plaintext](../../../../../../plaintext.md) sharing a factor with $n$, write $3d=1+t\varphi(n)$. Modulo $p$, either $m=0$ or [Fermat's little theorem](../../../../../../fermat-little-theorem.md) gives $m^{3d}=m$; the same holds modulo $q$. The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) then gives $c^d=m\pmod n$. One may alternatively invert $3$ modulo $\operatorname{lcm}(p-1,q-1)$, but inversion modulo $\varphi(n)$ is sufficient for this paper.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
