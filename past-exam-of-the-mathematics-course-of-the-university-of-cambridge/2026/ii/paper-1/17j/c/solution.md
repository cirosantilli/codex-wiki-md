<h1 id="17j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume no deletion works. For each $x\in A_i$, some $A_j$ contains $A_i\setminus\{x\}$; otherwise deleting $x$ preserves the [antichain](../../../../../../antichain.md). For different deleted elements these witnesses are distinct, since one witness containing both complements would contain $A_i$. Thus every element of $A_i$ belongs to at least $|A_i|$ sets.

Use the incidence graph with left class $\bigcup_iA_i$ and right class $\{A_i\}$. Along every incidence edge, the degree of the element is at least the degree $|A_i|$ of the set vertex. Part (b) gives a matching from the union into the $k$ sets, forcing $|\bigcup_iA_i|\le k$, a contradiction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17J](../../17j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
