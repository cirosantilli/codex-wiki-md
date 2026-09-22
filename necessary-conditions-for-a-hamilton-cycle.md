# Necessary conditions for a Hamilton cycle

↑ **Parent:** [Hamilton cycle](hamilton-cycle.md)

A [Hamiltonian graph](hamiltonian-graph.md) must be a [connected graph](connected-graph.md) and have [minimum degree](minimum-degree-of-a-graph.md) $\delta(G)\geq2$: each [vertex](vertex-graph-theory.md) has two distinct neighbours on its [Hamilton cycle](hamilton-cycle.md). It also has no [cut vertex](cut-vertex.md). Indeed, deleting any [vertex](vertex-graph-theory.md) from the [Hamilton cycle](hamilton-cycle.md) leaves a [graph path](path-in-a-graph.md) through every remaining [vertex](vertex-graph-theory.md), so the remaining [graph](graph-split.md) is connected. These are quick ways to rule out a [Hamilton cycle](hamilton-cycle.md).[Diestel, Graph Theory, §10.1, printed pp. 323–324: necessary minimum degree two and 2-connectivity](graph-theory-by-reinhard-diestel/hamilton-cycles.md)

Even these conditions together are not sufficient: the [complete bipartite graph](complete-bipartite-graph.md) $K_{2,3}$ is connected, has [minimum degree](minimum-degree-of-a-graph.md) two and no [cut vertex](cut-vertex.md), but has no [Hamilton cycle](hamilton-cycle.md). Every [graph cycle](cycle-in-a-graph.md) in a [bipartite graph](bipartite-graph-split.md) alternates between its two parts, using equally many [vertices](vertex-graph-theory.md) from each; it cannot use all two and all three.

In the other direction, [Dirac's theorem](dirac-s-theorem.md) gives a sufficient condition: a finite [simple graph](simple-graph.md) with $n\geq3$ and $\delta(G)\geq n/2$ has a [Hamilton cycle](hamilton-cycle.md). Failure of this inequality proves nothing by itself: the [cycle graph](cycle-graph.md) $C_5$ has a [Hamilton cycle](hamilton-cycle.md) despite $\delta(C_5)=2<5/2$.[Diestel, Graph Theory, §10.1, Theorem 10.1.1, printed p. 324](graph-theory-by-reinhard-diestel/hamilton-cycles.md)

## ↑ Ancestors (9)

1. [Hamilton cycle](hamilton-cycle.md)
2. [Cycle graph](cycle-graph.md)
3. [Cycle in a graph](cycle-in-a-graph.md)
4. [Path in a graph](path-in-a-graph.md)
5. [Graph theory](graph-theory-split.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
