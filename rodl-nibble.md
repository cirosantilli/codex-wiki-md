<h1 id="rodl-nibble">Rödl nibble</h1>

↑ **Parent:** [Semi-random method](semi-random-method.md)

For a nearly $D$-regular $s$-uniform [hypergraph](hypergraph-split.md), sample each edge independently with [probability](probability.md) $\alpha/D$, where $\alpha$ is small. Retain the isolated sampled edges as a [matching in a hypergraph](matching-in-a-hypergraph.md), and delete every vertex incident to any sampled edge before the next round. A vertex survives with [probability](probability.md) $(1-\alpha/D)^{d(v)}\approx e^{-\alpha}$; a sampled edge meets another sampled edge with [probability](probability.md) at most $s\alpha(1+o(1))$. Thus accepted edges cover order $\alpha$ of the vertices and collision waste is order $\alpha^2$. Small [hypergraph codegrees](hypergraph-codegree.md) control the overlap terms in residual-degree calculations. Repeating a bounded number of rounds while tracking near-regularity is the characteristic [Rödl nibble](rodl-nibble.md) mechanism.

## ↑ Ancestors (7)

1. [Semi-random method](semi-random-method.md)
2. [Probabilistic combinatorics](probabilistic-combinatorics-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Auxiliary matching construction for hypergraph edge colouring](auxiliary-matching-construction-for-hypergraph-edge-colouring.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/4/solution.md)
- [Rödl nibble](rodl-nibble.md)
- [Semi-random method](semi-random-method.md)
