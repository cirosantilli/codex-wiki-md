<h1 id="hierholzer-s-algorithm">Hierholzer's algorithm</h1>

↑ **Parent:** [Euler circuit criterion](euler-circuit-criterion.md)

[Hierholzer's algorithm](hierholzer-s-algorithm.md) constructs an [Euler circuit](euler-circuit.md) by growing closed [trails](trail-in-a-graph.md) along unused [edges](edge-of-a-graph.md) and splicing them at shared [vertices](vertex-graph-theory.md), as in the [Euler circuit criterion](euler-circuit-criterion.md). Each [edge](edge-of-a-graph.md) must have a distinct record. An implementation using [adjacency lists](adjacency-list.md), a [stack](stack-data-structure.md), and a used flag for each [edge](edge-of-a-graph.md) runs in $O(|V|+|E|)$ time, including the connectivity and [vertex degree](degree-graph-theory.md) checks. Store both incidences of a [self-loop](loop-graph-theory.md), while marking its single [edge](edge-of-a-graph.md) record used only once.

## ↑ Ancestors (7)

1. [Euler circuit criterion](euler-circuit-criterion.md)
2. [Eulerian graph](eulerian-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Euler circuit](euler-circuit.md)
- [Euler circuit criterion](euler-circuit-criterion.md)
- [Hierholzer's algorithm](hierholzer-s-algorithm.md)
