# Crossing lemma for multigraphs

↑ **Parent:** [Crossing lemma](crossing-lemma.md)

Here a loopless [multigraph](multigraph.md) has $v$ [vertices](vertex-graph-theory.md), $e$ [edges](edge-of-a-graph.md), and at most $\mu$ parallel [edges](edge-of-a-graph.md) per pair. In a minimum-crossing drawing, crossings between incident [edges](edge-of-a-graph.md) can be removed by exchanging their initial segments, so every crossing involves four distinct [vertices](vertex-graph-theory.md). For each parallel class choose an [edge](edge-of-a-graph.md) with probability $1/\mu$ per [edge](edge-of-a-graph.md), with the remaining probability choosing none. Retain [vertices](vertex-graph-theory.md) independently with probability $p$. The sampled [simple graph](simple-graph.md) has expected [edge](edge-of-a-graph.md) count $p^2e/\mu$, expected [vertex](vertex-graph-theory.md) count $pv$, and expected crossing count $p^4\operatorname{cr}(G)/\mu^2$. Deleting one [edge](edge-of-a-graph.md) per crossing and using the [planar graph edge bound](planar-graph-edge-bound.md) gives $p^4\operatorname{cr}(G)/\mu^2\geq p^2e/\mu-3pv$. Choose $p=4\mu v/e$.

## ↑ Ancestors (7)

1. [Crossing lemma](crossing-lemma.md)
2. [Crossing number](crossing-number.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/3/solution.md)
- [Székely distinct-distance bound](szekely-distinct-distance-bound.md)
