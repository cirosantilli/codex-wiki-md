# Kruskal safe edge

↑ **Parent:** [Kruskal's algorithm](kruskal-s-algorithm.md)

An [edge](edge-of-a-graph.md) is safe for the current accepted [forest](forest.md) $F$ if some [minimum spanning tree](minimum-spanning-tree.md) contains both $F$ and that [edge](edge-of-a-graph.md). The [loop invariant](loop-invariant.md) is that some [minimum spanning tree](minimum-spanning-tree.md) contains every accepted [edge](edge-of-a-graph.md). It holds initially for the empty [edge](edge-of-a-graph.md) set. Suppose the next accepted [edge](edge-of-a-graph.md) $e$ joins a current [connected component of a graph](component-graph-theory.md) $S$ to its complement. No earlier rejected [edge](edge-of-a-graph.md) crosses this [cut of a graph](cut-graph-theory.md): once its endpoints are in one [connected component of a graph](component-graph-theory.md), subsequent merges never separate them. Thus $e$ is a lightest [edge](edge-of-a-graph.md) across that [cut of a graph](cut-graph-theory.md).

For the short exchange argument, take a [minimum spanning tree](minimum-spanning-tree.md) $T$ containing $F$. If $e$ is absent, adding it creates a [fundamental cycle](fundamental-cycle.md). This [graph cycle](cycle-in-a-graph.md) contains another [edge](edge-of-a-graph.md) $f$ crossing the same [cut of a graph](cut-graph-theory.md). No [edge](edge-of-a-graph.md) of $F$ crosses the [cut of a graph](cut-graph-theory.md), so $f$ is not in $F$. Replace $f$ by $e$: the result is a [spanning tree](spanning-tree.md) containing $F$ and $e$, with no greater total weight because $w(e)\leq w(f)$. It is therefore also a [minimum spanning tree](minimum-spanning-tree.md). This is the [minimum spanning tree cut property](minimum-spanning-tree-cut-property.md) in the form needed for tied weights.

In the example, $CD$ is safe after rejecting $AC$: the current [connected component of a graph](component-graph-theory.md) $\{A,B,C\}$ has crossing [edges](edge-of-a-graph.md) $CD,CE,BE$ of weights $4,6,7$. Its cheapest connection is $CD$. The rejected $AC$ is also the unique heaviest [edge](edge-of-a-graph.md) of the [graph cycle](cycle-in-a-graph.md) $A,B,C,A$, so the [minimum spanning tree cycle property](minimum-spanning-tree-cycle-property.md) excludes it from every optimum.

Negative and zero [edge](edge-of-a-graph.md) weights are allowed: the comparisons and exchange argument still apply. Ties can give several [minimum spanning trees](minimum-spanning-tree.md), though they need not; any order among equal-weight [edges](edge-of-a-graph.md) remains valid. Distinct [edge](edge-of-a-graph.md) weights guarantee a unique [minimum spanning tree](minimum-spanning-tree.md). To see why, take the lightest [edge](edge-of-a-graph.md) $e$ belonging to exactly one of two proposed optima, say $T$. Deleting $e$ from $T$ gives a [cut of a graph](cut-graph-theory.md); the other optimum has a [graph path](path-in-a-graph.md) across it, containing an [edge](edge-of-a-graph.md) $f$ absent from $T$. Hence $w(e)<w(f)$, and replacing $f$ by $e$ improves that other optimum, a contradiction. For disconnected input, process all [edges](edge-of-a-graph.md) to obtain a [minimum spanning forest](minimum-spanning-forest.md), one [minimum spanning tree](minimum-spanning-tree.md) per original [connected component of a graph](component-graph-theory.md); no [spanning tree](spanning-tree.md) of the whole [graph](graph-split.md) exists.[Robert Sedgewick and Kevin Wayne, Algorithms, 4th edition, companion KruskalMST.java, class documentation and constructor: arbitrary signed weights, ties, disconnected input and sorted processing](algorithms-4th-edition-by-robert-sedgewick-and-others/kruskalmst-java.md)

## ↑ Ancestors (8)

1. [Kruskal's algorithm](kruskal-s-algorithm.md)
2. [Minimum spanning tree](minimum-spanning-tree.md)
3. [Spanning tree](spanning-tree.md)
4. [Tree (graph theory)](tree-graph-theory-split.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
