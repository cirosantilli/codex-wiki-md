# Eulerian graph

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eulerian_graph)

An [Eulerian graph](eulerian-graph.md) has an [Euler circuit](euler-circuit.md): a closed [trail](trail-in-a-graph.md) traversing every [edge](edge-of-a-graph.md) exactly once. Here the [graph](graph-split.md) is a finite [undirected graph](undirected-graph.md), possibly a [multigraph](multigraph.md) with [self-loops](loop-graph-theory.md). Parallel [edges](edge-of-a-graph.md) retain distinct identities, and each [self-loop](loop-graph-theory.md) contributes two to its [vertex degree](degree-graph-theory.md). Repeated [vertices](vertex-graph-theory.md) are allowed. This models inspecting every road segment once, even when a junction must be revisited.

For a nonempty set of [edges](edge-of-a-graph.md), the [Euler circuit criterion](euler-circuit-criterion.md) requires a [connected graph](connected-graph.md) only on the [edge support of a graph](edge-support-of-a-graph.md): [isolated vertices](isolated-vertex.md) impose no travel requirement. A single [vertex](vertex-graph-theory.md) with a [self-loop](loop-graph-theory.md) and two [vertices](vertex-graph-theory.md) joined by two parallel [edges](edge-of-a-graph.md) are both [Eulerian graphs](eulerian-graph.md). Neither requires three [vertices](vertex-graph-theory.md). With no [edges](edge-of-a-graph.md) and at least one [vertex](vertex-graph-theory.md), we allow the zero-length [trail](trail-in-a-graph.md) at that [vertex](vertex-graph-theory.md) as an [Euler circuit](euler-circuit.md); the [graph](graph-split.md) with no [vertices](vertex-graph-theory.md) has no such [walk](walk-in-a-graph.md).

The motivating [Seven Bridges of Königsberg](seven-bridges-of-konigsberg.md) problem asks for an [Eulerian trail](eulerian-trail.md), which need not return to its starting [vertex](vertex-graph-theory.md). In [Leonhard Euler](leonhard-euler.md)'s [Solutio problematis ad geometriam situs pertinentis by Leonhard Euler](solutio-problematis-ad-geometriam-situs-pertinentis-by-leonhard-euler.md), §2 poses the bridge-crossing question and §§4–6 encode land regions by letters. The river's shape drops out: only the connections matter. The paper was written in 1735 and published in 1741, according to the Euler Archive; the journal volume carries the nominal year 1736.[Euler Archive, E53: Solutio problematis ad geometriam situs pertinentis](euler-archive-e53-solutio-problematis-ad-geometriam-situs-pertinentis.md)

**Table of contents**

- [Edge support of a graph](edge-support-of-a-graph.md)
- [Seven Bridges of Königsberg](seven-bridges-of-konigsberg.md)
- [Eulerian trail](eulerian-trail.md)
- [Euler circuit](euler-circuit.md)
- [Euler circuit criterion](euler-circuit-criterion.md)
  - [Hierholzer's algorithm](hierholzer-s-algorithm.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Eulerian graph](eulerian-graph.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3/17f/a/solution.md)
