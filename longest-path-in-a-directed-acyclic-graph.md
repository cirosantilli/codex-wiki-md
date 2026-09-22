# Longest path in a directed acyclic graph

↑ **Parent:** [Longest path](longest-path.md)

Process [vertices](vertex-graph-theory.md) in a [topological sorting](topological-sorting.md), initializing a fixed source to zero and all other labels to $-\infty$. All possible predecessors have already been processed when a [vertex](vertex-graph-theory.md) is reached, so maximum-relaxation computes the best path ending there. [Induction](mathematical-induction.md) along the order proves correctness for arbitrary signed weights. Initializing every [vertex](vertex-graph-theory.md) to zero instead allows a path to start anywhere. Each [vertex](vertex-graph-theory.md) and [edge](edge-of-a-graph.md) is processed a constant number of times, giving $O(|V|+|E|)$ [running time](running-time.md). For a nonempty-path requirement, maximize the edge-extension candidates rather than including zero as the final answer.

## ↑ Ancestors (7)

1. [Longest path](longest-path.md)
2. [Path in a graph](path-in-a-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
