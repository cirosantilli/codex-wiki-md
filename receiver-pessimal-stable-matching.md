# Receiver-pessimal stable matching

↑ **Parent:** [Proposer-optimal stable matching](proposer-optimal-stable-matching.md)

For fixed [strict preferences](strict-preference.md), the same output of the [Gale-Shapley algorithm](gale-shapley-algorithm.md) gives each receiver its worst partner obtainable in any [stable matching](stable-matching-in-a-bipartite-graph.md), treating unmatched as last. "Worst" is restricted to stable possibilities: a receiver might still receive its favourite acceptable partner if every [stable matching](stable-matching-in-a-bipartite-graph.md) assigns it that partner. Reversing the proposing side gives receivers their best stable partners instead.

For a short proof, let $M$ be a [proposer-optimal stable matching](proposer-optimal-stable-matching.md) and $S$ any other [stable matching](stable-matching-in-a-bipartite-graph.md). If a receiver $r$ preferred $M(r)=\ell$ to $S(r)$, then proposer optimality would make $\ell$ prefer $r=M(\ell)$ to $S(\ell)$, since the partners differ and [preferences](preference-relation.md) are strict. The pair $(\ell,r)$ would block $S$. Therefore no receiver prefers its partner in $M$ to its partner in $S$. In the worked example, right-side ranks in $M_L$ are $2,2,3$ for $X,Y,Z$, whereas $M_R$ gives them $1,1,2$. Neither outcome is universally best for both sides.

## ↑ Ancestors (9)

1. [Proposer-optimal stable matching](proposer-optimal-stable-matching.md)
2. [Gale-Shapley algorithm](gale-shapley-algorithm.md)
3. [Stable matching in a bipartite graph](stable-matching-in-a-bipartite-graph.md)
4. [Matching (graph theory)](matching-graph-theory-split.md)
5. [Graph theory](graph-theory-split.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Gale-Shapley algorithm](gale-shapley-algorithm.md)
