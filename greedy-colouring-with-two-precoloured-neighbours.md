# Greedy colouring with two precoloured neighbours

↑ **Parent:** [Greedy coloring](greedy-coloring.md)

Let $x$ have two nonadjacent [neighbours](neighbour-of-a-vertex.md) $y,z$ in a finite [graph](graph-split.md) $G$, with $G-\{y,z\}$ [connected](connected-space.md). Then $\chi(G)\leq\Delta(G)$. Give $y,z$ one common colour. In a [spanning tree](spanning-tree.md) of the remaining [graph](graph-split.md) rooted at $x$, order [vertices](vertex-graph-theory.md) from larger to smaller [distance](distance.md) from the [root](root-of-a-root-system.md) and colour greedily in that order. Every [vertex](vertex-graph-theory.md) before $x$ has an uncoloured parent, so at most $\Delta(G)-1$ colours are forbidden there. At $x$, the two initial [neighbours](neighbour-of-a-vertex.md) use the same colour, so again at most $\Delta(G)-1$ distinct colours are forbidden. This constructs a proper [colouring](colouring-of-a-set.md) from a palette of $\Delta(G)$ colours. It is a useful local step in [Brooks' theorem](brooks-theorem.md).

## ↑ Ancestors (7)

1. [Greedy coloring](greedy-coloring.md)
2. [Graph coloring](graph-coloring-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2011/a/2/a/ii/solution.md)
- [Solution](past-exam-of-the-graph-theory-course-of-the-university-of-oxford/2011/2/a/ii/solution.md)
