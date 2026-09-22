# Shortest cycle by repeated shortest-path trees

↑ **Parent:** [Shortest path problem](shortest-path-problem-split.md)

In a positive-weight [directed graph](directed-graph.md), run the [Dijkstra algorithm](dijkstra-algorithm.md) from each source $s$ and minimize $d_s(u)+w(u,s)$ over closing [edges](edge-of-a-graph.md). In an [undirected graph](undirected-graph.md), minimize $d_s(u)+w(u,v)+d_s(v)$ only over [edges](edge-of-a-graph.md) absent from the current [shortest-path tree](shortest-path-tree.md). A [tree](tree-graph-theory-split.md) [edge](edge-of-a-graph.md) would otherwise give a spurious traversal out and back. A non-tree candidate contains a genuine cycle no longer than its score, even when the two [tree](tree-graph-theory-split.md) routes share a prefix.

For the undirected optimum, choose a shortest cycle and a source on it. If an incident cycle [edge](edge-of-a-graph.md) is absent from the [tree](tree-graph-theory-split.md), its candidate is bounded by the cycle length. Otherwise its two neighbours lie in distinct [tree](tree-graph-theory-split.md) branches, and some [edge](edge-of-a-graph.md) on the remaining cycle segment crosses branches. That [edge](edge-of-a-graph.md) is non-tree; shortest distances to its endpoints are bounded by the two complementary cycle segments, again giving a candidate no greater than the optimum. Thus the minimum candidate equals the shortest-cycle length. Repeated [Dijkstra algorithm](dijkstra-algorithm.md) runs take $O((|V|^2+|V||E|)\log(|V|+1))$ [running time](running-time.md) with a [binary heap](binary-heap.md).

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/8/b/solution.md)
