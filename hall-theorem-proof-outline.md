# Hall theorem proof outline

↑ **Parent:** [Hall's marriage theorem](hall-s-marriage-theorem.md)

For sufficiency, take a [matching in a graph](matching-graph-theory-split.md) of maximum size and suppose a left [vertex](vertex-graph-theory.md) $u$ is unmatched. Follow unused [edges](edge-of-a-graph.md) from left to right and matching [edges](edge-of-a-graph.md) back to the left. An unmatched reachable right [vertex](vertex-graph-theory.md) yields an [augmenting path in a matching](augmenting-path-in-a-matching.md), contradicting maximal size. Otherwise let $S,T$ be the reachable left and right [sets](set-split.md). Every member of $T$ is matched to a distinct member of $S\setminus\{u\}$, and every member of $S\setminus\{u\}$ is reached this way. Since $N(S)=T$, we obtain $|N(S)|=|S|-1$, contradicting the [Hall condition](hall-condition.md). Finiteness ensures that a maximum-size [matching in a graph](matching-graph-theory-split.md) exists.

The alternative [Hall induction through a tight set](hall-induction-through-a-tight-set.md) uses [mathematical induction](mathematical-induction.md): a proper nonempty [subset](subset.md) with $|N(S)|=|S|$ splits off a balanced [induced subgraph](induced-subgraph.md); without such a tight [set](set-split.md), deleting one chosen [edge](edge-of-a-graph.md)'s endpoints preserves the [Hall condition](hall-condition.md) on the smaller left side.

## ↑ Ancestors (7)

1. [Hall's marriage theorem](hall-s-marriage-theorem.md)
2. [Matching (graph theory)](matching-graph-theory-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
