# Minimum-weight acyclic subgraph

↑ **Parent:** [Minimum spanning forest](minimum-spanning-forest.md)

Among all [acyclic graphs](forest.md) contained in a finite weighted [undirected graph](undirected-graph.md), with no requirement to connect [vertices](vertex-graph-theory.md), one optimum is obtained by keeping only strictly negative [edges](edge-of-a-graph.md) and computing their [minimum spanning forest](minimum-spanning-forest.md). Removing a nonnegative [edge](edge-of-a-graph.md) never worsens weight or creates a cycle. Within a connected component of the negative-edge subgraph, any disconnected candidate [forest](forest.md) can be extended by a negative crossing [edge](edge-of-a-graph.md), strictly improving its weight. Hence an optimum must span each such component and minimise its tree weight. [Kruskal's algorithm](kruskal-s-algorithm.md) on the negative [edges](edge-of-a-graph.md) therefore solves the problem. Zero-weight [edges](edge-of-a-graph.md) are optional when they preserve acyclicity.

## ↑ Ancestors (7)

1. [Minimum spanning forest](minimum-spanning-forest.md)
2. [Forest](forest.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/8/c/solution.md)
