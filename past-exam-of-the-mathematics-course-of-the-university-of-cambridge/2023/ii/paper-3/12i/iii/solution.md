<h1 id="12i/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $0\leq j\leq9$, consider the ten prefixes

$$
u_j=b^j.
$$

If $0\leq i<j\leq9$, append

$$
z_j=b^{11-j}a.
$$

Then

$$
u_i z_j=b^{i+11-j}a\in L,
$$

because $i+11-j\leq10$, whereas

$$
u_jz_j=b^{11}a\notin L.
$$

Indeed, in a word ending in one $a$, the prefix before the final positive run of $a$'s must have length at most ten. Hence every pair $u_i,u_j$ is distinguished by some suffix. They occupy ten distinct [Myhill-Nerode equivalence](../../../../../../myhill-nerode-equivalence.md) classes, so the [minimal deterministic finite automaton](../../../../../../minimal-deterministic-finite-automaton.md) for $L$ has at least ten states.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [12I](../../12i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
