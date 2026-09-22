# Proposer-optimal stable matching

↑ **Parent:** [Gale-Shapley algorithm](gale-shapley-algorithm.md)

For fixed [strict preferences](strict-preference.md), a [proposer-optimal stable matching](proposer-optimal-stable-matching.md) gives each proposer its best partner obtainable in any [stable matching](stable-matching-in-a-bipartite-graph.md), with unmatched ranked last. The [Gale-Shapley algorithm](gale-shapley-algorithm.md) achieves all these individual optima simultaneously. In the worked example, $M_L$ gives $A,B,C$ partners ranked $1,2,2$, respectively; the alternative $M_R$ gives them ranks $2,3,3$.

Suppose a first rejection of a pair belonging to some [stable matching](stable-matching-in-a-bipartite-graph.md) $S$ occurs when $r$ rejects $\ell$ for $\ell'$. Every partner $\ell'$ prefers to $r$ has already rejected it, so none can be its partner in $S$. If $S(r)=\ell$, then $\ell'$ prefers $r$ to $S(\ell')$, while $r$ prefers $\ell'$ to $\ell$: a [blocking pair in stable matching](blocking-pair-in-stable-matching.md), a contradiction. Hence no rejected pair is stable, and each proposer receives its best stable partner. Under [strict preferences](strict-preference.md) this also makes the outcome independent of proposal order.

**Table of contents**

- [Receiver-pessimal stable matching](receiver-pessimal-stable-matching.md)

## ↑ Ancestors (8)

1. [Gale-Shapley algorithm](gale-shapley-algorithm.md)
2. [Stable matching in a bipartite graph](stable-matching-in-a-bipartite-graph.md)
3. [Matching (graph theory)](matching-graph-theory-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Gale-Shapley algorithm](gale-shapley-algorithm.md)
- [Proposer-optimal stable matching](proposer-optimal-stable-matching.md)
- [Receiver-pessimal stable matching](receiver-pessimal-stable-matching.md)
