# Depth-first approximation for connected vertex cover

↑ **Parent:** [Connected vertex cover](connected-vertex-cover.md)

For a nontrivial [connected graph](connected-graph.md), return the [internal vertices of a rooted tree](internal-vertex-of-a-rooted-tree.md) in a [depth-first search](depth-first-search.md) tree. Undirected [depth-first search](depth-first-search.md) has only ancestor-descendant [edges](edge-of-a-graph.md), so every [edge](edge-of-a-graph.md) meets an internal [vertex](vertex-graph-theory.md); the internal [vertices](vertex-graph-theory.md) are connected along parent paths. For a maximum-size [proper matching in a rooted tree](proper-matching-in-a-rooted-tree.md) $M$ of that tree, existence of which is assumed, $|I|=|V|-|L|\leq|V|-|U(M)|=2|M|$. Every [vertex cover](vertex-cover.md) has size at least $|M|$, proving the factor two. The implementation needs only [depth-first search](depth-first-search.md), hence linear [time complexity](time-complexity.md); it does not compute the analysis [matching in a graph](matching-graph-theory-split.md).

## ↑ Ancestors (7)

1. [Connected vertex cover](connected-vertex-cover.md)
2. [Vertex cover](vertex-cover.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
