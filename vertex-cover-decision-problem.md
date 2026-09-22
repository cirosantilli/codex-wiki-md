# Vertex cover decision problem

↑ **Parent:** [Vertex cover](vertex-cover.md)

The [vertex cover decision problem](vertex-cover-decision-problem.md) asks whether a finite [simple graph](simple-graph.md) $G$ has a [vertex cover](vertex-cover.md) containing at most $k$ [vertices](vertex-graph-theory.md). For an uncovered [edge](edge-of-a-graph.md) $uv$, any valid [vertex cover](vertex-cover.md) contains $u$ or $v$. Branch on these two possibilities, delete the chosen [vertex](vertex-graph-theory.md) and its incident [edges](edge-of-a-graph.md), and decrease $k$ by one. An edgeless [graph](graph-split.md) accepts and a nonempty [graph](graph-split.md) with $k=0$ rejects. The [search tree](search-tree.md) has at most $2^k$ leaves, giving [running time](running-time.md) $O(2^k(|V|+|E|))$ with straightforward copying. Thus this parameterization is [fixed-parameter tractable](fixed-parameter-tractability.md).

## ↑ Ancestors (6)

1. [Vertex cover](vertex-cover.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Fixed-parameter tractability](fixed-parameter-tractability.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms/3/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/3/b/solution.md)
- [Vertex cover decision problem](vertex-cover-decision-problem.md)
