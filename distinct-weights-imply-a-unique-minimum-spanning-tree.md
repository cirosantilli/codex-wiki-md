# Distinct weights imply a unique minimum spanning tree

↑ **Parent:** [Minimum spanning tree](minimum-spanning-tree.md)

For a finite connected weighted graph with distinct [edge](edge-of-a-graph.md) weights, [Kruskal's algorithm](kruskal-s-algorithm.md) produces the unique [minimum spanning tree](minimum-spanning-tree.md). If another optimal tree existed, take an [edge](edge-of-a-graph.md) belonging only to the algorithm's tree and slightly increase its weight without changing the strict [edge](edge-of-a-graph.md) order. The algorithm then returns exactly the same tree, which must still be optimal, but the other tree's weight is unchanged and is now strictly smaller, a contradiction. Distinct weights are sufficient, not necessary: a triangle with weights $1,1,2$ has a unique optimum formed from the two weight-one [edges](edge-of-a-graph.md).

## ↑ Ancestors (7)

1. [Minimum spanning tree](minimum-spanning-tree.md)
2. [Spanning tree](spanning-tree.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/8/d/solution.md)
