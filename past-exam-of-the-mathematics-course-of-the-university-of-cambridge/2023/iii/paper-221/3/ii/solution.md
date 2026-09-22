<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a distribution faithful to a [Directed acyclic graph](../../../../../../directed-acyclic-graph.md), the smallest Markov blanket of a vertex consists of

- its parents,
- its children, and
- every other parent of one of its children.

Conditioning on this set blocks every path from the vertex to all remaining vertices. Each listed neighbor is necessary under [faithfulness of a directed acyclic graph](../../../../../../faithfulness-of-a-directed-acyclic-graph.md): omitting a parent or child leaves its direct edge active, while omitting a child's other parent leaves the collider path through that conditioned child active. Faithfulness rules out accidental cancellations that could otherwise make a smaller blanket sufficient.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
