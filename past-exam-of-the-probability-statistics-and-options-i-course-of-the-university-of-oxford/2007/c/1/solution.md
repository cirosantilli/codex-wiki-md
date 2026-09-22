<h1 id="c/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Euler's theorem](../../../../euler-s-theorem.md) states that if $\gcd(a,m)=1$, then $a^{\phi(m)}\equiv1\pmod m$, where $\phi$ is [Euler's totient function](../../../../euler-totient-function.md). This includes [Fermat's little theorem](../../../../fermat-little-theorem.md) when $m$ is prime.

For each prime-power factor $p_i^{e_i}$, the integer $\phi(p_i^{e_i})$ divides the defined [least common multiple](../../../../least-common-multiple.md) $\lambda(m)$. [Euler's theorem](../../../../euler-s-theorem.md) modulo that prime power therefore gives

$$
a^{\lambda(m)}
=\left(a^{\phi(p_i^{e_i})}\right)^{\lambda(m)/\phi(p_i^{e_i})}
\equiv1\pmod{p_i^{e_i}}.
$$

The prime powers are pairwise coprime, so their product divides $a^{\lambda(m)}-1$. Equivalently the [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) gives

$$
\boxed{a^{\lambda(m)}\equiv1\pmod m.}
$$

For the specified composite integer,

$$
\lambda(561)=\operatorname{lcm}(2,10,16)=80,
\qquad560=7\cdot80.
$$

Raising $a^{80}\equiv1\pmod{561}$ to the seventh power proves

$$
\boxed{a^{560}\equiv1\pmod{561}\quad(\gcd(a,561)=1).}
$$

Thus 561 is a [Carmichael number](../../../../carmichael-number.md). We use exactly the source's definition of $\lambda$ as the [least common multiple](../../../../least-common-multiple.md) of prime-power totients; its validity here does not require replacing it by a smaller exponent at powers of two.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [C](../../c.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
