<h1 id="17j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A matching from $X$ to $Y$ consists of disjoint edges saturating every vertex of $X$. The criterion is [Hall marriage theorem](../../../../../../hall-s-marriage-theorem.md).

For sufficiency, induct on $|X|$. If a nonempty proper $S\subset X$ is tight, $|N(S)|=|S|$, apply induction to $S,N(S)$ and to the graph left after deleting them. If no proper set is tight, choose any edge $xy$, delete its endpoints, and Hall still holds because every nonempty proper subset formerly had at least one spare neighbour. Induction completes the matching. Necessity is immediate.

## ↑ Ancestors (11)

1. [A](../a.md)
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
