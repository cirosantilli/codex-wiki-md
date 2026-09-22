# Connected graph

↑ **Parent:** [Connectivity (graph theory)](connectivity-graph-theory.md)

An undirected [graph](graph-split.md) is connected when every pair $u,v$ of [vertices](vertex-graph-theory.md) is joined by a finite [graph path](path-in-a-graph.md). The length-zero [graph path](path-in-a-graph.md) consisting of $u$ alone is allowed, so a single-[vertex](vertex-graph-theory.md) [graph](graph-split.md) is connected. We use the term here for nonempty [graphs](graph-split.md); conventions for the [graph](graph-split.md) with no [vertices](vertex-graph-theory.md) vary. Adjacent [vertices](vertex-graph-theory.md) are connected, but connected [vertices](vertex-graph-theory.md) need not be adjacent: in our six-[vertex](vertex-graph-theory.md) example, $A$ reaches $F$ along $A,C,D,F$, although $AF$ is absent.

Allowing [walks](walk-in-a-graph.md) instead of [graph paths](path-in-a-graph.md) gives the same test for a [connected graph](connected-graph.md). Whenever a finite [walk](walk-in-a-graph.md) revisits a [vertex](vertex-graph-theory.md), delete the intervening closed portion; repeating this leaves a [graph path](path-in-a-graph.md) with the same endpoints. This simple shortening argument explains why revisiting locations cannot help decide [reachability](reachability-in-a-graph.md).[MIT, Connectivity and Trees, Theorem 1](https://ocw.mit.edu/courses/6-1200j-mathematics-for-computer-science-spring-2024/mit6_1200j_s24_lec13.pdf)

Connectivity can conceal fragile connections. Removing $CD$ from our [graph](graph-split.md) produces two [connected components of a graph](component-graph-theory.md), on $\{A,B,C\}$ and $\{D,E,F\}$: $CD$ is a [bridge in a graph](bridge-graph-theory.md). Removing $AB$ instead preserves connectivity, because $A,C,B$ supplies an alternative [graph path](path-in-a-graph.md). If [edges](edge-of-a-graph.md) represent communication links, this calculation says precisely which single link failure separates the two groups. It is a conclusion about this model, independent of the lengths in its drawing.

A [tree](tree-graph-theory-split.md) is a nonempty [connected graph](connected-graph.md) without a [graph cycle](cycle-in-a-graph.md); equivalently, each pair of [vertices](vertex-graph-theory.md) has exactly one [graph path](path-in-a-graph.md) between them. Delete $BC$ and $EF$ from our example. The remaining [edges](edge-of-a-graph.md)

$$
\{AB,AC,CD,DE,DF\}
$$

form a [spanning tree](spanning-tree.md): all six [vertices](vertex-graph-theory.md) remain, with $6-1=5$ [edges](edge-of-a-graph.md). The [graph path](path-in-a-graph.md) $A,C,D,F$ is now unique, and every remaining [edge](edge-of-a-graph.md) is a [bridge in a graph](bridge-graph-theory.md). Adding $BC$ back creates exactly one [graph cycle](cycle-in-a-graph.md), $B,A,C,B$. Thus [graph cycles](cycle-in-a-graph.md) express alternative routes, while a [tree](tree-graph-theory-split.md) retains just enough connections for [reachability](reachability-in-a-graph.md). More generally, a finite [connected graph](connected-graph.md) on $n\geq1$ [vertices](vertex-graph-theory.md) has at least $n-1$ [edges](edge-of-a-graph.md), with equality exactly for a [tree](tree-graph-theory-split.md). One proof repeatedly removes an [edge](edge-of-a-graph.md) on a [graph cycle](cycle-in-a-graph.md), preserving connectivity, until a [spanning tree](spanning-tree.md) remains.[The Basics (author-hosted chapter preview)](graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview.md)

For a finite [graph](graph-split.md), [breadth-first search](breadth-first-search.md) tests connectivity by starting at one [vertex](vertex-graph-theory.md) and discovering neighbours in successive layers. Starting at $A$, the layers in our example are $\{A\}$, $\{B,C\}$, $\{D\}$, $\{E,F\}$. Every [vertex](vertex-graph-theory.md) is discovered, and the layer numbers give [graph distances](distance-graph-theory.md) from $A$. Recording one discovery [edge](edge-of-a-graph.md) for each new [vertex](vertex-graph-theory.md) constructs a [spanning tree](spanning-tree.md). This turns an existence question into both a concrete route and a certificate of connectivity.

**Table of contents**

- [Component (graph theory)](component-graph-theory.md)
  - [Supermodularity of graph component count](supermodularity-of-graph-component-count.md)
  - [Tree component](tree-component.md)
  - [Largest component of a graph](largest-component-of-a-graph.md)

## ↑ Ancestors (7)

1. [Connectivity (graph theory)](connectivity-graph-theory.md)
2. [Graph](graph-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (64)

- [2-core of a graph](2-core-of-a-graph.md)
- [Bipartite graph](bipartite-graph-split.md)
- [Bipartite planar graph edge bound](bipartite-planar-graph-edge-bound.md)
- [Bradley-Terry likelihood Hessian](bradley-terry-likelihood-hessian.md)
- [Branch set of a graph minor](branch-set-of-a-graph-minor.md)
- [Bridge (graph theory)](bridge-graph-theory.md)
- [Bridges and connectivity in the 2-core](bridges-and-connectivity-in-the-2-core.md)
- [Cayley graph](cayley-graph.md)
- [Chordal graph](chordal-graph.md)
- [Connected graph](connected-graph.md)
- [Connectivity (graph theory)](connectivity-graph-theory.md)
- [Cut of a flow network](cut-of-a-flow-network.md)
- [Cut vertex](cut-vertex.md)
- [Depth-first search](depth-first-search.md)
- [Differential sky map monopole degeneracy](differential-sky-map-monopole-degeneracy.md)
- [Diffusion on a graph](diffusion-on-a-graph.md)
- [Directed percolation](directed-percolation.md)
- [Euler circuit](euler-circuit.md)
- [Euler formula for a connected planar graph](euler-formula-for-a-connected-planar-graph.md)
- [Eulerian graph](eulerian-graph.md)
- [Eulerian trail](eulerian-trail.md)
- [Facial boundary walk](facial-boundary-walk.md)
- [Fixed-temperature law of simulated annealing](fixed-temperature-law-of-simulated-annealing.md)
- [Foster's theorem](foster-s-theorem.md)
- [Graph excess](graph-excess.md)
- [Graph kernel](graph-kernel.md)
- [Graph minor](graph-minor-split.md)
- [Graphic matroid](graphic-matroid.md)
- [Harmonic maximum principle on a finite graph](harmonic-maximum-principle-on-a-finite-graph.md)
- [Incidence pseudoinverse decomposition](incidence-pseudoinverse-decomposition.md)
- [K-core of a graph](k-core-of-a-graph.md)
- [Kruskal's algorithm](kruskal-s-algorithm.md)
- [Kruskal's algorithm worked example](kruskal-s-algorithm-worked-example.md)
- [Mean spanning-tree path current](mean-spanning-tree-path-current.md)
- [Necessary conditions for a Hamilton cycle](necessary-conditions-for-a-hamilton-cycle.md)
- [Nonplanarity by edge counts](nonplanarity-by-edge-counts.md)
- [Oriented incidence matrix](oriented-incidence-matrix.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/17f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2/17f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3/14i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/16h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/16h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/17g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-111/2/b/solution.md)
- [Planar graph edge bound](planar-graph-edge-bound.md)
- [Quasi-transitive graph](quasi-transitive-graph.md)
- [Robbins' theorem](robbins-theorem.md)
- [Spanning tree](spanning-tree.md)
- [Transpositions on a connected graph generate the symmetric group](transpositions-on-a-connected-graph-generate-the-symmetric-group.md)
- [Tree (graph theory)](tree-graph-theory-split.md)
