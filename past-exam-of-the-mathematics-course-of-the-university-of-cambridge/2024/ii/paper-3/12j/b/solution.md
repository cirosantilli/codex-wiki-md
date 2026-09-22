<h1 id="12j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let a deterministic automaton for $L$ have $p$ states. During the first $p$ input symbols of an accepted word $w$ of length at least $p$, the run visits $p+1$ states, so two coincide. Write $w=xyz$ so that $y$ labels the nonempty loop between those visits and $|xy|\leq p$. Traversing that loop any number of times leaves the remainder of the accepting run unchanged, giving $xy^iz\in L$ for every $i\geq0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12J](../../12j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
