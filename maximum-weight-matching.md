# Maximum-weight matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory-split.md)

Assign each [edge](edge-of-a-graph.md) $e$ a real benefit $w_e$. A [maximum-weight matching](maximum-weight-matching.md) maximizes $\sum_{e\in M}w_e$ over all [matchings in a graph](matching-graph-theory-split.md) $M$; the empty [matching in a graph](matching-graph-theory-split.md) is allowed. Setting every $w_e=1$ recovers a [maximum cardinality matching](maximum-cardinality-matching.md), but otherwise the objectives can disagree.

On the same [path graph](path-graph.md) $P_4$, give the middle [edge](edge-of-a-graph.md) benefit $3$ and each outer [edge](edge-of-a-graph.md) benefit $1$. The [matching in a graph](matching-graph-theory-split.md) $\{(2,3)\}$ has total benefit $3$, while the two-[edge](edge-of-a-graph.md) [matching in a graph](matching-graph-theory-split.md) $\{(1,2),(3,4)\}$ has total benefit $2$. Thus the smaller choice is the unique [maximum-weight matching](maximum-weight-matching.md). If instead the requirement is to find a [maximum cardinality matching](maximum-cardinality-matching.md) and then maximize benefit among those, the outer [edges](edge-of-a-graph.md) must be chosen. Requiring a [perfect matching](perfect-matching.md) before optimizing cost is another distinct problem, covered by [minimum-weight perfect matching](minimum-weight-perfect-matching.md). With negative benefits a [maximum-weight matching](maximum-weight-matching.md) can even be empty, so it need not be a [maximal matching](maximal-matching.md).

## ↑ Ancestors (6)

1. [Matching (graph theory)](matching-graph-theory-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Augmenting path in a matching](augmenting-path-in-a-matching.md)
- [Matching (graph theory)](matching-graph-theory-split.md)
- [Maximum-weight matching](maximum-weight-matching.md)
- [Stable matching in a bipartite graph](stable-matching-in-a-bipartite-graph.md)
