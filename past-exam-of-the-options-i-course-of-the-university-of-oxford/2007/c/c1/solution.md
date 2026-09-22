<h1 id="c/c1/solution">Solution</h1>

↑ **Parent:** [C1](../c1.md)

Euler's theorem states that $a^{\phi(m)}\equiv1\pmod m$ whenever $\gcd(a,m)=1$, where $\phi(m)$ counts the invertible [residue](../../../../residue.md) classes. For each prime-power divisor, the same theorem gives $a^{\phi(p_i^{e_i})}\equiv1\pmod{p_i^{e_i}}$. Since the exponent defined in the source is a multiple of every one of these exponents, raising that congruence to the corresponding integer power gives

$$
a^{\lambda(m)}\equiv1\pmod{p_i^{e_i}}.
$$

The prime powers are pairwise [coprime](../../../../coprime-integers.md), so their product divides $a^{\lambda(m)}-1$, proving the congruence modulo $m$.

For the displayed composite integer,

$$
\lambda(561)=\operatorname{lcm}(2,10,16)=80,\qquad560=7\cdot80.
$$

Thus every integer [coprime](../../../../coprime-integers.md) to 561 satisfies $\boxed{a^{560}\equiv1\pmod{561}}$. This is a [Carmichael number](../../../../carmichael-number.md). The source's prime-power least common multiple need not be the minimal universal exponent for all moduli; for powers of two its definition can exceed the usual [Carmichael function](../../../../carmichael-function.md). No minimality claim is needed here.

## ↑ Ancestors (12)

1. [C1](../c1.md)
2. [C](../../c.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
