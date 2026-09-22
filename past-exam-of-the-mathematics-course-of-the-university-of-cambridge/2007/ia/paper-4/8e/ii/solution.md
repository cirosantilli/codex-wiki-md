<h1 id="8e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Fermat-Euler theorem](../../../../../../euler-s-theorem.md) states that, for a positive [integer](../../../../../../integer.md) $q$ and an [integer](../../../../../../integer.md) $a$ coprime to $q$, $a^{\varphi(q)}\equiv1\pmod q$, where the [Euler totient function](../../../../../../euler-totient-function.md) $\varphi(q)$ counts residue classes coprime to $q$. The case $q=1$ is trivial. For $q>1$, let $r_1,\ldots,r_{\varphi(q)}$ be a [reduced residue system](../../../../../../reduced-residue-system.md). Multiplication by $a$ permutes it: equality of two resulting residues can be cancelled using the modular inverse of $a$, and the products remain coprime to $q$. Multiplying the residues before and after the permutation gives

$$
a^{\varphi(q)}r_1\cdots r_{\varphi(q)}\equiv r_1\cdots r_{\varphi(q)}\pmod q.
$$

Every factor on the right is a unit, so its product can be cancelled. This proves

$$
\boxed{a^{\varphi(q)}\equiv1\pmod q.}
$$

The [integer](../../../../../../integer.md) $359$ is [prime](../../../../../../prime-number.md): none of the [primes](../../../../../../prime-number.md) $2,3,5,7,11,13,17$ up to $\sqrt{359}<19$ divides it. Therefore $\varphi(359)=358$. Apply the theorem to $60$ and use the supplied congruence:

$$
10^{179}\equiv(60^2)^{179}=60^{358}\equiv1\pmod{359}.
$$

To connect this to individual digits rather than merely assert periodicity, use long-division remainders $r_0=1$ and

$$
10r_{n-1}=359a_n+r_n,\qquad0\le r_n<359.
$$

Induction gives $r_n\equiv10^n\pmod{359}$. Since $10$ is coprime to $359$, no remainder is zero. The congruence above therefore implies $r_{n+179}=r_n$ for every $n\ge0$, using the unique representative in $1,\ldots,358$. In particular

$$
a_{n+179}=\left\lfloor\frac{10r_{n+178}}{359}\right\rfloor
=\left\lfloor\frac{10r_{n-1}}{359}\right\rfloor=a_n.
$$

Hence

$$
\boxed{a_{n+179}=a_n\quad(n\ge1).}
$$

This is the mechanism of [decimal period from multiplicative order](../../../../../../decimal-period-from-multiplicative-order.md): the period divides $179$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
