<h1 id="energy-increment-proof-of-szemeredi-regularity">Energy-increment proof of Szemerédi regularity</h1>

↑ **Parent:** [Szemerédi regularity lemma](szemeredi-regularity-lemma.md)

Use [equitable regularity energy](equitable-regularity-energy.md) with exceptional vertices retained as singleton cells. The [refinement variance identity for regularity energy](refinement-variance-identity-for-regularity-energy.md) shows that splitting along an irregular pair's witnesses raises energy by more than $\varepsilon^4|V_i||V_j|/n^2$. More than $\varepsilon k^2$ irregular ordered pairs therefore raise energy by more than $\varepsilon^5/4$ when the exceptional set occupies at most half the vertices.

For [equalization with a controlled exceptional set](equalization-with-a-controlled-exceptional-set.md), cut each of the at most $k2^k$ witness atoms into pieces of size $\lfloor L/4^k\rfloor$ and put leftovers into singleton exceptional cells. This is a refinement, so it cannot decrease energy. At most $n2^{-k}$ vertices are lost. Start with enough cells that this loss, over $\lceil4\varepsilon^{-5}\rceil$ rounds, is at most $\varepsilon n/2$; the initial exceptional set uses the other half. The number of cells grows by a bounded recurrence depending only on $\varepsilon$ and the prescribed minimum. Energy lies in $[0,1]$, so the process terminates.

## ↑ Ancestors (9)

1. [Szemerédi regularity lemma](szemeredi-regularity-lemma.md)
2. [Regular pair of vertex sets](regular-pair-of-vertex-sets.md)
3. [Edge density of a bipartite graph](edge-density-of-a-bipartite-graph.md)
4. [Probabilistic combinatorics](probabilistic-combinatorics-split.md)
5. [Graph theory](graph-theory-split.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Irregular pair of vertex sets](irregular-pair-of-vertex-sets.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-11/2/i/solution.md)
