# Union of two matchings

↑ **Parent:** [Matching (graph theory)](matching-graph-theory-split.md)

In the spanning [subgraph](subgraph.md) formed by the union of two [matchings in a graph](matching-graph-theory-split.md) $M_1,M_2$, every [vertex](vertex-graph-theory.md) has [vertex degree](degree-graph-theory.md) at most two. A common [edge](edge-of-a-graph.md) is an isolated two-[vertex](vertex-graph-theory.md) [connected component of a graph](component-graph-theory.md). Every other nontrivial [connected component of a graph](component-graph-theory.md) is a [graph path](path-in-a-graph.md) or an even [graph cycle](cycle-in-a-graph.md), with the [edges](edge-of-a-graph.md) alternating between the two [matchings in a graph](matching-graph-theory-split.md).

Suppose the original [graph](graph-split.md) is a [bipartite graph](bipartite-graph-split.md) with [vertex sets](vertex-set.md) $A,B$, $M_1$ covers a specified [subset](subset.md) $X\subseteq A$, and $M_2$ covers a specified [subset](subset.md) $Y\subseteq B$. Their union contains a [matching in a graph](matching-graph-theory-split.md) covering $X\cup Y$. On an even [graph cycle](cycle-in-a-graph.md), either alternating choice covers every [vertex](vertex-graph-theory.md). On an odd-length [graph path](path-in-a-graph.md), the larger alternating choice covers every [vertex](vertex-graph-theory.md). On an even-length [graph path](path-in-a-graph.md), both endpoints lie in the same side: choose $M_1$ if they lie in $A$, or $M_2$ if they lie in $B$. Every required endpoint is covered by that choice, and every internal [vertex](vertex-graph-theory.md) meets both choices. Select each common [edge](edge-of-a-graph.md) as well; isolated [vertices](vertex-graph-theory.md) are not in $X\cup Y$. Different [connected components of a graph](component-graph-theory.md) do not interfere.

## ↑ Ancestors (6)

1. [Matching (graph theory)](matching-graph-theory-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Matching covering maximum-degree vertices in a bipartite graph](matching-covering-maximum-degree-vertices-in-a-bipartite-graph.md)
- [Solution](past-exam-of-the-graph-theory-course-of-the-university-of-oxford/2023/1/b/ii/solution.md)
