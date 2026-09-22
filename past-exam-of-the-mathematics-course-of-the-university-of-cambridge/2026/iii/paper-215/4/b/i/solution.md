<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For any two states $X,Y$, the closed neighbourhood of $X\cup Y$ has at most $2s(\Delta+1)\leq2n/3$ vertices. The remaining induced graph therefore has at least $n/3$ vertices and maximum degree at most $\Delta$, so the [greedy independent-set bound](../../../../../../../greedy-independent-set-bound.md) supplies an independent set $Z$ of size $s$ there. No vertex of $Z$ is adjacent to a vertex of $X\cup Y$. Replace the elements of $X$ one at a time by the elements of $Z$, and then replace the elements of $Z$ one at a time by those of $Y$. Every intermediate set is independent, and every prescribed swap has positive transition probability. Hence the chain is irreducible.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 215](../../../../paper-215-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
