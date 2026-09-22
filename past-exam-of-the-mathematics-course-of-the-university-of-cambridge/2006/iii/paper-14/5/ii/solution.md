<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each [hypergraph edge](../../../../../../edge-of-a-hypergraph.md) $W$, let $B_W$ be the event that one of its two colours occupies more than $3r/4$ vertices. By colour symmetry and the [union bound](../../../../../../boole-s-inequality.md), the preceding calculation gives

$$
\mathbb P(B_W)<2e^{-r/8}.
$$

Again the dependency [graph](../../../../../../graph-split.md) joins intersecting [hypergraph edges](../../../../../../edge-of-a-hypergraph.md) and has $D+1\leq r(\Delta+1)$. The assumed degree bound implies

$$
 e\,(2e^{-r/8})(D+1)
\leq2er e^{-r/8}(\Delta+1)<1.
$$

The symmetric [Lovász local lemma](../../../../../../lovasz-local-lemma.md) gives positive [probability](../../../../../../probability.md) that no $B_W$ occurs. Thus **there is a two-colouring in which each colour occupies at most $3r/4$ vertices of every [hypergraph edge](../../../../../../edge-of-a-hypergraph.md)**. Equivalently, both colour counts in every [hypergraph edge](../../../../../../edge-of-a-hypergraph.md) lie between $r/4$ and $3r/4$; no rounding difficulty arises because the counts are integers and the bad events use strict inequalities.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
