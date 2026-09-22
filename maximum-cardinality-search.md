# Maximum cardinality search

↑ **Parent:** [Perfect elimination ordering](perfect-elimination-ordering.md)

[Maximum cardinality search](maximum-cardinality-search.md) is a [graph](graph-split.md) search in which an unselected [vertex](vertex-graph-theory.md)'s score counts its already selected [graph neighbours](neighbour-of-a-vertex.md). Repeatedly select a [vertex](vertex-graph-theory.md) of maximum score, breaking ties arbitrarily, and update its unselected [graph neighbours](neighbour-of-a-vertex.md). On a [chordal graph](chordal-graph.md), the reverse selection order is a [perfect elimination ordering](perfect-elimination-ordering.md). On $C_4$, selecting $(a,b,c,d)$ instead yields candidate deletion order $(d,c,b,a)$; $d$'s later [graph neighbours](neighbour-of-a-vertex.md) $a,c$ are not adjacent, so the [clique](clique-graph-theory.md) check fails.[§4.2; Algorithm 4.2](chordal-graphs-and-semidefinite-optimization-by-lieven-vandenberghe-and-others.md)

## ↑ Ancestors (7)

1. [Perfect elimination ordering](perfect-elimination-ordering.md)
2. [Chordal graph](chordal-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Maximum cardinality search](maximum-cardinality-search.md)
- [Perfect elimination ordering](perfect-elimination-ordering.md)
