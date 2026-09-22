# Chromatic number from acyclic longest paths

↑ **Parent:** [Acyclic orientation](acyclic-orientation.md)

For a finite [graph](graph-split.md), let $\lambda(D)$ count the [vertices](vertex-graph-theory.md) on a longest [directed path](directed-path.md) in an [acyclic orientation](acyclic-orientation.md) $D$. Its [minimum](minimum-of-a-subset-of-a-total-order.md) over those [orientations](orientation-of-a-graph.md) is the [chromatic number](chromatic-number.md). A proper $k$-colouring gives an [orientation](orientation-of-a-graph.md) from smaller to larger colours, so every [directed path](directed-path.md) has strictly increasing colours and at most $k$ [vertices](vertex-graph-theory.md). Conversely, assign to each [vertex](vertex-graph-theory.md) the number of [vertices](vertex-graph-theory.md) in a longest [directed path](directed-path.md) ending there. Along an [edge](edge-of-a-graph.md) $u\to v$ this number increases: an ending [path](path-in-a-graph.md) at $u$ cannot contain $v$ without forming a [directed cycle](directed-cycle.md), so it can be extended. The resulting labels give a proper [colouring](colouring-of-a-set.md) using at most $\lambda(D)$ colours. These two constructions prove equality. [Counting](counting.md) [edges](edge-of-a-graph.md) instead of [vertices](vertex-graph-theory.md) in [path](path-in-a-graph.md) length subtracts one from the displayed [minimum](minimum-of-a-subset-of-a-total-order.md).

## ↑ Ancestors (7)

1. [Acyclic orientation](acyclic-orientation.md)
2. [Orientation of a graph](orientation-of-a-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2011/a/2/b/iii/solution.md)
- [Solution](past-exam-of-the-graph-theory-course-of-the-university-of-oxford/2011/2/b/iii/solution.md)
