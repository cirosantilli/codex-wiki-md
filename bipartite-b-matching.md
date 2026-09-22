# Bipartite b-matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory-split.md)

For a [bipartite graph](bipartite-graph-split.md) with [bipartition](bipartition-of-a-graph.md) $L,R$ and [nonnegative integer](natural-number.md) bounds $b_v$, a [bipartite b-matching](bipartite-b-matching.md) is an [edge](edge-of-a-graph.md) [subset](subset.md) $F$ whose [degree of a vertex](degree-graph-theory.md) is at most $b_v$ at each $v$. Taking $b_v=1$ gives a [matching in a graph](matching-graph-theory-split.md). To maximize $|F|$, build a [flow network](flow-network-split.md) with arcs $s\to u$ of [flow network edge capacity](flow-network-edge-capacity.md) $b_u$ for $u\in L$, arcs $u\to v$ of [flow network edge capacity](flow-network-edge-capacity.md) one for $uv\in E$, and arcs $v\to t$ of [flow network edge capacity](flow-network-edge-capacity.md) $b_v$ for $v\in R$. The [integral max-flow theorem](integral-max-flow-theorem.md) gives an integral optimum. Select precisely the middle arcs with [flow](flow.md) one. [Flow conservation](flow-conservation.md) identifies their endpoint degrees with the outside arc [flows](flow.md), and the [flow value](strength-of-a-flow.md) is $|F|$. Conversely, every such [edge](edge-of-a-graph.md) [subset](subset.md) supplies a [feasible flow](feasible-flow.md) of that value. This proves the reduction and its optimality.

## ↑ Ancestors (6)

1. [Matching (graph theory)](matching-graph-theory-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bipartite b-matching](bipartite-b-matching.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/1/c/solution.md)
- [Path-cycle matching](path-cycle-matching.md)
