# Graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_(discrete_mathematics))

A graph consists of [vertices](#vertex-graph-theory) joined by [edges](graph-theory.md#edge-of-a-graph).

**Table of contents**

- [Graph adjacency](#graph-adjacency)
- [Simple graph](#simple-graph)
- [Loop (graph theory)](#loop-graph-theory)
- [Torus graph](#torus-graph)
- [Dual graph](#dual-graph)
- [Cubic graph](#cubic-graph)
  - [Heawood graph](#heawood-graph)
    - [Heawood torus map](#heawood-torus-map)
- [Strong product of graphs](#strong-product-of-graphs)
  - [Strong graph power](#strong-graph-power)
    - [Shannon capacity of a graph](#shannon-capacity-of-a-graph)
      - [Haemers rank bound](#haemers-rank-bound)
        - [Polynomial representation of a graph](#polynomial-representation-of-a-graph)
      - [Complement-pair capacity gain](#complement-pair-capacity-gain)
        - [Nonadditivity of Shannon capacity](#nonadditivity-of-shannon-capacity)
      - [Pentagon capacity code](#pentagon-capacity-code)
- [Incidence matrix](#incidence-matrix)
- [Amenable graph](#amenable-graph)
  - [Følner set](#folner-set)
- [Multigraph](#multigraph)
  - [Bouquet graph](#bouquet-graph)
- [Distance-transitive graph](#distance-transitive-graph)
  - [Distance-transitive action on a graph](#distance-transitive-action-on-a-graph)
  - [Symplectic dual polar graph](#symplectic-dual-polar-graph)
- [Vertex-transitive graph](#vertex-transitive-graph)
- [Triangular lattice](#triangular-lattice)
- [False twin](#false-twin)
  - [False-twin class](#false-twin-class)
- [Graph power](#graph-power)
  - [Square of a cycle](#square-of-a-cycle)
- [Graph cut](#graph-cut)
  - [Balanced component cut](#balanced-component-cut)
- [Oriented incidence matrix](#oriented-incidence-matrix)
  - [Incidence pseudoinverse decomposition](#incidence-pseudoinverse-decomposition)
- [Cartesian product of graphs](#cartesian-product-of-graphs)
- [Ladder graph](#ladder-graph)
  - [Doubly infinite ladder graph](#doubly-infinite-ladder-graph)
- [Cubic lattice](#cubic-lattice)
  - [Amenable boundary growth of lattice boxes](#amenable-boundary-growth-of-lattice-boxes)
- [Vertex set](#vertex-set)
- [Graph blow-up](#graph-blow-up)
  - [Dense clique family blow-up lemma](#dense-clique-family-blow-up-lemma)
  - [Vertex cloning in a graph](#vertex-cloning-in-a-graph)
- [Multipartite graph](#multipartite-graph)
- [Reachability in a graph](#reachability-in-a-graph)
- [Graph search](#graph-search)
- [Tripartite graph](#tripartite-graph)
  - [Tripartite graph encoding of a grid](#tripartite-graph-encoding-of-a-grid)
- [Graph automorphism](#graph-automorphism)
  - [Quasi-transitive graph](#quasi-transitive-graph)
- [Bridge (graph theory)](#bridge-graph-theory)
- [Hypercube graph](#hypercube-graph)
  - [Gray code](#gray-code)
- [Square lattice](#square-lattice)
- [Connectivity (graph theory)](#connectivity-graph-theory)
  - [Connected graph](#connected-graph)
    - [Component (graph theory)](#component-graph-theory)
      - [Supermodularity of graph component count](#supermodularity-of-graph-component-count)
      - [Tree component](#tree-component)
      - [Largest component of a graph](#largest-component-of-a-graph)
- [Vertex (graph theory)](#vertex-graph-theory)
- [Graph isomorphism](#graph-isomorphism)
- [Triangle in a graph](#triangle-in-a-graph)
  - [Edge-disjoint triangles](#edge-disjoint-triangles)
  - [Triangle count](#triangle-count)
  - [Triangle-free graph](#triangle-free-graph)
    - [Triangle-free chromatic lower bound at bounded maximum degree](#triangle-free-chromatic-lower-bound-at-bounded-maximum-degree)
  - [Edge-triangle incidence bound](#edge-triangle-incidence-bound)
- [Vertex neighbourhood](#vertex-neighbourhood)

## Graph adjacency

↑ **Parent:** [Graph](graph.md)

Two [vertices](#vertex-graph-theory) of a [graph](graph.md) are adjacent if an [edge](graph-theory.md#edge-of-a-graph) joins them. A [graph automorphism](#graph-automorphism) preserves this relation in both directions. In an intersection graph, adjacency can be defined by a prescribed dimension or cardinality of an intersection, so any ambient symmetry preserving that statistic acts by [graph automorphisms](#graph-automorphism).

## Simple graph

↑ **Parent:** [Graph](graph.md)

A simple [graph](graph.md) has no [self-loops](#loop-graph-theory) and at most one [edge](graph-theory.md#edge-of-a-graph) between each pair of distinct [vertices](#vertex-graph-theory). An undirected simple [graph](graph.md) is determined by a [set](set.md) of unordered [vertex](#vertex-graph-theory) pairs.

## Loop (graph theory)

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_(graph_theory))

A self-loop is an [edge](graph-theory.md#edge-of-a-graph) whose two endpoints are the same [vertex](#vertex-graph-theory). In undirected total-degree counting it contributes two to the [degree of a vertex](graph-theory.md#degree-graph-theory), since both endpoints are incident to that [vertex](#vertex-graph-theory). Simple [graphs](graph.md) exclude self-loops; the [linearized chord diagram model](graph-theory.md#linearized-chord-diagram-model) retains them and starts from one self-loop.

## Torus graph

↑ **Parent:** [Graph](graph.md)

For $N\geq3$, the square torus graph has vertex set $(\mathbb Z/N\mathbb Z)^2$ and joins vertices differing by one in exactly one coordinate. It has $N^2$ vertices and $2N^2$ bonds. Translations act transitively on vertices; translations together with a quarter turn act transitively on bonds. A rectangle of side lengths at most $N-2$ has the same induced subgraph as its planar [square lattice](#square-lattice) counterpart.

## Dual graph

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_graph)

For a [graph](graph.md) with a cellular embedding on a surface, the dual has one vertex for each face and an edge crossing each original edge between its adjacent faces. Each edge is counted, including a loop when the two incident faces coincide. The [planar dual graph](graph-theory.md#planar-dual-graph) is the case of a planar embedding.

## Cubic graph

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cubic_graph)

A [graph](graph.md) whose every [vertex](#vertex-graph-theory) has [degree of a vertex](graph-theory.md#degree-graph-theory) three.

### Heawood graph

↑ **Parent:** [Cubic graph](#cubic-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heawood_graph)

The bipartite [cubic graph](#cubic-graph) with vertices $A_i,B_i$, $i\in\mathbb Z/7\mathbb Z$, and edges $A_iB_i,A_iB_{i+1},A_iB_{i-2}$. The three offsets give a [Tait coloring](graph-theory.md#tait-coloring).

#### Heawood torus map

↑ **Parent:** [Heawood graph](#heawood-graph)

Triangulate a [torus](topology.md#torus) using the seven vertices of the [complete graph](graph-theory.md#complete-graph) $K_7$ and oriented triangles $(i,i+1,i+3)$ and $(i,i+3,i+2)$, with indices modulo seven. Every edge occurs twice with opposite orientations; each vertex has a cyclic link. The [Euler characteristic](homology.md#euler-characteristic) is $7-21+14=0$. Its [dual graph](#dual-graph) is the [Heawood graph](#heawood-graph). This dual map has seven disc faces, each adjacent to all the others, so it needs seven face colors although its edges have a [Tait coloring](graph-theory.md#tait-coloring).

## Strong product of graphs

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strong_product_of_graphs)

Its vertices are pairs of vertices. Two distinct pairs are adjacent exactly when, in each coordinate, their entries are equal or adjacent in the corresponding [graph](graph.md). Cartesian products of independent sets are independent, giving supermultiplicativity of the [independence number](graph-theory.md#independence-number).

### Strong graph power

↑ **Parent:** [Strong product of graphs](#strong-product-of-graphs)

An iterated [strong graph product](#strong-product-of-graphs) has vertices that are words of length $m$ in the graph's vertex set. Distinct words are nonadjacent exactly when some coordinate contains distinct nonadjacent entries. This differs from the distance-based [graph power](#graph-power).

#### Shannon capacity of a graph

↑ **Parent:** [Strong graph power](#strong-graph-power)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shannon_capacity_of_a_graph)

The capacity is the exponential growth rate of the independence numbers of strong graph powers. Products of independent sets make these numbers supermultiplicative, and [Fekete lemma](real-analysis.md#fekete-s-lemma) gives the limit and its equality to the supremum. Passing to every second power gives $c(G\boxtimes G)=c(G)^2$.

##### Haemers rank bound

↑ **Parent:** [Shannon capacity of a graph](#shannon-capacity-of-a-graph)

A fitting matrix over a field has nonzero diagonal entries and zero entries at distinct nonadjacent vertices. Its tensor powers fit strong graph powers. On an independent set the restricted matrix is diagonal and nonsingular, so its cardinality is at most the matrix rank. This yields the capacity upper bound over every field.

###### Polynomial representation of a graph

↑ **Parent:** [Haemers rank bound](#haemers-rank-bound)

Choose points $a_v\in F^r$ and polynomials $f_v$ in a finite-dimensional polynomial space $M$, with $f_v(a_v)\ne0$ and $f_v(a_w)=0$ for distinct nonadjacent vertices. Evaluation produces a fitting matrix of rank at most $\dim_F M$. Equivalently, tensoring the polynomial spaces gives linearly independent polynomials for every independent code in a strong power, proving $c(G)\leq\dim_F M$.

##### Complement-pair capacity gain

↑ **Parent:** [Shannon capacity of a graph](#shannon-capacity-of-a-graph)

In each word pattern with equally many $G$ and complement coordinates, pair the coordinates of the two types and put the same vertex label in each pair. Distinct labels are separated in one of the two graphs, making an independent code of size $n^m$ for a pattern of length $2m$. Distinct patterns lie in different graph components, so their codes combine to an independent set of size $\binom{2m}m n^m$. Taking $2m$th roots gives the displayed bound.

###### Nonadditivity of Shannon capacity

↑ **Parent:** [Complement-pair capacity gain](#complement-pair-capacity-gain)

Capacity of a disjoint union can strictly exceed the sum of the capacities. On the five-element subsets of a twenty-point set, join distinct sets when their intersection is odd. Linear polynomials over $\mathbb F_2$ bound its capacity by twenty; squarefree quadratic polynomials over $\mathbb F_3$ bound its complement's capacity by $\binom{20}2=190$. The complement-pair lower bound is $2\sqrt{\binom{20}5}>210$, establishing strict nonadditivity.

##### Pentagon capacity code

↑ **Parent:** [Shannon capacity of a graph](#shannon-capacity-of-a-graph)

These five words are independent in the strong square of the [cycle graph](graph-theory.md#cycle-graph) $C_5$: a nonzero difference is a nonedge in the first or the second coordinate. A three-dimensional orthonormal representation with common vertical squared component $1/\sqrt5$ proves the matching upper bound. Consequently $c(C_5)=\vartheta(C_5)=\sqrt5$.

## Incidence matrix

↑ **Parent:** [Graph](graph.md)

A vertex-edge incidence matrix records which [vertices](#vertex-graph-theory) are endpoints of each [edge](graph-theory.md#edge-of-a-graph) of a [graph](graph.md). The unsigned convention uses entries one at the endpoints, with a convention for loops. Choosing an orientation gives the [oriented incidence matrix](#oriented-incidence-matrix), with minus one at the initial endpoint and plus one at the terminal endpoint. These are different conventions and should be specified when using the matrix in a computation.

## Amenable graph

↑ **Parent:** [Graph](graph.md)

A bounded-degree infinite [graph](graph.md) is amenable when there are finite nonempty vertex sets $W_n$ such that $|\partial^+W_n|/|W_n|\to0$, where $\partial^+W_n$ is the set of vertices outside $W_n$ adjacent to it. These are graph [Følner sets](#folner-set). Amenability makes surface contributions negligible compared with volume. The square lattice and any periodic finite decoration of it are examples.

<h3 id="folner-set">Følner set</h3>

↑ **Parent:** [Amenable graph](#amenable-graph)

A finite nonempty vertex set in an [amenable graph](#amenable-graph) is a Følner set with tolerance $\varepsilon$ if its external boundary has size at most $\varepsilon$ times its volume. A graph [Følner sequence](geometric-group-theory.md#folner-sequence) consists of such sets with tolerances tending to zero. For a bounded-degree [graph](graph.md), every fixed-thickness boundary layer also has negligible relative volume along this sequence.

## Multigraph

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multigraph)

A multigraph permits distinct [edges](graph-theory.md#edge-of-a-graph) with the same pair of endpoints. Whether loops are also allowed is a convention that must be specified for a particular result. Counting edges with multiplicity differs from counting adjacent vertices.

### Bouquet graph

↑ **Parent:** [Multigraph](#multigraph)

A bouquet graph consists of one vertex and $j$ [self-loops](#loop-graph-theory). Its vertex has degree $2j$, and its [graph excess](graph-theory.md#graph-excess) is $j-1$. The two-loop bouquet is one of the three possible kernels of a [bicyclic graph](graph-theory.md#bicyclic-graph); in a simple subdivision, each loop must expand to a cycle of length at least three.

## Distance-transitive graph

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Distance-transitive_graph)

An automorphism group is transitive on ordered pairs of vertices at every fixed distance. [Grassmann graphs](differential-geometry.md#grassmann-graph) provide examples with the finite general linear group as a distance-transitive automorphism group.

### Distance-transitive action on a graph

↑ **Parent:** [Distance-transitive graph](#distance-transitive-graph)

A subgroup of the [graph automorphism](#graph-automorphism) group acts distance-transitively when it is [transitive](set-theory.md#transitive-relation) on the [ordered pairs](set.md#ordered-pair) of [vertices](#vertex-graph-theory) at each fixed [graph distance](graph-theory.md#distance-graph-theory). Thus two vertex pairs at the same distance can be matched by one automorphism from that subgroup. Existence of such a subgroup implies that the full automorphism group has the same property, making the graph a [distance-transitive graph](#distance-transitive-graph). The specified subgroup need not be the entire automorphism group.

### Symplectic dual polar graph

↑ **Parent:** [Distance-transitive graph](#distance-transitive-graph)

Vertices are [Lagrangian subspaces](symplectic-geometry.md#lagrangian-subspace) of a $2m$-dimensional [symplectic vector space](linear-algebra.md#symplectic-vector-space), joined when they intersect in codimension one. A pair with intersection dimension $m-r$ admits a [symplectic basis](linear-algebra.md#symplectic-basis) in which $U=\langle e_1,\ldots,e_m\rangle$ and $W=\langle f_1,\ldots,f_r,e_{r+1},\ldots,e_m\rangle$. Replacing $e_i$ successively by $f_i$ gives an isotropic path of length $r$, while one edge can increase intersection dimension with a fixed target by at most one. Equal-distance ordered pairs have the same adapted form, so the [symplectic group](symplectic-geometry.md#symplectic-group) acts [distance-transitively](#distance-transitive-action-on-a-graph).

## Vertex-transitive graph

↑ **Parent:** [Graph](graph.md)

A [graph](graph.md) whose automorphisms act transitively on its vertices: any chosen [vertex of a graph](#vertex-graph-theory) can be carried to any other by a symmetry preserving adjacency. Consequently rooted [self-avoiding walk](combinatorics.md#self-avoiding-walk) counts are independent of the chosen root.

## Triangular lattice

↑ **Parent:** [Graph](graph.md)

The planar [graph](graph.md) with vertices $\{a(1,0)+b(1/2,\sqrt3/2):a,b\in\mathbb Z\}$ and [edges](graph-theory.md#edge-of-a-graph) between vertices at Euclidean distance one. Every [vertex of a graph](#vertex-graph-theory) has six neighbors. Its [site percolation](site-percolation.md) model is a particularly tractable setting for [conformal invariance of planar percolation](probability-theory.md#conformal-invariance-of-planar-percolation).

## False twin

↑ **Parent:** [Graph](graph.md)

Distinct [vertices](#vertex-graph-theory) with equal open neighbourhoods are false twins. They are nonadjacent: adjacency would put one [vertex](#vertex-graph-theory) in the other's open neighbourhood but not its own. Equal open neighbourhoods define [false-twin classes](#false-twin-class), which are independent sets and have uniform adjacency to every other such class.

### False-twin class

↑ **Parent:** [False twin](#false-twin)

A false-twin class is an equivalence class of [vertices](#vertex-graph-theory) with identical open neighbourhoods. In [edge-triangle symmetrization](graph-theory.md#edge-triangle-symmetrization), merging nonadjacent false-twin classes by cloning the better local score never decreases the objective. A secondary maximization of squared class sizes forces all distinct classes to be adjacent, giving a [complete multipartite graph](graph-theory.md#complete-multipartite-graph).

## Graph power

↑ **Parent:** [Graph](graph.md)

The $j$th power of a [graph](graph.md) joins distinct [vertices](#vertex-graph-theory) whenever their distance in the original [graph](graph.md) is at most $j$. For example, the [square of a cycle](#square-of-a-cycle) adds [edges](graph-theory.md#edge-of-a-graph) connecting [vertices](#vertex-graph-theory) two steps apart. Graph powers turn constraints on short paths into adjacency constraints.

### Square of a cycle

↑ **Parent:** [Graph power](#graph-power)

In a cycle square, each triple of consecutive [vertices](#vertex-graph-theory) is a [clique](graph-theory.md#clique-graph-theory). A proper three-colouring therefore repeats with period three and closes exactly when the length is divisible by three. For all other cycle lengths at least four colours are needed; the five-cycle square is a complete five-vertex [graph](graph.md).

## Graph cut

↑ **Parent:** [Graph](graph.md)

A graph cut consists of the [edges](graph-theory.md#edge-of-a-graph) joining a vertex subset to its complement. In a two-group [stochastic block model](statistical-modelling.md#stochastic-block-model), crossing and within-group [edges](graph-theory.md#edge-of-a-graph) have different [Bernoulli distributions](discrete-probability-distribution.md#bernoulli-distribution). The [Kullback-Leibler divergence](probability-and-statistics.md#kullback-leibler-divergence) between two such models is the sum of the changed-edge divergences, with their order determined by which partition regards the [edge](graph-theory.md#edge-of-a-graph) as crossing.

### Balanced component cut

↑ **Parent:** [Graph cut](#graph-cut)

If every [graph component](#component-graph-theory) has at most $(k+1)n/[k(2k+1)]$ [vertices](#vertex-graph-theory), assigning whole [graph components](#component-graph-theory) to two sides gives an empty [graph cut](#graph-cut) with the displayed bound. To prove it, maximize the smaller side's weight $S\leq n/2$. If $S<kn/(2k+1)$, every component on the larger side has weight at least $n-2S$, because moving a smaller one would improve the smaller side. There are at least $k+1$ such components, since their total exceeds $k$ times the permitted maximum weight. Thus $n-S\geq(k+1)(n-2S)$, a contradiction. The proof also works for arbitrary positive weights.

## Oriented incidence matrix

↑ **Parent:** [Graph](graph.md)

An oriented incidence matrix records an arbitrarily chosen orientation of each [edge](graph-theory.md#edge-of-a-graph) of a [graph](graph.md). Use one row per [edge](graph-theory.md#edge-of-a-graph), with $+1$ and $-1$ at its endpoints and zeros elsewhere; the transpose convention is also common. The product $D\theta$ records endpoint differences. For a [connected graph](#connected-graph), $\ker D=\operatorname{span}\{\mathbf1\}$, since zero difference propagates along every [graph path](graph-theory.md#path-in-a-graph).

### Incidence pseudoinverse decomposition

↑ **Parent:** [Oriented incidence matrix](#oriented-incidence-matrix)

For a [connected graph](#connected-graph), the [Moore-Penrose inverse](linear-algebra.md#moore-penrose-inverse) of its [oriented incidence matrix](#oriented-incidence-matrix) satisfies $D^\dagger D=I-\Pi_1$, because this product is the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto $(\ker D)^\perp$. Thus every signal decomposes into its constant mean and $D^\dagger D\theta$. Writing $L=\max_e\|(D^\dagger)_{\cdot,e}\|_2$, a [sub-Gaussian random vector](probability-and-statistics.md#sub-gaussian-random-vector) noise gives a simultaneous bound on $\|(D^\dagger)^\top z\|_\infty$ with scale $L\sqrt{\log(m/\delta)}$.

## Cartesian product of graphs

↑ **Parent:** [Graph](graph.md)

For two [graphs](graph.md) $G,H$, their [Cartesian product of graphs](#cartesian-product-of-graphs) has [graph vertices](#vertex-graph-theory) $(g,h)\in V(G)\times V(H)$. Two [graph vertices](#vertex-graph-theory) are adjacent if either their $G$ coordinates agree and their $H$ coordinates are adjacent, or conversely their $H$ coordinates agree and their $G$ coordinates are adjacent. The [ladder graph](#ladder-graph) is the product of a [graph path](graph-theory.md#path-in-a-graph) with $K_2$.

## Ladder graph

↑ **Parent:** [Graph](graph.md)

A [ladder graph](#ladder-graph) is the [Cartesian product of graphs](#cartesian-product-of-graphs) of a [graph path](graph-theory.md#path-in-a-graph) with the two-vertex [complete graph](graph-theory.md#complete-graph) $K_2$. Its two parallel rails are joined by a rung at each position. The [doubly infinite ladder graph](#doubly-infinite-ladder-graph) uses an infinite rail indexed by $\mathbb Z$.

### Doubly infinite ladder graph

↑ **Parent:** [Ladder graph](#ladder-graph)

The [doubly infinite ladder graph](#doubly-infinite-ladder-graph) has [graph vertices](#vertex-graph-theory) $\mathbb Z\times\{0,1\}$, horizontal [edges](graph-theory.md#edge-of-a-graph) $\{(j,s),(j+1,s)\}$, and vertical [edges](graph-theory.md#edge-of-a-graph) $\{(j,0),(j,1)\}$.

## Cubic lattice

↑ **Parent:** [Graph](graph.md)

The [cubic lattice](#cubic-lattice) in dimension $d$ has [graph vertex](#vertex-graph-theory) [set](set.md) $\mathbb Z^d$ and an [edge](graph-theory.md#edge-of-a-graph) between $x,y$ exactly when $\sum_i|x_i-y_i|=1$. For $d=2$ it is the [square lattice](#square-lattice). Every [graph vertex](#vertex-graph-theory) has $2d$ [graph neighbours](graph-theory.md#neighbour-of-a-vertex), so it is a [locally finite graph](graph-theory.md#locally-finite-graph).

### Amenable boundary growth of lattice boxes

↑ **Parent:** [Cubic lattice](#cubic-lattice)

For the nearest-neighbour graph on $\mathbb Z^d$, a box $B_n=[-n,n]^d\cap\mathbb Z^d$ has $(2n+1)^d$ [graph vertices](#vertex-graph-theory) and outer [graph vertex](#vertex-graph-theory) boundary of size $2d(2n+1)^{d-1}$. Thus $|\partial^+B_n|/|B_n|\to0$. This boundary-to-volume property is the geometric mechanism that contradicts a positive volume density of trifurcation points in the uniqueness proof. It realizes the boundary-growth property of the translation [amenable group](geometric-group-theory.md#amenable-group) on the lattice.

## Vertex set

↑ **Parent:** [Graph](graph.md)

The vertex set is the underlying [set](set.md) $V$ of a [graph](graph.md) or [hypergraph](hypergraph.md). In a hypergraph, its hyperedges are subsets of this set; in a simple graph, edges are two-element subsets.

## Graph blow-up

↑ **Parent:** [Graph](graph.md)

A blow-up replaces each vertex of a [graph](graph.md) by an [independent set](graph-theory.md#independent-set-graph-theory), and each original edge by all edges between the corresponding two sets. Replacing every vertex of $K_r$ by $t$ vertices gives the [balanced complete multipartite blow-up](graph-theory.md#balanced-complete-multipartite-blow-up) $K_r(t)$.

### Dense clique family blow-up lemma

↑ **Parent:** [Graph blow-up](#graph-blow-up)

A family of positively many $s$-cliques forces a logarithmic balanced [graph blow-up](#graph-blow-up), which can also contain a matching of that many members of the family. To induct on $s$, prune faces with few extensions, apply induction to the remaining $(s-1)$-faces, and use a matching of those faces as one side of a bipartite incidence [graph](graph.md). The [common neighbourhood from bipartite density](graph-theory.md#common-neighbourhood-from-bipartite-density) estimate selects logarithmically many disjoint faces with polynomially many common extension [vertices](#vertex-graph-theory).

### Vertex cloning in a graph

↑ **Parent:** [Graph blow-up](#graph-blow-up)

Cloning a vertex replaces it by several nonadjacent vertices with identical neighbourhoods. In [homomorphism density](graph-theory.md#homomorphism-density), conditioning on the images of all other vertices reduces cloning to the inequality $\mathbb E p^t\ge(\mathbb E p)^t$ from the [Jensen inequality](real-analysis.md#jensen-s-inequality). Iterated cloning shows that positive clique homomorphism density forces any fixed complete multipartite blow-up.

## Multipartite graph

↑ **Parent:** [Graph](graph.md)

A graph is $r$-partite when its vertices can be partitioned into $r$ classes, each an [independent set](graph-theory.md#independent-set-graph-theory). Edges may be missing between different classes. If all possible edges between different classes occur, it is a [complete multipartite graph](graph-theory.md#complete-multipartite-graph).

## Reachability in a graph

↑ **Parent:** [Graph](graph.md)

A vertex $v$ is reachable from $u$ if a finite path leads from $u$ to $v$, respecting edge directions in a directed [graph](graph.md). For a finite graph, [graph search](#graph-search) decides [reachability](#reachability-in-a-graph) by maintaining the [set](set.md) of discovered vertices; every step discovers a new vertex or examines an edge, so the procedure terminates.

## Graph search

↑ **Parent:** [Graph](graph.md)

A [graph search](#graph-search) explores vertices through incident edges while recording visited vertices. On a finite [graph](graph.md), depth-first or breadth-first exploration terminates and decides [reachability](#reachability-in-a-graph); recording predecessors also gives a path. Restricting to vertices reachable from a start and able to reach an accepting vertex identifies the productive part of a [deterministic finite automaton](foundations-of-mathematics.md#deterministic-finite-automaton).

## Tripartite graph

↑ **Parent:** [Graph](graph.md)

A tripartite [graph](graph.md) has a [set partition](combinatorics.md#set-partition) of its [vertices](#vertex-graph-theory) into three classes, with every [edge](graph-theory.md#edge-of-a-graph) joining different classes. Each pair of classes induces a [bipartite graph](graph-theory.md#bipartite-graph), and every [triangle in a graph](#triangle-in-a-graph) uses one [vertex](#vertex-graph-theory) from each class.

### Tripartite graph encoding of a grid

↑ **Parent:** [Tripartite graph](#tripartite-graph)

For $A\subseteq[n]^2$, use three disjoint labelled [vertex](#vertex-graph-theory) classes $X=[n]$, $Y=[n]$, $Z=[2n]$. Each $(x,y)\in A$ inserts the three [edges](graph-theory.md#edge-of-a-graph) $xy,x(x+y),y(x+y)$, producing pairwise [edge-disjoint triangles](#edge-disjoint-triangles). Every [triangle in a graph](#triangle-in-a-graph) with labels $(x,y,z)$ corresponds to the three points $(x,y),(x,z-x),(z-y,y)$ of $A$. It is canonical when $z=x+y$; otherwise it gives a [corner in an integer grid](additive-combinatorics.md#corner-in-an-integer-grid) with nonzero displacement $z-x-y$.

## Graph automorphism

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_automorphism)

A graph automorphism is a bijection of the vertex set that preserves adjacency. It preserves graph distances and transports simple random-walk hitting problems between vertices.

### Quasi-transitive graph

↑ **Parent:** [Graph automorphism](#graph-automorphism)

A [graph](graph.md) is quasi-transitive if some group of [graph automorphisms](#graph-automorphism) has finitely many vertex orbits. This is also called a graph of finite type. A [connected graph](#connected-graph) that is infinite and a [locally finite graph](graph-theory.md#locally-finite-graph) then has uniformly bounded degrees. Every orbit is infinite: a finite invariant orbit would have finite neighborhoods, and finitely many orbit types would put the entire graph in one such neighborhood. This permits finite sets to be moved arbitrarily far apart by [graph automorphisms](#graph-automorphism).

## Bridge (graph theory)

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bridge_(graph_theory))

A bridge is an edge whose deletion increases the number of components of a graph. Equivalently, it belongs to no cycle; within its original component, deleting it makes the [connected graph](#connected-graph) disconnected.

## Hypercube graph

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypercube_graph)

The $d$-dimensional hypercube graph has vertex set $\{0,1\}^d$ and joins two vertices exactly when they differ in one coordinate. It is a $d$-regular [bipartite graph](graph-theory.md#bipartite-graph) on $2^d$ vertices.

### Gray code

↑ **Parent:** [Hypercube graph](#hypercube-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gray_code)

A Gray code orders binary strings so that successive strings differ in exactly one bit. Consequently it describes a path in a [hypercube graph](#hypercube-graph); a cyclic Gray code describes a cycle.

## Square lattice

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square_lattice)

The square lattice has vertex set $\mathbb Z^2$ and joins vertices whose Euclidean distance is one.

## Connectivity (graph theory)

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Connectivity_(graph_theory))

Connectivity studies the existence of paths between [vertices of a graph](#vertex-graph-theory) and the persistence of paths after vertex or edge deletions. A [connected graph](#connected-graph) is the basic case in which every pair of vertices is linked by a path.

### Connected graph

↑ **Parent:** [Connectivity (graph theory)](#connectivity-graph-theory)

A graph is connected when every pair of [vertices](#vertex-graph-theory) is joined by a path.

#### Component (graph theory)

↑ **Parent:** [Connected graph](#connected-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Component_(graph_theory))

A connected component is a maximal connected subgraph.

##### Supermodularity of graph component count

↑ **Parent:** [Component (graph theory)](#component-graph-theory)

For open-edge sets $S,T$ in a fixed finite graph, including isolated [graph vertices](#vertex-graph-theory) in $k$, one has $k(S\cap T)+k(S\cup T)\ge k(S)+k(T)$. Incidence-vector spans have rank $r(S)=|V|-k(S)$; their union span is the sum of the two spans, while the intersection-edge span is contained in the intersection of spans. The vector-space [dimension formula for a sum of subspaces](vector-space.md#dimension-formula-for-a-sum-of-subspaces) proves submodularity of $r$, equivalently supermodularity of $k$.

##### Tree component

↑ **Parent:** [Component (graph theory)](#component-graph-theory)

A tree component is a [graph component](#component-graph-theory) whose induced [graph](graph.md) is a [tree](combinatorics.md#tree-graph-theory). A [tree component](#tree-component) with $j$ [vertices](#vertex-graph-theory) has exactly $j-1$ [edges](graph-theory.md#edge-of-a-graph).

##### Largest component of a graph

↑ **Parent:** [Component (graph theory)](#component-graph-theory)

The largest [graph component](#component-graph-theory) is one with the most [vertices](#vertex-graph-theory). Ties may be broken arbitrarily; $L_1$ records the order, which is unaffected by the tie. For a sequence of [random graphs](graph-theory.md#random-graph), the size of its [giant component](graph-theory.md#giant-component) is a central observable.

## Vertex (graph theory)

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vertex_(graph_theory))

A vertex is one of the objects joined by the [edges](graph-theory.md#edge-of-a-graph) of a graph.

## Graph isomorphism

↑ **Parent:** [Graph](graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_isomorphism)

Two graphs are isomorphic when a [bijection](function.md#bijection) between their vertex sets preserves adjacency.

## Triangle in a graph

↑ **Parent:** [Graph](graph.md)

A triangle is a set of three vertices joined by all three possible edges, equivalently a copy of $K_3$.

### Edge-disjoint triangles

↑ **Parent:** [Triangle in a graph](#triangle-in-a-graph)

A family of [triangles in a graph](#triangle-in-a-graph) is edge-disjoint if no [edge](graph-theory.md#edge-of-a-graph) belongs to two members. Any deletion of [edges](graph-theory.md#edge-of-a-graph) producing a [triangle-free graph](#triangle-free-graph) must remove at least one distinct [edge](graph-theory.md#edge-of-a-graph) for each member. The [triangles in a graph](#triangle-in-a-graph) may share [vertices](#vertex-graph-theory).

### Triangle count

↑ **Parent:** [Triangle in a graph](#triangle-in-a-graph)

The triangle count of a finite simple [graph](graph.md) is the number of unordered triples of [vertices](#vertex-graph-theory) inducing a [triangle in a graph](#triangle-in-a-graph). In a [tripartite graph](#tripartite-graph) with parts $X,Y,Z$ and adjacency [indicator functions](measure-theory.md#indicator-function) $g_{XY},g_{YZ},g_{XZ}$, it equals $|X||Y||Z|\mathbb E_{x,y,z}g_{XY}(x,y)g_{YZ}(y,z)g_{XZ}(x,z)$, using uniform [expectations](probability-theory.md#expected-value) on nonempty parts.

### Triangle-free graph

↑ **Parent:** [Triangle in a graph](#triangle-in-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Triangle-free_graph)

A triangle-free graph contains no [triangle](#triangle-in-a-graph).

#### Triangle-free chromatic lower bound at bounded maximum degree

↑ **Parent:** [Triangle-free graph](#triangle-free-graph)

Choose $n=d^7$ and a [binomial random graph](graph-theory.md#binomial-random-graph) of edge probability $d/n$. With high probability its maximum degree is at most $2d$, it has $o(n)$ triangles, and every [independent set](graph-theory.md#independent-set-graph-theory) has size at most $4n\log d/d$. Delete one vertex per triangle. The resulting [triangle-free graph](#triangle-free-graph) has chromatic number at least $d/(8\log d)$. Appending a disjoint star of degree $2d$, if necessary, makes the maximum degree exactly $2d$ without lowering the chromatic number. Thus the order $\Delta/\log\Delta$ is unavoidable.

### Edge-triangle incidence bound

↑ **Parent:** [Triangle in a graph](#triangle-in-a-graph)

If every edge of a graph lies in at least one triangle, then the number of triangles is at least one third of the number of edges. Count edge-triangle incidences: each edge contributes at least one and each triangle contributes three.

## Vertex neighbourhood

↑ **Parent:** [Graph](graph.md)

The neighbourhood $\Gamma(v)$ of a vertex $v$ is the set of vertices adjacent to $v$.

## ↑ Ancestors (5)

1. [Graph theory](graph-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (280)

- [A cycle and a transposition generate the symmetric group exactly at coprime separation](finite-group-theory.md#a-cycle-and-a-transposition-generate-the-symmetric-group-exactly-at-coprime-separation)
- [Admissible crystallographic Coxeter graph](lie-theory.md#admissible-crystallographic-coxeter-graph)
- [Aldous spectral gap theorem](markov-process.md#aldous-spectral-gap-theorem)
- [Alternating count of common-center graphs](graph-theory.md#alternating-count-of-common-center-graphs)
- [Amenable graph](#amenable-graph)
- [Average degree of a graph](graph-theory.md#average-degree-of-a-graph)
- [Balanced complete multipartite blow-up](graph-theory.md#balanced-complete-multipartite-blow-up)
- [Bernoulli invariant laws of finite symmetric exclusion](stochastic-process.md#bernoulli-invariant-laws-of-finite-symmetric-exclusion)
- [Bipartite stability from few odd cycles](graph-theory.md#bipartite-stability-from-few-odd-cycles)
- [Canonical paths for the weighted matching chain](markov-process.md#canonical-paths-for-the-weighted-matching-chain)
- [Caro-Wei bound](graph-theory.md#caro-wei-bound)
- [Cartesian product of graphs](#cartesian-product-of-graphs)
- [Chordal graph](graph-theory.md#chordal-graph)
- [Clique conflict graph](graph-theory.md#clique-conflict-graph)
- [Clique number](graph-theory.md#clique-number)
- [Clique removal lemma](probabilistic-combinatorics.md#clique-removal-lemma)
- [Colouring number of a hereditary graph property](graph-theory.md#colouring-number-of-a-hereditary-graph-property)
- [Common-center graph property](graph-theory.md#common-center-graph-property)
- [Complement theta number](graph-theory.md#complement-theta-number)
- [Connectedness of adjacent-level incidence in a Boolean lattice](extremal-set-theory.md#connectedness-of-adjacent-level-incidence-in-a-boolean-lattice)
- [Connectivity of random k-out graphs](graph-theory.md#connectivity-of-random-k-out-graphs)
- [Cubic graph](#cubic-graph)
- [Cut vertex](graph-theory.md#cut-vertex)
- [Degree sequence](graph-theory.md#degree-sequence)
- [Dense clique family blow-up lemma](#dense-clique-family-blow-up-lemma)
- [Dense minor with bounded order and high minimum degree](graph-theory.md#dense-minor-with-bounded-order-and-high-minimum-degree)
- [Diameter bound for a fixed-density binomial random graph](graph-theory.md#diameter-bound-for-a-fixed-density-binomial-random-graph)
- [Directed edge occupation in a random-walk commute](markov-process.md#directed-edge-occupation-in-a-random-walk-commute)
- [Dual graph](#dual-graph)
- [Edge contraction](graph-theory.md#edge-contraction)
- [Edge of a graph](graph-theory.md#edge-of-a-graph)
- [Edge-triangle symmetrization](graph-theory.md#edge-triangle-symmetrization)
- [Edit-distance stability for clique-free graphs](graph-theory.md#edit-distance-stability-for-clique-free-graphs)
- [Entropy bound for graphs with isolated-vertex-free intersections](information-theory.md#entropy-bound-for-graphs-with-isolated-vertex-free-intersections)
- [Enumeration of subgraph-closed graph properties](graph-theory.md#enumeration-of-subgraph-closed-graph-properties)
- [Equitable regularity energy](probabilistic-combinatorics.md#equitable-regularity-energy)
- [Expander mixing lemma](graph-theory.md#expander-mixing-lemma)
- [Extremal graph for disjoint cliques](graph-theory.md#extremal-graph-for-disjoint-cliques)
- [Fill-path criterion for symmetric elimination](numerical-analysis.md#fill-path-criterion-for-symmetric-elimination)
- [Finite lattice approximation for monotone clique circuits](computer-science.md#finite-lattice-approximation-for-monotone-clique-circuits)
- [Følner set](#folner-set)
- [Forced merging of large components](graph-theory.md#forced-merging-of-large-components)
- [Foster's theorem](markov-process.md#foster-s-theorem)
- [Four-cycle counting by common neighbours](graph-theory.md#four-cycle-counting-by-common-neighbours)
- [Four-tile mixed-boundary transplantation between a disk and a nonorientable surface](riemannian-geometry.md#four-tile-mixed-boundary-transplantation-between-a-disk-and-a-nonorientable-surface)
- [Global survival threshold of the contact process](stochastic-process.md#global-survival-threshold-of-the-contact-process)
- [Graph adjacency](#graph-adjacency)
- [Graph blow-up](#graph-blow-up)
- [Graph exhaustion](graph-theory.md#graph-exhaustion)
- [Graph intersection](graph-theory.md#graph-intersection)
- [Graph minor](graph-theory.md#graph-minor)
- [Graph of a function](function.md#graph-of-a-function)
- [Graph power](#graph-power)
- [Graph property](graph-theory.md#graph-property)
- [Graph search](#graph-search)
- [Graph total variation denoising](inverse-problem.md#graph-total-variation-denoising)
- [Greedy coloring](graph-theory.md#greedy-coloring)
- [Hereditary graph enumeration theorem](graph-theory.md#hereditary-graph-enumeration-theorem)
- [Hereditary graph property](graph-theory.md#hereditary-graph-property)
- [High-minimum-degree multipartite stability subgraph](graph-theory.md#high-minimum-degree-multipartite-stability-subgraph)
- [Hypergraph](hypergraph.md)
- [Hypergraph independent set](hypergraph.md#hypergraph-independent-set)
- [Hypergraph link graph](hypergraph.md#hypergraph-link-graph)
- [Incidence matrix](#incidence-matrix)
- [Independence digraph of events](probabilistic-combinatorics.md#independence-digraph-of-events)
- [Independent sets in every large subset of a dense random graph](graph-theory.md#independent-sets-in-every-large-subset-of-a-dense-random-graph)
- [Independent transversal](graph-theory.md#independent-transversal)
- [Interchange process](markov-process.md#interchange-process)
- [Irregular pair of vertex sets](probabilistic-combinatorics.md#irregular-pair-of-vertex-sets)
- [Isoperimetric number of a graph](combinatorics.md#isoperimetric-number-of-a-graph)
- [Kernel cover of a real projective plane wedged with a circle](algebraic-topology.md#kernel-cover-of-a-real-projective-plane-wedged-with-a-circle)
- [Killed-walk occupation voltage](markov-process.md#killed-walk-occupation-voltage)
- [Kirchhoff's theorem](combinatorics.md#kirchhoff-s-theorem)
- [Kneser graph](graph-theory.md#kneser-graph)
- [Lévy family of graphs](probability-theory.md#levy-family-of-graphs)
- [Local survival threshold of the contact process](stochastic-process.md#local-survival-threshold-of-the-contact-process)
- [Logarithmic Erdős-Stone theorem](graph-theory.md#logarithmic-erdos-stone-theorem)
- [Loop (graph theory)](#loop-graph-theory)
- [Lovász number](graph-theory.md#lovasz-number)
- [Matrix graph](numerical-analysis.md#matrix-graph)
- [Max-TSP](mathematical-optimization.md#max-tsp)
- [Maximum degree](graph-theory.md#maximum-degree)
- [Minimum degree algorithm](numerical-analysis.md#minimum-degree-algorithm)
- [Minimum degree of an extremal forbidden-subgraph graph](graph-theory.md#minimum-degree-of-an-extremal-forbidden-subgraph-graph)
- [Modular intersection graph](extremal-set-theory.md#modular-intersection-graph)
- [Monochromatic line-graph percolation counterexample](site-percolation.md#monochromatic-line-graph-percolation-counterexample)
- [Near-perfect matching](graph-theory.md#near-perfect-matching)
- [Neighbour of a vertex](graph-theory.md#neighbour-of-a-vertex)
- [Network meta-analysis](statistical-inference.md#network-meta-analysis)
- [Octahedral graph](graph-theory.md#octahedral-graph)
- [Odd-cycle copies from positive triangle density](probabilistic-combinatorics.md#odd-cycle-copies-from-positive-triangle-density)
- [Orientation of a graph](graph-theory.md#orientation-of-a-graph)
- [Oriented incidence matrix](#oriented-incidence-matrix)
- [Outdegree orientation criterion](graph-theory.md#outdegree-orientation-criterion)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-11.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-11.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-11.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-11.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-28.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-28.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-11.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-11.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-11.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1.md#17f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1.md#18h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-12.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-13.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-36.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-36.md#2/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-37.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-37.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-37.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-3.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2.md#17f/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2.md#17f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2.md#21g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#17f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#17f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-22.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#3f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-10.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-11.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-19.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-10.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-26.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-26.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-26.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-26.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-59.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-59.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-59.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-28.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#14i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#14i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#14i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-12.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-109.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-3.md#8e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#16h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#15h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#19i/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#19i/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#15h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#16h/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#16h/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#16h/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#17i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-110.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#17g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339.md#2/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339.md#2/c/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#17g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#17f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#17f/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-134.md#1/a/solution)
- [Perfect elimination ordering](graph-theory.md#perfect-elimination-ordering)
- [Petersen graph](graph-theory.md#petersen-graph)
- [Positive clique error of a truncated lattice meet](computer-science.md#positive-clique-error-of-a-truncated-lattice-meet)
- [Potts model](statistical-physics.md#potts-model)
- [Prim's algorithm](combinatorics.md#prim-s-algorithm)
- [Prime-degree transposition criterion](group-theory.md#prime-degree-transposition-criterion)
- [Prime-regular subgraph from Boolean polynomial constraints](combinatorics.md#prime-regular-subgraph-from-boolean-polynomial-constraints)
- [Quasi-transitive graph](#quasi-transitive-graph)
- [Rado graph](graph-theory.md#rado-graph)
- [Random branch-set construction of a complete graph minor](graph-theory.md#random-branch-set-construction-of-a-complete-graph-minor)
- [Random k-out graph](graph-theory.md#random-k-out-graph)
- [Reachability in a graph](#reachability-in-a-graph)
- [Refinement of a set partition](combinatorics.md#refinement-of-a-set-partition)
- [Refinement variance identity for regularity energy](probabilistic-combinatorics.md#refinement-variance-identity-for-regularity-energy)
- [Resolvent bound for a discrete SIR epidemic](mathematical-biology.md#resolvent-bound-for-a-discrete-sir-epidemic)
- [Reverse-delete algorithm](combinatorics.md#reverse-delete-algorithm)
- [Right-angled Artin group](geometric-group-theory.md#right-angled-artin-group)
- [Root-moment bound for open self-avoiding walks](combinatorics.md#root-moment-bound-for-open-self-avoiding-walks)
- [Rooted branch-set reduction](graph-theory.md#rooted-branch-set-reduction)
- [Rooted dense minor linkage](graph-theory.md#rooted-dense-minor-linkage)
- [Self-avoiding walk](combinatorics.md#self-avoiding-walk)
- [Semicoloring](graph-theory.md#semicoloring)
- [Semicoloring by independent hyperplanes](graph-theory.md#semicoloring-by-independent-hyperplanes)
- [Simple graph](#simple-graph)
- [Simultaneous giant for fixed random-edge choice](graph-theory.md#simultaneous-giant-for-fixed-random-edge-choice)
- [Spectral graph theory](graph-theory.md#spectral-graph-theory)
- [Speed of a graph property](graph-theory.md#speed-of-a-graph-property)
- [Square of a cycle](#square-of-a-cycle)
- [Squaring and zig-zag iteration yields bounded-degree expanders](functional-analysis.md#squaring-and-zig-zag-iteration-yields-bounded-degree-expanders)
- [Strict vector coloring](graph-theory.md#strict-vector-coloring)
- [Strictly balanced graph](graph-theory.md#strictly-balanced-graph)
- [Strong product of graphs](#strong-product-of-graphs)
- [Subgraph-closed graph property](graph-theory.md#subgraph-closed-graph-property)
- [Topology of disk tiles glued along disjoint boundary arcs](topology.md#topology-of-disk-tiles-glued-along-disjoint-boundary-arcs)
- [Tree component](#tree-component)
- [Tree (graph theory)](combinatorics.md#tree-graph-theory)
- [Triangle count](#triangle-count)
- [Triangle removal lemma](probabilistic-combinatorics.md#triangle-removal-lemma)
- [Triangle support line between bipartite and tripartite Turan graphs](graph-theory.md#triangle-support-line-between-bipartite-and-tripartite-turan-graphs)
- [Triangular lattice](#triangular-lattice)
- [Triangulation of an undirected graph](graph-theory.md#triangulation-of-an-undirected-graph)
- [Trifurcation boundary-counting lemma](bond-percolation.md#trifurcation-boundary-counting-lemma)
- [Tripartite graph](#tripartite-graph)
- [Turán density](hypergraph.md#turan-density)
- [Two-component spanning forest](combinatorics.md#two-component-spanning-forest)
- [Undirected graph](graph-theory.md#undirected-graph)
- [Uniform hypergraph](hypergraph.md#uniform-hypergraph)
- [Uniform random graph process](graph-theory.md#uniform-random-graph-process)
- [Uniform-spanning-tree path representation of loop-erased random walk](markov-process.md#uniform-spanning-tree-path-representation-of-loop-erased-random-walk)
- [Vector coloring](graph-theory.md#vector-coloring)
- [Vertex cover](graph-theory.md#vertex-cover)
- [Vertex cycle cover](graph-theory.md#vertex-cycle-cover)
- [Vertex exposure for chromatic number](graph-theory.md#vertex-exposure-for-chromatic-number)
- [Vertex set](#vertex-set)
- [Vertex-transitive graph](#vertex-transitive-graph)
- [Walk in a graph](graph-theory.md#walk-in-a-graph)
- [Weighted Szemerédi regularity lemma](probabilistic-combinatorics.md#weighted-szemeredi-regularity-lemma)
- [Zig-zag product](functional-analysis.md#zig-zag-product)
