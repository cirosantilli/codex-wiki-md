<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

If $m$ and $n$ are [coprime](../../../../../coprime-integers.md), every divisor of $mn$ is uniquely $ab$ with $a\mid m$ and $b\mid n$. Hence, for a [multiplicative arithmetic function](../../../../../multiplicative-function.md) $f$,

$$
g(mn)=\sum_{a\mid m}\sum_{b\mid n}f(ab)
=\left(\sum_{a\mid m}f(a)\right)
 \left(\sum_{b\mid n}f(b)\right)=g(m)g(n).
$$

The [Möbius function](../../../../../mobius-function.md) is $\mu(n)=0$ if a prime square divides $n$, and $\mu(n)=(-1)^r$ if $n$ is a product of $r$ distinct primes. The [Euler totient function](../../../../../euler-totient-function.md) $\phi(n)$ counts residues modulo $n$ coprime to $n$. From the prime factorizations,

$$
\frac{\phi(n)}n=\prod_{p\mid n}\left(1-\frac1p\right)
=\sum_{d\mid n}\frac{\mu(d)}d.
$$

Both sides of the second identity are multiplicative, and at a prime power $p^a$,

$$
\sum_{d\mid p^a}\frac{\mu(d)^2}{\phi(d)}
=1+\frac1{p-1}=\frac p{p-1}
=\frac{p^a}{\phi(p^a)}.
$$

Therefore

$$
\boxed{\frac{n}{\phi(n)}=
\sum_{d\mid n}\frac{\mu(d)^2}{\phi(d)}}.
$$

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
