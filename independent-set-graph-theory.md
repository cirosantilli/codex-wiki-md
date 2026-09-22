# Independent set (graph theory)

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Independent_set_(graph_theory))

An [independent set](independent-set-graph-theory.md) selects mutually compatible objects when an [edge](edge-of-a-graph.md) of a [graph](graph-split.md) represents a conflict. For example, if [vertices](vertex-graph-theory.md) are activities and [edges](edge-of-a-graph.md) join activities that cannot occur together, an [independent set](independent-set-graph-theory.md) is a collection that can share one time slot. Finding the largest such collection is measured by the [independence number](independence-number.md).[Barak, Introduction to Theoretical Computer Science, Chapter 14, The independent set problem](https://introtcs.org/public/lec_12_NP.html)

In a finite [simple graph](simple-graph.md) $G=(V,E)$, an [independent set](independent-set-graph-theory.md) is a [subset](subset.md) $I\subseteq V$ with no [edge](edge-of-a-graph.md) joining two selected [vertices](vertex-graph-theory.md):

$$
u,v\in I,\ u\ne v\Longrightarrow\{u,v\}\notin E.
$$

The empty [set](set-split.md) and every singleton [set](set-split.md) are [independent sets](independent-set-graph-theory.md). In the [cycle graph](cycle-graph.md) $C_5$ drawn under [vertex cover](vertex-cover.md), $\{0,2\}$ is an [independent set](independent-set-graph-theory.md), but $\{0,4\}$ is not: the closing [edge](edge-of-a-graph.md) $40$ joins those two [vertices](vertex-graph-theory.md). Choosing nonconsecutive labels is insufficient unless the wraparound [edge](edge-of-a-graph.md) is checked.

An [independent set](independent-set-graph-theory.md) of maximum size has [cardinality](cardinality.md) equal to the [independence number](independence-number.md). Being unable to add another [vertex](vertex-graph-theory.md) only makes an [independent set](independent-set-graph-theory.md) inclusion-maximal. In the [star graph](star-graph-theory.md) $K_{1,3}$, the centre alone is inclusion-maximal, since it is adjacent to every leaf, but the three leaves form a larger [independent set](independent-set-graph-theory.md). This distinction mirrors the difference between an inclusion-minimal [vertex cover](vertex-cover.md) and a [minimum vertex cover](minimum-vertex-cover.md).

Every [independent set](independent-set-graph-theory.md) $I$ has a [vertex cover](vertex-cover.md) $V\setminus I$ as its [complement of a set](complement-of-a-set.md); a largest [independent set](independent-set-graph-theory.md) has a [minimum vertex cover](minimum-vertex-cover.md) as its complement. In every [proper vertex colouring](proper-vertex-coloring.md), each [colour class](colour-class.md) is an [independent set](independent-set-graph-theory.md), so [graph coloring](graph-coloring-split.md) partitions the [vertices](vertex-graph-theory.md) into mutually compatible groups.

**Table of contents**

- [Independence polynomial](independence-polynomial.md)
- [Maximal independent set](maximal-independent-set.md)
- [Independent transversal](independent-transversal.md)
- [Degree-ordered independent-set entropy bound](degree-ordered-independent-set-entropy-bound.md)
- [Independence number](independence-number.md)
  - [Caro-Wei bound](caro-wei-bound.md)
  - [Triangle-free graph with sub-power independence number](triangle-free-graph-with-sub-power-independence-number.md)
- [Greedy independent-set bound](greedy-independent-set-bound.md)
- [Locally sparse graph independence bound](locally-sparse-graph-independence-bound.md)
  - [Shearer independence bound for a triangle-free graph](shearer-independence-bound-for-a-triangle-free-graph.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Independent set of a matroid](independent-set-of-a-matroid.md)
