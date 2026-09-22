<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

For every [prime](../../../../../prime-number.md) factor $p_i$ of $N$, [Fermat's little theorem](../../../../../fermat-little-theorem.md) gives $a^{p_i-1}\equiv1\pmod{p_i}$. Since $p_i-1$ divides the [least common multiple](../../../../../least-common-multiple.md) $\lambda(N)$, it follows that $p_i\mid a^{\lambda(N)}-1$. The [primes](../../../../../prime-number.md) are distinct and hence pairwise [coprime](../../../../../coprime-integers.md), so their product divides this integer. Thus

$$
\boxed{a^{\lambda(N)}\equiv1\pmod N.}
$$

For the specified product, $N=1729$ and $\lambda(N)=\operatorname{lcm}(6,12,18)=36$. Since $N-1=1728=48\cdot36$, raising the preceding [modular congruence](../../../../../modular-congruence.md) to the forty-eighth power proves $a^{N-1}\equiv1\pmod N$ for every $a$ [coprime](../../../../../coprime-integers.md) to $N$. This is the defining phenomenon of a [Carmichael number](../../../../../carmichael-number.md).

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
