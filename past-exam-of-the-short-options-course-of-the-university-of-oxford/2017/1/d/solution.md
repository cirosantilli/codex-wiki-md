<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) says that for pairwise [coprime](../../../../coprime-integers.md) positive moduli $m_1,\ldots,m_r$ and arbitrary [integers](../../../../integer-split.md) $a_1,\ldots,a_r$, the simultaneous [modular congruences](../../../../modular-congruence.md)

$$
n\equiv a_i\pmod{m_i}\qquad(1\leq i\leq r)
$$

have a solution, unique modulo $M=\prod_i m_i$.

Choose $2017$ distinct [prime numbers](../../../../prime-number-split.md) $q_1,\ldots,q_{2017}$. Their [prime powers](../../../../prime-power.md) $q_i^{2017}$ are pairwise [coprime](../../../../coprime-integers.md). Apply the [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) to

$$
\boxed{n\equiv-i\pmod{q_i^{2017}}\qquad(1\leq i\leq2017).}
$$

For the resulting [integer](../../../../integer-split.md) $n$, each $n+i$ is divisible by $q_i^{2017}$, the required power of an [integer](../../../../integer-split.md) greater than one. Adding a sufficiently large multiple of $\prod_iq_i^{2017}$ makes $n$ positive without changing any [modular congruence](../../../../modular-congruence.md). Thus **such a positive $n$ exists**, indeed infinitely many do. This is the general construction of [consecutive integers divisible by prescribed prime powers](../../../../consecutive-integers-divisible-by-prescribed-prime-powers.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
