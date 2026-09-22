<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First test for an [isolated vertex](../../../../../../isolated-vertex.md), reporting infeasibility if one exists. Otherwise compute a [maximum cardinality matching](../../../../../../maximum-cardinality-matching.md) $M$ using a general-[graph](../../../../../../graph-split.md) [polynomial-time algorithm](../../../../../../polynomial-time-algorithm.md), then add one arbitrary incident [edge](../../../../../../edge-of-a-graph.md) for each [unmatched vertex in a matching](../../../../../../unmatched-vertex-in-a-matching.md). The proof in (i) shows that the resulting [edge cover](../../../../../../edge-cover.md) has **minimum [cardinality](../../../../../../cardinality.md) $|V|-|M|$**.

The final scan takes $O(|V|+|E|)$ time with [adjacency lists](../../../../../../adjacency-list.md); the [maximum cardinality matching](../../../../../../maximum-cardinality-matching.md) computation is polynomial. One may obtain it from a general-[graph](../../../../../../graph-split.md) [maximum-weight matching](../../../../../../maximum-weight-matching.md) routine with every weight equal to one.[max\_weight\_matching, unit weights give maximum cardinality; Notes: cubic vertex-count running time](../../../../../../maximum-weight-matching-documentation-by-networkx.md)

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Combinatorial optimisation](../../../../combinatorial-optimisation-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
