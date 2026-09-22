<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

For $b>1$, [Euler's theorem](../../../../../euler-s-theorem.md) allows $d=\varphi(b)>0$, since $a,b$ are [coprime integers](../../../../../coprime-integers.md). At $b=1$ every congruence holds and one may take $d=1$. Let $y$ be the [multiplicative order](../../../../../multiplicative-order.md) of $a$ modulo $b$. Write a nonnegative exponent $x=qy+r$ with $0\le r<y$ using the [Euclidean division](../../../../../euclidean-division.md). Then $a^x\equiv a^r\pmod b$, so $a^x\equiv1$ implies $r=0$ by minimality of $y$. Thus $y\mid x$. Negative exponents, if included, give the same conclusion using the inverse residue of $a$.

A [prime divisor of a Fermat number](../../../../../prime-divisor-of-a-fermat-number.md) $F_n=2^{2^n}+1$ is odd, and satisfies $2^{2^n}\equiv-1\pmod p$. Therefore $2^{2^{n+1}}\equiv1\pmod p$, so its [multiplicative order](../../../../../multiplicative-order.md) divides $2^{n+1}$. It does not divide $2^n$, since $-1\ne1$ modulo the odd prime. Every divisor of $2^{n+1}$ is a power of two, hence

$$
\boxed{\operatorname{ord}_p(2)=2^{n+1}}.
$$

By [Fermat's little theorem](../../../../../fermat-little-theorem.md) and the divisibility just proved, $2^{n+1}\mid p-1$, giving $\boxed{p\equiv1\pmod{2^{n+1}}}$.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
