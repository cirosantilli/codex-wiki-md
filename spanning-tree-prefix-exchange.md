# Spanning-tree prefix exchange

↑ **Parent:** [Spanning tree](spanning-tree.md)

Suppose two [spanning trees](spanning-tree.md) have the same first $n$ edges in nondecreasing weight order. If the first tree's next edge $e$ is no heavier than the second tree's next edge, it can be inserted into the second tree while preserving the common prefix and without increasing any sorted edge weight. If $e$ already occurs there, it ties for the next position. Otherwise its [fundamental cycle](fundamental-cycle.md) contains an edge $f$ outside the prefix, since the prefix together with $e$ is acyclic. Every such $f$ is at least as heavy as $e$. Exchanging $f$ for $e$ preserves the [spanning tree](spanning-tree.md). Replacing a multiset entry by a no-larger entry cannot increase any [order statistic](order-statistic.md). Tied edges can be ordered to preserve the prescribed prefix.

## ↑ Ancestors (6)

1. [Spanning tree](spanning-tree.md)
2. [Tree (graph theory)](tree-graph-theory-split.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/8/c/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/8/c/ii/solution.md)
