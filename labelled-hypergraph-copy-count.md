# Labelled hypergraph copy count

↑ **Parent:** [Hypergraph](hypergraph-split.md)

For [hypergraphs](hypergraph-split.md) $F,H$, a labelled copy is an [injective function](injective-function.md) $\phi:V(F)\to V(H)$ taking every [hypergraph edge](edge-of-a-hypergraph.md) of $F$ to an [hypergraph edge](edge-of-a-hypergraph.md) of $H$. Specified [vertex of a hypergraph](vertex-of-a-hypergraph.md) classes may additionally require $\phi(i)\in V_i$. The count is the sum, over these [injective](injective-function.md) maps, of the product of the host [hypergraph edge](edge-of-a-hypergraph.md) indicators. Without injectivity the same expression counts [hypergraph](hypergraph-split.md) homomorphisms. On a common host of size $n$, their counts differ by at most $\binom{|V(F)|}{2}n^{|V(F)|-1}$: every noninjective map identifies at least one pair of abstract [vertices of a hypergraph](vertex-of-a-hypergraph.md), each prescribed equality permits at most $n^{|V(F)|-1}$ maps, and the [union bound](boole-s-inequality.md) completes the estimate. An induced copy additionally preserves nonedges, so its indicator product includes nonedge factors. The [counting lemma for octahedrally quasirandom three-uniform hypergraphs](counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs.md) estimates these labelled products when the requisite centered triple indicators have small box [norm](norm.md).

## ↑ Ancestors (6)

1. [Hypergraph](hypergraph-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Counting lemma for octahedrally quasirandom three-uniform hypergraphs](counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88/4/iii/solution.md)
