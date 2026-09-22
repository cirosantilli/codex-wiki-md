<h1 id="2e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The integer $137$ is prime: none of the primes $2,3,5,7,11$ below $\sqrt{137}$ divides it. Since $43\not\equiv0\pmod{137}$, [Fermat's little theorem](../../../../../../fermat-little-theorem.md) gives $43^{136}\equiv1$. Therefore $43^{135}$ is the [modular inverse](../../../../../../modular-multiplicative-inverse.md) of $43$. The [extended Euclidean algorithm](../../../../../../extended-euclidean-algorithm.md) yields

$$
137=3(43)+8,\quad43=5(8)+3,\quad8=2(3)+2,\quad3=2+1,
$$

and back-substitution gives $1=51(43)-16(137)$. Consequently

$$
\boxed{43^{135}\equiv51\pmod{137}.}
$$

Indeed, $43\cdot51=2193=16\cdot137+1$, directly checking the required [modular inverse](../../../../../../modular-multiplicative-inverse.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2E](../../2e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
