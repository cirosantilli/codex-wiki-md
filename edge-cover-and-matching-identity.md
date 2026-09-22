# Edge cover and matching identity

↑ **Parent:** [Matching (graph theory)](matching-graph-theory-split.md)

If a finite [graph](graph-split.md) has no [isolated vertex](isolated-vertex.md), its minimum [edge cover](edge-cover.md) [cardinality](cardinality.md) $\rho(G)$ and [matching number](matching-number.md) $\nu(G)$ sum to its number of [vertices](vertex-graph-theory.md).

**Proof.** Start with a [maximum cardinality matching](maximum-cardinality-matching.md) $M$. Its [unmatched vertices in a matching](unmatched-vertex-in-a-matching.md) form an [independent set](independent-set-graph-theory.md), since an [edge](edge-of-a-graph.md) between two of them could be added. Add one incident [edge](edge-of-a-graph.md) for each such [vertex](vertex-graph-theory.md). They are distinct, giving an [edge cover](edge-cover.md) of size $|M|+|V|-2|M|=|V|-\nu(G)$.

Conversely, in any inclusion-minimal [edge cover](edge-cover.md) $F$, every [edge](edge-of-a-graph.md) has an endpoint of [vertex degree](degree-graph-theory.md) one in $(V,F)$; otherwise it could be removed. Thus each component is a [star graph](star-graph-theory.md): two [vertices](vertex-graph-theory.md) of [vertex degree](degree-graph-theory.md) at least two in one component would produce a [graph path](path-in-a-graph.md) containing an [edge](edge-of-a-graph.md) with both endpoints of [vertex degree](degree-graph-theory.md) at least two. If there are $t$ components, $|F|=|V|-t$. Selecting one [edge](edge-of-a-graph.md) from each [star graph](star-graph-theory.md) gives a [matching in a graph](matching-graph-theory-split.md) of size $t$, so $\nu(G)\geq t$ and $|F|\geq|V|-\nu(G)$. A minimum-[cardinality](cardinality.md) [edge cover](edge-cover.md) is inclusion-minimal, completing the proof. The constructive first half also gives a [polynomial-time algorithm](polynomial-time-algorithm.md) once a [maximum cardinality matching](maximum-cardinality-matching.md) is available.

## ↑ Ancestors (6)

1. [Matching (graph theory)](matching-graph-theory-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Edge cover](edge-cover.md)
- [Minimum-weight edge cover by matching savings](minimum-weight-edge-cover-by-matching-savings.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/3/d/i/solution.md)
