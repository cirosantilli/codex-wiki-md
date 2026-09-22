# Matching (graph theory)

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matching_(graph_theory))

A [matching in a graph](matching-graph-theory-split.md) is a [set](set-split.md) $M$ of [edges](edge-of-a-graph.md) of an [undirected graph](undirected-graph.md) with no shared endpoints: each [vertex](vertex-graph-theory.md) has capacity for at most one selected [edge](edge-of-a-graph.md). It describes simultaneous compatible pairs, such as jobs assigned to distinct available workers, or tasks each occupying two resources that cannot be shared. The empty [set](set-split.md) is a valid [matching in a graph](matching-graph-theory-split.md).[Matching, Covering and Packing, opening paragraph, printed p. 1: independent edges and matchings](graph-theory-by-reinhard-diestel.md)

For a finite [simple graph](simple-graph.md) $G=(V,E)$, write $x_e=1$ when $e$ is selected and $x_e=0$ otherwise. The vertex capacity constraint is exactly

$$
x_e\in\{0,1\}\quad(e\in E),\qquad
\sum_{e\in E:\,v\in e}x_e\leq1\quad(v\in V).
$$

These are constraints on a discrete selection, not a requirement that every [vertex](vertex-graph-theory.md) be used. A [matching in a graph](matching-graph-theory-split.md) with [matching saturation](matching-saturation.md) of all [vertices](vertex-graph-theory.md) is a [perfect matching](perfect-matching.md); an [unmatched vertex in a matching](unmatched-vertex-in-a-matching.md) uses none of its capacity.

The objective must be specified separately. A [maximum cardinality matching](maximum-cardinality-matching.md) selects as many [edges](edge-of-a-graph.md) as possible; a [maximum-weight matching](maximum-weight-matching.md) selects the greatest total benefit; a [minimum-weight perfect matching](minimum-weight-perfect-matching.md) minimizes cost while requiring every [vertex](vertex-graph-theory.md) to be paired. A [maximal matching](maximal-matching.md) only says that no additional [edge](edge-of-a-graph.md) fits alongside the current choices. The four-[vertex](vertex-graph-theory.md) [path graph](path-graph.md) below separates these notions: choosing the middle [edge](edge-of-a-graph.md) blocks both outer [edges](edge-of-a-graph.md), yet replacing it by those two [edges](edge-of-a-graph.md) pairs more [vertices](vertex-graph-theory.md).

This model is useful because conflicts are local at [vertices](vertex-graph-theory.md), while the quality of a selection can depend on coordinated changes along a whole [augmenting path in a matching](augmenting-path-in-a-matching.md). A [greedy matching](greedy-matching.md) gives a quick feasible selection; [Berge's theorem](berge-s-theorem.md) explains when searching for such changes has reached a [maximum cardinality matching](maximum-cardinality-matching.md). Repeating the pairing problem over time leads instead to [proper edge colouring](proper-edge-coloring.md), where each time slot is a [matching in a graph](matching-graph-theory-split.md).

**Table of contents**

- [Unmatched vertex in a matching](unmatched-vertex-in-a-matching.md)
- [Matching saturation](matching-saturation.md)
- [Stable matching in a bipartite graph](stable-matching-in-a-bipartite-graph.md)
  - [Mutual-worst edge in stable matchings](mutual-worst-edge-in-stable-matchings.md)
  - [Gale-Shapley algorithm](gale-shapley-algorithm.md)
    - [Proposer-optimal stable matching](proposer-optimal-stable-matching.md)
      - [Receiver-pessimal stable matching](receiver-pessimal-stable-matching.md)
  - [Blocking pair in stable matching](blocking-pair-in-stable-matching.md)
- [Near-perfect matching](near-perfect-matching.md)
- [Matching generating function](matching-generating-function.md)
  - [Annealing ratios for a matching generating function](annealing-ratios-for-a-matching-generating-function.md)
- [Alternating path in a matching](alternating-path-in-a-matching.md)
- [Augmenting path in a matching](augmenting-path-in-a-matching.md)
  - [Berge's theorem](berge-s-theorem.md)
  - [Short augmenting paths in a dense bipartite graph](short-augmenting-paths-in-a-dense-bipartite-graph.md)
- [Perfect matching](perfect-matching.md)
  - [Flexible vertex in a balanced bipartite graph](flexible-vertex-in-a-balanced-bipartite-graph.md)
  - [Minimum-weight perfect matching](minimum-weight-perfect-matching.md)
  - [One-factorization](one-factorization.md)
- [Maximal matching](maximal-matching.md)
  - [Greedy matching](greedy-matching.md)
- [Matching number](matching-number.md)
- [Maximum cardinality matching](maximum-cardinality-matching.md)
- [Maximum-weight matching](maximum-weight-matching.md)
- [Hall's marriage theorem](hall-s-marriage-theorem.md)
  - [Hall condition](hall-condition.md)
    - [Hall obstruction](hall-obstruction.md)
  - [Hall allocation model](hall-allocation-model.md)
  - [System of distinct representatives](system-of-distinct-representatives.md)
  - [Hall theorem proof outline](hall-theorem-proof-outline.md)
  - [Random bipartite matching from empty-rectangle exclusion](random-bipartite-matching-from-empty-rectangle-exclusion.md)
  - [Hall matching of maximal separated sets](hall-matching-of-maximal-separated-sets.md)
  - [Degree-weighted Hall condition](degree-weighted-hall-condition.md)
  - [Measurable Hall theorem](measurable-hall-theorem.md)
  - [Hall induction through a tight set](hall-induction-through-a-tight-set.md)
  - [Regular bipartite graph has a perfect matching](regular-bipartite-graph-has-a-perfect-matching.md)
- [Regular-graph matching bound from unmatched vertices](regular-graph-matching-bound-from-unmatched-vertices.md)
  - [Disjoint union of triangles as a sharp matching example](disjoint-union-of-triangles-as-a-sharp-matching-example.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
