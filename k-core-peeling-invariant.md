# K-core peeling invariant

↑ **Parent:** [Graph theory](graph-theory-split.md)

During repeated deletion of vertices of current degree below $k$, every subgraph of minimum degree at least $k$ is contained in the active induced subgraph. If an active vertex has degree below $k$, its degree in any subgraph of the active graph is no greater, so no candidate can contain it. This proves the invariant inductively. A queue of threshold crossings and [adjacency lists](adjacency-list.md) implements peeling in $O(|V|+|E|)$ time.

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [K-core](k-core.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/7/d/solution.md)
