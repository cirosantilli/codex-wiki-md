# Bottleneck shortest path problem

↑ **Parent:** [Shortest path problem](shortest-path-problem-split.md)

Unlike the sum in the usual [shortest path problem](shortest-path-problem-split.md), the bottleneck cost of a nonempty [graph path](path-in-a-graph.md) is its largest [edge](edge-of-a-graph.md) weight. The optimum is the smallest threshold at which the endpoints become connected by edges of weight at most that threshold. Sorting edges and increasing the threshold, with a [disjoint-set data structure](disjoint-set-data-structure.md) maintaining components, finds this value. The [minimax path property of a minimum spanning tree](minimax-path-property-of-a-minimum-spanning-tree.md) provides a single tree representing such optimal routes for every pair of vertices.

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Minimax path property of a minimum spanning tree](minimax-path-property-of-a-minimum-spanning-tree.md)
- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2023/7/b/ii/solution.md)
- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2023/7/b/iii/solution.md)
