# Simple graph

↑ **Parent:** [Graph](graph-split.md)

An undirected simple [graph](graph-split.md) is exactly a pair of [sets](set-split.md)

$$
G=(V,E),\qquad E\subseteq\{\{u,v\}:u,v\in V,\ u\ne v\}.
$$

Thus every [edge](edge-of-a-graph.md) is a two-element [set](set-split.md) of distinct [vertices](vertex-graph-theory.md). The [unordered pair](unordered-pair.md) $\{u,v\}$ equals $\{v,u\}$, so there is no direction. The distinctness condition excludes [self-loops](loop-graph-theory.md), and using a [set](set-split.md) of [edges](edge-of-a-graph.md) excludes parallel copies. A [simple graph](simple-graph.md) may have [vertices](vertex-graph-theory.md) with no incident [edges](edge-of-a-graph.md); $E$ does not by itself determine $V$. For example, $(\{A,B\},\{AB\})$ and $(\{A,B,C\},\{AB\})$ have the same [edge](edge-of-a-graph.md) [set](set-split.md) but different [vertex sets](vertex-set.md).[MIT, Graphs and Coloring, Section 1.1](https://ocw.mit.edu/courses/6-1200j-mathematics-for-computer-science-spring-2024/mit6_1200j_s24_lec11.pdf)

In the six-[vertex](vertex-graph-theory.md) example, the [vertex neighbourhood](vertex-neighbourhood.md) of $C$ is $\Gamma(C)=\{A,B,D\}$, so its [degree of a vertex](degree-graph-theory.md) is $\deg(C)=3$. In label order $A,B,C,D,E,F$, the [degree sequence](degree-sequence.md) is

$$
(2,2,3,3,2,2),\qquad \sum_{v\in V}\deg(v)=14=2\cdot7=2|E|.
$$

This is the [handshaking lemma](degree-sum-formula.md): count each [edge](edge-of-a-graph.md) once at each of its two endpoints. The [average degree of a graph](average-degree-of-a-graph.md) here is $14/6=7/3$. The [degree sequence](degree-sequence.md) is a compact consistency check on an [edge](edge-of-a-graph.md) list; an odd sum could not describe any finite undirected [graph](graph-split.md). It also forces the number of odd [degrees of vertices](degree-graph-theory.md) to be even, since the even terms do not affect the parity of the sum.

The [adjacency matrix](adjacency-matrix.md) in the figure uses label order $A,B,C,D,E,F$. Its entry $M_{uv}$ is one exactly when $\{u,v\}\in E$, and zero otherwise. It is a [symmetric matrix](symmetric-matrix.md) with zero diagonal, and each row sum gives the corresponding [vertex degree](degree-graph-theory.md). For example, row $C$ is $(1,1,0,1,0,0)$. The fourteen ones count both directions of the seven undirected [edges](edge-of-a-graph.md); they do not indicate fourteen different [edges](edge-of-a-graph.md). This translates a picture into a representation suitable for calculation.

The restrictions matter. A [directed graph](directed-graph.md) uses an [ordered pair](ordered-pair.md) to distinguish $u\to v$ from $v\to u$, so [reachability](reachability-in-a-graph.md) can depend on direction. A [multigraph](multigraph.md) can contain several distinct [edges](edge-of-a-graph.md) between the same [vertices](vertex-graph-theory.md); adding another $CD$ would raise $\deg(C)$ and $\deg(D)$ to four without adding a new neighbour. A [self-loop](loop-graph-theory.md) at $A$ contributes two to its undirected [vertex degree](degree-graph-theory.md), making it four, because both endpoints lie at $A$. Specify whether [self-loops](loop-graph-theory.md) are allowed in a [multigraph](multigraph.md). Finally, a [weighted graph](weighted-graph.md) attaches numerical information to [edges](edge-of-a-graph.md): if links carry travel times, minimizing the number of [edges](edge-of-a-graph.md) need not minimize total time. These are changes to the model, rather than changes to how the same [simple graph](simple-graph.md) is drawn.

## ↑ Ancestors (6)

1. [Graph](graph-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (48)

- [Bipartite graph](bipartite-graph.md)
- [Bipartite planar graph edge bound](bipartite-planar-graph-edge-bound.md)
- [Branch set of a graph minor](branch-set-of-a-graph-minor.md)
- [Cayley's formula](cayley-s-formula.md)
- [Chordal graph](chordal-graph.md)
- [Chromatic index bounds](chromatic-index-bounds.md)
- [Chromatic number](chromatic-number.md)
- [Chromatic polynomial](chromatic-polynomial.md)
- [Closed walk](closed-walk.md)
- [Configuration model](configuration-model.md)
- [Crossing lemma for multigraphs](crossing-lemma-for-multigraphs.md)
- [Cut vertex](cut-vertex.md)
- [Degree matrix](degree-matrix.md)
- [Deletion-contraction recurrence for the chromatic polynomial](deletion-contraction-recurrence-for-the-chromatic-polynomial.md)
- [Depth-first search](depth-first-search.md)
- [DFS lowpoint](dfs-lowpoint.md)
- [Edge contraction](edge-contraction.md)
- [Edge of a graph](edge-of-a-graph.md)
- [Erdős-Gallai theorem](erdos-gallai-theorem.md)
- [Graph](graph-split.md)
- [Graph coloring](graph-coloring.md)
- [Graph minor](graph-minor.md)
- [Graph subdivision](graph-subdivision.md)
- [Greedy coloring](greedy-coloring.md)
- [Hamilton cycle](hamilton-cycle.md)
- [Hamiltonian graph](hamiltonian-graph.md)
- [Independence number](independence-number.md)
- [Independent set (graph theory)](independent-set-graph-theory.md)
- [Kuratowski's theorem](kuratowski-s-theorem.md)
- [Minimum vertex cover](minimum-vertex-cover.md)
- [Necessary conditions for a Hamilton cycle](necessary-conditions-for-a-hamilton-cycle.md)
- [Nonplanarity by edge counts](nonplanarity-by-edge-counts.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/3/solution.md)
- [Perfect elimination ordering](perfect-elimination-ordering.md)
- [Planar graph edge bound](planar-graph-edge-bound.md)
- [Pósa's theorem](posa-s-theorem.md)
- [Proper edge coloring](proper-edge-coloring.md)
- [Second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md)
- [Second-order logic](second-order-logic.md)
- [Short-cycle expectation in a uniform regular graph](short-cycle-expectation-in-a-uniform-regular-graph.md)
- [Simple graph](simple-graph.md)
- [Topological minor](topological-minor.md)
- [Tree (graph theory)](tree-graph-theory.md)
- [Vertex cover](vertex-cover.md)
- [Walk in a graph](walk-in-a-graph.md)
