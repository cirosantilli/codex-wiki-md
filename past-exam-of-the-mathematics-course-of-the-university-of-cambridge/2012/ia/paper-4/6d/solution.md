<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

[Fermat's little theorem](../../../../../fermat-little-theorem.md) says that for a prime $p$ and $p\nmid a$, $a^{p-1}\equiv1\pmod p$; equivalently $a^p\equiv a\pmod p$ for every [integer](../../../../../integer.md) $a$. The [Wilson theorem](../../../../../wilson-s-theorem.md) says $(p-1)!\equiv-1\pmod p$ for a prime $p$ (and, conversely, this congruence characterizes primes among [integers](../../../../../integer.md) greater than one).

For $p=2$, $x=1$ is a [square root of minus one modulo a prime](../../../../../square-root-of-minus-one-modulo-a-prime.md). If $p$ is odd and $x^2\equiv-1$, [Fermat's little theorem](../../../../../fermat-little-theorem.md) gives

$$
1\equiv x^{p-1}=(-1)^{(p-1)/2}\pmod p,
$$

so $(p-1)/2$ is even and $p\equiv1\pmod4$. Conversely, put $h=(p-1)/2$. Pairing $j$ with $p-j$ in the [factorial](../../../../../factorial.md) gives $(p-1)!\equiv(-1)^h(h!)^2$. For $p\equiv1\pmod4$, $h$ is even, so the [Wilson theorem](../../../../../wilson-s-theorem.md) yields $(h!)^2\equiv-1$. Thus

$$
\boxed{p=2\text{ or }p\equiv1\pmod4,}
$$

and in the latter case $x=h!$ supplies a solution.

For the [multiplicative order](../../../../../multiplicative-order.md) assertion, divide $k$ by $d$: $k=qd+r$, $0\leq r<d$. Since $x^d\equiv1$ and $x^k\equiv1$, it follows that $x^r\equiv1$. Minimality of the positive order excludes $0<r<d$, hence $r=0$ and

$$
\boxed{d\mid k.}
$$

In particular $d\mid p-1$ by [Fermat's little theorem](../../../../../fermat-little-theorem.md). Negative $k$, if included, are handled by the same division using the modular inverse of $x$.

A [Fermat number](../../../../../fermat-number.md) in the paper has $n\geq1$. If a prime $p$ divides $F_n=2^{2^n}+1$, it is odd and $2^{2^n}\equiv-1\pmod p$. Squaring gives $2^{2^{n+1}}\equiv1$, so the order $d$ divides $2^{n+1}$. It does not divide $2^n$, since $-1\ne1$ modulo an odd prime. Every divisor of $2^{n+1}$ is a power of two, so the only possibility is

$$
\boxed{\operatorname{ord}_p(2)=2^{n+1}.}
$$

If two different [Fermat numbers](../../../../../fermat-number.md) shared a [prime factor](../../../../../prime-factor.md), the same element $2$ modulo that prime would have two different orders. This is impossible, proving pairwise [coprimality](../../../../../coprime-integers.md). Also $2^{n+1}\mid p-1$, so for $n\geq1$ every such prime is $1$ modulo $4$. No prime $3$ modulo $4$ can occur.

A prime $1$ modulo $4$ need not occur: take **$p=13$**. It is prime, $2^6=64\equiv-1\pmod{13}$, and $2^4\equiv3\ne1$. Since the order divides $12$, the first congruence excludes every divisor of $6$ and the second excludes $4$; hence the order is $12$. This is not a power of two, so $13$ is not a [prime divisor of a Fermat number](../../../../../prime-divisor-of-a-fermat-number.md). The index restriction matters: the conventional extra number $F_0=3$ is outside the paper's positive-$n$ family.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
