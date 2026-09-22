# Robbins' theorem

↑ **Parent:** [Strong orientation](strong-orientation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Robbins'_theorem)

A finite nonempty [connected graph](connected-graph.md) whose [edges](edge-of-a-graph.md) are undirected admits a [strong orientation](strong-orientation.md) if and only if it has no [bridge in a graph](bridge-graph-theory.md). This statement holds for finite [multigraphs](multigraph.md) as well as finite [simple graphs](simple-graph.md); [self-loops](loop-graph-theory.md) do not help connect distinct [vertices](vertex-graph-theory.md). The single-[vertex](vertex-graph-theory.md) case is allowed, with length-zero [directed paths](directed-path.md).[Hassin and Megiddo, On Orientations and Shortest Paths (1989), printed pp. 591–592: bridge-connectedness, strong connectivity and Theorem 2.6 (Robbins)](on-orientations-and-shortest-paths-by-refael-hassin-and-others.md)

Necessity comes from the two sides separated by deleting a [bridge in a graph](bridge-graph-theory.md): its chosen arrow crosses in only one direction. For sufficiency, the cited constructive proof uses [depth-first search](depth-first-search.md) to find a [cycle in a graph](cycle-in-a-graph.md), orients it cyclically, contracts it, and repeats. Undoing the contractions replaces junctions by [directed cycles](directed-cycle.md), retaining two-way [reachability](reachability-in-a-graph.md). Contraction can produce [multiple edges](multiple-edges.md), so these must remain distinct. This is a construction outline; the input [graph](graph-split.md) is finite and bridgeless, and remaining [edges](edge-of-a-graph.md) within contracted pieces can receive arbitrary directions.[Hassin and Megiddo (1989), Theorem 2.6 proof, printed p. 592: cycle orientation and contraction, explicitly described as a different constructive proof from Robbins's](on-orientations-and-shortest-paths-by-refael-hassin-and-others.md)

## ↑ Ancestors (7)

1. [Strong orientation](strong-orientation.md)
2. [Orientation of a graph](orientation-of-a-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
