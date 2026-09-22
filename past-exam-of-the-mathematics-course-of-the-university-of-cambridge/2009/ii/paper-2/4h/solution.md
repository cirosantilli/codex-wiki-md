<h1 id="4h/solution">Solution</h1>

↑ **Parent:** [4H](../4h.md)

The supplied congruence is a [congruence of squares](../../../../../congruence-of-squares.md), since $25=5^2$. Hence

$$
3953\mid(2886-5)(2886+5).
$$

A nontrivial square root modulo a product of two odd primes may agree with $+5$ modulo one prime and $-5$ modulo the other. Taking greatest common divisors separates these factors. The [Euclidean algorithm](../../../../../euclidean-algorithm.md) gives

$$
\gcd(3953,2881)=67,\qquad\gcd(3953,2891)=59.
$$

For example the successive remainders for the first computation are $1072,737,335,67,0$; for the second they are $1062,767,295,177,118,59,0$. Therefore

$$
\boxed{3953=59\cdot67.}
$$

Both numbers are prime by trial division by primes at most their square roots. More generally, given $a^2\equiv b^2\pmod N$ with $a\not\equiv\pm b\pmod N$, computing $\gcd(N,a-b)$ often produces a proper factor. The method requires no prior knowledge of which prime gives which sign, and is the basic factor-extraction step in congruence-of-squares algorithms.

## ↑ Ancestors (10)

1. [4H](../4h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
