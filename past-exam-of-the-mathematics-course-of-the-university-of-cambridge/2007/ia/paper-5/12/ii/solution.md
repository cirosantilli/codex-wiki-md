<h1 id="12/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Fermat-Euler theorem](../../../../../../euler-s-theorem.md) states that for integers $m\ge1$ and $a$ with $\gcd(a,m)=1$,

$$
\boxed{a^{\varphi(m)}\equiv1\pmod m,}
$$

where [Euler's totient function](../../../../../../euler-totient-function.md) $\varphi(m)$ counts the residue classes coprime to $m$. The case $m=1$ is trivial. For $m\ge2$, list a reduced residue system $r_1,\ldots,r_{\varphi(m)}$. Multiplication by $a$ permutes these classes: each $ar_i$ is coprime to $m$, and $ar_i\equiv ar_j$ implies $r_i\equiv r_j$ since $a$ has a multiplicative inverse modulo $m$. Multiplying the permuted residues gives

$$
a^{\varphi(m)}\prod_i r_i\equiv\prod_i r_i\pmod m.
$$

The product is itself coprime to $m$ and can be cancelled using its inverse, proving the theorem.

The integer 359 is prime: none of the primes $2,3,5,7,11,13,17$, all the primes not exceeding $\sqrt{359}<19$, divides it. Therefore $\varphi(359)=358$ and 60 is coprime to 359. Using the supplied congruence and the [Fermat-Euler theorem](../../../../../../euler-s-theorem.md),

$$
\boxed{10^{179}\equiv(60^2)^{179}=60^{358}\equiv1\pmod{359}.}
$$

Now express the decimal expansion by long division. Put $r_0=1$ and for $n\ge1$ define

$$
10r_{n-1}=359a_n+r_n,\qquad 0\le a_n\le9,\quad0\le r_n<359.
$$

Thus $r_n\equiv10^n\pmod{359}$, and none of these remainders is zero. The congruence $10^{179}\equiv1$ implies $r_{n+179}\equiv r_n$; since both are the unique representatives between zero and 358, they are equal. A digit is determined by the preceding remainder, namely $a_n=\lfloor10r_{n-1}/359\rfloor$, so

$$
\boxed{a_{n+179}=a_n\quad\text{for every }n\ge1.}
$$

This proves the required pure periodicity from the first digit. In fact its least period is 179: the [multiplicative order](../../../../../../multiplicative-order.md) of 10 modulo 359 divides the prime 179 and is not one, since $10\not\equiv1\pmod{359}$. The connection between the remainder recurrence and the period is the [decimal period from multiplicative order](../../../../../../decimal-period-from-multiplicative-order.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12](../../12.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
