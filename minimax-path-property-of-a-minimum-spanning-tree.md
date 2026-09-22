# Minimax path property of a minimum spanning tree

↑ **Parent:** [Minimum spanning tree](minimum-spanning-tree.md)

Every path in a [minimum spanning tree](minimum-spanning-tree.md) solves the [bottleneck shortest path problem](bottleneck-shortest-path-problem.md) between its endpoints. If $e$ is a maximum-weight edge on the tree path, deleting it gives a [graph cut](graph-cut.md) separating the endpoints. A competing path with every edge lighter than $e$ would contain a crossing edge $f$; replacing $e$ with $f$ would decrease the tree's total weight, a contradiction. Equal weights cause no problem: the argument excludes a strictly smaller bottleneck and does not require a unique tree.

## ↑ Ancestors (7)

1. [Minimum spanning tree](minimum-spanning-tree.md)
2. [Spanning tree](spanning-tree.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bottleneck shortest path problem](bottleneck-shortest-path-problem.md)
- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2023/7/b/iii/solution.md)
