# Graph theory

↑ **Parent:** [Foundations of mathematics](foundations-of-mathematics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_theory)

[Graph theory](graph-theory.md) studies [vertices](graph.md#vertex-graph-theory) and the [edges](#edge-of-a-graph) connecting them: which [graph paths](#path-in-a-graph) exist, how efficiently we can travel, and which connections are indispensable. A road map becomes a [graph](graph.md) when junctions are [vertices](graph.md#vertex-graph-theory) and road segments are [edges](#edge-of-a-graph); a communications network uses routers and links instead. The drawing helps us see connections, but its apparent lengths need not be the costs being optimized. Record travel times or transmission costs separately in a [weighted graph](random-walk.md#weighted-graph).

The appeal of [graph theory](graph-theory.md) is that one model serves many practical questions. [Graph paths](#path-in-a-graph) describe routes, [connected components of a graph](graph.md#component-graph-theory) identify isolated regions, and [minimum spanning trees](tree-graph-theory.md#minimum-spanning-tree) connect all locations cheaply. The [shortest path problem](shortest-path-problem.md) asks a different question: find the cheapest journey between specified locations. Our four-[vertex](graph.md#vertex-graph-theory) example below makes that distinction concrete and shows how the [Dijkstra algorithm](shortest-path-problem.md#dijkstra-algorithm) discovers a route without trying every [graph path](#path-in-a-graph).

**Table of contents**

- [Network robustness](#network-robustness)
  - [Network redundancy](#network-redundancy)
  - [Network resilience](#network-resilience)
    - [Cascading failure](#cascading-failure)
- [Network motif](#network-motif)
- [Réka Albert](#reka-albert)
  - [Work by Réka Albert](#work-by-reka-albert)
- [Albert-László Barabási](#albert-laszlo-barabasi)
  - [Work by Albert-László Barabási](#work-by-albert-laszlo-barabasi)
- [Duncan J. Watts](#duncan-j-watts)
  - [Work by Duncan J. Watts](#work-by-duncan-j-watts)
- [Community detection](#community-detection)
- [Network null model](#network-null-model)
- [Network modularity](#network-modularity)
- [Louvain method](#louvain-method)
- [Eigenvector centrality](#eigenvector-centrality)
- [Degree-preserving edge rewiring](#degree-preserving-edge-rewiring)
- [Scale-free network](#scale-free-network)
- [Degree distribution](#degree-distribution)
- [Small-worldness](#small-worldness)
- [Small-world network](#small-world-network)
- [Clustering coefficient](#clustering-coefficient)
- [Spanning forest](#spanning-forest)
- [Circle graph](#circle-graph)
  - [Permutation graph](#permutation-graph)
    - [Permutation diagram](#permutation-diagram)
- [Graph bandwidth](#graph-bandwidth)
- [Interval graph](#interval-graph)
- [Pathwidth](#pathwidth)
- [Chip-firing game](#chip-firing-game)
  - [Abelian sandpile model](#abelian-sandpile-model)
- [De Bruijn graph](#de-bruijn-graph)
- [Geometric spanner](#geometric-spanner)
- [Graph excess](#graph-excess)
  - [Bicyclic graph](#bicyclic-graph)
    - [Labelled bicyclic graph count](#labelled-bicyclic-graph-count)
    - [Bicyclic kernel classification](#bicyclic-kernel-classification)
- [2-core of a graph](#2-core-of-a-graph)
  - [Leaf pruning for the 2-core](#leaf-pruning-for-the-2-core)
  - [Why the 2-core is unique](#why-the-2-core-is-unique)
  - [Bridges and connectivity in the 2-core](#bridges-and-connectivity-in-the-2-core)
  - [Graph kernel](#graph-kernel)
- [k-core of a graph](#k-core-of-a-graph)
- [Chordal graph](#chordal-graph)
  - [Triangulation of an undirected graph](#triangulation-of-an-undirected-graph)
  - [Perfect elimination ordering](#perfect-elimination-ordering)
    - [Simplicial vertex (graph theory)](#simplicial-vertex-graph-theory)
    - [Maximum cardinality search](#maximum-cardinality-search)
- [Johnson graph](#johnson-graph)
  - [Distance in a Johnson graph](#distance-in-a-johnson-graph)
  - [Maximal cliques of a Johnson graph](#maximal-cliques-of-a-johnson-graph)
- [Maximum degree](#maximum-degree)
- [Four-cycle counting by common neighbours](#four-cycle-counting-by-common-neighbours)
- [Shortest path problem](shortest-path-problem.md)
  - [Shortest path](shortest-path-problem.md#shortest-path)
  - [Label-setting shortest-path algorithm](shortest-path-problem.md#label-setting-shortest-path-algorithm)
  - [Bellman inequalities](shortest-path-problem.md#bellman-inequalities)
  - [Label-correcting shortest-path algorithm](shortest-path-problem.md#label-correcting-shortest-path-algorithm)
  - [Bellman-Ford algorithm](shortest-path-problem.md#bellman-ford-algorithm)
    - [Synchronous Bellman-Ford recurrence](shortest-path-problem.md#synchronous-bellman-ford-recurrence)
    - [Bellman-Ford negative-cycle detection](shortest-path-problem.md#bellman-ford-negative-cycle-detection)
    - [All-to-one Bellman-Ford recurrence](shortest-path-problem.md#all-to-one-bellman-ford-recurrence)
  - [Dijkstra algorithm](shortest-path-problem.md#dijkstra-algorithm)
    - [Tentative distance](shortest-path-problem.md#tentative-distance)
    - [Edge relaxation](shortest-path-problem.md#edge-relaxation)
    - [Shortest-path predecessor](shortest-path-problem.md#shortest-path-predecessor)
- [Graph property](#graph-property)
  - [Common-center graph property](#common-center-graph-property)
    - [Certificates for the common-center graph property](#certificates-for-the-common-center-graph-property)
    - [Alternating count of common-center graphs](#alternating-count-of-common-center-graphs)
  - [Speed of a graph property](#speed-of-a-graph-property)
  - [Hereditary graph property](#hereditary-graph-property)
    - [Colouring number of a hereditary graph property](#colouring-number-of-a-hereditary-graph-property)
      - [Hereditary graph enumeration theorem](#hereditary-graph-enumeration-theorem)
    - [Clique-independent partition class](#clique-independent-partition-class)
  - [Subgraph-closed graph property](#subgraph-closed-graph-property)
    - [Enumeration of subgraph-closed graph properties](#enumeration-of-subgraph-closed-graph-properties)
- [Orientation of a graph](#orientation-of-a-graph)
  - [Acyclic orientation](#acyclic-orientation)
    - [Order-induced acyclic orientation](#order-induced-acyclic-orientation)
  - [Strong orientation](#strong-orientation)
    - [Robbins' theorem](#robbins-theorem)
  - [Outdegree orientation criterion](#outdegree-orientation-criterion)
- [Graph intersection](#graph-intersection)
- [Kneser graph](#kneser-graph)
  - [Lovász theorem on Kneser graphs](#lovasz-theorem-on-kneser-graphs)
- [Cut vertex](#cut-vertex)
  - [Biconnected component](#biconnected-component)
  - [DFS discovery time](#dfs-discovery-time)
  - [DFS lowpoint](#dfs-lowpoint)
- [Hypergraph](hypergraph.md)
  - [Subhypergraph](hypergraph.md#subhypergraph)
    - [Induced subhypergraph](hypergraph.md#induced-subhypergraph)
  - [Matching in a hypergraph](hypergraph.md#matching-in-a-hypergraph)
  - [Hypergraph link graph](hypergraph.md#hypergraph-link-graph)
    - [Fano completion through three matchings](hypergraph.md#fano-completion-through-three-matchings)
  - [Hypergraph colouring](hypergraph.md#hypergraph-colouring)
    - [Hypergraph chromatic index](hypergraph.md#hypergraph-chromatic-index)
      - [Auxiliary matching construction for hypergraph edge colouring](hypergraph.md#auxiliary-matching-construction-for-hypergraph-edge-colouring)
    - [Property B](hypergraph.md#property-b)
      - [Bipartite three-uniform hypergraph](hypergraph.md#bipartite-three-uniform-hypergraph)
    - [Hypergraph chromatic number](hypergraph.md#hypergraph-chromatic-number)
  - [Linear hypergraph](hypergraph.md#linear-hypergraph)
  - [Vertex of a hypergraph](hypergraph.md#vertex-of-a-hypergraph)
  - [Labelled hypergraph copy count](hypergraph.md#labelled-hypergraph-copy-count)
  - [Multipartite hypergraph](hypergraph.md#multipartite-hypergraph)
  - [Edge of a hypergraph](hypergraph.md#edge-of-a-hypergraph)
  - [Polychromatic hypergraph colouring](hypergraph.md#polychromatic-hypergraph-colouring)
    - [Four-vertex obstruction to polychromatic three-colouring](hypergraph.md#four-vertex-obstruction-to-polychromatic-three-colouring)
  - [Hypergraph isomorphism](hypergraph.md#hypergraph-isomorphism)
  - [Hyperedge](hypergraph.md#hyperedge)
  - [Polychromatic coloring of a hypergraph](hypergraph.md#polychromatic-coloring-of-a-hypergraph)
    - [Polychromatic coloring of integer translates](hypergraph.md#polychromatic-coloring-of-integer-translates)
  - [Extremal hypergraph theory](hypergraph.md#extremal-hypergraph-theory)
    - [Fano-plane Turán theorem](hypergraph.md#fano-plane-turan-theorem)
      - [Fano stability](hypergraph.md#fano-stability)
    - [Cyclic Turán covering construction](hypergraph.md#cyclic-turan-covering-construction)
    - [Turán density](hypergraph.md#turan-density)
      - [Hypergraph supersaturation by sampling](hypergraph.md#hypergraph-supersaturation-by-sampling)
      - [de Caen bound for hypergraph Turán density](hypergraph.md#de-caen-bound-for-hypergraph-turan-density)
  - [Multihypergraph](hypergraph.md#multihypergraph)
  - [Hypergraph independent set](hypergraph.md#hypergraph-independent-set)
    - [Hypergraph container](hypergraph.md#hypergraph-container)
      - [Hypergraph container theorem](hypergraph.md#hypergraph-container-theorem)
      - [Golden rule for container algorithms](hypergraph.md#golden-rule-for-container-algorithms)
      - [Container fingerprint](hypergraph.md#container-fingerprint)
  - [Hypergraph vertex degree](hypergraph.md#hypergraph-vertex-degree)
    - [Hypergraph degree measure](hypergraph.md#hypergraph-degree-measure)
    - [Hypergraph codegree](hypergraph.md#hypergraph-codegree)
  - [Uniform hypergraph](hypergraph.md#uniform-hypergraph)
    - [Hereditary hypergraph property](hypergraph.md#hereditary-hypergraph-property)
      - [Normalized speed of a hereditary hypergraph property](hypergraph.md#normalized-speed-of-a-hereditary-hypergraph-property)
    - [Octahedral quasirandomness of a three-uniform hypergraph](hypergraph.md#octahedral-quasirandomness-of-a-three-uniform-hypergraph)
      - [Counting lemma for octahedrally quasirandom three-uniform hypergraphs](hypergraph.md#counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs)
    - [Link hypergraph](hypergraph.md#link-hypergraph)
    - [Countable random uniform hypergraph](hypergraph.md#countable-random-uniform-hypergraph)
    - [Hypergraph extension property](hypergraph.md#hypergraph-extension-property)
      - [Universal countable uniform hypergraph](hypergraph.md#universal-countable-uniform-hypergraph)
        - [Maximal-vertex deletion in a countable universal hypergraph](hypergraph.md#maximal-vertex-deletion-in-a-countable-universal-hypergraph)
    - [Strong regularity for three-uniform hypergraphs](hypergraph.md#strong-regularity-for-three-uniform-hypergraphs)
      - [Triad in a hypergraph regularity partition](hypergraph.md#triad-in-a-hypergraph-regularity-partition)
        - [Tetrahedron counting lemma](hypergraph.md#tetrahedron-counting-lemma)
    - [Hypergraph removal](hypergraph.md#hypergraph-removal)
      - [Tetrahedron removal lemma](hypergraph.md#tetrahedron-removal-lemma)
    - [Complete uniform hypergraph](hypergraph.md#complete-uniform-hypergraph)
      - [Strong saturation of a uniform hypergraph](hypergraph.md#strong-saturation-of-a-uniform-hypergraph)
        - [Exterior-power quotient bound for strong hypergraph saturation](hypergraph.md#exterior-power-quotient-bound-for-strong-hypergraph-saturation)
      - [Three-uniform tetrahedron](hypergraph.md#three-uniform-tetrahedron)
    - [Hypergraph complement](hypergraph.md#hypergraph-complement)
- [Walk in a graph](#walk-in-a-graph)
  - [Trail in a graph](#trail-in-a-graph)
  - [Closed walk](#closed-walk)
- [Undirected graph](#undirected-graph)
  - [Multiple edges](#multiple-edges)
- [Graph minor](graph-minor.md)
  - [Topological minor](graph-minor.md#topological-minor)
  - [Rooted branch-set reduction](graph-minor.md#rooted-branch-set-reduction)
  - [Complete graph minor density threshold](graph-minor.md#complete-graph-minor-density-threshold)
    - [Dense minor with bounded order and high minimum degree](graph-minor.md#dense-minor-with-bounded-order-and-high-minimum-degree)
  - [Branch set of a graph minor](graph-minor.md#branch-set-of-a-graph-minor)
    - [Random branch-set construction of a complete graph minor](graph-minor.md#random-branch-set-construction-of-a-complete-graph-minor)
  - [Edge contraction](graph-minor.md#edge-contraction)
- [Vertex cover](#vertex-cover)
  - [Minimum vertex cover](#minimum-vertex-cover)
    - [Vertex cover number](#vertex-cover-number)
  - [3-SAT reduction to vertex cover](#3-sat-reduction-to-vertex-cover)
- [Binomial random graph](#binomial-random-graph)
  - [Poisson threshold for vertices lying in no triangle](#poisson-threshold-for-vertices-lying-in-no-triangle)
  - [Deferred edge exposure in greedy independent-set colouring](#deferred-edge-exposure-in-greedy-independent-set-colouring)
  - [Strictly balanced graph](#strictly-balanced-graph)
    - [Poisson limit for strictly balanced subgraph counts](#poisson-limit-for-strictly-balanced-subgraph-counts)
  - [Missing common-neighbour count in a binomial random graph](#missing-common-neighbour-count-in-a-binomial-random-graph)
    - [Diameter bound for a fixed-density binomial random graph](#diameter-bound-for-a-fixed-density-binomial-random-graph)
  - [Chromatic number of a binomial random graph](#chromatic-number-of-a-binomial-random-graph)
    - [Independent sets in every large subset of a dense random graph](#independent-sets-in-every-large-subset-of-a-dense-random-graph)
  - [Vertex exposure for chromatic number](#vertex-exposure-for-chromatic-number)
  - [Chromatic number of the half-density binomial random graph](#chromatic-number-of-the-half-density-binomial-random-graph)
  - [Clique count in a binomial random graph](#clique-count-in-a-binomial-random-graph)
    - [Fixed-size clique appearance threshold](#fixed-size-clique-appearance-threshold)
      - [Growing clique size can invalidate a first-moment appearance criterion](#growing-clique-size-can-invalidate-a-first-moment-appearance-criterion)
    - [Overlap formula for the variance of a clique count](#overlap-formula-for-the-variance-of-a-clique-count)
      - [Growing-clique overlap bound](#growing-clique-overlap-bound)
  - [Triangle count in a binomial random graph](#triangle-count-in-a-binomial-random-graph)
    - [Triangle variance in a binomial random graph](#triangle-variance-in-a-binomial-random-graph)
      - [Triangle-existence threshold in a binomial random graph](#triangle-existence-threshold-in-a-binomial-random-graph)
    - [Poisson limit for triangles in a binomial random graph](#poisson-limit-for-triangles-in-a-binomial-random-graph)
  - [Triangle with an attached leaf in a binomial random graph](#triangle-with-an-attached-leaf-in-a-binomial-random-graph)
- [Graph coloring](graph-coloring.md)
  - [Two-coloring](graph-coloring.md#two-coloring)
  - [Proper vertex coloring](graph-coloring.md#proper-vertex-coloring)
  - [Semi-random palette refinement for triangle-free colouring](graph-coloring.md#semi-random-palette-refinement-for-triangle-free-colouring)
  - [Colour savings from sparse neighbourhoods](graph-coloring.md#colour-savings-from-sparse-neighbourhoods)
  - [Coloring entropy weight](graph-coloring.md#coloring-entropy-weight)
    - [Entropy weight of a graph cover](graph-coloring.md#entropy-weight-of-a-graph-cover)
  - [Greedy coloring](graph-coloring.md#greedy-coloring)
    - [Extension of a partial colouring by neighbour-colour savings](graph-coloring.md#extension-of-a-partial-colouring-by-neighbour-colour-savings)
      - [Neighbour-colour saving](graph-coloring.md#neighbour-colour-saving)
  - [Three-colourability problem](graph-coloring.md#three-colourability-problem)
  - [Three-colour clause gadget](graph-coloring.md#three-colour-clause-gadget)
  - [Boolean-pair colouring gadget](graph-coloring.md#boolean-pair-colouring-gadget)
  - [Greedy colouring by removing independent sets](graph-coloring.md#greedy-colouring-by-removing-independent-sets)
  - [Lovász number](graph-coloring.md#lovasz-number)
    - [Orthonormal representation of a graph](graph-coloring.md#orthonormal-representation-of-a-graph)
      - [Tensor-product capacity bound from an orthonormal representation](graph-coloring.md#tensor-product-capacity-bound-from-an-orthonormal-representation)
    - [Complement theta number](graph-coloring.md#complement-theta-number)
  - [Vector coloring](graph-coloring.md#vector-coloring)
    - [Strict vector coloring](graph-coloring.md#strict-vector-coloring)
    - [Random hyperplane rounding](graph-coloring.md#random-hyperplane-rounding)
  - [Semicoloring](graph-coloring.md#semicoloring)
    - [Semicoloring by independent hyperplanes](graph-coloring.md#semicoloring-by-independent-hyperplanes)
  - [Edge coloring](graph-coloring.md#edge-coloring)
    - [Proper edge coloring](graph-coloring.md#proper-edge-coloring)
      - [Edge coloring as scheduling](graph-coloring.md#edge-coloring-as-scheduling)
    - [List edge coloring](graph-coloring.md#list-edge-coloring)
      - [List-chromatic index](graph-coloring.md#list-chromatic-index)
        - [Galvin theorem for bipartite list edge coloring](graph-coloring.md#galvin-theorem-for-bipartite-list-edge-coloring)
    - [Chromatic index](graph-coloring.md#chromatic-index)
      - [Chromatic index bounds](graph-coloring.md#chromatic-index-bounds)
    - [Tait coloring](graph-coloring.md#tait-coloring)
  - [Chromatic number](graph-coloring.md#chromatic-number)
    - [Chromatic number of Euclidean space](graph-coloring.md#chromatic-number-of-euclidean-space)
    - [Colour-critical vertex](graph-coloring.md#colour-critical-vertex)
    - [Mycielskian](graph-coloring.md#mycielskian)
      - [Grötzsch graph](graph-coloring.md#grotzsch-graph)
      - [Mycielski shadow vertex](graph-coloring.md#mycielski-shadow-vertex)
      - [Mycielski apex](graph-coloring.md#mycielski-apex)
      - [Mycielskian chromatic increase](graph-coloring.md#mycielskian-chromatic-increase)
      - [Mycielskian triangle preservation](graph-coloring.md#mycielskian-triangle-preservation)
      - [Triangle-free graphs with arbitrarily large chromatic number](graph-coloring.md#triangle-free-graphs-with-arbitrarily-large-chromatic-number)
    - [Graphs of arbitrarily high girth and chromatic number](graph-coloring.md#graphs-of-arbitrarily-high-girth-and-chromatic-number)
    - [Brooks' theorem](graph-coloring.md#brooks-theorem)
  - [Edge chromatic number](graph-coloring.md#edge-chromatic-number)
    - [Vizing's theorem](graph-coloring.md#vizing-s-theorem)
      - [Vizing fan lemma](graph-coloring.md#vizing-fan-lemma)
  - [Kempe chain](graph-coloring.md#kempe-chain)
  - [Chromatic polynomial](graph-coloring.md#chromatic-polynomial)
    - [Chromatic polynomial determines a Turán graph](graph-coloring.md#chromatic-polynomial-determines-a-turan-graph)
    - [Deletion-contraction recurrence for the chromatic polynomial](graph-coloring.md#deletion-contraction-recurrence-for-the-chromatic-polynomial)
    - [Chromatic polynomial after attaching a leaf](graph-coloring.md#chromatic-polynomial-after-attaching-a-leaf)
- [Graph](graph.md)
  - [Sparse graph](graph.md#sparse-graph)
  - [Graph adjacency](graph.md#graph-adjacency)
  - [Simple graph](graph.md#simple-graph)
  - [Loop (graph theory)](graph.md#loop-graph-theory)
  - [Torus graph](graph.md#torus-graph)
  - [Dual graph](graph.md#dual-graph)
  - [Cubic graph](graph.md#cubic-graph)
    - [Heawood graph](graph.md#heawood-graph)
      - [Heawood torus map](graph.md#heawood-torus-map)
  - [Strong product of graphs](graph.md#strong-product-of-graphs)
    - [Strong graph power](graph.md#strong-graph-power)
      - [Shannon capacity of a graph](graph.md#shannon-capacity-of-a-graph)
        - [Haemers rank bound](graph.md#haemers-rank-bound)
          - [Polynomial representation of a graph](graph.md#polynomial-representation-of-a-graph)
        - [Complement-pair capacity gain](graph.md#complement-pair-capacity-gain)
          - [Nonadditivity of Shannon capacity](graph.md#nonadditivity-of-shannon-capacity)
        - [Pentagon capacity code](graph.md#pentagon-capacity-code)
  - [Incidence matrix](graph.md#incidence-matrix)
  - [Amenable graph](graph.md#amenable-graph)
    - [Følner set](graph.md#folner-set)
  - [Multigraph](graph.md#multigraph)
    - [Bouquet graph](graph.md#bouquet-graph)
  - [Distance-transitive graph](graph.md#distance-transitive-graph)
    - [Distance-transitive action on a graph](graph.md#distance-transitive-action-on-a-graph)
    - [Symplectic dual polar graph](graph.md#symplectic-dual-polar-graph)
  - [Vertex-transitive graph](graph.md#vertex-transitive-graph)
  - [Triangular lattice](graph.md#triangular-lattice)
  - [False twin](graph.md#false-twin)
    - [False-twin class](graph.md#false-twin-class)
  - [Graph power](graph.md#graph-power)
    - [Square of a cycle](graph.md#square-of-a-cycle)
  - [Graph cut](graph.md#graph-cut)
    - [Balanced component cut](graph.md#balanced-component-cut)
  - [Oriented incidence matrix](graph.md#oriented-incidence-matrix)
    - [Incidence pseudoinverse decomposition](graph.md#incidence-pseudoinverse-decomposition)
  - [Cartesian product of graphs](graph.md#cartesian-product-of-graphs)
  - [Ladder graph](graph.md#ladder-graph)
    - [Doubly infinite ladder graph](graph.md#doubly-infinite-ladder-graph)
  - [Cubic lattice](graph.md#cubic-lattice)
    - [Amenable boundary growth of lattice boxes](graph.md#amenable-boundary-growth-of-lattice-boxes)
  - [Vertex set](graph.md#vertex-set)
  - [Graph blow-up](graph.md#graph-blow-up)
    - [Dense clique family blow-up lemma](graph.md#dense-clique-family-blow-up-lemma)
    - [Vertex cloning in a graph](graph.md#vertex-cloning-in-a-graph)
  - [Multipartite graph](graph.md#multipartite-graph)
  - [Reachability in a graph](graph.md#reachability-in-a-graph)
  - [Graph search](graph.md#graph-search)
    - [Best-first search](graph.md#best-first-search)
  - [Tripartite graph](graph.md#tripartite-graph)
    - [Tripartite graph encoding of a grid](graph.md#tripartite-graph-encoding-of-a-grid)
  - [Graph automorphism](graph.md#graph-automorphism)
    - [Quasi-transitive graph](graph.md#quasi-transitive-graph)
  - [Bridge (graph theory)](graph.md#bridge-graph-theory)
  - [Hypercube graph](graph.md#hypercube-graph)
    - [Gray code](graph.md#gray-code)
  - [Square lattice](graph.md#square-lattice)
  - [Connectivity (graph theory)](graph.md#connectivity-graph-theory)
    - [Connected graph](graph.md#connected-graph)
      - [Component (graph theory)](graph.md#component-graph-theory)
        - [Supermodularity of graph component count](graph.md#supermodularity-of-graph-component-count)
        - [Tree component](graph.md#tree-component)
        - [Largest component of a graph](graph.md#largest-component-of-a-graph)
  - [Vertex (graph theory)](graph.md#vertex-graph-theory)
  - [Graph isomorphism](graph.md#graph-isomorphism)
  - [Triangle in a graph](graph.md#triangle-in-a-graph)
    - [Edge-disjoint triangles](graph.md#edge-disjoint-triangles)
    - [Triangle count](graph.md#triangle-count)
    - [Triangle-free graph](graph.md#triangle-free-graph)
      - [Triangle-free chromatic lower bound at bounded maximum degree](graph.md#triangle-free-chromatic-lower-bound-at-bounded-maximum-degree)
    - [Edge-triangle incidence bound](graph.md#edge-triangle-incidence-bound)
  - [Vertex neighbourhood](graph.md#vertex-neighbourhood)
- [Independent set (graph theory)](#independent-set-graph-theory)
  - [Independence polynomial](#independence-polynomial)
  - [Maximal independent set](#maximal-independent-set)
  - [Independent transversal](#independent-transversal)
  - [Degree-ordered independent-set entropy bound](#degree-ordered-independent-set-entropy-bound)
  - [Independence number](#independence-number)
    - [Caro-Wei bound](#caro-wei-bound)
    - [Triangle-free graph with sub-power independence number](#triangle-free-graph-with-sub-power-independence-number)
  - [Greedy independent-set bound](#greedy-independent-set-bound)
  - [Locally sparse graph independence bound](#locally-sparse-graph-independence-bound)
    - [Shearer independence bound for a triangle-free graph](#shearer-independence-bound-for-a-triangle-free-graph)
- [Leaf of a graph](#leaf-of-a-graph)
- [Edge of a graph](#edge-of-a-graph)
- [Path in a graph](#path-in-a-graph)
  - [Hamiltonian path](#hamiltonian-path)
  - [Edge-disjoint paths](#edge-disjoint-paths)
  - [Ray in a graph](#ray-in-a-graph)
  - [Path graph](#path-graph)
  - [Cycle in a graph](#cycle-in-a-graph)
    - [Induced cycle](#induced-cycle)
    - [Girth](#girth)
    - [Odd cycle](#odd-cycle)
    - [Cycle graph](#cycle-graph)
      - [Wheel graph](#wheel-graph)
      - [Hamilton cycle](#hamilton-cycle)
        - [Hamiltonian graph](#hamiltonian-graph)
        - [Necessary conditions for a Hamilton cycle](#necessary-conditions-for-a-hamilton-cycle)
        - [Weighted Hamilton cycle](#weighted-hamilton-cycle)
        - [Icosian game](#icosian-game)
      - [Pancyclic graph](#pancyclic-graph)
  - [Long path from minimum degree](#long-path-from-minimum-degree)
  - [Erdős-Gallai path edge bound](#erdos-gallai-path-edge-bound)
- [Subgraph](#subgraph)
  - [Spanning subgraph](#spanning-subgraph)
  - [Induced subgraph](#induced-subgraph)
  - [Three-colourable two-thirds subgraph lemma](#three-colourable-two-thirds-subgraph-lemma)
- [Join (graph theory)](#join-graph-theory)
- [Disjoint union of graphs](#disjoint-union-of-graphs)
- [Intersection graph](#intersection-graph)
- [Complete graph](#complete-graph)
  - [Edge count of a complete graph](#edge-count-of-a-complete-graph)
  - [Clique (graph theory)](#clique-graph-theory)
    - [Maximum clique](#maximum-clique)
    - [Maximal clique](#maximal-clique)
    - [Edge-disjoint clique packing](#edge-disjoint-clique-packing)
      - [Clique-packing amplification of moment bounds](#clique-packing-amplification-of-moment-bounds)
      - [Clique conflict graph](#clique-conflict-graph)
    - [Clique number](#clique-number)
    - [Pairwise intersections need not give a common intersection](#pairwise-intersections-need-not-give-a-common-intersection)
  - [Adjacency-matrix quadratic relation for a complete graph](#adjacency-matrix-quadratic-relation-for-a-complete-graph)
- [Complete multipartite graph](#complete-multipartite-graph)
  - [Octahedral graph](#octahedral-graph)
  - [Balancing a multipartite edge-triangle objective](#balancing-a-multipartite-edge-triangle-objective)
  - [Balanced complete multipartite blow-up](#balanced-complete-multipartite-blow-up)
- [Laplacian matrix](#laplacian-matrix)
  - [Graph Laplacian eigenvalue](#graph-laplacian-eigenvalue)
  - [Weighted graph Laplacian](#weighted-graph-laplacian)
  - [Degree matrix](#degree-matrix)
  - [Graph Laplacian quadratic form](#graph-laplacian-quadratic-form)
  - [Kernel of a graph Laplacian](#kernel-of-a-graph-laplacian)
  - [Diffusion on a graph](#diffusion-on-a-graph)
  - [Laplacian spectrum of a complete graph](#laplacian-spectrum-of-a-complete-graph)
- [Minimum-cost flow problem](#minimum-cost-flow-problem)
  - [Minimum-cost maximum flow](#minimum-cost-maximum-flow)
  - [Two-resource path packing as minimum-cost circulation](#two-resource-path-packing-as-minimum-cost-circulation)
  - [Feasible flow](#feasible-flow)
  - [Capacitated flow optimality conditions](#capacitated-flow-optimality-conditions)
  - [Flow balance](#flow-balance)
  - [Uncapacitated minimum-cost flow](#uncapacitated-minimum-cost-flow)
    - [Network dual potential](#network-dual-potential)
      - [Dual network potentials from shortest-path distances](#dual-network-potentials-from-shortest-path-distances)
      - [Network reduced cost](#network-reduced-cost)
  - [Network simplex algorithm](#network-simplex-algorithm)
    - [Network simplex tree basis](#network-simplex-tree-basis)
- [Extremal graph theory](extremal-graph-theory.md)
  - [Supersaturation](extremal-graph-theory.md#supersaturation)
    - [Clique supersaturation by sampling](extremal-graph-theory.md#clique-supersaturation-by-sampling)
  - [Extremal number](extremal-graph-theory.md#extremal-number)
    - [Extremal graph for disjoint cliques](extremal-graph-theory.md#extremal-graph-for-disjoint-cliques)
    - [Monotonicity of the normalized extremal number](extremal-graph-theory.md#monotonicity-of-the-normalized-extremal-number)
    - [Mantel theorem](extremal-graph-theory.md#mantel-theorem)
      - [Triangle lower bound one edge above the Mantel threshold](extremal-graph-theory.md#triangle-lower-bound-one-edge-above-the-mantel-threshold)
  - [Turán's theorem](extremal-graph-theory.md#turan-s-theorem)
    - [Edit-distance stability for clique-free graphs](extremal-graph-theory.md#edit-distance-stability-for-clique-free-graphs)
      - [Bipartite stability from few odd cycles](extremal-graph-theory.md#bipartite-stability-from-few-odd-cycles)
    - [Turán graph](extremal-graph-theory.md#turan-graph)
      - [Triangle support line between bipartite and tripartite Turan graphs](extremal-graph-theory.md#triangle-support-line-between-bipartite-and-tripartite-turan-graphs)
    - [Zykov symmetrization](extremal-graph-theory.md#zykov-symmetrization)
      - [Edge-triangle symmetrization](extremal-graph-theory.md#edge-triangle-symmetrization)
    - [Quadratic Turan edge bound](extremal-graph-theory.md#quadratic-turan-edge-bound)
    - [Rhombus-free edge bound](extremal-graph-theory.md#rhombus-free-edge-bound)
      - [Triangular prism graph](extremal-graph-theory.md#triangular-prism-graph)
  - [Erdős-Stone theorem](extremal-graph-theory.md#erdos-stone-theorem)
    - [Logarithmic Erdős-Stone theorem](extremal-graph-theory.md#logarithmic-erdos-stone-theorem)
      - [Logarithmic clique blow-up from minimum degree](extremal-graph-theory.md#logarithmic-clique-blow-up-from-minimum-degree)
      - [Random obstruction to larger clique blow-ups](extremal-graph-theory.md#random-obstruction-to-larger-clique-blow-ups)
    - [High-minimum-degree multipartite stability subgraph](extremal-graph-theory.md#high-minimum-degree-multipartite-stability-subgraph)
      - [Minimum degree of an extremal forbidden-subgraph graph](extremal-graph-theory.md#minimum-degree-of-an-extremal-forbidden-subgraph-graph)
  - [Kővári–Sós–Turán theorem](extremal-graph-theory.md#kovari-sos-turan-theorem)
- [Flow network](flow-network.md)
  - [Circulation in a flow network](flow-network.md#circulation-in-a-flow-network)
  - [Vertex capacity](flow-network.md#vertex-capacity)
  - [Maximum flow problem](flow-network.md#maximum-flow-problem)
    - [Dinic's algorithm](flow-network.md#dinic-s-algorithm)
    - [Sports elimination by maximum flow](flow-network.md#sports-elimination-by-maximum-flow)
    - [Treatment capacity as a sink arc](flow-network.md#treatment-capacity-as-a-sink-arc)
    - [Server connectivity under component failures](flow-network.md#server-connectivity-under-component-failures)
    - [Edmonds–Karp algorithm](flow-network.md#edmonds-karp-algorithm)
    - [Maximum flow with vertex capacities](flow-network.md#maximum-flow-with-vertex-capacities)
      - [Vertex splitting](flow-network.md#vertex-splitting)
  - [Flow network edge capacity](flow-network.md#flow-network-edge-capacity)
  - [Capacity constraint](flow-network.md#capacity-constraint)
  - [Cut of a flow network](flow-network.md#cut-of-a-flow-network)
    - [Minimum cut](flow-network.md#minimum-cut)
      - [Diagonal cut in a nearest-neighbour lattice flow](flow-network.md#diagonal-cut-in-a-nearest-neighbour-lattice-flow)
    - [Cut capacity](flow-network.md#cut-capacity)
  - [Flow](flow-network.md#flow)
    - [Unit flow](flow-network.md#unit-flow)
    - [Divergence of a flow](flow-network.md#divergence-of-a-flow)
      - [Flow conservation](flow-network.md#flow-conservation)
    - [Strength of a flow](flow-network.md#strength-of-a-flow)
    - [Energy of a flow](flow-network.md#energy-of-a-flow)
      - [Finite-energy flow criterion for transience](flow-network.md#finite-energy-flow-criterion-for-transience)
  - [Max-flow min-cut theorem](flow-network.md#max-flow-min-cut-theorem)
    - [Residual reachability certificate for maximum flow](flow-network.md#residual-reachability-certificate-for-maximum-flow)
    - [Uniform capacity perturbation of a flow network](flow-network.md#uniform-capacity-perturbation-of-a-flow-network)
    - [Integral max-flow theorem](flow-network.md#integral-max-flow-theorem)
    - [Kőnig's theorem (graph theory)](flow-network.md#konig-s-theorem-graph-theory)
    - [Residual network](flow-network.md#residual-network)
      - [Residual maximum flow is the remaining optimality gap](flow-network.md#residual-maximum-flow-is-the-remaining-optimality-gap)
      - [Augmenting path](flow-network.md#augmenting-path)
        - [Widest augmenting path](flow-network.md#widest-augmenting-path)
          - [Geometric convergence of widest-path augmentation](flow-network.md#geometric-convergence-of-widest-path-augmentation)
        - [Ford-Fulkerson algorithm](flow-network.md#ford-fulkerson-algorithm)
          - [Integrality of the Ford-Fulkerson algorithm](flow-network.md#integrality-of-the-ford-fulkerson-algorithm)
    - [Parametric maximum flow with one source capacity](flow-network.md#parametric-maximum-flow-with-one-source-capacity)
- [Eulerian graph](#eulerian-graph)
  - [Edge support of a graph](#edge-support-of-a-graph)
  - [Seven Bridges of Königsberg](#seven-bridges-of-konigsberg)
  - [Eulerian trail](#eulerian-trail)
    - [Eulerian cycle](#eulerian-cycle)
  - [Euler circuit](#euler-circuit)
  - [Euler circuit criterion](#euler-circuit-criterion)
    - [Hierholzer's algorithm](#hierholzer-s-algorithm)
- [Line graph](#line-graph)
  - [Line graph of a regular graph is Eulerian](#line-graph-of-a-regular-graph-is-eulerian)
- [Graph drawing](#graph-drawing)
- [Planar graph](planar-graph.md)
  - [Kuratowski's theorem](planar-graph.md#kuratowski-s-theorem)
  - [Plane graph](planar-graph.md#plane-graph)
    - [Face of a plane graph](planar-graph.md#face-of-a-plane-graph)
      - [Outer face](planar-graph.md#outer-face)
      - [Facial boundary walk](planar-graph.md#facial-boundary-walk)
  - [Honeycomb lattice](planar-graph.md#honeycomb-lattice)
    - [Martini lattice](planar-graph.md#martini-lattice)
  - [Four color theorem](planar-graph.md#four-color-theorem)
  - [Five color theorem](planar-graph.md#five-color-theorem)
  - [Planar map](planar-graph.md#planar-map)
    - [Face of a planar map](planar-graph.md#face-of-a-planar-map)
    - [Rooted planar map](planar-graph.md#rooted-planar-map)
    - [Planar quadrangulation](planar-graph.md#planar-quadrangulation)
      - [Trivial bijection between planar maps and quadrangulations](planar-graph.md#trivial-bijection-between-planar-maps-and-quadrangulations)
  - [Planar dual graph](planar-graph.md#planar-dual-graph)
    - [Planar cluster-count identity](planar-graph.md#planar-cluster-count-identity)
    - [Dual bond percolation](planar-graph.md#dual-bond-percolation)
      - [Three-terminal cell partition duality](planar-graph.md#three-terminal-cell-partition-duality)
      - [Dual contour bound for a finite planar cluster](planar-graph.md#dual-contour-bound-for-a-finite-planar-cluster)
    - [Planar duality for rectangle crossings](planar-graph.md#planar-duality-for-rectangle-crossings)
      - [Exact self-dual rectangle crossing probability](planar-graph.md#exact-self-dual-rectangle-crossing-probability)
  - [Euler formula for a connected planar graph](planar-graph.md#euler-formula-for-a-connected-planar-graph)
    - [Small faces of a spherical polyhedral graph](planar-graph.md#small-faces-of-a-spherical-polyhedral-graph)
    - [Planar graph edge bound](planar-graph.md#planar-graph-edge-bound)
      - [Bipartite planar graph edge bound](planar-graph.md#bipartite-planar-graph-edge-bound)
      - [Nonplanarity by edge counts](planar-graph.md#nonplanarity-by-edge-counts)
    - [Planar girth edge bound](planar-graph.md#planar-girth-edge-bound)
    - [Triangle-pentagon planar edge bound](planar-graph.md#triangle-pentagon-planar-edge-bound)
      - [Icosidodecahedral graph](planar-graph.md#icosidodecahedral-graph)
- [Crossing number](#crossing-number)
  - [Crossing lemma](#crossing-lemma)
    - [Crossing lemma for multigraphs](#crossing-lemma-for-multigraphs)
- [Graph neighbourhood](#graph-neighbourhood)
  - [Neighbour of a vertex](#neighbour-of-a-vertex)
  - [Closed graph neighbourhood](#closed-graph-neighbourhood)
  - [External vertex boundary](#external-vertex-boundary)
  - [Common neighbour](#common-neighbour)
- [Degree (graph theory)](#degree-graph-theory)
  - [In-degree](#in-degree)
  - [Degree sequence](#degree-sequence)
  - [Outdegree](#outdegree)
  - [Average degree of a graph](#average-degree-of-a-graph)
  - [Regular graph](#regular-graph)
    - [Nested matching criterion for a regular subgraph](#nested-matching-criterion-for-a-regular-subgraph)
    - [Short-cycle expectation in a uniform regular graph](#short-cycle-expectation-in-a-uniform-regular-graph)
    - [Petersen graph](#petersen-graph)
    - [Constant eigenvector of a regular graph](#constant-eigenvector-of-a-regular-graph)
    - [Connected regular graph with two adjacency eigenvalues](#connected-regular-graph-with-two-adjacency-eigenvalues)
  - [Degree-biased vertex distribution](#degree-biased-vertex-distribution)
  - [Universal vertex](#universal-vertex)
  - [Minimum degree of a graph](#minimum-degree-of-a-graph)
  - [Maximum degree of a graph](#maximum-degree-of-a-graph)
  - [Locally finite graph](#locally-finite-graph)
    - [Graph exhaustion](#graph-exhaustion)
- [Cut (graph theory)](#cut-graph-theory)
  - [Edge cutset](#edge-cutset)
  - [Maximum cut](#maximum-cut)
  - [Random cut lower bound](#random-cut-lower-bound)
    - [Balanced random cut lower bound](#balanced-random-cut-lower-bound)
  - [Unfriendly partition](#unfriendly-partition)
    - [Unfriendly partition theorem for a finite graph](#unfriendly-partition-theorem-for-a-finite-graph)
    - [Unfriendly partition theorem for a countable locally finite graph](#unfriendly-partition-theorem-for-a-countable-locally-finite-graph)
    - [Random unfriendly partition of a countable infinite-degree graph](#random-unfriendly-partition-of-a-countable-infinite-degree-graph)
- [Bipartite graph](bipartite-graph.md)
  - [Bipartite lattice](bipartite-graph.md#bipartite-lattice)
  - [Crown graph](bipartite-graph.md#crown-graph)
  - [Biadjacency matrix](bipartite-graph.md#biadjacency-matrix)
  - [Normalized adjacency operator of a bipartite graph](bipartite-graph.md#normalized-adjacency-operator-of-a-bipartite-graph)
  - [Biregular graph](bipartite-graph.md#biregular-graph)
    - [Independent-set bound for biregular graphs](bipartite-graph.md#independent-set-bound-for-biregular-graphs)
    - [Quasirandom bipartite graph](bipartite-graph.md#quasirandom-bipartite-graph)
      - [Spectral discrepancy bound for a biregular graph](bipartite-graph.md#spectral-discrepancy-bound-for-a-biregular-graph)
      - [Centered four-cycle identity for a biregular graph](bipartite-graph.md#centered-four-cycle-identity-for-a-biregular-graph)
  - [Half graph](bipartite-graph.md#half-graph)
    - [Boundary rank obstruction in a half graph](bipartite-graph.md#boundary-rank-obstruction-in-a-half-graph)
  - [Odd-cycle characterization of bipartite graphs](bipartite-graph.md#odd-cycle-characterization-of-bipartite-graphs)
  - [Complete bipartite graph](bipartite-graph.md#complete-bipartite-graph)
    - [Common neighbourhood from bipartite density](bipartite-graph.md#common-neighbourhood-from-bipartite-density)
    - [Star (graph theory)](bipartite-graph.md#star-graph-theory)
  - [Two-colourability criterion for bipartite graphs](bipartite-graph.md#two-colourability-criterion-for-bipartite-graphs)
- [Graph homomorphism](#graph-homomorphism)
  - [Graph embedding](#graph-embedding)
  - [Homomorphism density](#homomorphism-density)
    - [Sidorenko conjecture](#sidorenko-conjecture)
      - [Sidorenko inequality for trees](#sidorenko-inequality-for-trees)
- [Directed graph](#directed-graph)
  - [Strongly connected component](#strongly-connected-component)
  - [Functional graph](#functional-graph)
  - [Kernel-perfect directed graph](#kernel-perfect-directed-graph)
    - [Kernel list-coloring lemma](#kernel-list-coloring-lemma)
  - [Kernel of a directed graph](#kernel-of-a-directed-graph)
  - [Plünnecke graph](#plunnecke-graph)
    - [Weighted cut lemma for commutative graphs](#weighted-cut-lemma-for-commutative-graphs)
    - [Graph magnification ratio](#graph-magnification-ratio)
  - [Coherent cyclic order of a digraph](#coherent-cyclic-order-of-a-digraph)
    - [Cyclic stability of a digraph order](#cyclic-stability-of-a-digraph-order)
  - [Tournament (graph theory)](#tournament-graph-theory)
    - [Transitive tournament](#transitive-tournament)
    - [Landau's theorem on tournament scores](#landau-s-theorem-on-tournament-scores)
    - [Median order of a tournament](#median-order-of-a-tournament)
      - [Half-sparse median-order embedding](#half-sparse-median-order-embedding)
    - [Regular tournament](#regular-tournament)
  - [Directed cycle](#directed-cycle)
    - [Spanning circuit family](#spanning-circuit-family)
      - [Circuit-cover bound by independence number](#circuit-cover-bound-by-independence-number)
  - [Rooted directed graph](#rooted-directed-graph)
    - [Bisimulation](#bisimulation)
      - [Bisimulation game](#bisimulation-game)
      - [Bisimilarity](#bisimilarity)
  - [Skeleton of a directed graph](#skeleton-of-a-directed-graph)
  - [Cycle cover of a directed graph](#cycle-cover-of-a-directed-graph)
  - [Directed edge](#directed-edge)
  - [Directed walk](#directed-walk)
    - [Closed directed walk](#closed-directed-walk)
  - [Directed path](#directed-path)
  - [Strong connectivity](#strong-connectivity)
  - [Adjacency matrix of a directed graph](#adjacency-matrix-of-a-directed-graph)
- [Adjacency matrix](#adjacency-matrix)
  - [Walk count from powers of an adjacency matrix](#walk-count-from-powers-of-an-adjacency-matrix)
- [Distance (graph theory)](#distance-graph-theory)
  - [Average shortest path length](#average-shortest-path-length)
  - [Path metric](#path-metric)
  - [Graph diameter](#graph-diameter)
    - [Linear independence of adjacency powers up to the diameter](#linear-independence-of-adjacency-powers-up-to-the-diameter)
- [Spectral graph theory](#spectral-graph-theory)
  - [Expander mixing lemma](#expander-mixing-lemma)
  - [Graph eigenvalue](#graph-eigenvalue)
- [Bipartite adjacency matrix](#bipartite-adjacency-matrix)
  - [Perfect matching from a nonzero determinant](#perfect-matching-from-a-nonzero-determinant)
- [Matching (graph theory)](matching-graph-theory.md)
  - [Unmatched vertex in a matching](matching-graph-theory.md#unmatched-vertex-in-a-matching)
  - [Matching saturation](matching-graph-theory.md#matching-saturation)
  - [Stable matching in a bipartite graph](matching-graph-theory.md#stable-matching-in-a-bipartite-graph)
    - [Mutual-worst edge in stable matchings](matching-graph-theory.md#mutual-worst-edge-in-stable-matchings)
    - [Gale-Shapley algorithm](matching-graph-theory.md#gale-shapley-algorithm)
      - [Proposer-optimal stable matching](matching-graph-theory.md#proposer-optimal-stable-matching)
        - [Receiver-pessimal stable matching](matching-graph-theory.md#receiver-pessimal-stable-matching)
    - [Blocking pair in stable matching](matching-graph-theory.md#blocking-pair-in-stable-matching)
  - [Near-perfect matching](matching-graph-theory.md#near-perfect-matching)
  - [Matching generating function](matching-graph-theory.md#matching-generating-function)
    - [Annealing ratios for a matching generating function](matching-graph-theory.md#annealing-ratios-for-a-matching-generating-function)
  - [Alternating path in a matching](matching-graph-theory.md#alternating-path-in-a-matching)
  - [Augmenting path in a matching](matching-graph-theory.md#augmenting-path-in-a-matching)
    - [Berge's theorem](matching-graph-theory.md#berge-s-theorem)
    - [Short augmenting paths in a dense bipartite graph](matching-graph-theory.md#short-augmenting-paths-in-a-dense-bipartite-graph)
  - [Perfect matching](matching-graph-theory.md#perfect-matching)
    - [Flexible vertex in a balanced bipartite graph](matching-graph-theory.md#flexible-vertex-in-a-balanced-bipartite-graph)
    - [Minimum-weight perfect matching](matching-graph-theory.md#minimum-weight-perfect-matching)
    - [One-factorization](matching-graph-theory.md#one-factorization)
  - [Maximal matching](matching-graph-theory.md#maximal-matching)
    - [Greedy matching](matching-graph-theory.md#greedy-matching)
  - [Matching number](matching-graph-theory.md#matching-number)
  - [Maximum cardinality matching](matching-graph-theory.md#maximum-cardinality-matching)
  - [Maximum-weight matching](matching-graph-theory.md#maximum-weight-matching)
  - [Hall's marriage theorem](matching-graph-theory.md#hall-s-marriage-theorem)
    - [Hall condition](matching-graph-theory.md#hall-condition)
      - [Hall obstruction](matching-graph-theory.md#hall-obstruction)
    - [Hall allocation model](matching-graph-theory.md#hall-allocation-model)
    - [System of distinct representatives](matching-graph-theory.md#system-of-distinct-representatives)
    - [Hall theorem proof outline](matching-graph-theory.md#hall-theorem-proof-outline)
    - [Random bipartite matching from empty-rectangle exclusion](matching-graph-theory.md#random-bipartite-matching-from-empty-rectangle-exclusion)
    - [Hall matching of maximal separated sets](matching-graph-theory.md#hall-matching-of-maximal-separated-sets)
    - [Degree-weighted Hall condition](matching-graph-theory.md#degree-weighted-hall-condition)
    - [Measurable Hall theorem](matching-graph-theory.md#measurable-hall-theorem)
    - [Hall induction through a tight set](matching-graph-theory.md#hall-induction-through-a-tight-set)
    - [Regular bipartite graph has a perfect matching](matching-graph-theory.md#regular-bipartite-graph-has-a-perfect-matching)
  - [Regular-graph matching bound from unmatched vertices](matching-graph-theory.md#regular-graph-matching-bound-from-unmatched-vertices)
    - [Disjoint union of triangles as a sharp matching example](matching-graph-theory.md#disjoint-union-of-triangles-as-a-sharp-matching-example)
- [Ramsey theorem](#ramsey-theorem)
  - [Diagonal Ramsey number](#diagonal-ramsey-number)
    - [Binomial upper bound for a Ramsey number](#binomial-upper-bound-for-a-ramsey-number)
    - [Monochromatic-triangle counting formula](#monochromatic-triangle-counting-formula)
  - [Graph Ramsey number](#graph-ramsey-number)
    - [Triangle-free Ramsey lower bound by alteration](#triangle-free-ramsey-lower-bound-by-alteration)
    - [Off-diagonal graph Ramsey number](#off-diagonal-graph-ramsey-number)
      - [Clique-path Ramsey number](#clique-path-ramsey-number)
    - [Ramsey number of a star](#ramsey-number-of-a-star)
    - [Paw graph](#paw-graph)
      - [Ramsey number of the paw graph](#ramsey-number-of-the-paw-graph)
  - [Uniform hypergraph Ramsey number](#uniform-hypergraph-ramsey-number)
    - [Erdős-Hajnal bound for the three-edge hypergraph on four vertices](#erdos-hajnal-bound-for-the-three-edge-hypergraph-on-four-vertices)
  - [Canonical Ramsey theorem](#canonical-ramsey-theorem)
  - [Partition regular equation](#partition-regular-equation)
- [Dirac's theorem](#dirac-s-theorem)
- [Longest-path rotation](#longest-path-rotation)
  - [Neighbourhood bound for a square-free bipartite graph](#neighbourhood-bound-for-a-square-free-bipartite-graph)
- [Strongly regular graph](#strongly-regular-graph)
  - [Triangle-free graphs with three common neighbours](#triangle-free-graphs-with-three-common-neighbours)
  - [Adjacency-matrix relation for a strongly regular graph](#adjacency-matrix-relation-for-a-strongly-regular-graph)
  - [Three-eigenvalue characterization of a connected strongly regular graph](#three-eigenvalue-characterization-of-a-connected-strongly-regular-graph)
- [Moser spindle](#moser-spindle)
- [Probabilistic combinatorics](probabilistic-combinatorics.md)
  - [Semi-random method](probabilistic-combinatorics.md#semi-random-method)
    - [Rödl nibble](probabilistic-combinatorics.md#rodl-nibble)
  - [Probabilistic method](probabilistic-combinatorics.md#probabilistic-method)
    - [Triangle deletion in the alteration method](probabilistic-combinatorics.md#triangle-deletion-in-the-alteration-method)
    - [Dense integer sets with only logarithmic-length progressions](probabilistic-combinatorics.md#dense-integer-sets-with-only-logarithmic-length-progressions)
  - [With high probability](probabilistic-combinatorics.md#with-high-probability)
  - [Subcritical component bound for a binomial random graph](probabilistic-combinatorics.md#subcritical-component-bound-for-a-binomial-random-graph)
    - [Sharp subcritical largest-component scale](probabilistic-combinatorics.md#sharp-subcritical-largest-component-scale)
    - [Unicyclic component](probabilistic-combinatorics.md#unicyclic-component)
      - [Labelled unicyclic graph count](probabilistic-combinatorics.md#labelled-unicyclic-graph-count)
  - [Hamiltonicity-to-pancyclicity sprinkling principle](probabilistic-combinatorics.md#hamiltonicity-to-pancyclicity-sprinkling-principle)
  - [Random alteration method](probabilistic-combinatorics.md#random-alteration-method)
  - [Lovász local lemma](probabilistic-combinatorics.md#lovasz-local-lemma)
    - [Local lemma Ramsey lower bound](probabilistic-combinatorics.md#local-lemma-ramsey-lower-bound)
    - [Dependency-degree obstruction on a rooted tree](probabilistic-combinatorics.md#dependency-degree-obstruction-on-a-rooted-tree)
    - [Compactness extension of the Lovász local lemma](probabilistic-combinatorics.md#compactness-extension-of-the-lovasz-local-lemma)
    - [Asymmetric Lovász local lemma](probabilistic-combinatorics.md#asymmetric-lovasz-local-lemma)
    - [Dependency graph of events](probabilistic-combinatorics.md#dependency-graph-of-events)
      - [Independence digraph of events](probabilistic-combinatorics.md#independence-digraph-of-events)
    - [Lopsided Lovász local lemma](probabilistic-combinatorics.md#lopsided-lovasz-local-lemma)
      - [Correlation graph of events](probabilistic-combinatorics.md#correlation-graph-of-events)
  - [Dependent random choice](probabilistic-combinatorics.md#dependent-random-choice)
    - [Dense bipartite common-neighbour lemma](probabilistic-combinatorics.md#dense-bipartite-common-neighbour-lemma)
    - [Bounded-degree bipartite Ramsey bound](probabilistic-combinatorics.md#bounded-degree-bipartite-ramsey-bound)
    - [Common-neighbourhood sampling bound](probabilistic-combinatorics.md#common-neighbourhood-sampling-bound)
    - [Complete-bipartite Ramsey completion lemma](probabilistic-combinatorics.md#complete-bipartite-ramsey-completion-lemma)
    - [Rich set in a graph](probabilistic-combinatorics.md#rich-set-in-a-graph)
      - [Rich-set embedding lemma](probabilistic-combinatorics.md#rich-set-embedding-lemma)
  - [Edge density of a bipartite graph](probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph)
    - [Bipartite four-cycle count](probabilistic-combinatorics.md#bipartite-four-cycle-count)
      - [Bipartite four-cycle density](probabilistic-combinatorics.md#bipartite-four-cycle-density)
    - [Regular pair of vertex sets](probabilistic-combinatorics.md#regular-pair-of-vertex-sets)
      - [Dense regular pair from edge surplus](probabilistic-combinatorics.md#dense-regular-pair-from-edge-surplus)
      - [Irregular pair of vertex sets](probabilistic-combinatorics.md#irregular-pair-of-vertex-sets)
      - [Regular clique counting lemma](probabilistic-combinatorics.md#regular-clique-counting-lemma)
        - [Regular triangle counting lemma](probabilistic-combinatorics.md#regular-triangle-counting-lemma)
      - [Regular pair of bipartite partitions](probabilistic-combinatorics.md#regular-pair-of-bipartite-partitions)
        - [Bipartite Szemerédi regularity lemma](probabilistic-combinatorics.md#bipartite-szemeredi-regularity-lemma)
      - [Szemerédi regularity lemma](probabilistic-combinatorics.md#szemeredi-regularity-lemma)
        - [Weighted Szemerédi regularity lemma](probabilistic-combinatorics.md#weighted-szemeredi-regularity-lemma)
          - [Small-cell deletion in weighted regularity](probabilistic-combinatorics.md#small-cell-deletion-in-weighted-regularity)
        - [Energy-increment proof of Szemerédi regularity](probabilistic-combinatorics.md#energy-increment-proof-of-szemeredi-regularity)
        - [Induced regularity template lemma](probabilistic-combinatorics.md#induced-regularity-template-lemma)
        - [Clique removal lemma](probabilistic-combinatorics.md#clique-removal-lemma)
          - [Triangle removal lemma](probabilistic-combinatorics.md#triangle-removal-lemma)
        - [Equitable regularity energy](probabilistic-combinatorics.md#equitable-regularity-energy)
          - [Equalization with a controlled exceptional set](probabilistic-combinatorics.md#equalization-with-a-controlled-exceptional-set)
          - [Refinement variance identity for regularity energy](probabilistic-combinatorics.md#refinement-variance-identity-for-regularity-energy)
      - [Graph embedding lemma for regular pairs](probabilistic-combinatorics.md#graph-embedding-lemma-for-regular-pairs)
        - [Odd-cycle copies from positive triangle density](probabilistic-combinatorics.md#odd-cycle-copies-from-positive-triangle-density)
        - [Triangle embedding lemma for regular pairs](probabilistic-combinatorics.md#triangle-embedding-lemma-for-regular-pairs)
      - [Reduced graph of a regularity partition](probabilistic-combinatorics.md#reduced-graph-of-a-regularity-partition)
  - [Szemerédi's theorem](probabilistic-combinatorics.md#szemeredi-s-theorem)
    - [Dense three-term progressions force four-term progressions](probabilistic-combinatorics.md#dense-three-term-progressions-force-four-term-progressions)
  - [Locally dense graph thinning lemma](probabilistic-combinatorics.md#locally-dense-graph-thinning-lemma)
  - [Minimum-degree Ramsey lower bound](probabilistic-combinatorics.md#minimum-degree-ramsey-lower-bound)
- [Random graph](random-graph.md)
  - [Watts-Strogatz model](random-graph.md#watts-strogatz-model)
  - [Configuration model](random-graph.md#configuration-model)
    - [Bounded-degree pairing avoidance estimate](random-graph.md#bounded-degree-pairing-avoidance-estimate)
    - [Half-edge of a graph](random-graph.md#half-edge-of-a-graph)
  - [Preferential attachment](random-graph.md#preferential-attachment)
    - [Barabási-Albert model](random-graph.md#barabasi-albert-model)
    - [Linearized chord diagram model](random-graph.md#linearized-chord-diagram-model)
      - [First-vertex degree in the LCD model](random-graph.md#first-vertex-degree-in-the-lcd-model)
      - [Uniform linearized chord diagram](random-graph.md#uniform-linearized-chord-diagram)
  - [Random k-out graph](random-graph.md#random-k-out-graph)
    - [Connectivity of random k-out graphs](random-graph.md#connectivity-of-random-k-out-graphs)
  - [Rado graph](random-graph.md#rado-graph)
  - [Achlioptas process](random-graph.md#achlioptas-process)
    - [Continuity of fixed-choice percolation](random-graph.md#continuity-of-fixed-choice-percolation)
    - [Persistence of unsampled graph components](random-graph.md#persistence-of-unsampled-graph-components)
    - [Forced merging of large components](random-graph.md#forced-merging-of-large-components)
    - [Component-band vertex count](random-graph.md#component-band-vertex-count)
  - [Simultaneous giant for fixed random-edge choice](random-graph.md#simultaneous-giant-for-fixed-random-edge-choice)
  - [Giant component](random-graph.md#giant-component)
    - [Barely-supercritical largest-component expectation](random-graph.md#barely-supercritical-largest-component-expectation)
    - [Logarithmic-regime giant component](random-graph.md#logarithmic-regime-giant-component)
  - [Isolated vertex](random-graph.md#isolated-vertex)
  - [Erdős-Rényi model](random-graph.md#erdos-renyi-model)
    - [Breadth-first exploration of a binomial random graph](random-graph.md#breadth-first-exploration-of-a-binomial-random-graph)
    - [Uniform random graph process](random-graph.md#uniform-random-graph-process)
      - [Connectivity hitting time equals disappearance of isolated vertices](random-graph.md#connectivity-hitting-time-equals-disappearance-of-isolated-vertices)
      - [Marked-set connectivity threshold](random-graph.md#marked-set-connectivity-threshold)
    - [Tree-component expectation in the Erdős-Rényi model](random-graph.md#tree-component-expectation-in-the-erdos-renyi-model)
      - [Fixed-order tree-component window](random-graph.md#fixed-order-tree-component-window)
    - [Monotone graph property](random-graph.md#monotone-graph-property)
      - [Threshold function for a monotone graph property](random-graph.md#threshold-function-for-a-monotone-graph-property)
      - [Monotone coupling of binomial random graphs](random-graph.md#monotone-coupling-of-binomial-random-graphs)
    - [Sprinkling of a binomial random graph](random-graph.md#sprinkling-of-a-binomial-random-graph)
    - [Isolated vertices in the Erdős-Rényi model](random-graph.md#isolated-vertices-in-the-erdos-renyi-model)
      - [Isolated-vertex threshold in the Erdős-Rényi model](random-graph.md#isolated-vertex-threshold-in-the-erdos-renyi-model)
    - [Connectivity threshold in the Erdős-Rényi model](random-graph.md#connectivity-threshold-in-the-erdos-renyi-model)
      - [Connectivity of a fixed-density binomial random graph](random-graph.md#connectivity-of-a-fixed-density-binomial-random-graph)
      - [Critical-window connectivity probability of a binomial random graph](random-graph.md#critical-window-connectivity-probability-of-a-binomial-random-graph)
    - [Expected subgraph count in the Erdős-Rényi model](random-graph.md#expected-subgraph-count-in-the-erdos-renyi-model)
      - [Sparse clique-count concentration](random-graph.md#sparse-clique-count-concentration)
        - [Pendant extensions of sparse clique copies](random-graph.md#pendant-extensions-of-sparse-clique-copies)
      - [Vertex-disjoint sparse clique copies](random-graph.md#vertex-disjoint-sparse-clique-copies)
- [Complement graph](#complement-graph)
  - [Simultaneously bipartite graph and complement](#simultaneously-bipartite-graph-and-complement)
- [Menger theorem](#menger-theorem)
  - [Vertex separator](#vertex-separator)
  - [Local connectivity](#local-connectivity)
  - [Internally vertex-disjoint paths](#internally-vertex-disjoint-paths)
  - [Set version of Menger theorem](#set-version-of-menger-theorem)
    - [Fan lemma](#fan-lemma)
  - [Linked graph](#linked-graph)
    - [Four-connected planar obstruction to two-linkage](#four-connected-planar-obstruction-to-two-linkage)
    - [Rooted dense minor linkage](#rooted-dense-minor-linkage)
  - [Vertex connectivity](#vertex-connectivity)
    - [Rooted separation of a graph](#rooted-separation-of-a-graph)
    - [k-connected graph](#k-connected-graph)
      - [Dirac circumference theorem](#dirac-circumference-theorem)
        - [Longest-cycle attachment argument](#longest-cycle-attachment-argument)
      - [3-connected graph](#3-connected-graph)
  - [Edge connectivity](#edge-connectivity)
  - [Whitney inequalities for graph connectivity](#whitney-inequalities-for-graph-connectivity)
    - [Connectivity realization construction](#connectivity-realization-construction)
- [Graph subdivision](#graph-subdivision)
  - [Branch vertex of a graph subdivision](#branch-vertex-of-a-graph-subdivision)
  - [Branch path of a graph subdivision](#branch-path-of-a-graph-subdivision)
  - [Complete graph subdivision](#complete-graph-subdivision)
- [Bipartite vertex cover](#bipartite-vertex-cover)
- [Erdős-Gallai theorem](#erdos-gallai-theorem)
- [Prism graph](#prism-graph)
- [Squaregraph](#squaregraph)
- [Vertex cycle cover](#vertex-cycle-cover)
- [Pósa's theorem](#posa-s-theorem)
- [Pseudoforest](#pseudoforest)

## Network robustness

↑ **Parent:** [Graph theory](graph-theory.md)

Persistence of a specified network property under a specified class of perturbations. Robustness of connectivity and robustness of dynamical function are different questions.

### Network redundancy

↑ **Parent:** [Network robustness](#network-robustness)

Alternative routes or components can preserve function after failure, provided they do not share the same relevant failure mode.

### Network resilience

↑ **Parent:** [Network robustness](#network-robustness)

Maintenance or recovery of specified network performance after a disturbance, including its transient response and recovery time.

#### Cascading failure

↑ **Parent:** [Network resilience](#network-resilience)

A failure changes loads or dependencies so that further components fail. Connectivity of the surviving graph alone does not determine whether a cascade occurs.

## Network motif

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Network_motif)

A small interaction pattern occurring unusually often relative to a specified [network null model](#network-null-model). A circuit's wiring and proposed dynamical function should be distinguished from the statistical evidence that its pattern is enriched in a network.

<h2 id="reka-albert">Réka Albert</h2>

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Réka_Albert)

<h3 id="work-by-reka-albert">Work by Réka Albert</h3>

↑ **Parent:** [Réka Albert](#reka-albert)

<h2 id="albert-laszlo-barabasi">Albert-László Barabási</h2>

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Albert-László_Barabási)

<h3 id="work-by-albert-laszlo-barabasi">Work by Albert-László Barabási</h3>

↑ **Parent:** [Albert-László Barabási](#albert-laszlo-barabasi)

## Duncan J. Watts

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Duncan_Watts)

### Work by Duncan J. Watts

↑ **Parent:** [Duncan J. Watts](#duncan-j-watts)

## Community detection

↑ **Parent:** [Graph theory](graph-theory.md)

[Community detection](#community-detection) partitions a network into groups according to a specified structural criterion, often excess internal connectivity. The output depends on the objective, so a partition inferred from topology need not by itself establish distinct biological functions.

## Network null model

↑ **Parent:** [Graph theory](graph-theory.md)

A [network null model](#network-null-model) specifies the reference network ensemble or expected connectivity against which a pattern is measured. For standard [network modularity](#network-modularity), expected edge weight is $k_ik_j/(2m)$. The reference is part of the scientific model: choosing a different reference can change what counts as excess structure.

## Network modularity

↑ **Parent:** [Graph theory](graph-theory.md)

[Network modularity](#network-modularity) measures excess within-community edge weight relative to a [network null model](#network-null-model) based on [degrees of vertices](#degree-graph-theory). For an undirected unweighted [graph](graph.md), its standard form is $Q=(2m)^{-1}\sum_{ij}(A_{ij}-k_ik_j/(2m))\mathbf1\{c_i=c_j\}$. A single community containing every [vertex](graph.md#vertex-graph-theory) has $Q=0$; a partition with more internal connectivity than expected can have positive $Q$.

## Louvain method

↑ **Parent:** [Graph theory](graph-theory.md)

The [Louvain method](#louvain-method) is a greedy multilevel [community detection](#community-detection) algorithm maximizing [network modularity](#network-modularity). It alternates positive-gain single-vertex moves with contraction of communities into weighted [vertices](graph.md#vertex-graph-theory). Different vertex orders can produce different local optima; a result is not a certificate of globally maximum modularity.[§2, Method](mathematics-bibliography.md#fast-unfolding-of-communities-in-large-networks-by-vincent-d-blondel-and-others)

## Eigenvector centrality

↑ **Parent:** [Graph theory](graph-theory.md)

[Eigenvector centrality](#eigenvector-centrality) assigns nonnegative vertex scores proportional to the sum of neighbouring scores: $v_i=\lambda_{\max}^{-1}\sum_jA_{ij}v_j$. It uses a nonnegative [eigenvector](linear-operator-theory.md#eigenvector) of the [adjacency matrix](#adjacency-matrix) for its largest positive [eigenvalue](linear-operator-theory.md#eigenvalue). State the normalization, such as [Euclidean norm](normed-vector-space.md#euclidean-norm) one. For a three-leaf [star graph](bipartite-graph.md#star-graph-theory), hub and leaf scores have ratio $\sqrt3$.

## Degree-preserving edge rewiring

↑ **Parent:** [Graph theory](graph-theory.md)

[Degree-preserving edge rewiring](#degree-preserving-edge-rewiring) replaces two [edges](#edge-of-a-graph) $(u,v)$ and $(x,y)$ by $(u,y)$ and $(x,v)$, preserving every endpoint's [degree of a vertex](#degree-graph-theory). On [simple graphs](graph.md#simple-graph), reject proposed [self-loops](graph.md#loop-graph-theory) and duplicate edges. Symmetric random proposals with rejected moves retained preserve a uniform distribution on the reachable realizations; adequate mixing remains a separate requirement. Connectivity can change unless explicitly constrained.

## Scale-free network

↑ **Parent:** [Graph theory](graph-theory.md)

A [scale-free network](#scale-free-network) has a [degree distribution](#degree-distribution) with an approximately power-law tail over a meaningful range. Evidence requires degrees from enough [vertices](graph.md#vertex-graph-theory) to assess that range and compare alternative tail models. Large [clustering coefficients](#clustering-coefficient) or short [graph distances](#distance-graph-theory) alone do not establish this property.

## Degree distribution

↑ **Parent:** [Graph theory](graph-theory.md)

A [degree distribution](#degree-distribution) assigns the fraction or probability of [vertices](graph.md#vertex-graph-theory) having each [degree of a vertex](#degree-graph-theory). For an observed network, $P(k)=\#\{i:k_i=k\}/n$. Preserving every labelled degree preserves this distribution, but preserving only its mean does not.

## Small-worldness

↑ **Parent:** [Graph theory](graph-theory.md)

[Small-worldness](#small-worldness) compares a network's clustering and average shortest-path length to reference values through $\sigma=(C/C_{\rm rand})/(L/L_{\rm rand})$. The common $\sigma>1$ classification is a ratio-based convention rather than a significance test; random-reference variability must be assessed separately.[New measures of small-world-ness, Definition 2](mathematics-bibliography.md#network-‘small-world-ness’-a-quantitative-method-for-determining-canonical-network-equivalence-by-mark-d-humphries-and-others)

## Small-world network

↑ **Parent:** [Graph theory](graph-theory.md)

A [small-world network](#small-world-network) combines elevated local [clustering coefficients](#clustering-coefficient) with mean [graph distance](#distance-graph-theory) comparable to a chosen reference ensemble of [random graphs](random-graph.md). Both the reference ensemble and the clustering convention must be specified. A network can have these properties without having a power-law [degree distribution](#degree-distribution).

## Clustering coefficient

↑ **Parent:** [Graph theory](graph-theory.md)

For a [vertex](graph.md#vertex-graph-theory) with $k_i\geq2$ neighbours in a [simple graph](graph.md#simple-graph), its local [clustering coefficient](#clustering-coefficient) is $C_i=e_i/\binom{k_i}{2}$, where $e_i$ counts [edges](#edge-of-a-graph) among those neighbours. It is the fraction of possible neighbour-neighbour edges that are present. A common network summary averages these local coefficients, setting them to zero for degrees below two; this differs from weighting by the number of neighbour pairs.

## Spanning forest

↑ **Parent:** [Graph theory](graph-theory.md)

An acyclic spanning subgraph containing a [spanning tree](tree-graph-theory.md#spanning-tree) of each [connected component](geometry-and-topology.md#connected-component) of the original graph. For a graph with $n$ vertices and $c$ components, a spanning forest has $n-c$ edges.

## Circle graph

↑ **Parent:** [Graph theory](graph-theory.md)

The [intersection graph](#intersection-graph) of chords of a circle: each chord is a vertex, and two vertices are adjacent when their chords cross. Two chords with distinct endpoints cross exactly when their endpoints alternate around the circle.

### Permutation graph

↑ **Parent:** [Circle graph](#circle-graph)

The [intersection graph](#intersection-graph) of the segments in a [permutation diagram](#permutation-diagram). Two segments cross exactly when their endpoint orders disagree. A set of mutually noncrossing segments corresponds to a monotone subsequence of the endpoint [permutation](combinatorics.md#permutation).

#### Permutation diagram

↑ **Parent:** [Permutation graph](#permutation-graph)

A diagram of straight segments joining two parallel lines, with distinct endpoints on each line. Ordering the endpoints along the two lines encodes a [permutation](combinatorics.md#permutation); crossing segments define the associated [permutation graph](#permutation-graph).

## Graph bandwidth

↑ **Parent:** [Graph theory](graph-theory.md)

## Interval graph

↑ **Parent:** [Graph theory](graph-theory.md)

## Pathwidth

↑ **Parent:** [Graph theory](graph-theory.md)

## Chip-firing game

↑ **Parent:** [Graph theory](graph-theory.md)

A discrete process in which a vertex holding at least its degree in chips may send one chip along each incident edge. On the infinite line, a firing removes two chips from a site and gives one to each neighbor. When stabilization exists, commuting local firings explain why their order does not change the final stable configuration.

### Abelian sandpile model

↑ **Parent:** [Chip-firing game](#chip-firing-game)

## De Bruijn graph

↑ **Parent:** [Graph theory](graph-theory.md)

For an alphabet of size $q$, the order-$n$ directed [graph](graph.md) has words of length $n-1$ as [vertices](graph.md#vertex-graph-theory) and words of length $n$ as [edges](#edge-of-a-graph). An [edge](#edge-of-a-graph) goes from its prefix of length $n-1$ to its suffix of that length. An [Eulerian cycle](#eulerian-cycle) therefore lists every length-$n$ word once as a cyclic window, producing a [De Bruijn sequence](combinatorics.md#de-bruijn-sequence).

## Geometric spanner

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_spanner)

A geometric spanner is a [weighted graph](random-walk.md#weighted-graph) on points in [Euclidean space](normed-vector-space.md#euclidean-norm), with edge weights equal to their [Euclidean distances](topological-analysis.md#euclidean-distance), in which every pair has a [graph path](#path-in-a-graph) of [length](physics.md#length) at most $t$ times its direct distance. Its [stretch factor](metric-embedding.md#stretch-factor) is the largest ratio $d_G(u,v)/\|u-v\|$, where $d_G$ is shortest-path distance. A square's four perimeter edges, without diagonals, give stretch factor $\sqrt2$: adjacent points have ratio one, and diagonal pairs have route [length](physics.md#length) $2$ instead of $\sqrt2$. The aim is to retain short routes with fewer edges than a [complete graph](#complete-graph). [Gudmundsson, Narasimhan and Smid, Geometric Spanners, §1](https://people.scs.carleton.ca/~michiel/encyc_geometric_spanners.pdf).

## Graph excess

↑ **Parent:** [Graph theory](graph-theory.md)

Here excess means edges minus vertices. For a [connected graph](graph.md#connected-graph) it is one less than the number of independent cycles. Deleting a leaf and its incident edge, or suppressing a degree-two vertex, preserves excess. This convention differs by one from the cyclomatic number for connected graphs.

### Bicyclic graph

↑ **Parent:** [Graph excess](#graph-excess)

A connected bicyclic graph has two independent cycles, equivalently excess one. Its [2-core](#2-core-of-a-graph) has the same excess and every removed vertex lies in a tree attached to the core. The [graph kernel](#graph-kernel) captures the finite collection of possible branching structures.

#### Labelled bicyclic graph count

↑ **Parent:** [Bicyclic graph](#bicyclic-graph)

If $b_k$ counts labelled bicyclic cores on $k$ vertices, the [bicyclic kernel classification](#bicyclic-kernel-classification) gives $b_k\leq A k!k^2$. Three internally nonempty paths between two branching vertices give $b_k\geq k!\binom{k-3}{2}/12$ for $k\geq5$. Attach a forest with those core vertices as roots to obtain $C(n,n+1)=\sum_k\binom nk b_kkn^{n-k-1}$. After division by $n^{n+1}$ the relevant sum is $n^{-2}\sum_k k^3(n)_k/n^k$. Its upper bound follows from $(n)_k/n^k\leq e^{-k(k-1)/(2n)}$; its lower bound uses $\sqrt n\leq k\leq2\sqrt n$, where this product stays bounded below. The sum is bounded above and below by positive constants. The restriction $n\geq4$ is necessary: $C(3,4)=0$.

#### Bicyclic kernel classification

↑ **Parent:** [Bicyclic graph](#bicyclic-graph)

The [graph kernel](#graph-kernel) of a [bicyclic graph](#bicyclic-graph) satisfies $\sum_v(\deg v-2)=2$, with all degrees at least three. It therefore has either one degree-four vertex carrying two loops, a [bouquet graph](graph.md#bouquet-graph), or two degree-three vertices. In the latter case connectivity and degree counting give either three parallel edges, the three-edge [Theta graph](algebraic-topology.md#theta-graph), or one edge between the vertices and one loop at each, a [dumbbell graph](algebraic-topology.md#dumbbell-graph). All bicyclic cores are subdivisions of these three kernels, subject to simplicity restrictions on loop lengths and parallel paths.

## 2-core of a graph

↑ **Parent:** [Graph theory](graph-theory.md)

The [2-core](#2-core-of-a-graph) is what remains of a finite [simple graph](graph.md#simple-graph) after repeatedly removing every [vertex](graph.md#vertex-graph-theory) with fewer than two surviving [graph neighbours](#neighbour-of-a-vertex). It strips away dangling [trees](tree-graph-theory.md) while keeping the part that can support itself under this local rule. Precisely, for an [undirected graph](#undirected-graph) $G=(V,E)$, its [2-core](#2-core-of-a-graph) is the unique maximum by [set inclusion](set.md#set-inclusion) [induced subgraph](#induced-subgraph) $G[S]$ such that

$$
\deg_{G[S]}(v)\geq2\qquad\text{for every }v\in S.
$$

The empty [vertex set](graph.md#vertex-set) is allowed: the condition is then vacuous, without needing to define the [minimum degree](#minimum-degree-of-a-graph) of the empty [graph](graph.md). "Maximum by inclusion" means that $S$ contains every other [vertex set](graph.md#vertex-set) satisfying the condition. It is stronger than merely saying that one chosen set cannot be enlarged: the [2-core](#2-core-of-a-graph) simultaneously contains all possible qualifying [induced subgraphs](#induced-subgraph). In this particular family, every inclusion-maximal qualifying set does equal that unique maximum; the [union](set.md#set-union) argument in [why the 2-core is unique](#why-the-2-core-is-unique) explains why. [Batagelj and Zaveršnik, An O(m) Algorithm for Cores Decomposition of Networks, §2, definition of a core](computer-science-bibliography.md#an-o-m-algorithm-for-cores-decomposition-of-networks-by-vladimir-batagelj-and-matjaz-zaversnik)

For a complete worked example, let $ab$ denote the [edge](#edge-of-a-graph) $\{a,b\}$ and take

$$
V=\{a,b,c,d,e,f,g,z\},\qquad E=\{ab,bc,ca,cd,de,ef,dg\}.
$$

The [triangle in a graph](graph.md#triangle-in-a-graph) $abc$ has a branching tail attached at $c$, and $z$ is an [isolated vertex](random-graph.md#isolated-vertex). In alphabetical order the initial [degrees of vertices](#degree-graph-theory) are $(2,2,3,3,2,1,1,0)$. Deleting $f$ turns $e$ into a [leaf of a graph](#leaf-of-a-graph); deleting $g$ leaves $d$ with [degree of a vertex](#degree-graph-theory) two; deleting $z$ changes no other [degree of a vertex](#degree-graph-theory). Now delete $e$, which makes $d$ a [leaf of a graph](#leaf-of-a-graph), and finally delete $d$. Exactly the three [edges](#edge-of-a-graph) of $abc$ remain: $C_2(G)=G[\{a,b,c\}]$.

<a id="image-the-complete-leaf-pruning-for-the-2-core-trace-each-panel-recomputes-the-displayed-degrees-of-vertices-from-the-surviving-induced-subgraph-while-the-fifo-queue-determines-the-next-deletion"></a>
![](graph-two-core-leaf-pruning-trace.png)

**[Figure 1](#image-the-complete-leaf-pruning-for-the-2-core-trace-each-panel-recomputes-the-displayed-degrees-of-vertices-from-the-surviving-induced-subgraph-while-the-fifo-queue-determines-the-next-deletion). The complete leaf pruning for the 2-core trace: each panel recomputes the displayed degrees of vertices from the surviving induced subgraph, while the FIFO queue determines the next deletion**.

A [forest](tree-graph-theory.md#forest) has empty [2-core](#2-core-of-a-graph): every nonempty finite [forest](tree-graph-theory.md#forest) has an [isolated vertex](random-graph.md#isolated-vertex) or a [leaf of a graph](#leaf-of-a-graph), so deletion cannot stop at a nonempty remainder. In particular, an isolated [edge](#edge-of-a-graph), an [isolated vertex](random-graph.md#isolated-vertex), a [path graph](#path-graph), and the empty [graph](graph.md) all have empty [2-core](#2-core-of-a-graph). Every [cycle graph](#cycle-graph) is its own [2-core](#2-core-of-a-graph). Two disjoint [triangles in a graph](graph.md#triangle-in-a-graph) also form their own [2-core](#2-core-of-a-graph), so a [2-core](#2-core-of-a-graph) need not be a [connected graph](graph.md#connected-graph); attaching a [tree](tree-graph-theory.md) to either triangle changes neither surviving triangle.

### Leaf pruning for the 2-core

↑ **Parent:** [2-core of a graph](#2-core-of-a-graph)

Use [adjacency lists](data-structure.md#adjacency-list) and a [FIFO queue](data-structure.md#fifo-queue) to implement the deletion rule in [time complexity](theoretical-computer-science.md#time-complexity) $O(|V|+|E|)$. Compute each initial [degree of a vertex](#degree-graph-theory) once, mark every [vertex](graph.md#vertex-graph-theory) alive, and put all [vertices](graph.md#vertex-graph-theory) of [degree of a vertex](#degree-graph-theory) zero or one in the [FIFO queue](data-structure.md#fifo-queue). Each [vertex](graph.md#vertex-graph-theory) is inserted at most once. Repeatedly remove the front [vertex](graph.md#vertex-graph-theory) $v$, mark it dead, and traverse its original [adjacency list](data-structure.md#adjacency-list). For each still-alive [graph neighbour](#neighbour-of-a-vertex) $u$, decrease the stored [degree of a vertex](#degree-graph-theory) of $u$ by one; if it has just become one, append $u$. A [vertex](graph.md#vertex-graph-theory) already queued can drop from one to zero before its turn, but it stays queued and requires no second insertion. Stop when the [FIFO queue](data-structure.md#fifo-queue) is empty; the alive [vertices](graph.md#vertex-graph-theory) induce $C_2(G)$.

For the displayed example, initially enqueue $(f,g,z)$ in that order. The successive [FIFO queues](data-structure.md#fifo-queue), after each deletion and all its updates, are

$$
(f,g,z)\xrightarrow{-f}(g,z,e)\xrightarrow{-g}(z,e)\xrightarrow{-z}(e)\xrightarrow{-e}(d)\xrightarrow{-d}().
$$

This explains the delayed deletion of $d$: its initial [degree of a vertex](#degree-graph-theory) was three, but the relevant [degree of a vertex](#degree-graph-theory) is always its current one in the surviving [induced subgraph](#induced-subgraph). Removing only the original [vertices](graph.md#vertex-graph-theory) of [degree of a vertex](#degree-graph-theory) one would give the wrong answer.

Initialization inspects every [vertex](graph.md#vertex-graph-theory) and every [adjacency list](data-structure.md#adjacency-list) entry once. During deletion each original [adjacency list](data-structure.md#adjacency-list) is traversed at most once, so at most $2|E|$ entries are inspected in an [undirected graph](#undirected-graph). All insertions, removals and stored-degree updates cost constant time each. Thus total [time complexity](theoretical-computer-science.md#time-complexity) is $O(|V|+|E|)$ and additional storage, beyond the [adjacency lists](data-structure.md#adjacency-list), is $O(|V|)$. The cost includes [isolated vertices](random-graph.md#isolated-vertex); repeatedly rescanning the whole surviving [graph](graph.md) after each deletion would lose this bound. The single-threshold [FIFO queue](data-structure.md#fifo-queue) method is enough for the [2-core](#2-core-of-a-graph); the full [k-core of a graph](#k-core-of-a-graph) decomposition computes all thresholds.

### Why the 2-core is unique

↑ **Parent:** [2-core of a graph](#2-core-of-a-graph)

Suppose $T$ is any [vertex set](graph.md#vertex-set) whose [induced subgraph](#induced-subgraph) has every [degree of a vertex](#degree-graph-theory) at least two. No [vertex](graph.md#vertex-graph-theory) of $T$ can be the first one deleted from $T$: before such a deletion it still has its two [graph neighbours](#neighbour-of-a-vertex) within $T$, contradicting eligibility for deletion. Consequently every qualifying $T$ survives every legal deletion sequence. Once deletion stops, its remainder $R$ itself qualifies, because every surviving [vertex](graph.md#vertex-graph-theory) has at least two surviving [graph neighbours](#neighbour-of-a-vertex). Therefore $T\subseteq R$ for every qualifying $T$: $G[R]$ is the unique maximum and the final remainder is independent of deletion order. The intermediate [FIFO queues](data-structure.md#fifo-queue) and deletion orders can differ.

There is also a direct existence argument. If $A$ and $B$ qualify, then $A\cup B$ qualifies: each [vertex](graph.md#vertex-graph-theory) retains at least the two [graph neighbours](#neighbour-of-a-vertex) it already had in $A$ or in $B$. Taking the [union](set.md#set-union) of all qualifying [vertex sets](graph.md#vertex-set) produces the maximum. This rules out a collection of competing, incomparable inclusion-maximal answers. It also explains why restricting the search to connected [subgraphs](#subgraph) would change the question.

### Bridges and connectivity in the 2-core

↑ **Parent:** [2-core of a graph](#2-core-of-a-graph)

A [2-core](#2-core-of-a-graph) can contain [bridges in a graph](graph.md#bridge-graph-theory), and even [vertices](graph.md#vertex-graph-theory) that lie on no [cycle in a graph](#cycle-in-a-graph). Consider the [dumbbell graph](algebraic-topology.md#dumbbell-graph), also called a barbell in this example, made of two disjoint [triangles in a graph](graph.md#triangle-in-a-graph) joined by a [graph path](#path-in-a-graph) with two internal [vertices](graph.md#vertex-graph-theory):

$$
V=\{a,b,c,x,y,d,e,f\},\qquad E=\{ab,bc,ca,cx,xy,yd,de,ef,fd\}.
$$

Here $c,d$ have [degree of a vertex](#degree-graph-theory) three, and every other [vertex](graph.md#vertex-graph-theory) has [degree of a vertex](#degree-graph-theory) two. No deletion is possible, so the whole [graph](graph.md) is its [2-core](#2-core-of-a-graph). Yet $cx,xy,yd$ are [bridges in a graph](graph.md#bridge-graph-theory): deleting any one separates the two triangles. None belongs to a [cycle in a graph](#cycle-in-a-graph), and $x,y$ belong to no [cycle in a graph](#cycle-in-a-graph) either. Keeping only [edges](#edge-of-a-graph) on [graph cycles](#cycle-in-a-graph) would incorrectly discard the entire joining [graph path](#path-in-a-graph).

<a id="image-every-vertex-of-this-dumbbell-graph-survives-in-the-2-core-including-the-joining-graph-path-whose-three-edges-are-bridges-in-a-graph"></a>
![](graph-two-core-barbell-bridges.png)

**[Figure 2](#image-every-vertex-of-this-dumbbell-graph-survives-in-the-2-core-including-the-joining-graph-path-whose-three-edges-are-bridges-in-a-graph). Every vertex of this dumbbell graph survives in the 2-core, including the joining graph path whose three edges are bridges in a graph**.

Every [cycle in a graph](#cycle-in-a-graph) does survive pruning, because each of its [vertices](graph.md#vertex-graph-theory) keeps its two cycle [graph neighbours](#neighbour-of-a-vertex). The barbell shows that the converse fails: the [2-core](#2-core-of-a-graph) can be larger than the [union](set.md#set-union) of all [graph cycles](#cycle-in-a-graph). Its condition is local [minimum degree](#minimum-degree-of-a-graph), not protection against a single connection failing.

A [biconnected component](#biconnected-component) is a different object: a maximal connected [subgraph](#subgraph) with no [cut vertex](#cut-vertex) of its own. Under the block convention used here, the barbell has five [biconnected components](#biconnected-component): its two triangles and its three individual joining [edges](#edge-of-a-graph), each with its endpoints. Its [cut vertices](#cut-vertex) are $c,x,y,d$. A 2-connected component with at least three [vertices](graph.md#vertex-graph-theory) must remain connected after any single [vertex](graph.md#vertex-graph-theory) is deleted; the whole barbell fails that test. An informal phrase such as "biconnected core" therefore needs its own definition and must not be substituted for [2-core](#2-core-of-a-graph). Even an isolated [edge](#edge-of-a-graph) is a block under this convention, although its [2-core](#2-core-of-a-graph) is empty.

The usefulness of the [2-core](#2-core-of-a-graph) is this precise separation of local persistence from global robustness. In a [connected graph](graph.md#connected-graph) with nonempty [2-core](#2-core-of-a-graph), the deleted [vertices](graph.md#vertex-graph-theory) form a [forest](tree-graph-theory.md#forest), with each of its [connected components of a graph](graph.md#component-graph-theory) attached by exactly one [edge](#edge-of-a-graph) to the [2-core](#2-core-of-a-graph). Otherwise a deleted [graph cycle](#cycle-in-a-graph), or a [graph path](#path-in-a-graph) joining two surviving attachment points, would itself have survived. Stripping these attached [trees](tree-graph-theory.md) exposes a smaller structure for studying [graph cycles](#cycle-in-a-graph), [graph excess](#graph-excess) and the [graph kernel](#graph-kernel), while preserving the joining [bridges in a graph](graph.md#bridge-graph-theory) that organize that structure.

### Graph kernel

↑ **Parent:** [2-core of a graph](#2-core-of-a-graph)

For a [connected graph](graph.md#connected-graph) whose [2-core](#2-core-of-a-graph) contains a [vertex](graph.md#vertex-graph-theory) of [degree of a vertex](#degree-graph-theory) at least three, suppress each maximal [graph path](#path-in-a-graph) with degree-two internal [vertices](graph.md#vertex-graph-theory) to a single [edge](#edge-of-a-graph), allowing its two endpoints to coincide. Here suppression is the reverse of [graph subdivision](#graph-subdivision). The resulting [multigraph](graph.md#multigraph), retaining [self-loops](graph.md#loop-graph-theory) and parallel [edges](#edge-of-a-graph), is its [graph kernel](#graph-kernel). Each suppressed internal [vertex](graph.md#vertex-graph-theory) removes one [vertex](graph.md#vertex-graph-theory) and one [edge](#edge-of-a-graph), preserving [graph excess](#graph-excess); counting a [self-loop](graph.md#loop-graph-theory) twice toward [degree of a vertex](#degree-graph-theory), every remaining [vertex](graph.md#vertex-graph-theory) has [degree of a vertex](#degree-graph-theory) at least three. A purely cyclic [2-core](#2-core-of-a-graph) is a separate unicyclic case: it has no branching [vertex](graph.md#vertex-graph-theory) to anchor this construction.

For the barbell in [bridges and connectivity in the 2-core](#bridges-and-connectivity-in-the-2-core), the [graph kernel](#graph-kernel) has two [vertices](graph.md#vertex-graph-theory) $c,d$, one [self-loop](graph.md#loop-graph-theory) at each, and a single joining [edge](#edge-of-a-graph) $cd$. Suppressing $x,y$ contracts the joining [graph path](#path-in-a-graph) to that [bridge in a graph](graph.md#bridge-graph-theory); suppressing the two other [vertices](graph.md#vertex-graph-theory) on each triangle turns the triangle into a [self-loop](graph.md#loop-graph-theory). The [graph excess](#graph-excess) stays $9-8=3-2=1$. Thus forming a [graph kernel](#graph-kernel) compresses degree-two chains rather than deleting everything outside [graph cycles](#cycle-in-a-graph).

## k-core of a graph

↑ **Parent:** [Graph theory](graph-theory.md)

For a nonnegative [integer](integer.md) $k$, the [k-core of a graph](#k-core-of-a-graph) is the unique maximum by [set inclusion](set.md#set-inclusion) [induced subgraph](#induced-subgraph) in which every [degree of a vertex](#degree-graph-theory) is at least $k$, allowing the empty [graph](graph.md). Repeatedly delete [vertices](graph.md#vertex-graph-theory) whose current [degree of a vertex](#degree-graph-theory) is less than $k$. These [induced subgraphs](#induced-subgraph) are nested: $C_{k+1}(G)\subseteq C_k(G)$; the case $k=2$ is the [2-core](#2-core-of-a-graph). In their 2003 preprint, [Vladimir Batagelj](mathematics.md#vladimir-batagelj) and [Matjaž Zaveršnik](mathematics.md#matjaz-zaversnik) give an [algorithm](algorithm.md) for the entire core decomposition, using degree buckets and constant-time position updates. Their general bound is $O(|V|+|E|)$; the title's $O(m)$ form applies to [connected graphs](graph.md#connected-graph) with at least two [vertices](graph.md#vertex-graph-theory), where $m=|E|\geq|V|-1$. [Batagelj and Zaveršnik, An O(m) Algorithm for Cores Decomposition of Networks, §§2–4.1, especially Algorithm 1 and the general O(max(m,n)) bound](computer-science-bibliography.md#an-o-m-algorithm-for-cores-decomposition-of-networks-by-vladimir-batagelj-and-matjaz-zaversnik)

## Chordal graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chordal_graph)

A [chordal graph](#chordal-graph) is a finite [simple graph](graph.md#simple-graph) with no [induced cycle](#induced-cycle) of length at least four. Equivalently, every [cycle in a graph](#cycle-in-a-graph) with at least four [vertices](graph.md#vertex-graph-theory) has a chord: an [edge](#edge-of-a-graph) joining two nonconsecutive [vertices](graph.md#vertex-graph-theory) of that [graph cycle](#cycle-in-a-graph). The word "induced" matters: the [induced subgraph](#induced-subgraph) on the chosen [vertices](graph.md#vertex-graph-theory) must contain exactly the cycle's [edges](#edge-of-a-graph), with no chords. Triangles are allowed. This definition concerns adjacency, independently of how the [graph](graph.md) is drawn.

For the square [cycle graph](#cycle-graph) $C_4$, take [vertex set](graph.md#vertex-set) $\{a,b,c,d\}$ and set of [edges](#edge-of-a-graph) $\{ab,bc,cd,da\}$, where $ab$ abbreviates $\{a,b\}$. Its [graph neighbourhoods](#graph-neighbourhood) are $N(a)=N(c)=\{b,d\}$ and $N(b)=N(d)=\{a,c\}$. The square is an [induced cycle](#induced-cycle), so $C_4$ is not a [chordal graph](#chordal-graph). Add the single [edge](#edge-of-a-graph) $ac$: now $N(a)=\{b,c,d\}$, $N(b)=\{a,c\}$, $N(c)=\{a,b,d\}$, and $N(d)=\{a,c\}$. The only possible four-[vertex](graph.md#vertex-graph-theory) [graph cycle](#cycle-in-a-graph) has chord $ac$, so this new [graph](graph.md) is a [chordal graph](#chordal-graph). Its [maximal cliques](#maximal-clique) are exactly $\{a,b,c\}$ and $\{a,c,d\}$.

<a id="image-an-induced-cycle-loses-its-obstruction-when-one-diagonal-is-added-the-resulting-maximal-cliques-form-a-junction-tree"></a>
![](chordal-perfect-elimination-square-cliques.png)

**[Figure 3](#image-an-induced-cycle-loses-its-obstruction-when-one-diagonal-is-added-the-resulting-maximal-cliques-form-a-junction-tree). An induced cycle loses its obstruction when one diagonal is added; the resulting maximal cliques form a junction tree**.

Connect these two [maximal cliques](#maximal-clique) by a single [edge](#edge-of-a-graph) labelled with their intersection $\{a,c\}$. The result is a [junction tree](statistical-model.md#junction-tree), also called a clique tree: its nodes are [maximal cliques](#maximal-clique), and the nodes containing any fixed original [vertex](graph.md#vertex-graph-theory) induce a [connected graph](graph.md#connected-graph) inside the [tree](tree-graph-theory.md). Here $a,c$ occur in both nodes, while $b,d$ each occur in just one. This is the [running intersection property](statistical-model.md#running-intersection-property). More generally, a nonempty [connected graph](graph.md#connected-graph) is a [chordal graph](#chordal-graph) exactly when its [maximal cliques](#maximal-clique) admit such a [tree](tree-graph-theory.md); a disconnected [chordal graph](#chordal-graph) can be represented by one such [tree](tree-graph-theory.md) per [connected component of a graph](graph.md#component-graph-theory).[§3.1–3.2](mathematics-bibliography.md#an-introduction-to-chordal-graphs-and-clique-trees-by-jean-r-s-blair-and-others)

A [chordal graph](#chordal-graph) need not be a [planar graph](planar-graph.md): the [complete graph](#complete-graph) $K_5$ is a [chordal graph](#chordal-graph), since every pair of distinct [vertices](graph.md#vertex-graph-theory) is adjacent, but its ten [edges](#edge-of-a-graph) violate the [planar graph edge bound](planar-graph.md#planar-graph-edge-bound) $|E|\leq3|V|-6=9$. Conversely, even a plane drawing whose bounded faces are triangles can hide an [induced cycle](#induced-cycle): a [wheel graph](#wheel-graph) with a four-[vertex](graph.md#vertex-graph-theory) rim and a central [vertex](graph.md#vertex-graph-theory) joined to the whole rim still has the rim as an [induced cycle](#induced-cycle). Adding chords to obtain a [chordal graph](#chordal-graph) is called [triangulation of an undirected graph](#triangulation-of-an-undirected-graph); this is an adjacency condition, rather than a requirement about planar faces.

Why is this structure useful? The [maximal cliques](#maximal-clique) collect local interactions, and the [running intersection property](statistical-model.md#running-intersection-property) makes their overlaps sufficient for consistent communication. For [random variables](random-variable.md) $x_a,x_b,x_c,x_d$ with finite state sets, a [probabilistic graphical model](statistical-model.md#probabilistic-graphical-model) of the square-plus-diagonal form can have

$$
p(x_a,x_b,x_c,x_d)=Z^{-1}\psi_{abc}(x_a,x_b,x_c)\psi_{acd}(x_a,x_c,x_d),
$$

where the two nonnegative [clique potentials](statistical-model.md#clique-potential) have a positive [normalizing constant](continuous-probability-distribution.md#normalizing-constant) $Z$. Eliminating $x_b$ produces the two-variable [junction-tree sum-product message](statistical-model.md#junction-tree-sum-product-message)

$$
m(x_a,x_c)=\sum_{x_b}\psi_{abc}(x_a,x_b,x_c),\qquad Z=\sum_{x_a,x_c,x_d}m(x_a,x_c)\psi_{acd}(x_a,x_c,x_d).
$$

The shared [clique](#clique-graph-theory) $\{a,c\}$ carries everything needed from the eliminated side. For $q$ possible states per [random variable](random-variable.md), this example uses two sums over $q^3$ configurations after reusing the message, rather than directly summing over $q^4$ configurations. The example's message is an exact finite sum, with no simulated data. Large [maximal cliques](#maximal-clique) still make exact inference expensive; [chordal graphs](#chordal-graph) provide a decomposition, not a universal guarantee of cheap inference.[§1; §6](mathematics-bibliography.md#recitation-8-junction-trees-by-massachusetts-institute-of-technology-department-of-electrical-engineering-and-computer-science)

### Triangulation of an undirected graph

↑ **Parent:** [Chordal graph](#chordal-graph)

Triangulation adds fill edges to an undirected [graph](graph.md) to make it a [chordal graph](#chordal-graph). Given an elimination ordering, join all remaining neighbors of each removed vertex. The completed graph has that [perfect elimination ordering](#perfect-elimination-ordering). Fill edges can enlarge the [cliques](#clique-graph-theory) used for exact [probabilistic graphical model](statistical-model.md#probabilistic-graphical-model) inference, without changing the original probability factors; they do not assert new biological relationships.

### Perfect elimination ordering

↑ **Parent:** [Chordal graph](#chordal-graph)

A [perfect elimination ordering](#perfect-elimination-ordering) of a finite [simple graph](graph.md#simple-graph) $G=(V,E)$ is a [permutation](combinatorics.md#permutation) $(v_1,\ldots,v_n)$ of its [vertices](graph.md#vertex-graph-theory) such that each set of later [graph neighbours](#neighbour-of-a-vertex)

$$
N_i^+=\{v_j:j>i,\ \{v_i,v_j\}\in E\}
$$

is a [clique](#clique-graph-theory). Thus $v_i$ is a [simplicial vertex](#simplicial-vertex-graph-theory) in the remaining [induced subgraph](#induced-subgraph) $G[\{v_i,\ldots,v_n\}]$. Empty and one-[vertex](graph.md#vertex-graph-theory) sets satisfy the [clique](#clique-graph-theory) condition automatically. The order here is the order of deletion: $v_1$ goes first.

The characterization is powerful: a finite [simple graph](graph.md#simple-graph) is a [chordal graph](#chordal-graph) if and only if it has a [perfect elimination ordering](#perfect-elimination-ordering). For one proof outline, the earliest [vertex](graph.md#vertex-graph-theory) of an [induced cycle](#induced-cycle) of length at least four would have two later [graph neighbours](#neighbour-of-a-vertex) on that [graph cycle](#cycle-in-a-graph) that are not adjacent, contradicting the [clique](#clique-graph-theory) condition. Conversely, every nonempty [chordal graph](#chordal-graph) has a [simplicial vertex](#simplicial-vertex-graph-theory), and every [induced subgraph](#induced-subgraph) of a [chordal graph](#chordal-graph) is a [chordal graph](#chordal-graph); repeatedly deleting such a [vertex](graph.md#vertex-graph-theory) supplies the ordering.[§2.2; Theorem 2.2](mathematics-bibliography.md#an-introduction-to-chordal-graphs-and-clique-trees-by-jean-r-s-blair-and-others)

In the square-plus-diagonal [chordal graph](#chordal-graph) above, $(b,d,a,c)$ is a [perfect elimination ordering](#perfect-elimination-ordering), with later [graph neighbourhoods](#graph-neighbourhood) $\{a,c\}$, $\{a,c\}$, $\{c\}$, and $\varnothing$. Starting instead with $a$ fails: its [graph neighbours](#neighbour-of-a-vertex) $b,c,d$ do not form a [clique](#clique-graph-theory), because $bd$ is absent. Thus even a [chordal graph](#chordal-graph) can have a poor elimination ordering.

For a larger example, join three triangles along shared [edges](#edge-of-a-graph), using

$$
V=\{a,b,c,d,e\},\qquad E=\{ab,ac,bc,bd,cd,ce,de\}.
$$

The exact [graph neighbourhoods](#graph-neighbourhood) are $N(a)=\{b,c\}$, $N(b)=\{a,c,d\}$, $N(c)=\{a,b,d,e\}$, $N(d)=\{b,c,e\}$, and $N(e)=\{c,d\}$. The ordering $(a,b,c,d,e)$ has later [graph neighbourhoods](#graph-neighbourhood) $\{b,c\}$, $\{c,d\}$, $\{d,e\}$, $\{e\}$, and $\varnothing$, all [cliques](#clique-graph-theory); this certifies that the [graph](graph.md) is a [chordal graph](#chordal-graph) without enumerating its [graph cycles](#cycle-in-a-graph). Its [maximal cliques](#maximal-clique) $\{a,b,c\}$, $\{b,c,d\}$, $\{c,d,e\}$ form a [junction tree](statistical-model.md#junction-tree) in that order, with intersections $\{b,c\}$ and $\{c,d\}$.

<a id="image-a-perfect-elimination-ordering-removes-three-overlapping-triangles-without-fill-in-choosing-the-central-vertex-first-adds-three-edges"></a>
![](chordal-perfect-elimination-triangle-chain.png)

**[Figure 4](#image-a-perfect-elimination-ordering-removes-three-overlapping-triangles-without-fill-in-choosing-the-central-vertex-first-adds-three-edges). A perfect elimination ordering removes three overlapping triangles without fill-in; choosing the central vertex first adds three edges**.

To find an ordering, [maximum cardinality search](#maximum-cardinality-search) starts with all scores zero, repeatedly selects an unselected [vertex](graph.md#vertex-graph-theory) of largest score, and increases each unselected [graph neighbour](#neighbour-of-a-vertex)'s score by one. Reverse the selection order to obtain a candidate [perfect elimination ordering](#perfect-elimination-ordering). For the three-triangle [graph](graph.md), one valid selection sequence is $(e,d,c,b,a)$, with scores at selection $0,1,2,2,2$; reversing it gives the displayed deletion order. On a [chordal graph](#chordal-graph) every tie choice works. On an arbitrary [graph](graph.md), test the resulting later [graph neighbourhoods](#graph-neighbourhood) for the [clique](#clique-graph-theory) condition to recognize [chordal graphs](#chordal-graph). Suitable [adjacency lists](data-structure.md#adjacency-list), score buckets and a linear-time verification method give $O(|V|+|E|)$ recognition.[§4.1–4.2; Algorithm 4.2](mathematics-bibliography.md#chordal-graphs-and-semidefinite-optimization-by-lieven-vandenberghe-and-others)

The deletion rule also explains [sparse Gaussian elimination](numerical-linear-algebra.md#sparse-gaussian-elimination). For a symmetric [positive-definite matrix](quadratic-form.md#positive-definite-matrix) whose [matrix graph](numerical-linear-algebra.md#matrix-graph) is $G$, eliminating pivot $v$ applies the [Schur complement](linear-algebra.md#schur-complement) update

$$
a_{uw}\longleftarrow a_{uw}-\frac{a_{uv}a_{vw}}{a_{vv}}.
$$

Only pairs of remaining [graph neighbours](#neighbour-of-a-vertex) of $v$ can acquire new off-diagonal entries. A [perfect elimination ordering](#perfect-elimination-ordering) already has all those [edges](#edge-of-a-graph), so [Cholesky decomposition](quadratic-form.md#cholesky-decomposition) creates no symbolic [fill-in](numerical-linear-algebra.md#fill-in). Positive definiteness ensures nonzero pivots in exact arithmetic. Special numerical cancellation can suppress predicted entries, and floating-point rounding affects their values.[§9.1; equation 9.2; Theorem 9.1](mathematics-bibliography.md#chordal-graphs-and-semidefinite-optimization-by-lieven-vandenberghe-and-others) In the three-triangle [graph](graph.md), deleting $c$ first instead connects every pair in $\{a,b,d,e\}$ and adds exactly $ad,ae,be$. The [graph](graph.md) was already a [chordal graph](#chordal-graph); the extra [fill-in](numerical-linear-algebra.md#fill-in) comes from the ordering.

One further reward is optimal [graph coloring](graph-coloring.md). Process a [perfect elimination ordering](#perfect-elimination-ordering) backwards and give each [vertex](graph.md#vertex-graph-theory) the smallest positive color absent from its already colored [graph neighbours](#neighbour-of-a-vertex). Those [graph neighbours](#neighbour-of-a-vertex) form a [clique](#clique-graph-theory), so this [greedy algorithm](algorithm.md#greedy-algorithm) uses at most the [clique number](#clique-number) $\omega(G)$ colors; any [clique](#clique-graph-theory) of that size requires at least that many. In the three-triangle [graph](graph.md), coloring $(e,d,c,b,a)$ gives colors $(1,2,3,1,2)$, so both the [chromatic number](graph-coloring.md#chromatic-number) and the [clique number](#clique-number) are three. Every [maximal clique](#maximal-clique) also occurs among $\{v_i\}\cup N_i^+$: take its earliest [vertex](graph.md#vertex-graph-theory) and use maximality. The same ordering therefore supports [graph coloring](graph-coloring.md), [maximal clique](#maximal-clique) extraction and sparse computation.

Historically, Donald J. Rose, Robert E. Tarjan and George S. Lueker's 1976 paper connected [graph](graph.md) elimination to symmetric [sparse matrices](vector-space.md#sparse-matrix) and gave a search-based $O(|V|+|E|)$ [algorithm](algorithm.md) for finding a [perfect elimination ordering](#perfect-elimination-ordering) when one exists. Its abstract distinguishes a minimal elimination ordering from a minimum one: removing avoidable [fill-in](numerical-linear-algebra.md#fill-in) does not by itself minimize the total number of added [edges](#edge-of-a-graph).[pp. 266–283; abstract](mathematics-bibliography.md#algorithmic-aspects-of-vertex-elimination-on-graphs-by-donald-j-rose-and-others)

#### Simplicial vertex (graph theory)

↑ **Parent:** [Perfect elimination ordering](#perfect-elimination-ordering)

A [simplicial vertex](#simplicial-vertex-graph-theory) is a [graph vertex](graph.md#vertex-graph-theory) whose [graph neighbourhood](#graph-neighbourhood) is a [clique](#clique-graph-theory). Every isolated [vertex](graph.md#vertex-graph-theory) and every [leaf of a graph](#leaf-of-a-graph) qualifies. In the three-triangle [chordal graph](#chordal-graph), initially $a,e$ qualify, but $b$ only becomes a [simplicial vertex](#simplicial-vertex-graph-theory) after deleting $a$. This is a property of adjacency in a [graph](graph.md); a [vertex of a simplicial complex](algebraic-topology.md#vertex-of-a-simplicial-complex) is an element of a different kind of structure.

#### Maximum cardinality search

↑ **Parent:** [Perfect elimination ordering](#perfect-elimination-ordering)

[Maximum cardinality search](#maximum-cardinality-search) is a [graph](graph.md) search in which an unselected [vertex](graph.md#vertex-graph-theory)'s score counts its already selected [graph neighbours](#neighbour-of-a-vertex). Repeatedly select a [vertex](graph.md#vertex-graph-theory) of maximum score, breaking ties arbitrarily, and update its unselected [graph neighbours](#neighbour-of-a-vertex). On a [chordal graph](#chordal-graph), the reverse selection order is a [perfect elimination ordering](#perfect-elimination-ordering). On $C_4$, selecting $(a,b,c,d)$ instead yields candidate deletion order $(d,c,b,a)$; $d$'s later [graph neighbours](#neighbour-of-a-vertex) $a,c$ are not adjacent, so the [clique](#clique-graph-theory) check fails.[§4.2; Algorithm 4.2](mathematics-bibliography.md#chordal-graphs-and-semidefinite-optimization-by-lieven-vandenberghe-and-others)

## Johnson graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Johnson_graph)

The Johnson graph has the $k$-element subsets of an $n$-element set as vertices, with two vertices adjacent exactly when their intersection has $k-1$ elements. Relabelling the ground set gives graph automorphisms. The [maximal cliques of a Johnson graph](#maximal-cliques-of-a-johnson-graph) allow reconstruction of those ground-set labels when the two clique sizes are different.

### Distance in a Johnson graph

↑ **Parent:** [Johnson graph](#johnson-graph)

One edge of a [Johnson graph](#johnson-graph) replaces one element of a $k$-subset, so it can increase intersection with a fixed target by at most one. Replacing each element outside the target by one missing target element gives a path reaching this lower bound. Equal-distance ordered pairs have equal sizes of intersection, the two differences and the remaining ground set; a [permutation](combinatorics.md#permutation) matching these four regions proves [distance transitivity](graph.md#distance-transitive-action-on-a-graph).

### Maximal cliques of a Johnson graph

↑ **Parent:** [Johnson graph](#johnson-graph)

For $1<k<n-1$, the maximal cliques of $J(n,k)$ are the families containing a fixed $(k-1)$-subset, of size $n-k+1$, and the families contained in a fixed $(k+1)$-subset, of size $k+1$. To see why these exhaust the possibilities, write two adjacent vertices as $D\cup\{a\}$ and $D\cup\{b\}$. A common adjacent vertex either contains $D$ or lies in $D\cup\{a,b\}$. A vertex of the first kind outside that union is not adjacent to a vertex of the second kind omitting an element of $D$, so a clique cannot mix these alternatives. For $J(n,3)$ and $n\ge5$, $n\ne6$, the clique sizes $n-2$ and four distinguish the families containing pairs. Their incidence recovers $J(n,2)$, whose stars of size $n-1$ distinguish the individual ground-set points from its triangular cliques.

## Maximum degree

↑ **Parent:** [Graph theory](graph-theory.md)

The maximum degree of a finite [graph](graph.md) is the largest number of edges incident to one vertex. A bound $d$ on degree bounds the number of vertices within distance $k$ of a fixed vertex by $1+d+\cdots+d^k$. Such counting bounds turn a large vertex count into a lower bound on diameter.

## Four-cycle counting by common neighbours

↑ **Parent:** [Graph theory](graph-theory.md)

For a simple [graph](graph.md), let $r_{ij}$ count the common neighbours of vertices $i,j$. Choosing two such neighbours makes a four-cycle, and each cycle is counted twice through its opposite pairs. The displayed identity follows even when extra edges are present, since cycles are counted as subgraphs rather than induced subgraphs. Also $\sum_{i<j}r_{ij}=\sum_v\binom{d(v)}2$. Applying [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to degrees and [Jensen inequality](real-analysis.md#jensen-s-inequality) to common-neighbour counts gives extremal edge and cycle bounds.

## Shortest path problem

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](shortest-path-problem.md)

## Graph property

↑ **Parent:** [Graph theory](graph-theory.md)

A [graph](graph.md) property is a class of finite [graphs](graph.md) closed under isomorphism. Its labelled order-$n$ slice consists of members on [vertex](graph.md#vertex-graph-theory) set $[n]$. Closure under taking arbitrary subgraphs and closure under taking only induced subgraphs lead respectively to [subgraph-closed graph properties](#subgraph-closed-graph-property) and [hereditary graph properties](#hereditary-graph-property).

### Common-center graph property

↑ **Parent:** [Graph property](#graph-property)

All edges of a simple undirected [graph](graph.md) have at least one common endpoint. The empty [graph](graph.md) is included when there is at least one vertex, and isolated vertices are permitted. This is the star predicate with isolated vertices allowed; a connected [star graph](bipartite-graph.md#star-graph-theory) is a special case. Its [decision-tree depth](theoretical-computer-science.md#decision-tree-depth) is the full number $\binom n2$ of edge bits for $n\geq3$.

#### Certificates for the common-center graph property

↑ **Parent:** [Common-center graph property](#common-center-graph-property)

For $n\geq3$, a full [star graph](bipartite-graph.md#star-graph-theory) requires every nonincident edge to be certified absent, and fixing those bits suffices. Rejection is certified by at most three present edges with empty common intersection; a triangle needs all three. Hence [query certificate complexity](theoretical-computer-science.md#certificate-complexity-of-a-boolean-function) is $\max\{3,\binom{n-1}{2}\}=\Theta(n^2)$ for this property.

#### Alternating count of common-center graphs

↑ **Parent:** [Common-center graph property](#common-center-graph-property)

For $n\geq3$, count the empty [graph](graph.md) once, all one-edge [graphs](graph.md) once, and each larger accepted [graph](graph.md) under its unique center. The latter weighted contribution is $n(n-2)$, giving $1-\binom n2+n(n-2)$. Its nonzero value proves evasiveness by the [alternating-sum criterion for decision-tree evasiveness](theoretical-computer-science.md#alternating-sum-criterion-for-decision-tree-evasiveness).

### Speed of a graph property

↑ **Parent:** [Graph property](#graph-property)

The speed counts the labelled [graphs](graph.md) with a given property on [vertex](graph.md#vertex-graph-theory) set $[n]$. For proper unbounded [hereditary graph properties](#hereditary-graph-property), its base-two logarithm has leading term $(1-1/r)\binom n2$, where $r$ is the property's colouring number.

### Hereditary graph property

↑ **Parent:** [Graph property](#graph-property)

A hereditary [graph](graph.md) property is closed under taking [induced subgraphs](#induced-subgraph). It can be described by forbidden induced [graphs](graph.md). Unlike subgraph closure, this condition allows [edges](#edge-of-a-graph) to be essential to membership. Its [colouring number of a hereditary graph property](#colouring-number-of-a-hereditary-graph-property) governs its quadratic enumeration rate.

#### Colouring number of a hereditary graph property

↑ **Parent:** [Hereditary graph property](#hereditary-graph-property)

This parameter measures the largest completely unrestricted clique-independent partition class contained in the property. It is zero for bounded-order hereditary classes and infinite for all [graphs](graph.md). For proper unbounded classes it is a positive integer; it differs from the degeneracy-based colouring number of an individual [graph](graph.md).

##### Hereditary graph enumeration theorem

↑ **Parent:** [Colouring number of a hereditary graph property](#colouring-number-of-a-hereditary-graph-property)

For a proper hereditary [graph](graph.md) property with unbounded orders, the colouring number determines the leading labelled speed. The lower bound comes from one contained [clique-independent partition class](#clique-independent-partition-class). For the upper bound, forbid one induced [graph](graph.md) from each next-size partition type and use the [induced regularity template lemma](probabilistic-combinatorics.md#induced-regularity-template-lemma). Its intermediate-pair [graph](graph.md) is clique-free, and sparse or almost-complete pairs have negligible entropy. Bounded-order properties have colouring number zero and are outside this formula.

#### Clique-independent partition class

↑ **Parent:** [Hereditary graph property](#hereditary-graph-property)

Graphs in $\mathcal C(a,b)$ admit a partition into $a$ total classes, of which $b$ are designated [cliques](#clique-graph-theory) and $a-b$ are designated independent sets. Cross [edges](#edge-of-a-graph) are arbitrary and empty classes are allowed. Balanced cross-edge choices give quadratic labelled speed coefficient $1-1/a$. Comparing this count with every $(a+1)$-class type shows that the hereditary colouring number of this class is exactly $a$.

### Subgraph-closed graph property

↑ **Parent:** [Graph property](#graph-property)

Membership is preserved under deleting [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph). This is the decreasing meaning of monotonicity in extremal [graph](graph.md) enumeration; it differs from an increasing [monotone graph property](random-graph.md#monotone-graph-property) used for random-graph thresholds. For a proper unbounded class, its least excluded chromatic number determines the leading quadratic logarithm of its labelled speed.

#### Enumeration of subgraph-closed graph properties

↑ **Parent:** [Subgraph-closed graph property](#subgraph-closed-graph-property)

Here $r+1$ is the least chromatic number of an excluded [graph](graph.md), for a proper unbounded subgraph-closed property. All subgraphs of a balanced [Turán graph](extremal-graph-theory.md#turan-graph) give the lower bound. For the upper bound, a regularity reduced [graph](graph.md) is clique-free, so its dense pairs have the [Turan theorem](extremal-graph-theory.md#turan-s-theorem) [edge](#edge-of-a-graph) bound; sparse pairs contribute only small binary entropy and the bounded partition description costs only a linear number of bits.

## Orientation of a graph

↑ **Parent:** [Graph theory](graph-theory.md)

A choice of direction for each edge of an undirected [graph](graph.md), producing a [directed graph](#directed-graph).

An [orientation of a graph](#orientation-of-a-graph) keeps the same [vertex set](graph.md#vertex-set) and the same individual [edges](#edge-of-a-graph). For every [edge](#edge-of-a-graph) $\{u,v\}$ with distinct endpoints, choose exactly one [directed edge](#directed-edge), either $u\to v$ or $v\to u$. Replacing it by both arrows is a different construction: it doubles the [edges](#edge-of-a-graph) and permits travel both ways along that connection. In an [orientation of a graph](#orientation-of-a-graph), the return journey must use another route.[§1.10, printed p. 28: an orientation retains the vertex and edge sets and assigns initial and terminal endpoints](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview)

All examples below use finite [simple graphs](graph.md#simple-graph): no [self-loops](graph.md#loop-graph-theory) and no [multiple edges](#multiple-edges). For a [multigraph](graph.md#multigraph), each individual nonloop [edge](#edge-of-a-graph) receives its own direction, so two [multiple edges](#multiple-edges) can point in opposite directions. A [self-loop](graph.md#loop-graph-theory) becomes $u\to u$, which is already a [directed cycle](#directed-cycle) of length one and therefore prevents an [acyclic orientation](#acyclic-orientation). A finite [simple graph](graph.md#simple-graph) with $m$ [edges](#edge-of-a-graph) has $2^m$ [orientations of a graph](#orientation-of-a-graph), since the two choices for each [edge](#edge-of-a-graph) are independent.

Think of [vertices](graph.md#vertex-graph-theory) as junctions and [edges](#edge-of-a-graph) as streets. An [orientation of a graph](#orientation-of-a-graph) makes each street one-way; [reachability](graph.md#reachability-in-a-graph) asks whether a legal journey exists from one specified junction to another. Two useful aims pull in different directions: an [acyclic orientation](#acyclic-orientation) rules out circular dependencies, while a [strong orientation](#strong-orientation) permits journeys between every ordered pair of junctions.

### Acyclic orientation

↑ **Parent:** [Orientation of a graph](#orientation-of-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Acyclic_orientation)

An [acyclic orientation](#acyclic-orientation) is an [orientation of a graph](#orientation-of-a-graph) whose resulting [directed graph](#directed-graph) has no [directed cycle](#directed-cycle), hence is a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph). A [directed cycle](#directed-cycle) must follow every arrow around its closed route. A [cycle in a graph](#cycle-in-a-graph) in the [skeleton of a directed graph](#skeleton-of-a-directed-graph) only requires the corresponding undirected [edges](#edge-of-a-graph); their arrows need not agree around the route.

For the same [triangle in a graph](graph.md#triangle-in-a-graph) with [vertex set](graph.md#vertex-set) $\{A,B,C\}$ and [edges](#edge-of-a-graph) $AB,BC,AC$, compare

$$
D_1:\ A\to B,\ B\to C,\ A\to C,
\qquad
D_2:\ A\to B,\ B\to C,\ C\to A.
$$

Both have an undirected [cycle in a graph](#cycle-in-a-graph) in their [skeleton of a directed graph](#skeleton-of-a-directed-graph). Only $D_2$ has a [directed cycle](#directed-cycle). In $D_1$, $C$ has no outgoing [directed edge](#directed-edge), so a route cannot continue from $C$ back to $A$.

<a id="image-the-same-triangle-in-a-graph-with-an-acyclic-orientation-and-an-orientation-of-a-graph-containing-a-directed-cycle"></a>
![](graph-orientation-triangle-acyclic-versus-cyclic.png)

**[Figure 5](#image-the-same-triangle-in-a-graph-with-an-acyclic-orientation-and-an-orientation-of-a-graph-containing-a-directed-cycle). The same triangle in a graph with an acyclic orientation and an orientation of a graph containing a directed cycle**.

Thus an [acyclic orientation](#acyclic-orientation) does not require its underlying [undirected graph](#undirected-graph) to be a [forest](tree-graph-theory.md#forest). Every [orientation of a graph](#orientation-of-a-graph) of a [forest](tree-graph-theory.md#forest) is acyclic, because a [directed cycle](#directed-cycle) would give an undirected [cycle in a graph](#cycle-in-a-graph). Conversely, every finite [simple graph](graph.md#simple-graph), including one with many [cycles in a graph](#cycle-in-a-graph), admits at least one [acyclic orientation](#acyclic-orientation) by the following ordering construction. On this [triangle in a graph](graph.md#triangle-in-a-graph), six of the eight [orientations of a graph](#orientation-of-a-graph) are acyclic; the other two follow the [directed cycle](#directed-cycle) in opposite senses.

#### Order-induced acyclic orientation

↑ **Parent:** [Acyclic orientation](#acyclic-orientation)

Choose a [strict total order](set.md#strict-total-order) $v_1<\cdots<v_n$ of the [vertices](graph.md#vertex-graph-theory) of a finite [simple graph](graph.md#simple-graph). Direct every [edge](#edge-of-a-graph) $v_iv_j$ from $v_i$ to $v_j$ when $i<j$. Along every [directed path](#directed-path), the index strictly increases. Returning to the starting [vertex](graph.md#vertex-graph-theory) would require an impossible strict increase back to the initial index, so this is an [acyclic orientation](#acyclic-orientation). The displayed $D_1$ comes from $A<B<C$.

The chosen [strict total order](set.md#strict-total-order) is a [topological order](combinatorics.md#topological-order) of the resulting [Directed acyclic graph](combinatorics.md#directed-acyclic-graph). Conversely, every [acyclic orientation](#acyclic-orientation) of a finite [simple graph](graph.md#simple-graph) has a [topological order](combinatorics.md#topological-order), and orienting its [edges](#edge-of-a-graph) from earlier to later in that order recovers it. Different [topological orders](combinatorics.md#topological-order) can induce the same [acyclic orientation](#acyclic-orientation), since [vertices](graph.md#vertex-graph-theory) with no [edge](#edge-of-a-graph) between them need not impose a choice of arrow.[printed pp. 4–6: job scheduling, topological sorting and its edge-order correctness condition](computer-science-bibliography.md#6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-14-graphs-ii-depth-first-search)

An order respects [reachability](graph.md#reachability-in-a-graph) but does not create it: $u<v$ in a chosen [topological order](combinatorics.md#topological-order) does not imply a [directed path](#directed-path) from $u$ to $v$. For example, orient the two [edges](#edge-of-a-graph) of the [graph path](#path-in-a-graph) $A,B,C$ using $A<C<B$. The arrows are $A\to B$ and $C\to B$; there is no [directed path](#directed-path) from $A$ to $C$, despite $A<C$. In $D_1$, however, $A$ reaches $C$ both directly and via $B$. Following outgoing [directed edges](#directed-edge) with [graph search](graph.md#graph-search) decides this directional [reachability](graph.md#reachability-in-a-graph).[printed pp. 1–2: directed adjacency lists contain outgoing edges; a search sees vertices reachable from its start](computer-science-bibliography.md#6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-14-graphs-ii-depth-first-search)

### Strong orientation

↑ **Parent:** [Orientation of a graph](#orientation-of-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strong_orientation)

A [strong orientation](#strong-orientation) is an [orientation of a graph](#orientation-of-a-graph) with [strong connectivity](#strong-connectivity): for every ordered pair $(u,v)$ of [vertices](graph.md#vertex-graph-theory), there is a [directed path](#directed-path) from $u$ to $v$. A length-zero [directed path](#directed-path) permits $u=v$. Ordinary [connectivity](graph.md#connectivity-graph-theory) of the underlying [undirected graph](#undirected-graph) is necessary, but does not ensure this two-way [reachability](graph.md#reachability-in-a-graph) after directions are chosen. The acyclic $D_1$ is not a [strong orientation](#strong-orientation); the cyclic $D_2$ is, since a journey can continue around its [directed cycle](#directed-cycle).

Attach a new [vertex](graph.md#vertex-graph-theory) $D$ to that [triangle in a graph](graph.md#triangle-in-a-graph) by the single [edge](#edge-of-a-graph) $CD$. This [edge](#edge-of-a-graph) is a [bridge in a graph](graph.md#bridge-graph-theory). If oriented $C\to D$, no [directed path](#directed-path) leaves $D$ for the [triangle in a graph](graph.md#triangle-in-a-graph); if oriented $D\to C$, no [directed path](#directed-path) from the [triangle in a graph](graph.md#triangle-in-a-graph) reaches $D$. Neither choice gives a [strong orientation](#strong-orientation), even when the [triangle in a graph](graph.md#triangle-in-a-graph) itself is cyclically oriented. By contrast, the four-[vertex](graph.md#vertex-graph-theory) [cycle graph](#cycle-graph) has the [strong orientation](#strong-orientation)

$$
A\to B\to C\to D\to A.
$$

Following this [directed cycle](#directed-cycle) reaches any requested [vertex](graph.md#vertex-graph-theory) in at most three steps. Removing any one of its undirected [edges](#edge-of-a-graph) leaves a [graph path](#path-in-a-graph) through all four [vertices](graph.md#vertex-graph-theory), so it has no [bridge in a graph](graph.md#bridge-graph-theory).

<a id="image-a-bridge-in-a-graph-obstructs-a-strong-orientation-while-a-bridgeless-cycle-graph-admits-one"></a>
![](graph-strong-orientation-bridge-obstruction-versus-cycle.png)

**[Figure 6](#image-a-bridge-in-a-graph-obstructs-a-strong-orientation-while-a-bridgeless-cycle-graph-admits-one). A bridge in a graph obstructs a strong orientation, while a bridgeless cycle graph admits one**.

For more than one [vertex](graph.md#vertex-graph-theory), a [strong orientation](#strong-orientation) cannot also be an [acyclic orientation](#acyclic-orientation): [directed paths](#directed-path) from $u$ to $v$ and back give a nonempty [closed directed walk](#closed-directed-walk), from which removing repeated portions leaves a [directed cycle](#directed-cycle). A [directed graph](#directed-graph) containing one [directed cycle](#directed-cycle) need not have [strong connectivity](#strong-connectivity), as the attached $D$ shows.

#### Robbins' theorem

↑ **Parent:** [Strong orientation](#strong-orientation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Robbins'_theorem)

A finite nonempty [connected graph](graph.md#connected-graph) whose [edges](#edge-of-a-graph) are undirected admits a [strong orientation](#strong-orientation) if and only if it has no [bridge in a graph](graph.md#bridge-graph-theory). This statement holds for finite [multigraphs](graph.md#multigraph) as well as finite [simple graphs](graph.md#simple-graph); [self-loops](graph.md#loop-graph-theory) do not help connect distinct [vertices](graph.md#vertex-graph-theory). The single-[vertex](graph.md#vertex-graph-theory) case is allowed, with length-zero [directed paths](#directed-path).[Hassin and Megiddo, On Orientations and Shortest Paths (1989), printed pp. 591–592: bridge-connectedness, strong connectivity and Theorem 2.6 (Robbins)](mathematics-bibliography.md#on-orientations-and-shortest-paths-by-refael-hassin-and-others)

Necessity comes from the two sides separated by deleting a [bridge in a graph](graph.md#bridge-graph-theory): its chosen arrow crosses in only one direction. For sufficiency, the cited constructive proof uses [depth-first search](algorithm.md#depth-first-search) to find a [cycle in a graph](#cycle-in-a-graph), orients it cyclically, contracts it, and repeats. Undoing the contractions replaces junctions by [directed cycles](#directed-cycle), retaining two-way [reachability](graph.md#reachability-in-a-graph). Contraction can produce [multiple edges](#multiple-edges), so these must remain distinct. This is a construction outline; the input [graph](graph.md) is finite and bridgeless, and remaining [edges](#edge-of-a-graph) within contracted pieces can receive arbitrary directions.[Hassin and Megiddo (1989), Theorem 2.6 proof, printed p. 592: cycle orientation and contraction, explicitly described as a different constructive proof from Robbins's](mathematics-bibliography.md#on-orientations-and-shortest-paths-by-refael-hassin-and-others)

### Outdegree orientation criterion

↑ **Parent:** [Orientation of a graph](#orientation-of-a-graph)

A finite undirected [graph](graph.md) can be oriented with [outdegree](#outdegree) at least an integer $k\geq0$ at every vertex if and only if every vertex subset $U$ is incident to at least $k|U|$ distinct edges. The [max-flow min-cut theorem](flow-network.md#max-flow-min-cut-theorem) and [integral max-flow theorem](flow-network.md#integral-max-flow-theorem) prove sufficiency by assigning distinct edges to vertices through an incidence [flow network](flow-network.md); each assigned edge is oriented away from that vertex. Necessity follows by counting outgoing edges from $U$.

## Graph intersection

↑ **Parent:** [Graph theory](graph-theory.md)

For two [graphs](graph.md) on the same [vertex set](graph.md#vertex-set), their graph intersection retains exactly the [edges](#edge-of-a-graph) belonging to both.

## Kneser graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kneser_graph)

The Kneser graph has as [vertices](graph.md#vertex-graph-theory) the $k$-element subsets of $[n]$, with an [edge](#edge-of-a-graph) between two exactly when they are disjoint. A [graph colouring](graph-coloring.md) of this [graph](graph.md) partitions the $k$-sets into [intersecting families](extremal-set-theory.md#intersecting-family).

<h3 id="lovasz-theorem-on-kneser-graphs">Lovász theorem on Kneser graphs</h3>

↑ **Parent:** [Kneser graph](#kneser-graph)

For integers $n\geq2k\geq2$, the [chromatic number](graph-coloring.md#chromatic-number) of the [Kneser graph](#kneser-graph) is $n-2k+2$. The upper bound colours by the least element among the first $n-2k+1$ elements, with one final colour for all other sets. The [Gale hemisphere lemma](euclidean-geometry.md#gale-hemisphere-lemma) and the [Lusternik-Schnirelmann-Borsuk theorem](algebraic-topology.md#lusternik-schnirelmann-theorem) give the matching lower bound.

## Cut vertex

↑ **Parent:** [Graph theory](graph-theory.md)

A [cut vertex](#cut-vertex), also called an [articulation point](#cut-vertex), is a [vertex](graph.md#vertex-graph-theory) $v$ of an [undirected graph](#undirected-graph) whose deletion increases the number of [connected components of a graph](graph.md#component-graph-theory). Write $k(G)$ for that count, including isolated [vertices](graph.md#vertex-graph-theory), and $G-v$ for the [graph](graph.md) obtained by removing $v$ and every incident [edge](#edge-of-a-graph). Then the test is $k(G-v)>k(G)$, even when the original [graph](graph.md) is disconnected. By contrast, deleting a [bridge in a graph](graph.md#bridge-graph-theory) removes just one [edge](#edge-of-a-graph) and keeps both endpoint [vertices](graph.md#vertex-graph-theory). These are different failure models. [Sedgewick and Wayne, Algorithms, §4.1: bridges and articulation points](https://algs4.cs.princeton.edu/41graph/)

First take two [triangles in a graph](graph.md#triangle-in-a-graph), $ABC$ and $ADE$, sharing only the [vertex](graph.md#vertex-graph-theory) $A$. This [simple graph](graph.md#simple-graph) has

$$
V=\{A,B,C,D,E\},\qquad E=\{AB,AC,BC,AD,AE,DE\}.
$$

Here $XY$ abbreviates the [unordered pair](set.md#unordered-pair) $\{X,Y\}$. Removing $A$ leaves the two [connected components of a graph](graph.md#component-graph-theory) $\{B,C\}$ and $\{D,E\}$, so $k(G-A)=2>1=k(G)$. Removing any other [vertex](graph.md#vertex-graph-theory) leaves a [connected graph](graph.md#connected-graph). Thus $A$ is the only [cut vertex](#cut-vertex). Every [edge](#edge-of-a-graph) lies on a [triangle in a graph](graph.md#triangle-in-a-graph), so deleting any single [edge](#edge-of-a-graph) still leaves a [graph path](#path-in-a-graph) between its endpoints along the other two [edges](#edge-of-a-graph). There are no [bridges in a graph](graph.md#bridge-graph-theory).

<a id="image-two-triangles-in-a-graph-share-a-cut-vertex-a-although-no-edge-is-a-bridge-in-a-graph"></a>
![](articulation-without-bridges.png)

**[Figure 7](#image-two-triangles-in-a-graph-share-a-cut-vertex-a-although-no-edge-is-a-bridge-in-a-graph). Two triangles in a graph share a cut vertex $A$, although no edge is a bridge in a graph**.

The generator computes the [adjacency lists](data-structure.md#adjacency-list) and checks every [vertex](graph.md#vertex-graph-theory) deletion, giving the following complete table:

| Deleted [vertex](graph.md#vertex-graph-theory) $v$ | Original [graph neighbours](#neighbour-of-a-vertex) of $v$ | $k(G-v)$ |
| --- | --- | --- |
| $A$ | $B,C,D,E$ | $2$ |
| $B$ | $A,C$ | $1$ |
| $C$ | $A,B$ | $1$ |
| $D$ | $A,E$ | $1$ |
| $E$ | $A,D$ | $1$ |

Now take two disjoint [triangles in a graph](graph.md#triangle-in-a-graph), $ABC$ and $DEF$, joined by the [edge](#edge-of-a-graph) $CD$:

$$
V=\{A,B,C,D,E,F\},\qquad E=\{AB,AC,BC,CD,DE,DF,EF\}.
$$

Deleting only $CD$ preserves all six [vertices](graph.md#vertex-graph-theory) and leaves [connected components of a graph](graph.md#component-graph-theory) $\{A,B,C\}$ and $\{D,E,F\}$: $CD$ is the only [bridge in a graph](graph.md#bridge-graph-theory). Deleting $C$ also removes $AC$ and $BC$, leaving [connected components of a graph](graph.md#component-graph-theory) $\{A,B\}$ and $\{D,E,F\}$. Deleting $D$ instead leaves $\{A,B,C\}$ and $\{E,F\}$. Thus $C,D$ are exactly the [cut vertices](#cut-vertex).

<a id="image-edge-deletion-keeps-its-endpoints-cut-vertex-deletion-removes-all-incident-edges"></a>
![](graph-articulation-versus-bridge.png)

**[Figure 8](#image-edge-deletion-keeps-its-endpoints-cut-vertex-deletion-removes-all-incident-edges). Edge deletion keeps its endpoints; cut vertex deletion removes all incident edges**.

Again the [adjacency lists](data-structure.md#adjacency-list) and all [vertex](graph.md#vertex-graph-theory) deletion counts are computed directly:

| Deleted [vertex](graph.md#vertex-graph-theory) $v$ | Original [graph neighbours](#neighbour-of-a-vertex) of $v$ | $k(G-v)$ |
| --- | --- | --- |
| $A$ | $B,C$ | $1$ |
| $B$ | $A,C$ | $1$ |
| $C$ | $A,B,D$ | $2$ |
| $D$ | $C,E,F$ | $2$ |
| $E$ | $D,F$ | $1$ |
| $F$ | $D,E$ | $1$ |

For a disconnected example, adjoin an isolated [vertex](graph.md#vertex-graph-theory) $Z$ to the first [graph](graph.md). Now $k(G)=2$, deleting $A$ gives $k(G-A)=3$, and deleting $Z$ gives $k(G-Z)=1$. The original [graph](graph.md) was already disconnected, but $A$ is still a [cut vertex](#cut-vertex); $Z$ is not. The empty [graph](graph.md) has count zero, so deleting the only [vertex](graph.md#vertex-graph-theory) of a one-[vertex](graph.md#vertex-graph-theory) [graph](graph.md) does not create a [cut vertex](#cut-vertex). Nor is either endpoint of a single isolated [edge](#edge-of-a-graph) a [cut vertex](#cut-vertex), although that [edge](#edge-of-a-graph) is a [bridge in a graph](graph.md#bridge-graph-theory).

In a communications network, a [cut vertex](#cut-vertex) models a router whose failure separates surviving routers. The shared-$A$ example shows why having an alternative [graph path](#path-in-a-graph) around each individual [edge](#edge-of-a-graph) does not protect against failure of the common router. An additional [edge](#edge-of-a-graph) from $B$ to $D$ removes this particular vulnerability: after deleting $A$, $B,D$ still join the two sides. A [bridge in a graph](graph.md#bridge-graph-theory) instead models a vulnerable link. This distinction tells us whether to add another cable between existing devices or a route avoiding an indispensable device; it describes [connectivity](graph.md#connectivity-graph-theory), rather than traffic capacity or failure probabilities.

The beautiful structural consequence is that a [graph](graph.md) splits into [biconnected components](#biconnected-component) joined at [cut vertices](#cut-vertex). Within each nontrivial robust piece, a single [vertex](graph.md#vertex-graph-theory) failure cannot separate the other [vertices](graph.md#vertex-graph-theory); between pieces, the shared [cut vertices](#cut-vertex) reveal the bottlenecks. Also, a [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) [graph](graph.md) has no [cut vertex](#cut-vertex): deleting any [vertex](graph.md#vertex-graph-theory) from its [Hamilton cycle](#hamilton-cycle) leaves a [Hamiltonian path](#hamiltonian-path) through all remaining [vertices](graph.md#vertex-graph-theory).

Historically, Tarjan's June 1972 paper developed [depth-first search](algorithm.md#depth-first-search) as a tool for finding [biconnected components](#biconnected-component) in time linear in the numbers of [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph). [Robert Tarjan, Depth-First Search and Linear Graph Algorithms, SIAM Journal on Computing 1(2), 146–160 (1972)](https://epubs.siam.org/doi/10.1137/0201010) In his 1983 recollection, Tarjan credited Hopcroft with the original linear-time [biconnected component](#biconnected-component) [algorithm](algorithm.md) during their collaboration beginning in summer 1970, and described the published version as a refinement. The historical lesson is how a carefully organized traversal turns many separate deletion experiments into one computation. [Robert E. Tarjan, Citation Classic recollection (1983)](https://garfield.library.upenn.edu/classics1983/A1983QY47200001.pdf)

### Biconnected component

↑ **Parent:** [Cut vertex](#cut-vertex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Biconnected_component)

A [biconnected component](#biconnected-component) is a maximal connected [subgraph](#subgraph) with no [cut vertex](#cut-vertex) of its own. We use the block convention that also includes each [bridge in a graph](graph.md#bridge-graph-theory) with its two endpoint [vertices](graph.md#vertex-graph-theory), and each isolated [vertex](graph.md#vertex-graph-theory), as a [biconnected component](#biconnected-component). A [biconnected component](#biconnected-component) with at least three [vertices](graph.md#vertex-graph-theory) stays connected after any single [vertex](graph.md#vertex-graph-theory) deletion. Distinct [biconnected components](#biconnected-component) share at most one [vertex](graph.md#vertex-graph-theory); the [vertices](graph.md#vertex-graph-theory) belonging to more than one [biconnected component](#biconnected-component) are exactly the [cut vertices](#cut-vertex). The shared-$A$ example has two [biconnected components](#biconnected-component), its two [triangles in a graph](graph.md#triangle-in-a-graph). The joined-$CD$ example has three: $ABC$, the [bridge in a graph](graph.md#bridge-graph-theory) $CD$ with its endpoints, and $DEF$. The [edges](#edge-of-a-graph) partition into these pieces, while the shared [cut vertices](#cut-vertex) occur in several pieces. [Sedgewick and Wayne, Algorithms, §4.1, biconnected components exercises](https://algs4.cs.princeton.edu/41graph/)

### DFS discovery time

↑ **Parent:** [Cut vertex](#cut-vertex)

The [DFS discovery time](#dfs-discovery-time) of a [vertex](graph.md#vertex-graph-theory) is its first-visit number in [depth-first search](algorithm.md#depth-first-search), assigned by an increasing counter. Discovery [edges](#edge-of-a-graph) form a [rooted tree](tree-graph-theory.md#rooted-tree) in each [connected component of a graph](graph.md#component-graph-theory). For the joined-$CD$ example, starting at $A$ and visiting [graph neighbours](#neighbour-of-a-vertex) in [lexicographic order](extremal-set-theory.md#lexicographic-order) gives first visits $A,B,C,D,E,F$, numbered $1,2,3,4,5,6$; its discovery [edges](#edge-of-a-graph) are $AB,BC,CD,DE,EF$. These numbers encode the chosen traversal, not an invariant of the [graph](graph.md).

### DFS lowpoint

↑ **Parent:** [Cut vertex](#cut-vertex)

For a finite [simple graph](graph.md#simple-graph) that is an [undirected graph](#undirected-graph), the [DFS lowpoint](#dfs-lowpoint) of $v$ is the smallest [DFS discovery time](#dfs-discovery-time) reachable by following zero or more discovery [edges](#edge-of-a-graph) down its [rooted tree](tree-graph-theory.md#rooted-tree), then at most one non-discovery [edge](#edge-of-a-graph) to an ancestor. Staying at $v$ is allowed. Ignore the reverse traversal of the discovery [edge](#edge-of-a-graph) to the [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree): it is the same [edge](#edge-of-a-graph), not an escape route. Start with $\operatorname{low}(v)=\operatorname{disc}(v)$. On returning from a [child in a rooted tree](tree-graph-theory.md#child-in-a-rooted-tree) $w$, replace $\operatorname{low}(v)$ by $\min\{\operatorname{low}(v),\operatorname{low}(w)\}$. For a non-discovery [edge](#edge-of-a-graph) from $v$ to an earlier ancestor $a$, replace it by $\min\{\operatorname{low}(v),\operatorname{disc}(a)\}$. This summarizes how far upward the explored branch can reconnect. [Tarjan (1972), §3, LOWPT recurrence, pp. 151–153](https://sites.cs.ucsb.edu/~gilbert/cs240a/notes/TarjanDFS.pdf)

The [cut vertex](#cut-vertex) criterion has a separate case for each [root of a tree](tree-graph-theory.md#root-of-a-tree) in the discovery [forest](tree-graph-theory.md#forest):
- A nonroot [vertex](graph.md#vertex-graph-theory) $u$ is a [cut vertex](#cut-vertex) exactly when some [child in a rooted tree](tree-graph-theory.md#child-in-a-rooted-tree) $w$ satisfies $\operatorname{low}(w)\geq\operatorname{disc}(u)$.
- A [root of a tree](tree-graph-theory.md#root-of-a-tree) is a [cut vertex](#cut-vertex) exactly when it has at least two [children in a rooted tree](tree-graph-theory.md#child-in-a-rooted-tree), counting discovery [edges](#edge-of-a-graph), rather than all [graph neighbours](#neighbour-of-a-vertex).
- A discovery [edge](#edge-of-a-graph) $uw$ is a [bridge in a graph](graph.md#bridge-graph-theory) exactly when $\operatorname{low}(w)>\operatorname{disc}(u)$. A non-discovery [edge](#edge-of-a-graph) is never a [bridge in a graph](graph.md#bridge-graph-theory).

Why does equality matter? If $\operatorname{low}(w)=\operatorname{disc}(u)$, the branch below $w$ can reconnect to $u$, so the discovery [edge](#edge-of-a-graph) $uw$ lies on a [graph cycle](#cycle-in-a-graph) and is not a [bridge in a graph](graph.md#bridge-graph-theory). Deleting the [vertex](graph.md#vertex-graph-theory) $u$ destroys that reconnection too. If $u$ has a [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree), the branch is then separated from that [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree), explaining the non-strict [cut vertex](#cut-vertex) test. For a [root of a tree](tree-graph-theory.md#root-of-a-tree), there is no earlier side to separate from; distinct discovery branches cannot have an [edge](#edge-of-a-graph) between them, since [depth-first search](algorithm.md#depth-first-search) would have explored them as one branch. This gives the two-[children in a rooted tree](tree-graph-theory.md#child-in-a-rooted-tree) rule. These are proof outlines of the criteria. [Sedgewick and Wayne, Biconnected.java: discovery, lowpoint and root tests](https://algs4.cs.princeton.edu/41graph/Biconnected.java.html)[Sedgewick and Wayne, Algorithms, §4.1: bridge detection](https://algs4.cs.princeton.edu/41graph/)

In the joined-$CD$ example with [DFS discovery times](#dfs-discovery-time) $1,2,3,4,5,6$, the [DFS lowpoints](#dfs-lowpoint) in label order are $1,1,1,4,4,4$. For $C$ and its [child in a rooted tree](tree-graph-theory.md#child-in-a-rooted-tree) $D$, $4>3$: $CD$ is a [bridge in a graph](graph.md#bridge-graph-theory), and $C$ is a [cut vertex](#cut-vertex). For $D$ and its [child in a rooted tree](tree-graph-theory.md#child-in-a-rooted-tree) $E$, $4=4$: $D$ is a [cut vertex](#cut-vertex), although $DE$ is not a [bridge in a graph](graph.md#bridge-graph-theory). The [root of a tree](tree-graph-theory.md#root-of-a-tree) $A$ has only one [child in a rooted tree](tree-graph-theory.md#child-in-a-rooted-tree), $B$, so it is not a [cut vertex](#cut-vertex). In the shared-$A$ example, the [root of a tree](tree-graph-theory.md#root-of-a-tree) $A$ has two [children in a rooted tree](tree-graph-theory.md#child-in-a-rooted-tree), $B$ and $D$, and is a [cut vertex](#cut-vertex), while every [DFS lowpoint](#dfs-lowpoint) is $1$ and no [edge](#edge-of-a-graph) passes the strict [bridge in a graph](graph.md#bridge-graph-theory) test.

Restart [depth-first search](algorithm.md#depth-first-search) at every undiscovered [vertex](graph.md#vertex-graph-theory) to cover a disconnected [graph](graph.md), applying the [root of a tree](tree-graph-theory.md#root-of-a-tree) rule separately in each [connected component of a graph](graph.md#component-graph-theory). With [adjacency lists](data-structure.md#adjacency-list) and constant-cost label operations, computing all [DFS lowpoints](#dfs-lowpoint), [cut vertices](#cut-vertex) and [bridges in a graph](graph.md#bridge-graph-theory) has [time complexity](theoretical-computer-science.md#time-complexity) $O(|V|+|E|)$ in [Big O notation](real-analysis.md#big-o-notation), because each [vertex](graph.md#vertex-graph-theory) is discovered once and each [edge](#edge-of-a-graph) is inspected twice. The simple parent-skipping rule assumes a [simple graph](graph.md#simple-graph). In a [multigraph](graph.md#multigraph), skip only the actual parent [edge](#edge-of-a-graph), identified individually: a parallel [edge](#edge-of-a-graph) to the same [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree) is a valid reconnection and can prevent the first [edge](#edge-of-a-graph) from being a [bridge in a graph](graph.md#bridge-graph-theory). The criteria here concern [undirected graphs](#undirected-graph); a [directed graph](#directed-graph) requires a different connectivity analysis.

## Hypergraph

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](hypergraph.md)

## Walk in a graph

↑ **Parent:** [Graph theory](graph-theory.md)

A [walk](#walk-in-a-graph) records a journey through a [graph](graph.md) as a finite alternating [sequence](sequence-and-series.md#sequence)

$$
W=(v_0,e_1,v_1,\ldots,e_m,v_m),\qquad m\geq0,
$$

where each [edge](#edge-of-a-graph) $e_i$ joins the consecutive [vertices](graph.md#vertex-graph-theory) $v_{i-1}$ and $v_i$. Both [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph) may repeat. Its length is $m$, counting [edge](#edge-of-a-graph) traversals with repetitions, rather than counting different [edges](#edge-of-a-graph) or measuring the drawing. Here a [graph path](#path-in-a-graph) means a [walk](#walk-in-a-graph) with no repeated [vertices](graph.md#vertex-graph-theory); a [trail](#trail-in-a-graph) instead forbids repeated [edges](#edge-of-a-graph). These conventions distinguish a journey's record from the [subgraph](#subgraph) consisting of the connections it used.[Paul Johnson, MAS341, Lecture 3: walks and trails](https://ptwiddle.github.io/MAS341-Graph-Theory-2017/lecturenotes/lecture3.html)

Unless stated otherwise, the examples below use a finite [simple graph](graph.md#simple-graph) that is an [undirected graph](#undirected-graph), so an [edge](#edge-of-a-graph) may be traversed in either direction. In a [multigraph](graph.md#multigraph), retain each [edge](#edge-of-a-graph)'s individual identity as well as its endpoint [vertices](graph.md#vertex-graph-theory): two parallel [edges](#edge-of-a-graph) are different choices for the same step. If [self-loops](graph.md#loop-graph-theory) are allowed, traversing one leaves the current [vertex](graph.md#vertex-graph-theory) unchanged but adds one to the length. In a [directed graph](#directed-graph), each step must follow its [directed edge](#directed-edge) from its initial to its terminal [vertex](graph.md#vertex-graph-theory), giving a [directed walk](#directed-walk); reversing a journey need not be possible.[Thomas Zaslavsky, Supplementary Notes for Graduate Graph Theory: edge identities and walks](https://people.math.binghamton.edu/zaslav/Oldcourses/581.S99/notes.html)

We allow the zero-length [walk](#walk-in-a-graph) $(v)$ at every [vertex](graph.md#vertex-graph-theory) $v$. It uses no [edges](#edge-of-a-graph), so it is also a [trail](#trail-in-a-graph) and a [graph path](#path-in-a-graph), and its coinciding endpoints make it a [closed walk](#closed-walk). This means staying put is a legitimate journey; a [graph](graph.md) with no [vertices](graph.md#vertex-graph-theory) has no such [walk](#walk-in-a-graph). Positive-length restrictions will be stated explicitly.[Lehman, Leighton and Meyer, Mathematics for Computer Science, §11.8.1: length-zero convention](mathematics-bibliography.md#mathematics-for-computer-science-by-eric-lehman-and-others)

Use the same constructed [graph](graph.md) throughout these three sections:

$$
V=\{A,B,C,D,E,F\},\qquad E=\{AB,BC,CA,AD,DE,EA,AF\}.
$$

Here $AB$ denotes the [unordered pair](set.md#unordered-pair) $\{A,B\}$, and $CA=AC$. Two [triangles in a graph](graph.md#triangle-in-a-graph), $ABC$ and $ADE$, share $A$, with one extra [edge](#edge-of-a-graph) $AF$. These are schematic connections, not measured roads; the highlighted connections in the diagram show which [edges](#edge-of-a-graph) are used, while the numbered [sequence](sequence-and-series.md#sequence) records their order.

<a id="image-one-constructed-graph-repeated-edges-in-a-walk-repeated-vertices-in-a-trail-and-a-graph-path"></a>
![](walks-trails-closed-walks-route-comparison.png)

**[Figure 9](#image-one-constructed-graph-repeated-edges-in-a-walk-repeated-vertices-in-a-trail-and-a-graph-path). One constructed graph: repeated edges in a walk, repeated vertices in a trail, and a graph path**.

The length-six [walk](#walk-in-a-graph) $B,C,A,B,C,A,F$ uses $BC$ and $CA$ twice, so it is not a [trail](#trail-in-a-graph). The length-six [trail](#trail-in-a-graph) $B,C,A,D,E,A,F$ returns to $A$ but uses six different [edges](#edge-of-a-graph), so it is not a [graph path](#path-in-a-graph). The length-three [graph path](#path-in-a-graph) $B,C,A,F$ repeats neither [vertices](graph.md#vertex-graph-theory) nor [edges](#edge-of-a-graph). Thus

$$
\{\text{graph paths}\}\subsetneq\{\text{trails}\}\subsetneq\{\text{walks}\}
$$

for this particular [graph](graph.md). The restrictions answer different routing questions: revisiting a junction is harmless for many journeys, whereas reusing a serviced road segment can matter for an inspection route. Travel costs require a [weighted graph](random-walk.md#weighted-graph); a [walk](#walk-in-a-graph)'s cost adds the weight of each traversal, even when an [edge](#edge-of-a-graph) is used again.

Every finite [walk](#walk-in-a-graph) from $s$ to $t$ contains a [graph path](#path-in-a-graph) from $s$ to $t$ after deleting detours. For a proof outline, if $v_i=v_j$ with $i<j$, delete the intervening [closed walk](#closed-walk). The retained steps still meet at the same [vertex](graph.md#vertex-graph-theory), and the length strictly decreases. Repeating terminates with no repeated [vertices](graph.md#vertex-graph-theory), or with the zero-length [graph path](#path-in-a-graph) when $s=t$. This explains why [reachability](graph.md#reachability-in-a-graph) can be formulated using either [walks](#walk-in-a-graph) or [graph paths](#path-in-a-graph). With nonnegative [edge](#edge-of-a-graph) weights, deletion also cannot increase cost, connecting the argument to the [shortest path problem](shortest-path-problem.md); with negative weights that cost conclusion fails.[Paul Johnson, MAS341, Lecture 3: deleting repeated-vertex detours](https://ptwiddle.github.io/MAS341-Graph-Theory-2017/lecturenotes/lecture3.html)

### Trail in a graph

↑ **Parent:** [Walk in a graph](#walk-in-a-graph)

A [trail](#trail-in-a-graph) is a [walk](#walk-in-a-graph) whose [edge](#edge-of-a-graph) [sequence](sequence-and-series.md#sequence) $e_1,\ldots,e_m$ has no repetitions. Its [vertices](graph.md#vertex-graph-theory) may repeat, including its first and last [vertices](graph.md#vertex-graph-theory). The zero-length [walk](#walk-in-a-graph) is a [trail](#trail-in-a-graph) because it repeats no [edge](#edge-of-a-graph). Every [graph path](#path-in-a-graph) is a [trail](#trail-in-a-graph), but the converse fails: the [trail](#trail-in-a-graph) in the shared example is

$$
B,BC,C,CA,A,AD,D,DE,E,EA,A,AF,F.
$$

Its six [edges](#edge-of-a-graph) $BC,CA,AD,DE,EA,AF$ are pairwise distinct, although $A$ occurs twice. Visiting a junction again and traversing a road segment again are different events.[Thomas Zaslavsky, Supplementary Notes for Graduate Graph Theory: trails and paths](https://people.math.binghamton.edu/zaslav/Oldcourses/581.S99/notes.html)

In an [undirected graph](#undirected-graph), traversing $AB$ and then $BA$ repeats the same [edge](#edge-of-a-graph); direction of travel does not give it a new identity. In a [multigraph](graph.md#multigraph) with distinct parallel [edges](#edge-of-a-graph) $p,q$ joining $X$ and $Y$, the [closed walk](#closed-walk) $(X,p,Y,q,X)$ is a [trail](#trail-in-a-graph), whereas $(X,p,Y,p,X)$ is not. Both have the same [vertex](graph.md#vertex-graph-theory) [sequence](sequence-and-series.md#sequence) $X,Y,X$. In a [directed graph](#directed-graph), separate [directed edges](#directed-edge) $X\to Y$ and $Y\to X$ may instead be used once each; record their identities and obey their directions. Thus testing a [trail](#trail-in-a-graph) means checking the actual [edge](#edge-of-a-graph) records, not merely checking consecutive endpoint labels.

For a finite [graph](graph.md), a [trail](#trail-in-a-graph) has length at most $|E|$; unrestricted [walks](#walk-in-a-graph) can have arbitrarily large length whenever a positive-length [closed walk](#closed-walk) exists, since it can be repeated. An [Eulerian trail](#eulerian-trail) is the special [trail](#trail-in-a-graph) that uses every [edge](#edge-of-a-graph), so its length is exactly $|E|$. Our length-six [trail](#trail-in-a-graph) omits $AB$ and is therefore not an [Eulerian trail](#eulerian-trail). In a road-inspection model, a [trail](#trail-in-a-graph) describes servicing its selected segments once while allowing returns to junctions; requiring service of every segment leads to the [Eulerian trail](#eulerian-trail) question. If extra travel between serviced segments is necessary, the complete journey can be a [walk](#walk-in-a-graph) even when each segment is serviced only once. This distinction keeps the service requirement separate from the route actually travelled.

### Closed walk

↑ **Parent:** [Walk in a graph](#walk-in-a-graph)

A [closed walk](#closed-walk) is a [walk](#walk-in-a-graph) with equal endpoint [vertices](graph.md#vertex-graph-theory), $v_m=v_0$. Under our convention this includes the zero-length [walk](#walk-in-a-graph) $(v)$; returning after traversing at least one [edge](#edge-of-a-graph) requires $m>0$. Closure imposes no other restriction on repeated [vertices](graph.md#vertex-graph-theory) or [edges](#edge-of-a-graph). In a [directed graph](#directed-graph), a [closed directed walk](#closed-directed-walk) must also follow every [directed edge](#directed-edge) in its permitted direction.[Lehman, Leighton and Meyer, Mathematics for Computer Science, §§9.2 and 11.8.1: closed walks](mathematics-bibliography.md#mathematics-for-computer-science-by-eric-lehman-and-others)

<a id="image-returning-to-a-backtracking-closed-walk-closed-trail-with-a-repeated-internal-vertex-and-graph-cycle"></a>
![](walks-trails-closed-walks-return-comparison.png)

**[Figure 10](#image-returning-to-a-backtracking-closed-walk-closed-trail-with-a-repeated-internal-vertex-and-graph-cycle). Returning to $A$: backtracking closed walk, closed trail with a repeated internal vertex, and graph cycle**.

In the shared [simple graph](graph.md#simple-graph), $A,F,A$ is a length-two [closed walk](#closed-walk) that immediately backtracks along $AF$. It is not a [trail](#trail-in-a-graph), since $AF$ is used twice, and it is not a [graph cycle](#cycle-in-a-graph). The length-six [closed walk](#closed-walk) $A,B,C,A,D,E,A$ is a [trail](#trail-in-a-graph), since its six [edges](#edge-of-a-graph) are distinct, but is not a [graph cycle](#cycle-in-a-graph): it returns to $A$ midway through the journey. The length-three [closed walk](#closed-walk) $A,B,C,A$ is a [graph cycle](#cycle-in-a-graph), with all [vertices](graph.md#vertex-graph-theory) distinct apart from the required endpoint repetition. In a [simple graph](graph.md#simple-graph) that is an [undirected graph](#undirected-graph), a [graph cycle](#cycle-in-a-graph) has length at least three; the two-step backtrack is excluded.[Lehman, Leighton and Meyer, Mathematics for Computer Science, §11.8.1: cycles and backtracking](mathematics-bibliography.md#mathematics-for-computer-science-by-eric-lehman-and-others)

A positive-length [closed walk](#closed-walk) therefore need not reveal a [graph cycle](#cycle-in-a-graph): even a [tree](tree-graph-theory.md) permits an out-and-back journey on an [edge](#edge-of-a-graph). A positive-length closed [trail](#trail-in-a-graph) in a [simple graph](graph.md#simple-graph) does contain a [graph cycle](#cycle-in-a-graph). For a proof outline, choose a shortest positive-length consecutive portion of the [trail](#trail-in-a-graph) whose endpoint [vertices](graph.md#vertex-graph-theory) coincide. It cannot repeat an internal [vertex](graph.md#vertex-graph-theory), since that would give a shorter such portion; it cannot have length one or two because [self-loops](graph.md#loop-graph-theory) and repeated [edges](#edge-of-a-graph) are excluded. It is consequently a [graph cycle](#cycle-in-a-graph). Cutting it out leaves another closed [trail](#trail-in-a-graph), possibly of length zero, so repetition partitions the original [edges](#edge-of-a-graph) into [graph cycles](#cycle-in-a-graph). In our six-step example these are the two [triangles in a graph](graph.md#triangle-in-a-graph). A closed [trail](#trail-in-a-graph) using every [edge](#edge-of-a-graph) would be an [Euler circuit](#euler-circuit); here $AF$ is omitted.

Counting return journeys makes [closed walks](#closed-walk) useful even when they repeat [edges](#edge-of-a-graph). For a finite [simple graph](graph.md#simple-graph) with [adjacency matrix](#adjacency-matrix) $M$, the [walk count from powers of an adjacency matrix](#walk-count-from-powers-of-an-adjacency-matrix) gives $(M^k)_{uv}$ length-$k$ [walks](#walk-in-a-graph) from $u$ to $v$, for every [nonnegative integer](arithmetic.md#natural-number) $k$. A proof outline is that [matrix multiplication](vector-space.md#matrix-multiplication) appends one allowed step, summing over the previous endpoint; $M^0$ is the [identity matrix](vector-space.md#identity-matrix), recording the unique zero-length [walk](#walk-in-a-graph) at each [vertex](graph.md#vertex-graph-theory). Consequently

$$
(M^k)_{vv}=\#\{\text{length-}k\text{ closed walks starting at }v\},\qquad \operatorname{tr}(M^k)=\sum_{v\in V}(M^k)_{vv}.
$$

The [trace](linear-algebra.md#matrix-trace) counts [closed walks](#closed-walk) with a specified starting [vertex](graph.md#vertex-graph-theory) and traversal order, not distinct [graph cycles](#cycle-in-a-graph). These formulas use adjacency entries, not arbitrary travel costs in a [weighted graph](random-walk.md#weighted-graph).[Alexander Wolitzky, Graph Theory and Social Networks, slides 9–10: powers of adjacency matrices](https://ocw.mit.edu/courses/14-15-networks-spring-2022/mit14_15s22_lec2.pdf)

In our example, $(M^2)_{AA}=5$: the five length-two [closed walks](#closed-walk) are $A,B,A$, $A,C,A$, $A,D,A$, $A,E,A$, and $A,F,A$. Also $(M^3)_{AA}=4$, going round either [triangle in a graph](graph.md#triangle-in-a-graph) in either direction, and $\operatorname{tr}(M^3)=12$: each of the two [triangles in a graph](graph.md#triangle-in-a-graph) supplies three choices of starting [vertex](graph.md#vertex-graph-theory) and two directions. These exact counts for the constructed [graph](graph.md) illustrate why return counts and [graph cycle](#cycle-in-a-graph) counts differ.

A [closed walk](#closed-walk) naturally models a delivery or inspection journey that returns to its depot. Repeated [vertices](graph.md#vertex-graph-theory) let it combine several excursions; repeated [edges](#edge-of-a-graph) let it serve a dead end and return. For an [Euclidean travelling salesman tour](mathematical-optimization.md#euclidean-travelling-salesman-tour), one can first construct a [closed walk](#closed-walk) visiting all locations and then use the [triangle inequality](topological-analysis.md#triangle-inequality) to shortcut repeated visits without increasing total length. That argument assumes direct travel between the retained locations is permitted, as in a [complete graph](#complete-graph) weighted by [Euclidean distance](topological-analysis.md#euclidean-distance); an arbitrary road network need not contain those shortcut [edges](#edge-of-a-graph).

## Undirected graph

↑ **Parent:** [Graph theory](graph-theory.md)

An undirected [graph](graph.md) has edges that are unordered pairs of vertices. In a simple undirected graph there are no loops or multiple edges. The [skeleton of a directed graph](#skeleton-of-a-directed-graph) forgets the directions of its edges and is an undirected graph.

### Multiple edges

↑ **Parent:** [Undirected graph](#undirected-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiple_edges)

[Multiple edges](#multiple-edges) are distinct [edges](#edge-of-a-graph) with the same pair of endpoint [vertices](graph.md#vertex-graph-theory) in an [undirected graph](#undirected-graph). A [multigraph](graph.md#multigraph) permits them; a [simple graph](graph.md#simple-graph) does not. In an [orientation of a graph](#orientation-of-a-graph) of a [multigraph](graph.md#multigraph), each such [edge](#edge-of-a-graph) receives its own direction, so two of them can supply opposite [directed edges](#directed-edge) between the same [vertices](graph.md#vertex-graph-theory).

## Graph minor

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](graph-minor.md)

## Vertex cover

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vertex_cover)

A [vertex cover](#vertex-cover) chooses [vertices](graph.md#vertex-graph-theory) that collectively touch every [edge](#edge-of-a-graph) of a [graph](graph.md). Think of placing monitors at junctions: if a monitor watches every connection incident to its junction, a [vertex cover](#vertex-cover) watches all connections. The [minimum vertex cover](#minimum-vertex-cover) asks how few monitors suffice. This is a model of covering connections through their endpoints, rather than of monitoring distances in the drawing.

For a finite [simple graph](graph.md#simple-graph) $G=(V,E)$, a [vertex cover](#vertex-cover) is a [subset](set.md#subset) $C\subseteq V$ satisfying

$$
\{u,v\}\in E\Longrightarrow u\in C\ \text{or}\ v\in C.
$$

Both endpoints may be selected; the condition requires at least one. An [isolated vertex](random-graph.md#isolated-vertex) covers no [edge](#edge-of-a-graph), so a [minimum vertex cover](#minimum-vertex-cover) never needs it.[Diestel, Graph Theory, fourth electronic edition, Section 2.1, definition of vertex cover](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

Take the [cycle graph](#cycle-graph) $C_5$ with [vertices](graph.md#vertex-graph-theory) $0,1,2,3,4$ and [edges](#edge-of-a-graph) $01,12,23,34,40$. The [set](set.md) $C=\{1,3,4\}$ is a [vertex cover](#vertex-cover): [vertex](graph.md#vertex-graph-theory) $1$ covers $01$ and $12$, [vertex](graph.md#vertex-graph-theory) $3$ covers $23$ and $34$, and [vertex](graph.md#vertex-graph-theory) $4$ covers $40$ as well as $34$. In particular, the closing [edge](#edge-of-a-graph) $40$ is covered even though [vertex](graph.md#vertex-graph-theory) $0$ is unselected.

The unselected [vertices](graph.md#vertex-graph-theory) $I=V\setminus C=\{0,2\}$ form an [independent set](#independent-set-graph-theory). This is the key connection: an [edge](#edge-of-a-graph) missed by $C$ would have both endpoints in $I$, precisely what an [independent set](#independent-set-graph-theory) forbids. For every [subset](set.md#subset) $C\subseteq V$,

$$
C\text{ is a vertex cover}\quad\Longleftrightarrow\quad V\setminus C\text{ is an independent set}.
$$

Here $V\setminus C$ is the [complement of a set](set.md#complement-of-a-set) within $V$; the [graph](graph.md) itself keeps all its [edges](#edge-of-a-graph). The [complement graph](#complement-graph) is a different construction.[Barak, Introduction to Theoretical Computer Science, Chapter 14, vertex-cover exercise](https://introtcs.org/public/lec_12_NP.html)

<a id="image-a-minimum-vertex-cover-and-its-maximum-independent-complement-on-the-same-five-cycle"></a>
![](vertex-cover-independent-complement.png)

**[Figure 11](#image-a-minimum-vertex-cover-and-its-maximum-independent-complement-on-the-same-five-cycle). A minimum vertex cover and its maximum independent complement on the same five-cycle**.

The endpoints of any [maximal matching](matching-graph-theory.md#maximal-matching) form a [vertex cover](#vertex-cover): an [edge](#edge-of-a-graph) avoiding all endpoints would enlarge that [matching in a graph](matching-graph-theory.md). Consequently a [graph](graph.md) with no [matching in a graph](matching-graph-theory.md) of size $s$ has a [vertex cover](#vertex-cover) of size at most $2(s-1)$. This supplies a convenient [vertex cover](#vertex-cover), but it need not be a [minimum vertex cover](#minimum-vertex-cover).

### Minimum vertex cover

↑ **Parent:** [Vertex cover](#vertex-cover)

A [minimum vertex cover](#minimum-vertex-cover) is a [vertex cover](#vertex-cover) of smallest [cardinality](cardinal-number.md#cardinality) among all [vertex covers](#vertex-cover) of the same finite [simple graph](graph.md#simple-graph). The optimum size is the [vertex cover number](#vertex-cover-number). By the [complement of a set](set.md#complement-of-a-set) correspondence, a [minimum vertex cover](#minimum-vertex-cover) leaves a largest possible [independent set](#independent-set-graph-theory) unselected.

Minimum size is stronger than merely being unable to remove a selected [vertex](graph.md#vertex-graph-theory). In the [star graph](bipartite-graph.md#star-graph-theory) $K_{1,3}$, the three leaves form a [vertex cover](#vertex-cover) from which no [vertex](graph.md#vertex-graph-theory) can be removed: each leaf covers its own [edge](#edge-of-a-graph). Nevertheless, the centre alone is a [minimum vertex cover](#minimum-vertex-cover) of size one. Such an inclusion-minimal [vertex cover](#vertex-cover) can therefore be much larger than a [minimum vertex cover](#minimum-vertex-cover).

#### Vertex cover number

↑ **Parent:** [Minimum vertex cover](#minimum-vertex-cover)

The [vertex cover number](#vertex-cover-number) records the size of a [minimum vertex cover](#minimum-vertex-cover):

$$
\tau(G)=\min\{|C|:C\subseteq V(G),\ C\text{ is a vertex cover of }G\}.
$$

The [vertex cover number](#vertex-cover-number) is a number, while a [minimum vertex cover](#minimum-vertex-cover) is a [set](set.md) attaining it. For the [cycle graph](#cycle-graph) $C_5$, the [independence number](#independence-number) is $2$, so the complement correspondence gives $\tau(C_5)=5-2=3$. The [vertex cover](#vertex-cover) $\{1,3,4\}$ above attains this size.

Every [matching in a graph](matching-graph-theory.md) gives a lower bound on the [vertex cover number](#vertex-cover-number). Its [edges](#edge-of-a-graph) have no shared endpoints, so covering each selected [edge](#edge-of-a-graph) requires a different [vertex](graph.md#vertex-graph-theory). Thus, for any [matching in a graph](matching-graph-theory.md) $M$ and any [vertex cover](#vertex-cover) $C$,

$$
|M|\leq |C|,\qquad \nu(G)\leq\tau(G),
$$

where $\nu(G)$ is the [matching number](matching-graph-theory.md#matching-number). Exhibiting a [matching in a graph](matching-graph-theory.md) and a [vertex cover](#vertex-cover) of the same size certifies that both are optimum. [Kőnig's theorem for bipartite matching](flow-network.md#konig-s-theorem-graph-theory) says that every finite [bipartite graph](bipartite-graph.md) admits this equality: $\nu(G)=\tau(G)$.[Diestel, Graph Theory, Section 2.1, Theorem 2.1.1 and its lower-bound argument](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

For the [complete bipartite graph](bipartite-graph.md#complete-bipartite-graph) $K_{2,3}$, let the left [vertices](graph.md#vertex-graph-theory) be $L=\{a,b\}$ and the right [vertices](graph.md#vertex-graph-theory) be $R=\{x,y,z\}$. All six [edges](#edge-of-a-graph) join $L$ to $R$. Selecting $C=L$ covers every [edge](#edge-of-a-graph); selecting $M=\{ax,by\}$ gives a [matching in a graph](matching-graph-theory.md) of size two. The lower bound and this [vertex cover](#vertex-cover) give $2\leq\tau(K_{2,3})\leq2$, so $\tau(K_{2,3})=\nu(K_{2,3})=2$. The remaining [vertices](graph.md#vertex-graph-theory) $R$ form a largest [independent set](#independent-set-graph-theory) of size three. Crossings of drawn [edges](#edge-of-a-graph) are not extra [vertices](graph.md#vertex-graph-theory).

<a id="image-two-disjoint-matching-edges-certify-that-the-two-left-vertices-are-a-minimum-cover-of-k₂-₃"></a>
![](bipartite-matching-cover-certificate.png)

**[Figure 12](#image-two-disjoint-matching-edges-certify-that-the-two-left-vertices-are-a-minimum-cover-of-k₂-₃). Two disjoint matching edges certify that the two left vertices are a minimum cover of K₂,₃**.

The [bipartite graph](bipartite-graph.md) hypothesis matters. In a [triangle in a graph](graph.md#triangle-in-a-graph), any two [vertices](graph.md#vertex-graph-theory) form a [minimum vertex cover](#minimum-vertex-cover), while any two [edges](#edge-of-a-graph) share an endpoint. Hence $\tau(K_3)=2$ and $\nu(K_3)=1$. Similarly, the [cycle graph](#cycle-graph) $C_5$ has $\tau(C_5)=3$ and $\nu(C_5)=2$. The inequality for the [matching number](matching-graph-theory.md#matching-number) remains valid, but equality can fail.

### 3-SAT reduction to vertex cover

↑ **Parent:** [Vertex cover](#vertex-cover)

A [polynomial-time many-one reduction](theoretical-computer-science.md#polynomial-time-many-one-reduction) represents each variable by an adjacent literal pair and each clause by a [triangle in a graph](graph.md#triangle-in-a-graph). Connect each occurrence vertex to its corresponding literal vertex. A [vertex cover](#vertex-cover) of size $n+2m$ must choose one literal vertex per variable and two vertices per clause, and its omitted clause vertex forces a true literal. Conversely a satisfying [Boolean valuation](mathematical-logic.md#boolean-valuation) supplies such a cover. This establishes [NP-hardness](theoretical-computer-science.md#np-hardness) of the vertex-cover decision problem from [3-SAT](theoretical-computer-science.md#3-sat).

## Binomial random graph

↑ **Parent:** [Graph theory](graph-theory.md)

The binomial random graph $G(n,p)$ has vertex set $\{1,\ldots,n\}$ and includes each of the $\binom n2$ possible edges independently with probability $p$.

### Poisson threshold for vertices lying in no triangle

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

For a fixed set of $r$ vertices, exclude all triangles meeting that set. Their total expectation is $r\log(n/c)+o(1)$. Distinct triangle pairs sharing an edge contribute $O_r(n^3p^5)=o(1)$ to the [Janson dependency sum](probability-inequality.md#janson-dependency-sum). [Harris' inequality](probability-inequality.md#harris-inequality) and [Janson inequality](probability-inequality.md#janson-inequality) bound the avoidance probability between matching exponentials, giving $(c/n)^r(1+o(1))$. The [factorial-moment criterion for Poisson convergence](continuous-time-markov-chain.md#factorial-moment-criterion-for-poisson-convergence) then gives the displayed law.

### Deferred edge exposure in greedy independent-set colouring

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

Construct an [independent set](#independent-set-graph-theory) by choosing a candidate vertex, exposing only its incident edges, and retaining its non-neighbours as candidates. Once the chosen independent set is removed, every exposed edge has a removed endpoint. Thus the remaining internal edges still have their independent original laws, conditional on the revealed history. This special exposure rule permits fresh-binomial estimates for successive classes; an arbitrary adaptively selected vertex subset does not have that property.

### Strictly balanced graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

A finite [graph](graph.md) $H$ with at least one [edge](#edge-of-a-graph) is strictly balanced when every proper nonempty [subgraph](#subgraph) $F$ has smaller edge-to-vertex ratio. It is connected and has no isolated [vertices](graph.md#vertex-graph-theory): otherwise a component of at least the average density, or deletion of isolated [vertices](graph.md#vertex-graph-theory), violates the inequality. The density condition suppresses overlapping copies at the sparse appearance scale.

#### Poisson limit for strictly balanced subgraph counts

↑ **Parent:** [Strictly balanced graph](#strictly-balanced-graph)

Here $v,e,a$ are the numbers of [vertices](graph.md#vertex-graph-theory), [edges](#edge-of-a-graph) and [graph automorphisms](graph.md#graph-automorphism) of $H$. Vertex-disjoint ordered $r$-tuples contribute $(n)_{rv}p^{re}/a^r\to(c^e/a)^r$ to the [factorial moment](continuous-time-markov-chain.md#factorial-moment). Adding a copy overlapping the previous union in $f$ [vertices](graph.md#vertex-graph-theory) and $g$ [edges](#edge-of-a-graph) changes the power of $n$ by $-f+(v/e)g\le0$, strictly when the intersection is a proper nonempty [subgraph](#subgraph). The first overlap is strict because $H$ is connected and the previous copies are disjoint. Finitely many overlap types therefore contribute $o(1)$. The [factorial-moment criterion for Poisson convergence](continuous-time-markov-chain.md#factorial-moment-criterion-for-poisson-convergence) gives the result.

### Missing common-neighbour count in a binomial random graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

Let $X$ count unordered [vertex](graph.md#vertex-graph-theory) pairs with no [common neighbour](#common-neighbour) in a [binomial random graph](#binomial-random-graph). Each other [vertex](graph.md#vertex-graph-theory) provides the required pair of [edges](#edge-of-a-graph) independently, with success probability $p^2$. A fixed pair has no common neighbour with probability $(1-p^2)^{n-2}$. Summing its indicators gives the displayed [expectation](expected-value.md).

#### Diameter bound for a fixed-density binomial random graph

↑ **Parent:** [Missing common-neighbour count in a binomial random graph](#missing-common-neighbour-count-in-a-binomial-random-graph)

For fixed $0<p<1$, the [missing common-neighbour count in a binomial random graph](#missing-common-neighbour-count-in-a-binomial-random-graph) has [expectation](expected-value.md) tending to zero. The [Markov inequality](probability-inequality.md#markov-s-inequality) therefore shows that every pair has a [common neighbour](#common-neighbour) with probability tending to one. On that event every [graph distance](#distance-graph-theory) is at most two, so the [graph](graph.md) is [connected](geometry-and-topology.md#connected-space) and its [graph diameter](#graph-diameter) is at most two.

### Chromatic number of a binomial random graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

For a fixed probability strictly between zero and one, the largest independent set has leading size $2\log_{1/(1-p)}n$, giving a lower bound for colouring. The matching upper bound uses [independent sets in every large subset of a dense random graph](#independent-sets-in-every-large-subset-of-a-dense-random-graph), then repeatedly colours and removes such sets. A sufficiently strong probability estimate makes the failure contribution negligible for the expectation.

#### Independent sets in every large subset of a dense random graph

↑ **Parent:** [Chromatic number of a binomial random graph](#chromatic-number-of-a-binomial-random-graph)

For fixed $p$ and $\gamma>0$, [Janson inequality](probability-inequality.md#janson-inequality) bounds the failure probability for a given large [vertex](graph.md#vertex-graph-theory) subset by $\exp(-c|U|^2/(\log n)^4)$. A union bound over all at most $2^n$ subsets still tends to zero. This uniform statement is essential because [vertex](graph.md#vertex-graph-theory) sets left by a greedy colouring procedure depend on the [graph](graph.md); one cannot assume each adaptively chosen remainder is an independent fresh random [graph](graph.md).

### Vertex exposure for chromatic number

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

Group random [edges](#edge-of-a-graph) by their larger endpoint. These independent coordinates each change [edges](#edge-of-a-graph) incident to only one [vertex](graph.md#vertex-graph-theory). Removing that [vertex](graph.md#vertex-graph-theory) leaves the same [graph](graph.md) under any two outcomes, so their [chromatic numbers](graph-coloring.md#chromatic-number) differ by at most one. The [McDiarmid inequality](probability-inequality.md#mcdiarmid-s-inequality) with $n$ coordinate ranges of length one gives the displayed concentration bound.

### Chromatic number of the half-density binomial random graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

For the [binomial random graph](#binomial-random-graph) $G(n,1/2)$, the [chromatic number](graph-coloring.md#chromatic-number) is $(1+o(1))n/(2\log_2n)$ [with high probability](probabilistic-combinatorics.md#with-high-probability). A [first moment method](probability-inequality.md#first-moment-method) bounds the [independence number](#independence-number) above. [Edge-disjoint clique packing](#edge-disjoint-clique-packing) in the [complement graph](#complement-graph), followed by an [edge-exposure martingale](martingale.md#edge-exposure-martingale) and a [union bound](probability-inequality.md#boole-s-inequality) over moderately large [vertex](graph.md#vertex-graph-theory) sets, supplies [independent sets](#independent-set-graph-theory) for [greedy colouring by removing independent sets](graph-coloring.md#greedy-colouring-by-removing-independent-sets).

### Clique count in a binomial random graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

If $X_t$ counts copies of the [complete graph](#complete-graph) $K_t$ in $G(n,p)$, then

$$
\mathbb EX_t=\binom ntp^{\binom t2}.
$$

Consequently $p n^{2/(t-1)}\to0$ implies $\mathbb P(X_t>0)\to0$ by the [first moment method](probability-inequality.md#first-moment-method).

#### Fixed-size clique appearance threshold

↑ **Parent:** [Clique count in a binomial random graph](#clique-count-in-a-binomial-random-graph)

For fixed $k\ge2$, a [binomial random graph](#binomial-random-graph) has no $k$-[cliques](#clique-graph-theory) with probability tending to one if $\mu_n\to0$, and has at least one with probability tending to one if $\mu_n\to\infty$. The first assertion uses the [first moment method](probability-inequality.md#first-moment-method). The second uses the [overlap formula for the variance of a clique count](#overlap-formula-for-the-variance-of-a-clique-count): overlapping $k$-sets with $l\ge2$ contribute $O(n^{-l}p^{-\binom l2})$, and each contribution tends to zero above this threshold. The fixed-size qualification matters.

##### Growing clique size can invalidate a first-moment appearance criterion

↑ **Parent:** [Fixed-size clique appearance threshold](#fixed-size-clique-appearance-threshold)

With these parameters the expected number of $(n-1)$-cliques is asymptotic to $\sqrt n$, yet the probability of any such [clique](#clique-graph-theory) tends to zero. The complement graph has about $\tfrac12\log n$ edges, and with probability tending to one two of them are vertex disjoint. Deleting one vertex cannot remove both edges. Thus divergence of the expected [clique](#clique-graph-theory) count alone does not give an appearance theorem for arbitrary growing [clique](#clique-graph-theory) size.

#### Overlap formula for the variance of a clique count

↑ **Parent:** [Clique count in a binomial random graph](#clique-count-in-a-binomial-random-graph)

For the number $X$ of $k$-[cliques](#clique-graph-theory) in a [binomial random graph](#binomial-random-graph) $G(n,p)$, with $0<p<1$ and $\mu=\mathbb EX$,

$$
\frac{\operatorname{Var}X}{\mu^2}=\sum_{j=2}^k\frac{\binom kj\binom{n-k}{k-j}}{\binom nk}\left(p^{-\binom j2}-1\right).
$$

Two $k$-sets overlapping in $j$ vertices share $\binom j2$ edges. Overlaps of zero or one vertex give independent indicators; $j=k$ includes the diagonal terms. The identity is useful for the [second moment method](probability-inequality.md#second-moment-method).

##### Growing-clique overlap bound

↑ **Parent:** [Overlap formula for the variance of a clique count](#overlap-formula-for-the-variance-of-a-clique-count)

Write $\mu_r=\binom nrp^{\binom r2}$ and $T_s=\binom rs\binom{n-r}{r-s}p^{-\binom s2}/\binom nr$. The first mean condition implies $p^{-1}\leq(en/r)^{2/(r-1)}$ eventually. For $2\leq s\leq r/2$, this yields $T_s\leq(C/s)^s$, and each fixed-$s$ term tends to zero when $n\geq r^3$. The second mean condition implies $p\leq((r+1)/n)^{2/r}$ eventually. Writing $s=r-j$ gives $T_{r-j}=\mu_r^{-1}\binom rj\binom{n-r}j p^{j(2r-j-1)/2}\leq\mu_r^{-1}(C/j)^j$ for $1\leq j\leq r/2$, and $T_r=\mu_r^{-1}$. Both bounding series are summable. The [overlap formula for the variance of a clique count](#overlap-formula-for-the-variance-of-a-clique-count) therefore gives relative variance tending to zero; the [second moment method](probability-inequality.md#second-moment-method) proves an $r$-[clique](#clique-graph-theory) exists [with high probability](probabilistic-combinatorics.md#with-high-probability).

### Triangle count in a binomial random graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

If $X$ counts triangles in $G(n,p)$, then

$$
\mathbb EX=\binom n3p^3
$$

and

$$
\operatorname{var}X
\leq\binom n3p^3
+2\binom n2\binom{n-2}2p^5.
$$

Thus $np\to\infty$ implies $\operatorname{var}X/(\mathbb EX)^2\to0$, and the [second moment method](probability-inequality.md#second-moment-method) gives $\mathbb P(X>0)\to1$.

#### Triangle variance in a binomial random graph

↑ **Parent:** [Triangle count in a binomial random graph](#triangle-count-in-a-binomial-random-graph)

For the [triangle count](graph.md#triangle-count) in a [binomial random graph](#binomial-random-graph), distinct triangle indicators are independent unless they share an [edge](#edge-of-a-graph). A shared-edge pair has [covariance](variance.md#covariance) $p^5(1-p)$, and there are $12\binom n4$ ordered pairs of that type. The individual indicator variances give the first term. Equivalently,

$$
\mathbb EX^2=\binom n3\sum_{\ell=0}^3\binom3\ell\binom{n-3}{3-\ell}p^{6-\binom\ell2},
$$

by counting ordered pairs according to the number of shared [vertices](graph.md#vertex-graph-theory).

##### Triangle-existence threshold in a binomial random graph

↑ **Parent:** [Triangle variance in a binomial random graph](#triangle-variance-in-a-binomial-random-graph)

If $np\to0$, the [triangle count in a binomial random graph](#triangle-count-in-a-binomial-random-graph) has [expectation](expected-value.md) at most $(np)^3/6\to0$, so the [Markov inequality](probability-inequality.md#markov-s-inequality) shows there are no [triangles in a graph](graph.md#triangle-in-a-graph) with probability tending to one. If $np\to\infty$, the [triangle variance in a binomial random graph](#triangle-variance-in-a-binomial-random-graph) divided by the squared mean is $O((np)^{-3})+O((n^2p)^{-1})\to0$. The [second moment method](probability-inequality.md#second-moment-method) then gives at least one [triangle in a graph](graph.md#triangle-in-a-graph) with probability tending to one. At the intermediate scale $np\to c\in(0,\infty)$, a nontrivial [Poisson limit for triangles in a binomial random graph](#poisson-limit-for-triangles-in-a-binomial-random-graph) describes the count.

#### Poisson limit for triangles in a binomial random graph

↑ **Parent:** [Triangle count in a binomial random graph](#triangle-count-in-a-binomial-random-graph)

Convergence holds in [total variation distance](probability-and-statistics.md#total-variation-distance). A triangle indicator depends only on its three edges, so its dependency neighborhood consists of itself and the $3(n-3)$ triangles sharing an edge. The [Poisson approximation with dependency neighborhoods](discrete-probability-distribution.md#poisson-approximation-with-dependency-neighborhoods) gives errors $b_1=O(n^4p^6)$ and $b_2=O(n^4p^5)$. Under the displayed scaling $p$ is of order $n^{-1}$, so both vanish. The probability of at least one triangle therefore tends to $1-e^{-\alpha}$.

### Triangle with an attached leaf in a binomial random graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

Partition the vertices into two sets of comparable size. If $np\to\infty$, the first set contains a triangle with probability tending to one. Conditional on any triangle chosen using only internal edges, the probability that none of its vertices has a neighbour in the second set is at most

$$
(1-p)^{3\lfloor n/2\rfloor}
\leq e^{-3p\lfloor n/2\rfloor}\longrightarrow0.
$$

Hence $G(n,p)$ contains a triangle with an attached leaf with probability tending to one.

## Graph coloring

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](graph-coloring.md)

## Graph

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](graph.md)

## Independent set (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Independent_set_(graph_theory))

An [independent set](#independent-set-graph-theory) selects mutually compatible objects when an [edge](#edge-of-a-graph) of a [graph](graph.md) represents a conflict. For example, if [vertices](graph.md#vertex-graph-theory) are activities and [edges](#edge-of-a-graph) join activities that cannot occur together, an [independent set](#independent-set-graph-theory) is a collection that can share one time slot. Finding the largest such collection is measured by the [independence number](#independence-number).[Barak, Introduction to Theoretical Computer Science, Chapter 14, The independent set problem](https://introtcs.org/public/lec_12_NP.html)

In a finite [simple graph](graph.md#simple-graph) $G=(V,E)$, an [independent set](#independent-set-graph-theory) is a [subset](set.md#subset) $I\subseteq V$ with no [edge](#edge-of-a-graph) joining two selected [vertices](graph.md#vertex-graph-theory):

$$
u,v\in I,\ u\ne v\Longrightarrow\{u,v\}\notin E.
$$

The empty [set](set.md) and every singleton [set](set.md) are [independent sets](#independent-set-graph-theory). In the [cycle graph](#cycle-graph) $C_5$ drawn under [vertex cover](#vertex-cover), $\{0,2\}$ is an [independent set](#independent-set-graph-theory), but $\{0,4\}$ is not: the closing [edge](#edge-of-a-graph) $40$ joins those two [vertices](graph.md#vertex-graph-theory). Choosing nonconsecutive labels is insufficient unless the wraparound [edge](#edge-of-a-graph) is checked.

An [independent set](#independent-set-graph-theory) of maximum size has [cardinality](cardinal-number.md#cardinality) equal to the [independence number](#independence-number). Being unable to add another [vertex](graph.md#vertex-graph-theory) only makes an [independent set](#independent-set-graph-theory) inclusion-maximal. In the [star graph](bipartite-graph.md#star-graph-theory) $K_{1,3}$, the centre alone is inclusion-maximal, since it is adjacent to every leaf, but the three leaves form a larger [independent set](#independent-set-graph-theory). This distinction mirrors the difference between an inclusion-minimal [vertex cover](#vertex-cover) and a [minimum vertex cover](#minimum-vertex-cover).

Every [independent set](#independent-set-graph-theory) $I$ has a [vertex cover](#vertex-cover) $V\setminus I$ as its [complement of a set](set.md#complement-of-a-set); a largest [independent set](#independent-set-graph-theory) has a [minimum vertex cover](#minimum-vertex-cover) as its complement. In every [proper vertex colouring](graph-coloring.md#proper-vertex-coloring), each [colour class](ramsey-theory.md#colour-class) is an [independent set](#independent-set-graph-theory), so [graph coloring](graph-coloring.md) partitions the [vertices](graph.md#vertex-graph-theory) into mutually compatible groups.

### Independence polynomial

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

### Maximal independent set

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

### Independent transversal

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

For a [graph](graph.md) whose vertices are partitioned into parts, an independent transversal is an [independent set](#independent-set-graph-theory) containing exactly one vertex from each part. If a cycle's parts each have twelve vertices, choose one vertex uniformly and independently per part. A cycle edge joining distinct parts is selected at both ends with [probability](probability-theory.md#probability) $1/144$. Each [event](probability-space.md#event) depends on at most $47$ others, since each part meets at most $24$ cycle edges. The [Lovász local lemma](probabilistic-combinatorics.md#lovasz-local-lemma) applies because $48e/144<1$, proving existence for an arbitrary such partition.

### Degree-ordered independent-set entropy bound

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

Order vertices by nonincreasing positive degrees $d_i$, and let $b_i$ count preceding neighbors. The [Madiman-Tetali inequality](information-theory.md#madiman-tetali-entropy-inequality) applied to preceding-neighbor sets and $b_i$ copies of singleton $i$ bounds the entropy of a uniformly chosen [independent set](#independent-set-graph-theory). In each local term, all-zero neighbor assignment permits two choices at $i$, while every other assignment permits at most one. The maximum-entropy bound gives $\log_2(2^{b_i+1}-1)$ for that term. Complete bipartite graphs $K_{d,d}$ attain equality when one part is ordered before the other.

### Independence number

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Independence_number)

The [independence number](#independence-number) is the largest [cardinality](cardinal-number.md#cardinality) of an [independent set](#independent-set-graph-theory) in a finite [simple graph](graph.md#simple-graph):

$$
\alpha(G)=\max\{|I|:I\subseteq V(G),\ I\text{ is an independent set of }G\}.
$$

It answers "how many mutually compatible objects can be selected at once?", while the [chromatic number](graph-coloring.md#chromatic-number) asks how many compatible groups are needed for all the [vertices](graph.md#vertex-graph-theory). Diestel uses this notation for a largest [independent set](#independent-set-graph-theory).[Diestel, Graph Theory, Chapter 2, Exercise 23](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

For the [cycle graph](#cycle-graph) $C_5$, the [independent set](#independent-set-graph-theory) $\{0,2\}$ shows that $\alpha(C_5)\geq2$. Three selected [vertices](graph.md#vertex-graph-theory) would require at least three unselected [vertices](graph.md#vertex-graph-theory) separating them around the [cycle graph](#cycle-graph), which has only five [vertices](graph.md#vertex-graph-theory). Thus $\alpha(C_5)=2$. There are five largest [independent sets](#independent-set-graph-theory), obtained by rotating $\{0,2\}$ around the [cycle graph](#cycle-graph), and five corresponding [minimum vertex covers](#minimum-vertex-cover).

For the [complete bipartite graph](bipartite-graph.md#complete-bipartite-graph) $K_{2,3}$, an [independent set](#independent-set-graph-theory) cannot contain a [vertex](graph.md#vertex-graph-theory) from each side, since every such pair is joined by an [edge](#edge-of-a-graph). The larger side has three [vertices](graph.md#vertex-graph-theory), so $\alpha(K_{2,3})=3$. A [triangle in a graph](graph.md#triangle-in-a-graph) has [independence number](#independence-number) one. A [graph](graph.md) with no [edges](#edge-of-a-graph) and $n$ [vertices](graph.md#vertex-graph-theory) has [independence number](#independence-number) $n$, including $\alpha(G)=0$ when $n=0$.

The complement correspondence between [vertex covers](#vertex-cover) and [independent sets](#independent-set-graph-theory) gives, with $n=|V(G)|$,

$$
\tau(G)+\alpha(G)=n.
$$

Every extra [vertex](graph.md#vertex-graph-theory) that can be left in an [independent set](#independent-set-graph-theory) is one fewer [vertex](graph.md#vertex-graph-theory) needed in a [minimum vertex cover](#minimum-vertex-cover). This identity holds for all finite [simple graphs](graph.md#simple-graph), including the [triangle in a graph](graph.md#triangle-in-a-graph) and the [cycle graph](#cycle-graph) $C_5$; it does not require the [bipartite graph](bipartite-graph.md) hypothesis of [Kőnig's theorem for bipartite matching](flow-network.md#konig-s-theorem-graph-theory).

For a nonempty [graph](graph.md), every [colour class](ramsey-theory.md#colour-class) of a [proper vertex colouring](graph-coloring.md#proper-vertex-coloring) contains at most $\alpha(G)$ [vertices](graph.md#vertex-graph-theory). Counting all the [vertices](graph.md#vertex-graph-theory) therefore gives

$$
\chi(G)\geq\frac{|V(G)|}{\alpha(G)}.
$$

Since the [chromatic number](graph-coloring.md#chromatic-number) is an [integer](integer.md), the bound rounds up: for the [cycle graph](#cycle-graph) $C_5$, $\chi(C_5)\geq\lceil5/2\rceil=3$. It is attained by assigning colour $A$ to $0,2$, colour $B$ to $1,3$, and colour $C$ to $4$. All five [edges](#edge-of-a-graph), including $40$, have differently coloured endpoints.

#### Caro-Wei bound

↑ **Parent:** [Independence number](#independence-number)

For a finite simple [graph](graph.md), $\alpha(G)\geq\sum_{v\in V(G)}1/(1+\deg v)\geq |V(G)|^2/(|V(G)|+2|E(G)|)$. Randomly order its [vertices](graph.md#vertex-graph-theory) and retain each [vertex](graph.md#vertex-graph-theory) preceding all its [graph neighbours](#neighbour-of-a-vertex). This gives an [independent set](#independent-set-graph-theory) with the first expression as its [expected value](expected-value.md). The second inequality is the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality).

#### Triangle-free graph with sub-power independence number

↑ **Parent:** [Independence number](#independence-number)

For every sufficiently large $n$, there is a triangle-free graph $G$ on $n$ vertices with $\alpha(G)<n^{0.7}$. One construction samples $G(2n,(2n)^{-0.69})$: with positive probability it has fewer than $n$ triangles and no independent set of size $n^{0.7}$. Delete one vertex from each triangle and then take an induced $n$-vertex subgraph.

### Greedy independent-set bound

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

Every finite graph of maximum degree at most $\Delta$ has an [independent set](#independent-set-graph-theory) of size at least $|V|/(\Delta+1)$. Greedily choose a vertex and delete its closed neighbourhood.

### Locally sparse graph independence bound

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

There is an absolute $c>0$ such that if an $n$-vertex graph has maximum degree at most $d$ and every vertex neighbourhood spans at most $d^2/f$ edges, where $2\leq f\leq d^2$, then

$$
\alpha(G)\geq c\frac{n\log f}{d}.
$$

The triangle-free case is commonly called Shearer's independence bound.

#### Shearer independence bound for a triangle-free graph

↑ **Parent:** [Locally sparse graph independence bound](#locally-sparse-graph-independence-bound)

Every triangle-free graph on $n$ vertices with maximum degree at most $d$ has

$$
\alpha(G)\geq c\frac{n\log d}{d}
$$

for an absolute constant $c>0$.

## Leaf of a graph

↑ **Parent:** [Graph theory](graph-theory.md)

A leaf is a vertex of degree one.

Thus a leaf is a [vertex of a graph](graph.md#vertex-graph-theory) with [degree of a vertex](#degree-graph-theory) equal to one.

## Edge of a graph

↑ **Parent:** [Graph theory](graph-theory.md)

An edge joins two vertices of a graph; in a simple graph it is an unordered pair of distinct vertices.

An [edge of a graph](#edge-of-a-graph) joins endpoints in a [graph](graph.md). For a [simple graph](graph.md#simple-graph) it is an unordered pair of distinct [vertices of a graph](graph.md#vertex-graph-theory); for a [directed graph](#directed-graph) its endpoints are ordered.

## Path in a graph

↑ **Parent:** [Graph theory](graph-theory.md)

A path of length $t$ is a sequence of $t+1$ distinct vertices in which consecutive vertices are adjacent.

### Hamiltonian path

↑ **Parent:** [Path in a graph](#path-in-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamiltonian_path)

A [Hamiltonian path](#hamiltonian-path) is a [path in a graph](#path-in-a-graph) that visits every [graph vertex](graph.md#vertex-graph-theory) exactly once. Removing any [edge](#edge-of-a-graph) from a [Hamilton cycle](#hamilton-cycle) produces a [Hamiltonian path](#hamiltonian-path). Conversely, a [Hamiltonian path](#hamiltonian-path) closes to a [Hamilton cycle](#hamilton-cycle) exactly when its endpoints are joined by an [edge](#edge-of-a-graph).

### Edge-disjoint paths

↑ **Parent:** [Path in a graph](#path-in-a-graph)

Paths are edge-disjoint when no graph edge occurs in two of them. They may share internal vertices. If $r$ edge-disjoint client-to-server paths exist, fewer than $r$ failed links cannot destroy them all. For simultaneous link and node failures one instead needs [internally vertex-disjoint paths](#internally-vertex-disjoint-paths), since one shared internal node could destroy several edge-disjoint paths at once.

### Ray in a graph

↑ **Parent:** [Path in a graph](#path-in-a-graph)

A [graph ray](#ray-in-a-graph) is an infinite [sequence](sequence-and-series.md#sequence) $v_0,v_1,\ldots$ of distinct [graph vertices](graph.md#vertex-graph-theory) with an [edge](#edge-of-a-graph) between consecutive [graph vertices](graph.md#vertex-graph-theory). Every infinite connected [locally finite graph](#locally-finite-graph) contains a [graph ray](#ray-in-a-graph) from each [graph vertex](graph.md#vertex-graph-theory), by the [König infinity lemma](tree-graph-theory.md#konig-s-lemma) applied to its finite self-avoiding [graph paths](#path-in-a-graph). An open [graph ray](#ray-in-a-graph) witnesses an infinite [percolation cluster](bond-percolation.md#percolation-cluster).

### Path graph

↑ **Parent:** [Path in a graph](#path-in-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Path_graph)

A path graph $P_n$ has $n$ vertices in a single chain and $n-1$ edges. Its endpoint [graph distance](#distance-graph-theory) is $n-1$ and, with unit resistances, its endpoint [effective resistance](random-walk.md#effective-resistance) is also $n-1$.

### Cycle in a graph

↑ **Parent:** [Path in a graph](#path-in-a-graph)

A cycle is a closed path: its final vertex is joined back to its initial vertex, and no other vertex is repeated.

#### Induced cycle

↑ **Parent:** [Cycle in a graph](#cycle-in-a-graph)

An [induced cycle](#induced-cycle) is a [cycle in a graph](#cycle-in-a-graph) whose [vertices](graph.md#vertex-graph-theory) induce exactly its cycle [edges](#edge-of-a-graph), with no [edge](#edge-of-a-graph) between nonconsecutive [vertices](graph.md#vertex-graph-theory). A triangle is an [induced cycle](#induced-cycle) of length three. A [chordal graph](#chordal-graph) forbids [induced cycles](#induced-cycle) of length at least four.

#### Girth

↑ **Parent:** [Cycle in a graph](#cycle-in-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Girth)

The girth of a graph containing a cycle is the length of its shortest cycle. A forest is conventionally assigned infinite girth.

#### Odd cycle

↑ **Parent:** [Cycle in a graph](#cycle-in-a-graph)

An odd cycle is a [cycle in a graph](#cycle-in-a-graph) with an [odd number](integer.md#odd-number) of edges.

#### Cycle graph

↑ **Parent:** [Cycle in a graph](#cycle-in-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cycle_graph)

The cycle graph $C_n$ has vertices $v_1,\ldots,v_n$ and edges $v_iv_{i+1}$, with indices read cyclically.

##### Wheel graph

↑ **Parent:** [Cycle graph](#cycle-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wheel_graph)

A wheel graph is the [join of graphs](#join-graph-theory) of a [cycle graph](#cycle-graph) and a single [vertex](graph.md#vertex-graph-theory). Every wheel with a rim of at least three [vertices](graph.md#vertex-graph-theory) has a $K_4$ [graph minor](graph-minor.md): partition the rim into three nonempty consecutive connected sets and use its centre as the fourth [branch set of a graph minor](graph-minor.md#branch-set-of-a-graph-minor).

##### Hamilton cycle

↑ **Parent:** [Cycle graph](#cycle-graph)

A [Hamilton cycle](#hamilton-cycle), also called a [Hamiltonian cycle](#hamilton-cycle), is a [cycle in a graph](#cycle-in-a-graph) containing every [vertex](graph.md#vertex-graph-theory) of the [graph](graph.md). Here the convention is a finite [simple graph](graph.md#simple-graph) whose [edges](#edge-of-a-graph) are undirected, with $n=|V|\geq3$. A traversal is a [sequence](sequence-and-series.md#sequence)

$$
v_0,v_1,\ldots,v_{n-1},v_n=v_0,
$$

where $v_0,\ldots,v_{n-1}$ are all the distinct [vertices](graph.md#vertex-graph-theory) and $\{v_i,v_{i+1}\}\in E$ for $0\leq i<n$. Thus "once" means once before the closing return: the start appears again at the end, and there are exactly $n$ traversed [edges](#edge-of-a-graph). The [graph](graph.md) may contain additional unused [edges](#edge-of-a-graph).[Diestel, Graph Theory, Chapter 10, opening paragraph, printed p. 323: Hamilton cycles, Hamilton paths, and the contrast with Euler tours](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/hamilton-cycles)

A [Hamiltonian path](#hamiltonian-path) visits all [vertices](graph.md#vertex-graph-theory) once without requiring a return. Removing an [edge](#edge-of-a-graph) from a [Hamilton cycle](#hamilton-cycle) gives a [Hamiltonian path](#hamiltonian-path); a particular [Hamiltonian path](#hamiltonian-path) closes only if its endpoints are adjacent. An [Euler circuit](#euler-circuit) instead traverses every [edge](#edge-of-a-graph) exactly once and can revisit [vertices](graph.md#vertex-graph-theory) midway. The two requirements are independent, as these original labelled examples show.

<a id="hamilton-euler-vertex-edge-comparison"></a>
![](hamilton-euler-vertex-edge-comparison.png)

**[Figure 13](#hamilton-euler-vertex-edge-comparison). Two graphs separate Hamilton cycle vertex coverage from Euler circuit edge coverage; arrows mark traversal order, not directed edges**.

For the [complete graph](#complete-graph) $K_4$, use $V=\{A,B,C,D\}$ and $E=\{AB,AC,AD,BC,BD,CD\}$, where $AB$ abbreviates the unordered pair $\{A,B\}$. The route $A,B,C,D,A$ is a [Hamilton cycle](#hamilton-cycle): it visits every [vertex](graph.md#vertex-graph-theory) and uses four of the six [edges](#edge-of-a-graph), omitting $AC$ and $BD$. It is not an [Euler circuit](#euler-circuit), and the [graph](graph.md) admits no [Euler circuit](#euler-circuit) at all: every [vertex degree](#degree-graph-theory) is three, contradicting the [Euler circuit criterion](#euler-circuit-criterion). The crossing of the drawn diagonals is not another [vertex](graph.md#vertex-graph-theory).

Conversely, take two [triangles in a graph](graph.md#triangle-in-a-graph) sharing only $X$, with $V=\{X,A,B,C,D\}$ and $E=\{XA,AB,BX,XC,CD,DX\}$. The route $X,A,B,X,C,D,X$ is an [Euler circuit](#euler-circuit), using all six [edges](#edge-of-a-graph) once; the [vertex degrees](#degree-graph-theory) are $4,2,2,2,2$. It cannot be a [Hamilton cycle](#hamilton-cycle), since $X$ occurs midway as well as at the start and end. More strongly, no [Hamilton cycle](#hamilton-cycle) exists: $X$ is a [cut vertex](#cut-vertex), and deleting it leaves the two separate [edges](#edge-of-a-graph) $AB$ and $CD$. Nevertheless, $A,B,X,C,D$ is a [Hamiltonian path](#hamiltonian-path), whose endpoints are not adjacent.

###### Hamiltonian graph

↑ **Parent:** [Hamilton cycle](#hamilton-cycle)

A [Hamiltonian graph](#hamiltonian-graph) is a [graph](graph.md) containing a [Hamilton cycle](#hamilton-cycle). This describes existence of a spanning [graph cycle](#cycle-in-a-graph), rather than requiring every [edge](#edge-of-a-graph) of the [graph](graph.md) to belong to that [graph cycle](#cycle-in-a-graph). In the finite [simple graph](graph.md#simple-graph) convention, $K_n$ is a [Hamiltonian graph](#hamiltonian-graph) for $n\geq3$, because any ordering of its [vertices](graph.md#vertex-graph-theory) closes using available [edges](#edge-of-a-graph).

###### Necessary conditions for a Hamilton cycle

↑ **Parent:** [Hamilton cycle](#hamilton-cycle)

A [Hamiltonian graph](#hamiltonian-graph) must be a [connected graph](graph.md#connected-graph) and have [minimum degree](#minimum-degree-of-a-graph) $\delta(G)\geq2$: each [vertex](graph.md#vertex-graph-theory) has two distinct neighbours on its [Hamilton cycle](#hamilton-cycle). It also has no [cut vertex](#cut-vertex). Indeed, deleting any [vertex](graph.md#vertex-graph-theory) from the [Hamilton cycle](#hamilton-cycle) leaves a [graph path](#path-in-a-graph) through every remaining [vertex](graph.md#vertex-graph-theory), so the remaining [graph](graph.md) is connected. These are quick ways to rule out a [Hamilton cycle](#hamilton-cycle).[Diestel, Graph Theory, §10.1, printed pp. 323–324: necessary minimum degree two and 2-connectivity](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/hamilton-cycles)

Even these conditions together are not sufficient: the [complete bipartite graph](bipartite-graph.md#complete-bipartite-graph) $K_{2,3}$ is connected, has [minimum degree](#minimum-degree-of-a-graph) two and no [cut vertex](#cut-vertex), but has no [Hamilton cycle](#hamilton-cycle). Every [graph cycle](#cycle-in-a-graph) in a [bipartite graph](bipartite-graph.md) alternates between its two parts, using equally many [vertices](graph.md#vertex-graph-theory) from each; it cannot use all two and all three.

In the other direction, [Dirac's theorem](#dirac-s-theorem) gives a sufficient condition: a finite [simple graph](graph.md#simple-graph) with $n\geq3$ and $\delta(G)\geq n/2$ has a [Hamilton cycle](#hamilton-cycle). Failure of this inequality proves nothing by itself: the [cycle graph](#cycle-graph) $C_5$ has a [Hamilton cycle](#hamilton-cycle) despite $\delta(C_5)=2<5/2$.[Diestel, Graph Theory, §10.1, Theorem 10.1.1, printed p. 324](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/hamilton-cycles)

###### Weighted Hamilton cycle

↑ **Parent:** [Hamilton cycle](#hamilton-cycle)

A [weighted Hamilton cycle](#weighted-hamilton-cycle) is a [Hamilton cycle](#hamilton-cycle) in a [weighted graph](random-walk.md#weighted-graph), with cost equal to the sum of its traversed [edge](#edge-of-a-graph) weights. Here weights represent symmetric nonnegative costs, rather than conductances. Asking whether a [Hamilton cycle](#hamilton-cycle) exists is a feasibility question; asking for the cheapest one is an instance of the [travelling salesman problem](mathematical-optimization.md#travelling-salesman-problem). A [complete graph](#complete-graph) supplies every possible connection between distinct [vertices](graph.md#vertex-graph-theory), making feasibility automatic for $n\geq3$, while choosing the cheapest visiting order remains a separate [mathematical optimization](mathematical-optimization.md) problem.

<a id="weighted-hamilton-cycle-four-vertex-tours"></a>
![](weighted-hamilton-cycle-four-vertex-tours.png)

**[Figure 14](#weighted-hamilton-cycle-four-vertex-tours). A fictitious weighted graph on four vertices: its three Hamilton cycles, identified under reversal and cyclic rotation, have costs 14, 19 and 21**.

Assign the [complete graph](#complete-graph) $K_4$ the symmetric [edge](#edge-of-a-graph) costs $w_{AB}=2$, $w_{BC}=3$, $w_{CD}=4$, $w_{AD}=5$, $w_{AC}=6$ and $w_{BD}=7$, in arbitrary units. Fix the start at $A$ and identify each [Hamilton cycle](#hamilton-cycle) with its reverse. The three possibilities are

$$
\begin{aligned}
A,B,C,D,A &: 2+3+4+5=14,\\
A,B,D,C,A &: 2+7+4+6=19,\\
A,C,B,D,A &: 6+3+7+5=21.
\end{aligned}
$$

These exhaust the possibilities: the [permutations](combinatorics.md#permutation) of the other three [vertices](graph.md#vertex-graph-theory) give $3!=6$ orders, paired into three reversals. Hence the perimeter tour really is optimal for this toy instance. The diagram's geometric lengths are not costs, and no [triangle inequality](topological-analysis.md#triangle-inequality) is assumed.

The usefulness of this model is to distinguish visiting required sites from covering required connections. If tasks are assigned to [vertices](graph.md#vertex-graph-theory) and the route must return after one visit to each, a [weighted Hamilton cycle](#weighted-hamilton-cycle) captures the ordering requirement. If the job instead requires each [edge](#edge-of-a-graph) once, the relevant object is an [Euler circuit](#euler-circuit). The [shortest path problem](shortest-path-problem.md) asks only for a cheapest route between specified endpoints. A 1954 primary research paper gave a concrete motivation for the [travelling salesman problem](mathematical-optimization.md#travelling-salesman-problem): certify that a particular tour through 49 cities has minimum road-distance cost.[Solution of a Large-Scale Traveling-Salesman Problem by G. Dantzig, R. Fulkerson and S. Johnson, abstract; Journal of the Operations Research Society of America 2(4), pp. 393–410 (1954)](mathematics-bibliography.md#solution-of-a-large-scale-traveling-salesman-problem-by-george-b-dantzig-and-others)

These are abstract route models. If a cost stands for a whole [graph path](#path-in-a-graph) through an underlying network, travelling between consecutive task [vertices](graph.md#vertex-graph-theory) can pass through intermediate network [vertices](graph.md#vertex-graph-theory) more than once. One visit per task therefore does not imply one visit per physical junction. One-way connections require a [directed graph](#directed-graph); changing costs or extra timing constraints require a richer model than the fixed symmetric toy instance.

###### Icosian game

↑ **Parent:** [Hamilton cycle](#hamilton-cycle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Icosian_game)

The [Icosian game](#icosian-game) made the [vertex](graph.md#vertex-graph-theory)-visit puzzle tangible. The report of its 1857 presentation describes a plane projection of a regular [dodecahedron](euclidean-geometry.md#dodecahedron), with holes at the [vertices](graph.md#vertex-graph-theory) for ivory pins. The Trinity College Dublin archive connects this game with the search for closed routes visiting each [vertex](graph.md#vertex-graph-theory) exactly once. This puzzle supplies a historical illustration of the [Hamilton cycle](#hamilton-cycle) requirement.[The Icosian Calculus, Hamilton papers archive: opening historical introduction and quoted report of the 1857 British Association presentation: dodecahedron projection and ivory pins](mathematics-bibliography.md#the-icosian-calculus-hamilton-papers-archive)

##### Pancyclic graph

↑ **Parent:** [Cycle graph](#cycle-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pancyclic_graph)

An $n$-vertex graph is pancyclic when it contains $C_\ell$ for every $3\leq\ell\leq n$.

### Long path from minimum degree

↑ **Parent:** [Path in a graph](#path-in-a-graph)

Every connected $n$-vertex graph of minimum degree $\delta$ contains a path of length at least $\min(2\delta,n-1)$.

<h3 id="erdos-gallai-path-edge-bound">Erdős-Gallai path edge bound</h3>

↑ **Parent:** [Path in a graph](#path-in-a-graph)

An $n$-vertex graph containing no path of length $t$ has at most $(t-1)n/2$ edges.

This path-length bound is a different result from the [Erdős-Gallai theorem](#erdos-gallai-theorem) on degree sequences.

## Subgraph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subgraph)

A subgraph is obtained from a graph by selecting some of its vertices and edges while retaining every selected edge's endpoints.

### Spanning subgraph

↑ **Parent:** [Subgraph](#subgraph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spanning_subgraph)

A spanning subgraph retains every vertex of the original graph and some or all of its edges. Adding the omitted edges can only enlarge the [graph neighbourhood](#graph-neighbourhood) and the [external vertex boundary](#external-vertex-boundary) of each fixed vertex set.

### Induced subgraph

↑ **Parent:** [Subgraph](#subgraph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Induced_subgraph)

The subgraph induced by a vertex set $W$ contains every edge of the original graph whose two endpoints lie in $W$.

### Three-colourable two-thirds subgraph lemma

↑ **Parent:** [Subgraph](#subgraph)

Every finite graph $G$ has a three-colourable subgraph with at least $2e(G)/3$ edges. Give vertices three independent uniform colours and retain edges whose endpoints have different colours. Each edge survives with probability $2/3$, so the expected number surviving is $2e(G)/3$.

## Join (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Join_(graph_theory))

The join $\Gamma_1*\Gamma_2$ is obtained from the [disjoint union of graphs](#disjoint-union-of-graphs) $\Gamma_1\sqcup\Gamma_2$ by adding every edge between a vertex of $\Gamma_1$ and a vertex of $\Gamma_2$.

## Disjoint union of graphs

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Disjoint_union_of_graphs)

The disjoint union $\Gamma_1\sqcup\Gamma_2$ has the vertices and edges of the two graphs and no edge joining the two parts.

## Intersection graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intersection_graph)

An [intersection graph](#intersection-graph) has one [vertex](graph.md#vertex-graph-theory) for each member of a family of [sets](set.md). Two distinct [vertices](graph.md#vertex-graph-theory) have an [edge](#edge-of-a-graph) exactly when their associated [sets](set.md) have a nonempty [intersection](set.md#set-intersection). A [clique](#clique-graph-theory) therefore describes pairwise intersections; it need not give a single element common to all those [sets](set.md).

## Complete graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_graph)

A [complete graph](#complete-graph) is a [simple graph](graph.md#simple-graph) in which every two distinct [vertices](graph.md#vertex-graph-theory) are joined by an [edge](#edge-of-a-graph). The finite [complete graph](#complete-graph) on $n$ [vertices](graph.md#vertex-graph-theory) is denoted $K_n$. Here the [edges](#edge-of-a-graph) are undirected, and [self-loops](graph.md#loop-graph-theory) are excluded. The usual pictures below use $n\geq1$: $K_1$ is a single [vertex](graph.md#vertex-graph-theory), $K_2$ a single [edge](#edge-of-a-graph), and $K_3$ a [triangle in a graph](graph.md#triangle-in-a-graph).[§1.1, printed p. 3 of the third electronic edition (2005): pairwise adjacency, complete graphs and triangle notation](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

Completeness describes all the possible pairs, rather than a drawing style. Different layouts can represent the same [graph](graph.md) through a [graph isomorphism](graph.md#graph-isomorphism). Crossing lines away from the drawn [vertices](graph.md#vertex-graph-theory) do not add new [vertices](graph.md#vertex-graph-theory) or [edges](#edge-of-a-graph).

<a id="image-complete-graphs-with-one-through-five-vertices"></a>
![](complete-graphs-small-orders.png)

**[Figure 15](#image-complete-graphs-with-one-through-five-vertices). Complete graphs with one through five vertices**. Each original drawing joins every pair of distinct [vertices](graph.md#vertex-graph-theory) exactly once. The [complete graphs](#complete-graph) $K_1,K_2,K_3,K_4,K_5$ have respectively $0,1,3,6,10$ [edges](#edge-of-a-graph). Intersections of drawn lines in the $K_5$ panel are not additional [vertices](graph.md#vertex-graph-theory).

There are $\binom n2=n(n-1)/2$ unordered pairs of distinct [vertices](graph.md#vertex-graph-theory), so this is the [edge count of a complete graph](#edge-count-of-a-complete-graph). Each [vertex](graph.md#vertex-graph-theory) has [vertex degree](#degree-graph-theory) $n-1$. The [degree-sum formula](combinatorics.md#degree-sum-formula) gives the same count: $2|E|=n(n-1)$. These formulas make a [complete graph](#complete-graph) the upper extreme for [edge](#edge-of-a-graph) counts among [simple graphs](graph.md#simple-graph) of a fixed size.

This is useful when modelling pairwise relationships. If every pair of objects needs its own direct connection, ten [vertices](graph.md#vertex-graph-theory) require $45$ [edges](#edge-of-a-graph), while twenty require $190$. Adding one more [vertex](graph.md#vertex-graph-theory) to $K_n$ introduces $n$ further [edges](#edge-of-a-graph). This counts a specified direct-link model; it does not require every communication system to implement every relationship with a separate physical connection.

A [proper vertex coloring](graph-coloring.md#proper-vertex-coloring) of $K_n$ must give every [vertex](graph.md#vertex-graph-theory) a different color, so its [chromatic number](graph-coloring.md#chromatic-number) is $n$. For $n\geq1$, its [independence number](#independence-number) is $1$: two distinct [vertices](graph.md#vertex-graph-theory) already have an [edge](#edge-of-a-graph) between them. Thus [complete graphs](#complete-graph) provide immediate test cases for [graph coloring](graph-coloring.md) and [independent sets](#independent-set-graph-theory).

### Edge count of a complete graph

↑ **Parent:** [Complete graph](#complete-graph)

For a [finite set](set.md#finite-set) of $n$ [vertices](graph.md#vertex-graph-theory), a [simple graph](graph.md#simple-graph) selects some of their unordered pairs as [edges](#edge-of-a-graph). There are $n(n-1)$ ordered pairs of distinct [vertices](graph.md#vertex-graph-theory); each unordered pair is counted twice, giving $\binom n2$ possibilities. Hence every [simple graph](graph.md#simple-graph) $G$ on those [vertices](graph.md#vertex-graph-theory) satisfies

$$
|E(G)|\leq\binom n2,
$$

with equality exactly when $G$ is a [complete graph](#complete-graph). The [binomial coefficient](binomial-coefficient.md) also shows why the count grows quadratically with the number of [vertices](graph.md#vertex-graph-theory).

### Clique (graph theory)

↑ **Parent:** [Complete graph](#complete-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clique_(graph_theory))

A [clique](#clique-graph-theory) in a [simple graph](graph.md#simple-graph) $G$ is a [set](set.md) $C$ of [vertices](graph.md#vertex-graph-theory) such that every pair of distinct members is adjacent. Equivalently, its [induced subgraph](#induced-subgraph) $G[C]$ is a [complete graph](#complete-graph). The surrounding [graph](graph.md) need not itself be complete: a [clique](#clique-graph-theory) describes complete pairwise connectivity within a selected group.

Consider the original [graph](graph.md) with

$$
V=\{a,b,c,d,e\},\qquad
E=\{ab,ac,bc,cd,de\}.
$$

The [set](set.md) $\{a,b,c\}$ is a [clique](#clique-graph-theory) because all three pairs $ab,ac,bc$ are [edges](#edge-of-a-graph). The [set](set.md) $\{b,c,d\}$ is not a [clique](#clique-graph-theory): the [edge](#edge-of-a-graph) $bd$ is missing. A [path in a graph](#path-in-a-graph) connecting all selected [vertices](graph.md#vertex-graph-theory) is therefore insufficient; every pair must have a direct [edge](#edge-of-a-graph).

<a id="image-a-maximum-clique-and-a-smaller-maximal-clique-in-the-same-graph"></a>
![](maximum-clique-and-maximal-edges.png)

**[Figure 16](#image-a-maximum-clique-and-a-smaller-maximal-clique-in-the-same-graph). A maximum clique and a smaller maximal clique in the same graph**. Left: the three highlighted [vertices](graph.md#vertex-graph-theory) $a,b,c$ form the unique [maximum clique](#maximum-clique). Right: the [edge](#edge-of-a-graph) $cd$ gives a [maximal clique](#maximal-clique) of size two, because no outside [vertex](graph.md#vertex-graph-theory) is adjacent to both endpoints. Both panels use the same original [graph](graph.md); highlighted [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph) select different [cliques](#clique-graph-theory).

Here the [clique number](#clique-number) is $3$. The [maximum clique](#maximum-clique) is $\{a,b,c\}$, but $\{c,d\}$ and $\{d,e\}$ are also [maximal cliques](#maximal-clique). This distinction is useful when an [algorithm](algorithm.md) stops as soon as its current [clique](#clique-graph-theory) cannot be enlarged: that stopping condition establishes maximality, while finding the largest possible [clique](#clique-graph-theory) is a separate requirement.

#### Maximum clique

↑ **Parent:** [Clique (graph theory)](#clique-graph-theory)

A [maximum clique](#maximum-clique) is a [clique](#clique-graph-theory) with the greatest possible number of [vertices](graph.md#vertex-graph-theory) in the [graph](graph.md). Its size is the [clique number](#clique-number). Every [maximum clique](#maximum-clique) is a [maximal clique](#maximal-clique), since adding a [vertex](graph.md#vertex-graph-theory) would produce a larger [clique](#clique-graph-theory). A [graph](graph.md) can have several [maximum cliques](#maximum-clique); the word maximum specifies their common size, rather than uniqueness.

#### Maximal clique

↑ **Parent:** [Clique (graph theory)](#clique-graph-theory)

A [maximal clique](#maximal-clique) is a [clique](#clique-graph-theory) not strictly contained in another [clique](#clique-graph-theory). This is distinct from a [maximum clique](#maximum-clique), whose size equals the [clique number](#clique-number). In a triangulated [probabilistic graphical model](statistical-model.md#probabilistic-graphical-model), [maximal cliques](#maximal-clique) are the natural nodes of a [junction tree](statistical-model.md#junction-tree).

Maximality is a condition on [set inclusion](set.md#set-inclusion): no outside [vertex](graph.md#vertex-graph-theory) is adjacent to every member of the current [clique](#clique-graph-theory). In the five-[vertex](graph.md#vertex-graph-theory) example, $\{c,d\}$ is maximal because $a,b$ are not adjacent to $d$, while $e$ is not adjacent to $c$. Yet $\{a,b,c\}$ is larger. Checking every possible one-[vertex](graph.md#vertex-graph-theory) extension is enough: if a larger containing [clique](#clique-graph-theory) existed, any one of its new [vertices](graph.md#vertex-graph-theory) could already be added.[§1.1, printed p. 4 of the third electronic edition (2005): maximal sets refer to inclusion](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

#### Edge-disjoint clique packing

↑ **Parent:** [Clique (graph theory)](#clique-graph-theory)

An edge-disjoint clique packing is a collection of $r$-[cliques](#clique-graph-theory) no two of which share an [edge](#edge-of-a-graph); they may share [vertices](graph.md#vertex-graph-theory). Its maximum cardinality $Z_r(G)$ changes by at most one when a single [edge](#edge-of-a-graph) is toggled. Removing that [edge](#edge-of-a-graph) destroys at most one packed [clique](#clique-graph-theory), which makes this variable suitable for an [edge-exposure martingale](martingale.md#edge-exposure-martingale).

##### Clique-packing amplification of moment bounds

↑ **Parent:** [Edge-disjoint clique packing](#edge-disjoint-clique-packing)

Let $X$ count $k$-[cliques](#clique-graph-theory) in a [binomial random graph](#binomial-random-graph) on $m$ [vertices](graph.md#vertex-graph-theory) and $Y$ count distinct ordered pairs sharing an [edge](#edge-of-a-graph). The [clique conflict graph](#clique-conflict-graph) gives $Z_k\ge X^2/(X+Y)$: order its [vertices](graph.md#vertex-graph-theory) randomly and keep each one preceding all its neighbours, then apply the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Another application gives $\mathbb EZ_k\ge(\mathbb EX)^2/(\mathbb EX+\mathbb EY)$. If $\mathbb EY/(\mathbb EX)^2=O(k^4/m^2)$ and $1/\mathbb EX$ is no larger, then $\mathbb EZ_k=\Omega(m^2/k^4)$. Changing one [edge](#edge-of-a-graph) changes $Z_k$ by at most one, so the [Azuma-Hoeffding inequality](martingale.md#azuma-s-inequality) for an [edge-exposure martingale](martingale.md#edge-exposure-martingale) yields the displayed exponential absence bound. This supports a [union bound](probability-inequality.md#boole-s-inequality) over exponentially many adaptive candidate subsets.

##### Clique conflict graph

↑ **Parent:** [Edge-disjoint clique packing](#edge-disjoint-clique-packing)

The clique conflict graph has one [vertex](graph.md#vertex-graph-theory) for each $r$-[clique](#clique-graph-theory) of a fixed [graph](graph.md), and joins two when they share an [edge](#edge-of-a-graph). Its [independent sets](#independent-set-graph-theory) correspond exactly to [edge-disjoint clique packings](#edge-disjoint-clique-packing). The [Caro-Wei bound](#caro-wei-bound) converts clique-count and overlap estimates into a packing lower bound.

#### Clique number

↑ **Parent:** [Clique (graph theory)](#clique-graph-theory)

The [clique number](#clique-number) $\omega(G)$ is the maximum number of [vertices](graph.md#vertex-graph-theory) in a [clique](#clique-graph-theory) of a finite [graph](graph.md):

$$
\omega(G)=\max\{|C|:C\text{ is a clique in }G\}.
$$

We use $\omega(G)=0$ for the [graph](graph.md) with no [vertices](graph.md#vertex-graph-theory). For a nonempty [complete graph](#complete-graph), $\omega(K_n)=n$; for the five-[vertex](graph.md#vertex-graph-theory) example, $\omega(G)=3$.

If the [graph](graph.md) contains $K_k$ and no $K_{k+1}$ as [subgraphs](#subgraph), its [clique number](#clique-number) is exactly $k$, because every larger [clique](#clique-graph-theory) contains a [clique](#clique-graph-theory) with $k+1$ [vertices](graph.md#vertex-graph-theory). Also $\chi(G)\geq\omega(G)$: a [proper vertex coloring](graph-coloring.md#proper-vertex-coloring) must assign different colors to all members of any [clique](#clique-graph-theory). This lower bound need not be an equality; the [cycle graph](#cycle-graph) $C_5$ has [clique number](#clique-number) $2$ and [chromatic number](graph-coloring.md#chromatic-number) $3$.

#### Pairwise intersections need not give a common intersection

↑ **Parent:** [Clique (graph theory)](#clique-graph-theory)

A [clique](#clique-graph-theory) records pairwise relationships. If [vertices](graph.md#vertex-graph-theory) represent [sets](set.md) and an [edge](#edge-of-a-graph) means a nonempty [intersection](set.md#set-intersection), a [clique](#clique-graph-theory) does not by itself guarantee an element common to every [set](set.md). Take

$$
A=\{1,2\},\qquad B=\{2,3\},\qquad C=\{1,3\}.
$$

Then $A\cap B=\{2\}$, $B\cap C=\{3\}$ and $C\cap A=\{1\}$, so their [intersection graph](#intersection-graph) is $K_3$. But $A\cap B\cap C=\varnothing$. The [graph](graph.md) faithfully records all three pairwise intersections; the stronger claim of a single shared element requires additional hypotheses.

### Adjacency-matrix quadratic relation for a complete graph

↑ **Parent:** [Complete graph](#complete-graph)

For the adjacency matrix $A$ of $K_n$,

$$
A=J-I,
\qquad
A^2=(n-2)A+(n-1)I.
$$

Hence $I,A,A^2$ are linearly dependent for every $n\geq2$.

## Complete multipartite graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_multipartite_graph)

A complete multipartite graph partitions its vertices into independent sets and joins every pair of vertices from different parts.

### Octahedral graph

↑ **Parent:** [Complete multipartite graph](#complete-multipartite-graph)

The octahedral graph is the [graph](graph.md) obtained from $K_6$ by removing a [perfect matching](matching-graph-theory.md#perfect-matching); equivalently it is $K_{2,2,2}$. Its [chromatic number](graph-coloring.md#chromatic-number) is three, and it contains two vertex-disjoint [triangles in a graph](graph.md#triangle-in-a-graph). A [complete bipartite graph](bipartite-graph.md#complete-bipartite-graph) with a single additional internal edge cannot contain it: every triangle in that host uses the additional edge.

### Balancing a multipartite edge-triangle objective

↑ **Parent:** [Complete multipartite graph](#complete-multipartite-graph)

With two part sizes of fixed sum and all other sizes fixed, this objective has form constant plus $(1-cB)a_ia_j$, where $B$ is the sum of the other sizes. A nonpositive coefficient permits merging the pair, while a positive coefficient favours balancing it. Choose an optimum with fewest nonzero parts: all remaining coefficients are positive, and the integer sizes differ by at most one. For real sizes they are exactly equal. This explains extremizers among [Turán graphs](extremal-graph-theory.md#turan-graph).

### Balanced complete multipartite blow-up

↑ **Parent:** [Complete multipartite graph](#complete-multipartite-graph)

The balanced complete multipartite blow-up $K_r(t)$ replaces each [vertex](graph.md#vertex-graph-theory) of the [complete graph](#complete-graph) $K_r$ by an [independent set](#independent-set-graph-theory) of $t$ [vertices](graph.md#vertex-graph-theory), placing every possible [edge](#edge-of-a-graph) between different sets and none inside a set. Every fixed [graph](graph.md) of [chromatic number](graph-coloring.md#chromatic-number) at most $r$ embeds into $K_r(t)$ for sufficiently large $t$.

## Laplacian matrix

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplacian_matrix)

The [Graph Laplacian](#laplacian-matrix) converts local differences along [edges](#edge-of-a-graph) into a [linear map](vector-space.md#linear-map). Throughout this section, $G=(V,E)$ is a finite [undirected graph](#undirected-graph) with no [self-loops](graph.md#loop-graph-theory) or repeated [edges](#edge-of-a-graph), and each [edge](#edge-of-a-graph) has weight one. In a fixed order of [vertices](graph.md#vertex-graph-theory), let $A$ be the [adjacency matrix](#adjacency-matrix) and $D$ the [degree matrix](#degree-matrix). The combinatorial [Graph Laplacian](#laplacian-matrix) is

$$
L=D-A,\qquad (Lx)_i=\sum_{j:\{i,j\}\in E}(x_i-x_j).
$$

Thus the value at a [vertex](graph.md#vertex-graph-theory) is compared with its neighbours. Every row sums to zero, so $L\mathbf1=0$: a constant [vector](vector-space.md#vector) produces no differences. This definition and the associated [Graph Laplacian quadratic form](#graph-laplacian-quadratic-form) are developed in Spielman's authored survey.[Spielman, Spectral Graph Theory, Sections 16.3.1–16.3.2](https://www.cs.yale.edu/homes/spielman/PAPERS/SGTChapter.pdf)

For the three-[vertex](graph.md#vertex-graph-theory) [path graph](#path-graph) $A-B-C$, the [vertex degrees](#degree-graph-theory) are $1,2,1$, and in that order

$$
A=\begin{pmatrix}0&1&0\\1&0&1\\0&1&0\end{pmatrix},\qquad
D=\begin{pmatrix}1&0&0\\0&2&0\\0&0&1\end{pmatrix},\qquad
L=\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix}.
$$

Direct multiplication gives three [eigenvectors](linear-operator-theory.md#eigenvector) and their [eigenvalues](linear-operator-theory.md#eigenvalue):

$$
L\begin{pmatrix}1\\1\\1\end{pmatrix}=0,\qquad
L\begin{pmatrix}1\\0\\-1\end{pmatrix}=\begin{pmatrix}1\\0\\-1\end{pmatrix},\qquad
L\begin{pmatrix}1\\-2\\1\end{pmatrix}=3\begin{pmatrix}1\\-2\\1\end{pmatrix}.
$$

The constant [eigenvector](linear-operator-theory.md#eigenvector) has [eigenvalue](linear-operator-theory.md#eigenvalue) zero; the other two describe progressively stronger neighbour disagreement. Dividing these [eigenvectors](linear-operator-theory.md#eigenvector) by $\sqrt3,\sqrt2,\sqrt6$, respectively, gives an [orthonormal basis](inner-product.md#orthonormal-basis). The four-[vertex](graph.md#vertex-graph-theory) [cycle graph](#cycle-graph) is already worked out under [circulant matrix](linear-algebra.md#circulant-matrix), where [Fourier diagonalization of a circulant matrix](linear-algebra.md#fourier-diagonalization-of-a-circulant-matrix) gives its [eigenvalues](linear-operator-theory.md#eigenvalue).

Every formula here uses $L=D-A$ without degree normalization. For comparison, Chung's treatment uses the degree-scaled [matrix](vector-space.md#matrix) $D^{-1/2}LD^{-1/2}$, with a convention for isolated [vertices](graph.md#vertex-graph-theory); its [eigenvalues](linear-operator-theory.md#eigenvalue) must not be substituted into the examples here.[Chung, Lectures on Spectral Graph Theory, Section 1.2](https://www.math.ucsd.edu/~fan/cbms.pdf)

### Graph Laplacian eigenvalue

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

An [eigenvalue](linear-operator-theory.md#eigenvalue) of a [graph](graph.md)'s [Laplacian matrix](#laplacian-matrix). For a finite undirected graph, these eigenvalues are nonnegative, and the multiplicity of zero equals the number of [connected components](geometry-and-topology.md#connected-component).

### Weighted graph Laplacian

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

For a finite [undirected graph](#undirected-graph) without [self-loops](graph.md#loop-graph-theory), give each [edge](#edge-of-a-graph) a symmetric nonnegative weight $w_{ij}=w_{ji}$. In the [weighted graph](random-walk.md#weighted-graph), set $(A_w)_{ij}=w_{ij}$ for an [edge](#edge-of-a-graph) and zero otherwise, and $(D_w)_{ii}=\sum_jw_{ij}$ with all other entries zero. The [Weighted graph Laplacian](#weighted-graph-laplacian) is

$$
L_w=D_w-A_w,\qquad
(L_wx)_i=\sum_jw_{ij}(x_i-x_j),\qquad
x^TL_wx=\sum_{\{i,j\}\in E}w_{ij}(x_i-x_j)^2.
$$

Each [edge](#edge-of-a-graph) appears once in the [quadratic form](quadratic-form.md). For the [path graph](#path-graph) $A-B-C$ with weights $w_{AB}=2$ and $w_{BC}=3$,

$$
L_w=\begin{pmatrix}2&-2&0\\-2&5&-3\\0&-3&3\end{pmatrix},\qquad
x=\begin{pmatrix}2\\0\\-1\end{pmatrix},\qquad
x^TL_wx=2(2-0)^2+3(0-(-1))^2=11.
$$

The [Weighted graph Laplacian](#weighted-graph-laplacian) is still a [positive semidefinite matrix](quadratic-form.md#positive-semidefinite-matrix). Its [kernel](kernel-of-a-linear-map.md) consists of [vectors](vector-space.md#vector) constant on each [connected component of a graph](graph.md#component-graph-theory) after zero-weight [edges](#edge-of-a-graph) are removed: an [edge](#edge-of-a-graph) of weight zero imposes no constraint. In an [electrical network](random-walk.md#electrical-network), taking the weights to be [electrical conductances](electric-charge.md#electrical-conductance) makes $x^TL_wx$ the total power dissipated by [Joule heating](electric-charge.md#joule-heating) when $x$ gives the [voltages](random-walk.md#voltage) at the [vertices](graph.md#vertex-graph-theory). This physical interpretation explains why stronger connections penalize disagreement more heavily.[Spielman, Spectral Graph Theory, Section 16.3.2: resistor networks](https://www.cs.yale.edu/homes/spielman/PAPERS/SGTChapter.pdf)

### Degree matrix

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

The [degree matrix](#degree-matrix) is the [diagonal matrix](linear-algebra.md#diagonal-matrix) whose $i$th diagonal entry is the [degree of a vertex](#degree-graph-theory) $i$. For a finite [simple graph](graph.md#simple-graph), $d_i=\sum_jA_{ij}$, where $A$ is its [adjacency matrix](#adjacency-matrix). For a [Weighted graph Laplacian](#weighted-graph-laplacian), use the sum of incident [edge](#edge-of-a-graph) weights instead of the number of incident [edges](#edge-of-a-graph).

### Graph Laplacian quadratic form

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

Assign a real value $x_i$ to each [vertex](graph.md#vertex-graph-theory). The [Graph Laplacian quadratic form](#graph-laplacian-quadratic-form) measures disagreement across [edges](#edge-of-a-graph):

$$
x^TLx=\sum_{\{i,j\}\in E}(x_i-x_j)^2\geq0.
$$

This makes the [Graph Laplacian](#laplacian-matrix) a [positive semidefinite matrix](quadratic-form.md#positive-semidefinite-matrix). The [energy](energy.md) is small when neighbours have similar values, even if distant [vertices](graph.md#vertex-graph-theory) have very different values; it depends on connections rather than where the [graph](graph.md) is drawn. In the three-[vertex](graph.md#vertex-graph-theory) [path graph](#path-graph), take $x=(2,0,-1)^T$. Then

$$
Lx=(2,-1,-1)^T,\qquad
x^TLx=2\cdot2+0\cdot(-1)+(-1)\cdot(-1)=5,
$$

and the two [edges](#edge-of-a-graph) contribute $(2-0)^2=4$ and $(0-(-1))^2=1$.

<a id="image-edge-disagreement-and-eigenvectors-of-the-three-vertex-path-laplacian"></a>
![](graph-laplacian-edge-energy.png)

**[Figure 17](#image-edge-disagreement-and-eigenvectors-of-the-three-vertex-path-laplacian). Edge disagreement and eigenvectors of the three-vertex path Laplacian**.

For a short proof, expand $x^T(D-A)x$. Each [edge](#edge-of-a-graph) contributes $x_i^2+x_j^2$ through the [degree matrix](#degree-matrix) and $-2x_ix_j$ through the [adjacency matrix](#adjacency-matrix), yielding $(x_i-x_j)^2$. The sum over unordered [edges](#edge-of-a-graph) has no factor $1/2$; a sum over all ordered pairs does:

$$
x^TLx=\frac12\sum_{i,j}A_{ij}(x_i-x_j)^2.
$$

Equivalently, let $B$ be an [oriented incidence matrix](graph.md#oriented-incidence-matrix), with one row per [edge](#edge-of-a-graph). Then $Bx$ records endpoint differences and $L=B^TB$, independently of the chosen orientations. This translates a local comparison into a global [quadratic form](quadratic-form.md) and makes its nonnegativity visible.

### Kernel of a graph Laplacian

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

The [kernel](kernel-of-a-linear-map.md) of the [Graph Laplacian](#laplacian-matrix) consists exactly of [vectors](vector-space.md#vector) constant on each [connected component of a graph](graph.md#component-graph-theory). Indeed, $Lx=0$ implies $x^TLx=0$, so the [Graph Laplacian quadratic form](#graph-laplacian-quadratic-form) forces equality at the endpoints of every [edge](#edge-of-a-graph); equality then propagates along [graph paths](#path-in-a-graph). Conversely, these equalities make every entry of $Lx$ zero. Thus the [dimension](vector-space.md#dimension-vector-space) of the [kernel](kernel-of-a-linear-map.md), equivalently the multiplicity of the zero [eigenvalue](linear-operator-theory.md#eigenvalue), counts the [connected components of a graph](graph.md#component-graph-theory).

For the disconnected [graph](graph.md) with just two [edges](#edge-of-a-graph), $AB$ and $CD$, in order $A,B,C,D$,

$$
L=\begin{pmatrix}1&-1&0&0\\-1&1&0&0\\0&0&1&-1\\0&0&-1&1\end{pmatrix},\qquad
\ker L=\operatorname{span}\left\{\begin{pmatrix}1\\1\\0\\0\end{pmatrix},\begin{pmatrix}0\\0\\1\\1\end{pmatrix}\right\}.
$$

The two displayed [vectors](vector-space.md#vector) form a [basis](vector-space.md#basis) of the [kernel](kernel-of-a-linear-map.md). The other two [eigenvectors](linear-operator-theory.md#eigenvector) $(1,-1,0,0)^T$ and $(0,0,1,-1)^T$ each have [eigenvalue](linear-operator-theory.md#eigenvalue) two, so the full list of [eigenvalues](linear-operator-theory.md#eigenvalue), including multiplicities, is $0,0,2,2$. Separate [connected components of a graph](graph.md#component-graph-theory) allow independent constant levels; a single global constant is only one of these possibilities.

<a id="image-two-disconnected-edges-give-two-independent-zero-eigenvectors"></a>
![](graph-laplacian-connected-components.png)

**[Figure 18](#image-two-disconnected-edges-give-two-independent-zero-eigenvectors). Two disconnected edges give two independent zero eigenvectors**.

### Diffusion on a graph

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

The continuous-time [diffusion](thermodynamics.md#diffusion) model on a finite [undirected graph](#undirected-graph) uses the [Graph Laplacian](#laplacian-matrix) in the [ordinary differential equation](differential-equation.md#ordinary-differential-equation)

$$
\dot x=-Lx,\qquad \dot x_i=\sum_{j:\{i,j\}\in E}(x_j-x_i).
$$

Across each [edge](#edge-of-a-graph), the higher value sends an amount proportional to the difference to the lower value. The two contributions cancel in the sum over [vertices](graph.md#vertex-graph-theory), giving [conservation of mass](continuum-mechanics.md#mass-conservation):

$$
\frac{d}{dt}\sum_i x_i(t)=-\mathbf1^TLx(t)=0.
$$

If the entries represent masses, start with nonnegative entries; signed entries can instead describe deviations from a common level. For the three-[vertex](graph.md#vertex-graph-theory) [path graph](#path-graph), the initial [vector](vector-space.md#vector) $x(0)=(1,0,-1)^T$ is an [eigenvector](linear-operator-theory.md#eigenvector) with [eigenvalue](linear-operator-theory.md#eigenvalue) one, so the exact solution is

$$
x(t)=e^{-t}(1,0,-1)^T.
$$

More generally, an [eigenvector](linear-operator-theory.md#eigenvector) with [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda$ decays by $e^{-\lambda t}$. The [spectral theorem for real symmetric matrices](linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) supplies an [orthonormal basis](inner-product.md#orthonormal-basis) of these [eigenvectors](linear-operator-theory.md#eigenvector), and the [kernel of a graph Laplacian](#kernel-of-a-graph-laplacian) identifies the surviving terms. On a nonempty [connected graph](graph.md#connected-graph),

$$
\lim_{t\to\infty}x(t)=\bar x\mathbf1,\qquad \bar x=\frac1{|V|}\sum_i x_i(0).
$$

The limiting value is the original [arithmetic mean](arithmetic.md#arithmetic-mean). On a disconnected [graph](graph.md), each [connected component of a graph](graph.md#component-graph-theory) converges to its own original [arithmetic mean](arithmetic.md#arithmetic-mean). The same [matrix](vector-space.md#matrix) therefore measures neighbour disagreement, detects disconnected regions and governs relaxation toward agreement.

### Laplacian spectrum of a complete graph

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

The [Graph Laplacian](#laplacian-matrix) of the [complete graph](#complete-graph) $K_n$ has eigenvalue zero on the constant vector and eigenvalue $n$ on the $(n-1)$-dimensional subspace whose coordinates sum to zero.

## Minimum-cost flow problem

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minimum-cost_flow_problem)

A minimum-cost flow minimizes a linear edge cost subject to vertex flow balances and edge capacity intervals. Subtracting every lower capacity from its edge flow converts all lower bounds to zero while shifting the balance vector and objective by constants.

### Minimum-cost maximum flow

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

A maximum-value feasible network flow chosen to have the least total cost among all maximum-value flows. It combines a maximum-flow objective with a [minimum-cost flow](#minimum-cost-flow-problem) objective.

### Two-resource path packing as minimum-cost circulation

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

Consider nonnegative route variables with constraints $u\leq a$, $v\leq b$, $v+w\leq c$, $w+z\leq d$, and a linear reward $p_u u+p_v v+p_w w+p_z z$. It is a [minimum-cost flow](#minimum-cost-flow-problem) problem: use arcs $s\to t$ of capacity $a$ and cost $-p_u$, $s\to L$ of capacity $c$ and cost zero, $L\to t$ of capacity $b$ and cost $-p_v$, $L\to R$ of unlimited capacity and cost $-p_w$, $s\to R$ of unlimited capacity and cost $-p_z$, and $R\to t$ of capacity $d$ and cost zero. Close the network by an unlimited zero-cost arc $t\to s$. The four forward path flows are exactly $u,v,w,z$, so conservation gives the resource constraints. This reduction does not assert that general multi-commodity flow is ordinary minimum-cost flow.

### Feasible flow

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

A feasible flow satisfies every [flow balance](#flow-balance) and every capacity interval of a network problem. Feasibility is distinct from optimality: [capacitated flow optimality conditions](#capacitated-flow-optimality-conditions) additionally certify that no allowed balanced flow displacement reduces the cost. With only one independent [graph cycle](#cycle-in-a-graph), every balanced flow is determined by a single cycle parameter, and its feasible set is the intersection of the induced parameter intervals.

### Capacitated flow optimality conditions

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

For positive capacities and a feasible flow, optimality is equivalent to [network dual potentials](#network-dual-potential) for which the [network reduced cost](#network-reduced-cost) is nonnegative at a lower bound, zero in the interior, and nonpositive at an upper bound. These signs make every feasible displacement nonnegative in total cost. They are also equivalent to absence of negative-cost cycles in the [residual network](flow-network.md#residual-network). A zero-capacity edge is fixed and imposes no reduced-cost sign condition.

### Flow balance

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

A flow balance prescribes net outgoing minus incoming flow at a vertex. Positive $b_i$ is supply and negative $b_i$ is demand; zero is ordinary [flow conservation](flow-network.md#flow-conservation). Summing all balances requires total supply to equal total demand. In a [directed graph](#directed-graph), these equations are represented by the [oriented incidence matrix](graph.md#oriented-incidence-matrix).

### Uncapacitated minimum-cost flow

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

An uncapacitated [minimum-cost flow](#minimum-cost-flow-problem) has nonnegative edge flows without finite upper capacities. The [flow balances](#flow-balance) prescribe net supply at each vertex. For the [oriented incidence matrix](graph.md#oriented-incidence-matrix) convention with tail $+1$ and head $-1$, vertex [network dual potentials](#network-dual-potential) have [network reduced costs](#network-reduced-cost) $c_{ij}-\pi_i+\pi_j$. Nonnegative [network reduced costs](#network-reduced-cost) and [complementary slackness](linear-programming.md#complementary-slackness) certify a feasible optimum. A feasible negative-cost directed cycle makes the problem unbounded below.

#### Network dual potential

↑ **Parent:** [Uncapacitated minimum-cost flow](#uncapacitated-minimum-cost-flow)

A vertex potential in the dual of an [uncapacitated minimum-cost flow](#uncapacitated-minimum-cost-flow) yields the edge inequalities $\pi_i-\pi_j\leq c_{ij}$. Its objective is $\sum_i\pi_i b_i$. Adding a common constant leaves all [network reduced costs](#network-reduced-cost) and the objective unchanged when total net supply is zero. Potentials tight on a [spanning tree](tree-graph-theory.md#spanning-tree) are fixed up to this common constant.

##### Dual network potentials from shortest-path distances

↑ **Parent:** [Network dual potential](#network-dual-potential)

In a directed network with no negative-cost directed cycle, add a source having zero-cost arcs to all vertices and compute shortest-path distances $d_i$. The inequalities $d_j\le d_i+c_{ij}$ make $\pi_i=-d_i$ dual feasible for [uncapacitated minimum-cost flow](#uncapacitated-minimum-cost-flow). Shortest-path tree arcs are tight. An arbitrary spanning tree also fixes tight candidate potentials up to a constant, but it does not guarantee the non-tree inequalities; these must be checked.

##### Network reduced cost

↑ **Parent:** [Network dual potential](#network-dual-potential)

With the tail-positive incidence convention, a network edge's reduced cost is $r_{ij}=c_{ij}-\pi_i+\pi_j$. For [uncapacitated minimum-cost flow](#uncapacitated-minimum-cost-flow), dual feasibility requires $r_{ij}\geq0$ and [complementary slackness](linear-programming.md#complementary-slackness) requires $f_{ij}r_{ij}=0$. A negative non-tree reduced cost identifies an improving [graph cycle](#cycle-in-a-graph) pivot in the [network simplex algorithm](#network-simplex-algorithm). This sign convention differs from the row-column potentials of a [transportation problem](linear-programming.md#transportation-problem).

### Network simplex algorithm

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

The network simplex algorithm specializes the [simplex algorithm](numerical-analysis.md#simplex-algorithm) to network flows. A basis is represented by a spanning tree with nonbasic flows at their bounds; potentials give [reduced costs](linear-programming.md#reduced-cost), and entering arcs produce cycle pivots. [Degeneracy in linear programming](linear-programming.md#degeneracy-in-linear-programming) is particularly common in assignment instances.

#### Network simplex tree basis

↑ **Parent:** [Network simplex algorithm](#network-simplex-algorithm)

For a connected capacitated [minimum-cost flow](#minimum-cost-flow-problem) network, a [spanning tree](tree-graph-theory.md#spanning-tree) supplies basic flow variables. Every non-tree edge is fixed at its lower or upper bound. [Flow balance](#flow-balance) determines the tree flows; these must also obey [capacity constraints](flow-network.md#capacity-constraint). An entering edge creates one cycle, and adjusting flow on that cycle preserves balance until a bound is hit and an edge leaves the tree.

## Extremal graph theory

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](extremal-graph-theory.md)

## Flow network

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](flow-network.md)

## Eulerian graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eulerian_graph)

An [Eulerian graph](#eulerian-graph) has an [Euler circuit](#euler-circuit): a closed [trail](#trail-in-a-graph) traversing every [edge](#edge-of-a-graph) exactly once. Here the [graph](graph.md) is a finite [undirected graph](#undirected-graph), possibly a [multigraph](graph.md#multigraph) with [self-loops](graph.md#loop-graph-theory). Parallel [edges](#edge-of-a-graph) retain distinct identities, and each [self-loop](graph.md#loop-graph-theory) contributes two to its [vertex degree](#degree-graph-theory). Repeated [vertices](graph.md#vertex-graph-theory) are allowed. This models inspecting every road segment once, even when a junction must be revisited.

For a nonempty set of [edges](#edge-of-a-graph), the [Euler circuit criterion](#euler-circuit-criterion) requires a [connected graph](graph.md#connected-graph) only on the [edge support of a graph](#edge-support-of-a-graph): [isolated vertices](random-graph.md#isolated-vertex) impose no travel requirement. A single [vertex](graph.md#vertex-graph-theory) with a [self-loop](graph.md#loop-graph-theory) and two [vertices](graph.md#vertex-graph-theory) joined by two parallel [edges](#edge-of-a-graph) are both [Eulerian graphs](#eulerian-graph). Neither requires three [vertices](graph.md#vertex-graph-theory). With no [edges](#edge-of-a-graph) and at least one [vertex](graph.md#vertex-graph-theory), we allow the zero-length [trail](#trail-in-a-graph) at that [vertex](graph.md#vertex-graph-theory) as an [Euler circuit](#euler-circuit); the [graph](graph.md) with no [vertices](graph.md#vertex-graph-theory) has no such [walk](#walk-in-a-graph).

The motivating [Seven Bridges of Königsberg](#seven-bridges-of-konigsberg) problem asks for an [Eulerian trail](#eulerian-trail), which need not return to its starting [vertex](graph.md#vertex-graph-theory). In [Leonhard Euler](mathematics.md#leonhard-euler)'s [Solutio problematis ad geometriam situs pertinentis by Leonhard Euler](mathematics-bibliography.md#solutio-problematis-ad-geometriam-situs-pertinentis-by-leonhard-euler), §2 poses the bridge-crossing question and §§4–6 encode land regions by letters. The river's shape drops out: only the connections matter. The paper was written in 1735 and published in 1741, according to the Euler Archive; the journal volume carries the nominal year 1736.[Euler Archive, E53: Solutio problematis ad geometriam situs pertinentis](mathematics-bibliography.md#euler-archive-e53-solutio-problematis-ad-geometriam-situs-pertinentis)

### Edge support of a graph

↑ **Parent:** [Eulerian graph](#eulerian-graph)

For a finite undirected [multigraph](graph.md#multigraph) $G=(V,E)$, its [edge support of a graph](#edge-support-of-a-graph) is the [subgraph](#subgraph) $G_+=(V_+,E)$ with $V_+=\{v\in V:\deg(v)>0\}$. It removes exactly the [isolated vertices](random-graph.md#isolated-vertex), retaining every [edge](#edge-of-a-graph), including [self-loops](graph.md#loop-graph-theory) and parallel [edges](#edge-of-a-graph). When $E\ne\varnothing$, connectivity of this [subgraph](#subgraph) is the relevant condition for an [Eulerian trail](#eulerian-trail) or [Euler circuit](#euler-circuit).

<h3 id="seven-bridges-of-konigsberg">Seven Bridges of Königsberg</h3>

↑ **Parent:** [Eulerian graph](#eulerian-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seven_Bridges_of_Königsberg)

Model the four land regions by [vertices](graph.md#vertex-graph-theory) $A,B,C,D$ and the seven bridges by distinct [edges](#edge-of-a-graph): two $AB$, two $AC$, and one each of $AD,BD,CD$. Their [vertex degrees](#degree-graph-theory) are $(5,3,3,3)$. [Leonhard Euler](mathematics.md#leonhard-euler)'s paper records these connections in §6 and the obstruction in §9; §20 states the zero-or-two odd-region rule. Four odd [vertex degrees](#degree-graph-theory) exclude an [Eulerian trail](#eulerian-trail), even if returning to the starting [vertex](graph.md#vertex-graph-theory) is optional.[§§6, 9, 20](mathematics-bibliography.md#solutio-problematis-ad-geometriam-situs-pertinentis-by-leonhard-euler)

### Eulerian trail

↑ **Parent:** [Eulerian graph](#eulerian-graph)

An [Eulerian trail](#eulerian-trail), also called an [Eulerian path](#eulerian-trail), is a [trail in a graph](#trail-in-a-graph) traversing every [edge](#edge-of-a-graph) exactly once. The name [Eulerian path](#eulerian-trail) does not require a [graph path](#path-in-a-graph): [vertices](graph.md#vertex-graph-theory) may repeat. A [Hamiltonian path](#hamiltonian-path) instead visits every [vertex](graph.md#vertex-graph-theory) exactly once, and may omit [edges](#edge-of-a-graph). An [Eulerian trail](#eulerian-trail) may omit [isolated vertices](random-graph.md#isolated-vertex), so these are different coverage requirements.

For a finite undirected [multigraph](graph.md#multigraph) with at least one [edge](#edge-of-a-graph), allowing [self-loops](graph.md#loop-graph-theory), an [Eulerian trail](#eulerian-trail) exists exactly when the [edge support of a graph](#edge-support-of-a-graph) is a [connected graph](graph.md#connected-graph) and there are zero or two [vertices](graph.md#vertex-graph-theory) of odd [vertex degree](#degree-graph-theory). In the two-odd-[vertex](graph.md#vertex-graph-theory) case they must be the two distinct endpoints; in the zero-odd-[vertex](graph.md#vertex-graph-theory) case every [Eulerian trail](#eulerian-trail) is an [Euler circuit](#euler-circuit). Count a [self-loop](graph.md#loop-graph-theory) twice in the [vertex degree](#degree-graph-theory) but once in the [trail](#trail-in-a-graph), and count each parallel [edge](#edge-of-a-graph) separately.[pp. 1–3, Theorem 1.1.2 and the note about isolated vertices](mathematics-bibliography.md#math-530-graph-theory-combinatorial-mathematics-i-spring-2023/math-530-spring-2023-lecture-6-multigraphs-and-digraphs)

The [parity](quantum-mechanics.md#parity) obstruction is local: each intermediate visit pairs an arriving [edge](#edge-of-a-graph) with a departing [edge](#edge-of-a-graph). Only the distinct endpoints can have an unpaired incidence. The [handshaking lemma](combinatorics.md#degree-sum-formula), $\sum_{v\in V}\deg(v)=2|E|$, also shows that the number of [vertices](graph.md#vertex-graph-theory) with odd [vertex degree](#degree-graph-theory) is even. Sufficiency in the two-endpoint case reduces to the [Euler circuit criterion](#euler-circuit-criterion): add one extra [edge](#edge-of-a-graph) between the odd [vertices](graph.md#vertex-graph-theory), construct an [Euler circuit](#euler-circuit), rotate its record to start with the extra [edge](#edge-of-a-graph), then delete that [edge](#edge-of-a-graph). The remaining [trail](#trail-in-a-graph) has the required endpoints.

For the [Seven Bridges of Königsberg](#seven-bridges-of-konigsberg) [multigraph](graph.md#multigraph), the [vertex degrees](#degree-graph-theory) at $A,B,C,D$ are $(5,3,3,3)$, so no [Eulerian trail](#eulerian-trail) exists. Remove the unique [edge](#edge-of-a-graph) $AD$: the [vertex degrees](#degree-graph-theory) become $(4,3,3,2)$, and a six-[edge](#edge-of-a-graph) [Eulerian trail](#eulerian-trail) runs from $B$ to $C$. Label the parallel [edges](#edge-of-a-graph) $p_1,p_2$ between $A,B$ and $q_1,q_2$ between $A,C$; label $BD$ by $r$ and $CD$ by $s$. A complete record is $B,p_1,A,q_1,C,s,D,r,B,p_2,A,q_2,C$. It revisits $A,B,C$ while using every remaining [edge](#edge-of-a-graph) once.

<a id="image-four-odd-vertex-degrees-forbid-an-eulerian-trail-two-allow-distinct-endpoints-zero-allow-an-euler-circuit"></a>
![](eulerian-degree-parity-multigraphs.png)

**[Figure 19](#image-four-odd-vertex-degrees-forbid-an-eulerian-trail-two-allow-distinct-endpoints-zero-allow-an-euler-circuit). Four odd vertex degrees forbid an Eulerian trail; two allow distinct endpoints; zero allow an Euler circuit**.

#### Eulerian cycle

↑ **Parent:** [Eulerian trail](#eulerian-trail)

A [closed walk](#closed-walk) in a [graph](graph.md) that traverses each [edge](#edge-of-a-graph) exactly once. [Vertices](graph.md#vertex-graph-theory) may be revisited; the restriction concerns [edges](#edge-of-a-graph).

### Euler circuit

↑ **Parent:** [Eulerian graph](#eulerian-graph)

An [Euler circuit](#euler-circuit), also called an [Euler tour](#euler-circuit), is an [Eulerian trail](#eulerian-trail) whose final [vertex](graph.md#vertex-graph-theory) equals its initial [vertex](graph.md#vertex-graph-theory). Its length is $|E|$. It can revisit other [vertices](graph.md#vertex-graph-theory), unlike a [Hamiltonian cycle](#hamilton-cycle), which visits each [vertex](graph.md#vertex-graph-theory) once before returning to the start. For a finite undirected [multigraph](graph.md#multigraph) with at least one [edge](#edge-of-a-graph), an [Euler circuit](#euler-circuit) exists exactly when the [edge support of a graph](#edge-support-of-a-graph) is a [connected graph](graph.md#connected-graph) and every [vertex degree](#degree-graph-theory) is even.

For example, let $p,q$ be distinct parallel [edges](#edge-of-a-graph) joining $A,B$, let $\ell$ be a [self-loop](graph.md#loop-graph-theory) at $A$, and add an [isolated vertex](random-graph.md#isolated-vertex) $Z$. Then $(\deg(A),\deg(B),\deg(Z))=(4,2,0)$, and $A,\ell,A,p,B,q,A$ is an [Euler tour](#euler-circuit). The [self-loop](graph.md#loop-graph-theory) supplies one traversal and two incidences; $Z$ need not be visited. Replacing $p,q$ by a single [edge](#edge-of-a-graph) changes both [vertex degrees](#degree-graph-theory) to odd numbers and removes the possibility of an [Euler circuit](#euler-circuit). Thus collapsing parallel [edges](#edge-of-a-graph) can change the answer.

Two [triangles in a graph](graph.md#triangle-in-a-graph) sharing one [vertex](graph.md#vertex-graph-theory) $A$ give another instructive [Euler circuit](#euler-circuit): $A,B,C,A,D,E,A$. The shared [vertex](graph.md#vertex-graph-theory) has [vertex degree](#degree-graph-theory) four, the others have [vertex degree](#degree-graph-theory) two, and $A$ is revisited between the two closed [trails](#trail-in-a-graph). This is precisely the splice used by [Hierholzer's algorithm](#hierholzer-s-algorithm).

### Euler circuit criterion

↑ **Parent:** [Eulerian graph](#eulerian-graph)

Let $G=(V,E)$ be a finite undirected [multigraph](graph.md#multigraph), allowing [self-loops](graph.md#loop-graph-theory) and distinct parallel [edges](#edge-of-a-graph), with $E\ne\varnothing$. Then

$$
G\text{ has an Euler circuit}\quad\Longleftrightarrow\quad G_+\text{ is connected and }\deg(v)\equiv0\pmod2\text{ for every }v\in V,
$$

where $G_+$ is the [edge support of a graph](#edge-support-of-a-graph), and [vertex degrees](#degree-graph-theory) count each [self-loop](graph.md#loop-graph-theory) twice. There is no lower bound of three on the number of [vertices](graph.md#vertex-graph-theory). If $E=\varnothing$, the zero-length convention gives an [Euler circuit](#euler-circuit) exactly when $V\ne\varnothing$.[p. 1, Theorem 1.1.2(a) and isolated-vertex note; p. 2, trivial trail convention](mathematics-bibliography.md#math-530-graph-theory-combinatorial-mathematics-i-spring-2023/math-530-spring-2023-lecture-6-multigraphs-and-digraphs)

The two requirements are independent: two separate [vertices](graph.md#vertex-graph-theory), each carrying a [self-loop](graph.md#loop-graph-theory), have even [vertex degrees](#degree-graph-theory) but disconnected [edge support of a graph](#edge-support-of-a-graph), so no [Euler circuit](#euler-circuit) can cover both [edges](#edge-of-a-graph).

Necessity follows because a single [trail](#trail-in-a-graph) cannot cover [edges](#edge-of-a-graph) in different [connected components of a graph](graph.md#component-graph-theory), while a closed [trail](#trail-in-a-graph) pairs all arriving and departing incidences, including those at its starting [vertex](graph.md#vertex-graph-theory). For sufficiency, extend a [trail](#trail-in-a-graph) using unused [edges](#edge-of-a-graph) until no extension is possible. Even [vertex degree](#degree-graph-theory) [parity](quantum-mechanics.md#parity) prevents it from stopping anywhere except its starting [vertex](graph.md#vertex-graph-theory): a different stopping [vertex](graph.md#vertex-graph-theory) would have an odd number of used incidences and hence at least one unused incidence. The result is a closed [trail](#trail-in-a-graph).

If unused [edges](#edge-of-a-graph) remain, connectivity of the [edge support of a graph](#edge-support-of-a-graph) supplies a [vertex](graph.md#vertex-graph-theory) on the current closed [trail](#trail-in-a-graph) with an unused incident [edge](#edge-of-a-graph). Removing a closed [trail](#trail-in-a-graph) leaves even unused [vertex degrees](#degree-graph-theory), so the same argument constructs another closed [trail](#trail-in-a-graph) from that [vertex](graph.md#vertex-graph-theory). Splice it into the existing record. The two [trails](#trail-in-a-graph) use disjoint [edge](#edge-of-a-graph) identities, so the splice repeats no [edge](#edge-of-a-graph). Each splice uses more [edges](#edge-of-a-graph); finiteness ensures termination with an [Euler circuit](#euler-circuit). This is the constructive idea of [Hierholzer's algorithm](#hierholzer-s-algorithm).

<a id="image-hierholzer-s-algorithm-inserts-one-closed-trail-into-another-at-their-shared-vertex-using-each-of-six-edges-exactly-once"></a>
![](hierholzer-closed-trail-splicing.png)

**[Figure 20](#image-hierholzer-s-algorithm-inserts-one-closed-trail-into-another-at-their-shared-vertex-using-each-of-six-edges-exactly-once). Hierholzer's algorithm inserts one closed trail into another at their shared vertex, using each of six edges exactly once**.

In the drawing, arrows indicate the chosen traversal direction along undirected [edges](#edge-of-a-graph). The first closed [trail](#trail-in-a-graph) uses $AB,BC,CA$ and the second uses $AD,DE,EA$. Insert the second at the final occurrence of $A$ in $A,B,C,A$, giving $A,B,C,A,D,E,A$. A reader can check consecutive endpoints, closure, and the six distinct [edges](#edge-of-a-graph) directly. With [multigraphs](graph.md#multigraph), perform the same check on [edge](#edge-of-a-graph) identities, since endpoint pairs alone cannot distinguish parallel [edges](#edge-of-a-graph).

<h4 id="hierholzer-s-algorithm">Hierholzer's algorithm</h4>

↑ **Parent:** [Euler circuit criterion](#euler-circuit-criterion)

[Hierholzer's algorithm](#hierholzer-s-algorithm) constructs an [Euler circuit](#euler-circuit) by growing closed [trails](#trail-in-a-graph) along unused [edges](#edge-of-a-graph) and splicing them at shared [vertices](graph.md#vertex-graph-theory), as in the [Euler circuit criterion](#euler-circuit-criterion). Each [edge](#edge-of-a-graph) must have a distinct record. An implementation using [adjacency lists](data-structure.md#adjacency-list), a [stack](data-structure.md#stack-data-structure), and a used flag for each [edge](#edge-of-a-graph) runs in $O(|V|+|E|)$ time, including the connectivity and [vertex degree](#degree-graph-theory) checks. Store both incidences of a [self-loop](graph.md#loop-graph-theory), while marking its single [edge](#edge-of-a-graph) record used only once.

## Line graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Line_graph)

The line graph $L(G)$ has one vertex for each edge of $G$, with adjacency when two original edges share an endpoint.

### Line graph of a regular graph is Eulerian

↑ **Parent:** [Line graph](#line-graph)

If $G$ is connected and $r$-regular, then $L(G)$ is connected and every one of its vertices has degree $2r-2$. The [Euler circuit criterion](#euler-circuit-criterion) therefore applies.

## Graph drawing

↑ **Parent:** [Graph theory](graph-theory.md)

A [graph drawing](#graph-drawing) represents [vertices](graph.md#vertex-graph-theory) by distinct points in the [Euclidean plane](geometry-and-topology.md#euclidean-plane) and [edges](#edge-of-a-graph) by curves joining their endpoints. A crossing of [edges](#edge-of-a-graph) is not an extra [vertex](graph.md#vertex-graph-theory) unless we explicitly change the [graph](graph.md) to make it one. Curves may bend: the [graph](graph.md) records connections, not coordinates.

## Planar graph

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](planar-graph.md)

## Crossing number

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crossing_number)

The crossing number of a graph is the minimum number of edge-crossing pairs among its plane drawings. For a fixed drawing, deleting at most one edge per crossing pair leaves a planar graph.

### Crossing lemma

↑ **Parent:** [Crossing number](#crossing-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crossing_lemma)

If a simple graph has $n$ vertices and $e\geq4n$ edges, every plane drawing has at least

$$
\frac{e^3}{64n^2}
$$

crossings. Apply the linear planar bound to the random induced subgraph obtained by retaining vertices independently with probability $4n/e$.

#### Crossing lemma for multigraphs

↑ **Parent:** [Crossing lemma](#crossing-lemma)

Here a loopless [multigraph](graph.md#multigraph) has $v$ [vertices](graph.md#vertex-graph-theory), $e$ [edges](#edge-of-a-graph), and at most $\mu$ parallel [edges](#edge-of-a-graph) per pair. In a minimum-crossing drawing, crossings between incident [edges](#edge-of-a-graph) can be removed by exchanging their initial segments, so every crossing involves four distinct [vertices](graph.md#vertex-graph-theory). For each parallel class choose an [edge](#edge-of-a-graph) with probability $1/\mu$ per [edge](#edge-of-a-graph), with the remaining probability choosing none. Retain [vertices](graph.md#vertex-graph-theory) independently with probability $p$. The sampled [simple graph](graph.md#simple-graph) has expected [edge](#edge-of-a-graph) count $p^2e/\mu$, expected [vertex](graph.md#vertex-graph-theory) count $pv$, and expected crossing count $p^4\operatorname{cr}(G)/\mu^2$. Deleting one [edge](#edge-of-a-graph) per crossing and using the [planar graph edge bound](planar-graph.md#planar-graph-edge-bound) gives $p^4\operatorname{cr}(G)/\mu^2\geq p^2e/\mu-3pv$. Choose $p=4\mu v/e$.

## Graph neighbourhood

↑ **Parent:** [Graph theory](graph-theory.md)

The neighbourhood $N(S)$ of a vertex set $S$ consists of all vertices adjacent to at least one vertex of $S$.

### Neighbour of a vertex

↑ **Parent:** [Graph neighbourhood](#graph-neighbourhood)

A neighbour of a [vertex](graph.md#vertex-graph-theory) $v$ in a [graph](graph.md) is a [vertex](graph.md#vertex-graph-theory) joined to $v$ by an [edge](#edge-of-a-graph). These [vertices](graph.md#vertex-graph-theory) form the [graph neighbourhood](#graph-neighbourhood) $N(v)$.

### Closed graph neighbourhood

↑ **Parent:** [Graph neighbourhood](#graph-neighbourhood)

The closed neighbourhood of a vertex set is $N[S]=S\cup N(S)$.

### External vertex boundary

↑ **Parent:** [Graph neighbourhood](#graph-neighbourhood)

The external vertex boundary of a vertex set $S$ is

$$
\partial_vS=N(S)\setminus S=N[S]\setminus S.
$$

For comparisons at fixed $|S|$, minimizing $|\partial_vS|$ is equivalent to minimizing $|N[S]|$.

### Common neighbour

↑ **Parent:** [Graph neighbourhood](#graph-neighbourhood)

A common neighbour of vertices $u$ and $v$ is adjacent to both of them.

## Degree (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Degree_(graph_theory))

The degree of a vertex is the number of edges incident with it, equivalently the cardinality of its neighbourhood in a simple graph.

### In-degree

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)

### Degree sequence

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)

The degree sequence of a labelled [graph](graph.md) records the [degree of a vertex](#degree-graph-theory) at each label. The [handshaking lemma](combinatorics.md#degree-sum-formula) gives $\sum_i d_i=2|E|$. A nonincreasing list forgets the assignment of degrees to labels unless a particular ordering is specified.

### Outdegree

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)

The number of edges of a [directed graph](#directed-graph) directed away from a given vertex. Assigning directions to undirected edges is an [orientation of a graph](#orientation-of-a-graph).

### Average degree of a graph

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)

The average [vertex degree](#degree-graph-theory) of a [graph](graph.md) is the sum of its vertex degrees divided by its order. [Double counting](combinatorics.md#double-counting-proof-technique) edge endpoints gives $\overline d(G)=2e(G)/|V(G)|$. It lies between the [minimum degree of a graph](#minimum-degree-of-a-graph) and the [maximum degree of a graph](#maximum-degree-of-a-graph).

### Regular graph

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_graph)

A graph is $d$-regular when every vertex has degree $d$.

#### Nested matching criterion for a regular subgraph

↑ **Parent:** [Regular graph](#regular-graph)

Let $p$ be [prime](prime-number.md) and set $s=2p-2$. If a [bipartite graph](bipartite-graph.md) has edge-disjoint [perfect matchings](matching-graph-theory.md#perfect-matching) $M_0,\ldots,M_{\sigma-1}$ on nested nonempty [vertex](graph.md#vertex-graph-theory) sets, and $|V(M_{i+s})|>s|V(M_i)|/(s+1)$, then the union of $s+1$ consecutive [matchings in a graph](matching-graph-theory.md) has maximum degree at most $2p-1$ and more than $(p-1)|V(M_i)|$ [edges](#edge-of-a-graph). The [prime-regular subgraph from Boolean polynomial constraints](combinatorics.md#prime-regular-subgraph-from-boolean-polynomial-constraints) gives a $p$-regular subgraph. Its [perfect matching](matching-graph-theory.md#perfect-matching) decomposition gives a $k$-regular subgraph for every $k\leq p$. If none exists, every $s$ steps shrink the [vertex](graph.md#vertex-graph-theory) set by factor at most $s/(s+1)$, bounding $\sigma$ by a constant times $\log n$.

#### Short-cycle expectation in a uniform regular graph

↑ **Parent:** [Regular graph](#regular-graph)

For fixed $r,\ell\geq3$ and $rn$ even, a prescribed [graph cycle](#cycle-in-a-graph) in the [configuration model](random-graph.md#configuration-model) has two ordered distinct half-edges at each of its vertices. Therefore its expected count is $(n)_\ell[r(r-1)]^\ell/[2\ell\prod_{j=0}^{\ell-1}(rn-2j-1)]$. Conditioning on the chosen cycle leaves degrees $r-2$ at its vertices and $r$ elsewhere; forbid further edges along that cycle. The [bounded-degree pairing avoidance estimate](random-graph.md#bounded-degree-pairing-avoidance-estimate) changes by $o(1)$, so the simplicity probability conditional on the cycle divided by the unconditional probability tends to one. The displayed expectation therefore holds for the uniform [simple graph](graph.md#simple-graph), not just the unconditioned pairing model.

#### Petersen graph

↑ **Parent:** [Regular graph](#regular-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Petersen_graph)

The [graph](graph.md) whose vertices are two-element subsets of a five-element set, with two vertices adjacent when the subsets are disjoint. It has ten vertices, degree three, zero common neighbours for adjacent pairs and one for nonadjacent pairs. Its [adjacency matrix of a graph](#adjacency-matrix) satisfies $A^2+A-2I=J$ and has [eigenvalues](linear-operator-theory.md#eigenvalue) $3,1,-2$ of multiplicities $1,5,4$.

#### Constant eigenvector of a regular graph

↑ **Parent:** [Regular graph](#regular-graph)

If $A$ is the adjacency matrix of a $d$-regular graph and $\mathbf e=(1,\ldots,1)^T$, every row sum of $A$ is $d$, so

$$
A\mathbf e=d\mathbf e.
$$

If the graph is connected, the $d$-eigenspace is exactly $\operatorname{span}\{\mathbf e\}$.

#### Connected regular graph with two adjacency eigenvalues

↑ **Parent:** [Regular graph](#regular-graph)

A connected regular graph has exactly two distinct adjacency eigenvalues if and only if it is a [complete graph](#complete-graph) $K_n$ with $n\geq2$. Its eigenvalues are $n-1$ on the constant vectors and $-1$ on their orthogonal complement.

### Degree-biased vertex distribution

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)

In a finite graph with at least one edge, the degree-biased vertex distribution assigns probability proportional to the [degree of a vertex](#degree-graph-theory). It is the distribution of an endpoint on a specified side of a uniformly random edge.

### Universal vertex

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Universal_vertex)

A universal vertex is adjacent to every other vertex of its graph.

### Minimum degree of a graph

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)

The minimum degree $\delta(G)$ is the least degree of a vertex of $G$.

The minimum degree is $\delta(G)=\min_{v\in V(G)}\deg(v)$, the least [degree of a vertex](#degree-graph-theory) in the graph.

### Maximum degree of a graph

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)

The maximum degree $\Delta(G)$ is the greatest degree of a vertex of $G$.

It is the maximum of the [degree of a vertex](#degree-graph-theory) over all vertices.

### Locally finite graph

↑ **Parent:** [Degree (graph theory)](#degree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locally_finite_graph)

A graph is locally finite when every vertex has finite degree.

#### Graph exhaustion

↑ **Parent:** [Locally finite graph](#locally-finite-graph)

An exhaustion of a countable [graph](graph.md) is an increasing [sequence](sequence-and-series.md#sequence) of finite connected [graph vertex](graph.md#vertex-graph-theory) sets whose union is the whole [graph vertex](graph.md#vertex-graph-theory) set. In a [locally finite graph](#locally-finite-graph), every prescribed finite [graph path](#path-in-a-graph) together with all [graph neighbours](#neighbour-of-a-vertex) of its visited [graph vertices](graph.md#vertex-graph-theory) lies in a sufficiently large exhaustion set. This permits coupling finite-volume and infinite-volume [simple random walks](random-walk.md#simple-random-walk) up to a finite stopping time.

## Cut (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cut_(graph_theory))

A cut is a partition $V=A\sqcup B$ of the vertex set. Its size is the number of edges with one endpoint in each part.

### Edge cutset

↑ **Parent:** [Cut (graph theory)](#cut-graph-theory)

An edge cutset separating two vertices is a set of edges whose removal leaves no [path in a graph](#path-in-a-graph) between those vertices. For a vertex set containing exactly one of the two vertices, its [edge boundary](analysis-of-boolean-functions.md#edge-boundary-in-a-graph) is such a cutset.

### Maximum cut

↑ **Parent:** [Cut (graph theory)](#cut-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_cut)

A maximum cut has greatest size among all cuts of a finite graph.

### Random cut lower bound

↑ **Parent:** [Cut (graph theory)](#cut-graph-theory)

Every finite graph with $m$ edges has a [cut of a graph](#cut-graph-theory) of size at least $m/2$, and hence a spanning [bipartite graph](bipartite-graph.md) with at least $m/2$ edges. Put each vertex independently on either side with equal probability. Every edge crosses with probability $1/2$, so [linearity of expectation](expected-value.md#linearity-of-expectation) gives expected cut size $m/2$.

#### Balanced random cut lower bound

↑ **Parent:** [Random cut lower bound](#random-cut-lower-bound)

If a graph has even order $n$ and $m$ edges, it has a cut with equally sized parts and at least

$$
\frac{mn}{2(n-1)}
$$

crossing edges. Choose one part uniformly among the $n/2$-vertex subsets. A fixed edge is separated with probability

$$
2\frac{n/2}{n}\frac{n/2}{n-1}=\frac{n}{2(n-1)},
$$

and apply [linearity of expectation](expected-value.md#linearity-of-expectation).

### Unfriendly partition

↑ **Parent:** [Cut (graph theory)](#cut-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unfriendly_partition)

An unfriendly partition $V=A\sqcup B$ puts at least as many neighbours of every vertex in the opposite part as in its own part.

#### Unfriendly partition theorem for a finite graph

↑ **Parent:** [Unfriendly partition](#unfriendly-partition)

Every finite graph has an unfriendly partition. In a maximum cut, moving any vertex to the other side cannot increase the number of crossing edges, which is exactly the required neighbour inequality.

#### Unfriendly partition theorem for a countable locally finite graph

↑ **Parent:** [Unfriendly partition](#unfriendly-partition)

Take unfriendly partitions of an exhaustion by finite induced subgraphs and use a diagonal subsequence to stabilize the colour of each vertex. Local finiteness makes every neighbourhood stabilize after finitely many steps, so each unfriendly inequality passes to the limit.

#### Random unfriendly partition of a countable infinite-degree graph

↑ **Parent:** [Unfriendly partition](#unfriendly-partition)

Independently colour the vertices of a countable graph red or blue with equal probabilities. If every vertex has infinite degree, then each fixed vertex has infinitely many neighbours of each colour almost surely. A countable union of the exceptional null events is null, so such a colouring exists.

## Bipartite graph

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](bipartite-graph.md)

## Graph homomorphism

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_homomorphism)

A graph homomorphism from $H$ to $G$ is a [function](function.md) $f:V(H)\to V(G)$ that sends every edge $uv$ of $H$ to an edge $f(u)f(v)$ of $G$.

### Graph embedding

↑ **Parent:** [Graph homomorphism](#graph-homomorphism)

A graph embedding in the subgraph sense is an [injective](algebra.md#injective-function) [graph homomorphism](#graph-homomorphism). It preserves edges, while it may send a nonedge to an edge. An induced embedding additionally preserves nonedges. For [directed graphs](#directed-graph), every prescribed arrow must be preserved.

### Homomorphism density

↑ **Parent:** [Graph homomorphism](#graph-homomorphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homomorphism_density)

For finite graphs $H,G$, the homomorphism density $t(H,G)$ is the probability that a uniformly random map $V(H)\to V(G)$ is a [graph homomorphism](#graph-homomorphism). For bipartite graphs with prescribed vertex classes, the random map is chosen separately and uniformly into the corresponding classes.

#### Sidorenko conjecture

↑ **Parent:** [Homomorphism density](#homomorphism-density)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sidorenko_conjecture)

The Sidorenko conjecture states that every [bipartite graph](bipartite-graph.md) $H$ satisfies

$$
t(H,G)\geq t(K_2,G)^{|E(H)|}
$$

for every bipartite host graph $G$. Thus a random map is at least as likely to preserve every edge as the heuristic that treats the edge constraints independently predicts.

##### Sidorenko inequality for trees

↑ **Parent:** [Sidorenko conjecture](#sidorenko-conjecture)

Every [tree](tree-graph-theory.md) $T$ satisfies the [Sidorenko conjecture](#sidorenko-conjecture). If a bipartite host graph has edge density $\alpha$, then a uniformly random bipartition-respecting map from a $k$-vertex tree into the host is a [graph homomorphism](#graph-homomorphism) with probability at least $\alpha^{k-1}$.

## Directed graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Directed_graph)

A directed graph consists of [vertices](graph.md#vertex-graph-theory) joined by oriented edges.

### Strongly connected component

↑ **Parent:** [Directed graph](#directed-graph)

A strongly connected component is a maximal set of vertices in a [directed graph](#directed-graph) such that each can reach every other by a [directed path](#directed-path).

### Functional graph

↑ **Parent:** [Directed graph](#directed-graph)

A functional graph has exactly one outgoing [edge of a graph](#edge-of-a-graph) at every [vertex of a graph](graph.md#vertex-graph-theory), representing a [function](function.md) from its [vertex of a graph](graph.md#vertex-graph-theory) set to itself. In a finite functional graph, each weakly connected component contains one [directed cycle](#directed-cycle), with directed trees feeding into it. Iterating the represented [function](function.md) eventually reaches that [directed cycle](#directed-cycle).

### Kernel-perfect directed graph

↑ **Parent:** [Directed graph](#directed-graph)

A [digraph kernel](#kernel-of-a-directed-graph) is an [independent set](#independent-set-graph-theory) $K$ of [vertices](graph.md#vertex-graph-theory) such that each vertex outside $K$ has a [directed edge](#directed-edge) from itself to a vertex in $K$. A [directed graph](#directed-graph) is kernel-perfect if every [induced subgraph](#induced-subgraph) has a [digraph kernel](#kernel-of-a-directed-graph). Preference orientations of the [line graph](#line-graph) of a [bipartite graph](bipartite-graph.md) are kernel-perfect: a [stable matching in a bipartite graph](matching-graph-theory.md#stable-matching-in-a-bipartite-graph) is independent in the line graph, and stability supplies the required outgoing edge at every unmatched edge.

#### Kernel list-coloring lemma

↑ **Parent:** [Kernel-perfect directed graph](#kernel-perfect-directed-graph)

In a [kernel-perfect directed graph](#kernel-perfect-directed-graph), lists of size at least $d^+(v)+1$ admit a proper [graph coloring](graph-coloring.md). Choose a color $a$ and a [digraph kernel](#kernel-of-a-directed-graph) in the subgraph on vertices whose lists contain $a$. Color that kernel $a$, delete it, and remove $a$ from the remaining lists. Every vertex losing a color also loses an outgoing neighbour; hence the inequality persists. Induction on the [vertex](graph.md#vertex-graph-theory) count finishes the proof.

### Kernel of a directed graph

↑ **Parent:** [Directed graph](#directed-graph)

A digraph kernel is an [independent set](#independent-set-graph-theory) $K$ such that each [vertex](graph.md#vertex-graph-theory) outside $K$ has a [directed edge](#directed-edge) to a vertex in $K$. A directed cycle of even length has a kernel, obtained by taking alternate vertices; a directed triangle has none. The [kernel-perfect directed graph](#kernel-perfect-directed-graph) property requires existence of such a set in every [induced subgraph](#induced-subgraph).

<h3 id="plunnecke-graph">Plünnecke graph</h3>

↑ **Parent:** [Directed graph](#directed-graph)

A finite directed graph with layers $V_0,\ldots,V_n$ and edges only to the next layer is a Plünnecke graph when every edge $u\to v$ permits both commutation matchings. The successors of $v$ inject into the successors of $u$ through edges to the original successors; the predecessors of $u$ inject into those of $v$ through edges from the original predecessors. These conditions formalize interchanging adjacent summands in an additive graph. They persist on channels consisting of paths between prescribed endpoint sets.

#### Weighted cut lemma for commutative graphs

↑ **Parent:** [Plünnecke graph](#plunnecke-graph)

A minimum-weight set meeting every bottom-to-top path can be chosen entirely in the endpoint layers. The local step is a three-layer channel whose middle layer is a minimum cut. Replacing middle subsets by their successors or predecessors gives expansion inequalities. Sorting middle vertices by incoming degree and top vertices by their largest predecessor degree gives one edge-count inequality; reversing the graph gives the opposite inequality. Equality forces the bottom layer to have the same weight as the middle cut. Replacing the highest intermediate portion of a minimum cut by this bottom layer repeatedly proves the assertion.

#### Graph magnification ratio

↑ **Parent:** [Plünnecke graph](#plunnecke-graph)

This is the smallest ratio of the size of a $k$-step image to the size of its nonempty starting set in the bottom layer. For a [Plünnecke graph](#plunnecke-graph), the roots $D_k^{1/k}$ are nonincreasing. The minimum, rather than just the image of the whole layer, is essential.

### Coherent cyclic order of a digraph

↑ **Parent:** [Directed graph](#directed-graph)

A cyclic ordering of a [directed graph](#directed-graph) is considered unchanged by rotations or swaps of consecutive nonadjacent vertices. A representative is coherent when every backward edge $v_j\to v_i$ has a forward [directed path](#directed-path) from $v_i$ to $v_j$. Equivalently every edge is on a directed circuit that winds exactly once around the order. The number of backward edges on a circuit is invariant under the allowed changes. Every nontrivial [strongly connected directed graph](#strong-connectivity) admits such an order.

#### Cyclic stability of a digraph order

↑ **Parent:** [Coherent cyclic order of a digraph](#coherent-cyclic-order-of-a-digraph)

The cyclic stability is the largest size of an [independent set](#independent-set-graph-theory) appearing consecutively in a representative of a [coherent cyclic order of a digraph](#coherent-cyclic-order-of-a-digraph). It is at most the ordinary [independence number](#independence-number). A set with no forward path between its distinct vertices can be moved into a consecutive block by swapping nonadjacent vertices. Choose a representative minimizing the span of the set; a vertex in a gap can be moved left or right past the block, contradicting minimality unless there are no gaps.

### Tournament (graph theory)

↑ **Parent:** [Directed graph](#directed-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tournament_(graph_theory))

A tournament is an orientation of a [complete graph](#complete-graph): between each pair of distinct [vertices](graph.md#vertex-graph-theory) there is exactly one [directed edge](#directed-edge).

#### Transitive tournament

↑ **Parent:** [Tournament (graph theory)](#tournament-graph-theory)

<h4 id="landau-s-theorem-on-tournament-scores">Landau's theorem on tournament scores</h4>

↑ **Parent:** [Tournament (graph theory)](#tournament-graph-theory)

#### Median order of a tournament

↑ **Parent:** [Tournament (graph theory)](#tournament-graph-theory)

A median order maximizes the number of forward [directed edges](#directed-edge) in a linear ordering of the [vertices](graph.md#vertex-graph-theory) of a [tournament](#tournament-graph-theory). Every interval inherits a median order. Moving the first vertex of an interval to its end proves that it has at least as many outgoing as incoming edges in that interval; otherwise the move would increase the number of forward edges. Reversing all edges and the order gives the dual assertion for the last vertex.

##### Half-sparse median-order embedding

↑ **Parent:** [Median order of a tournament](#median-order-of-a-tournament)

A [graph embedding](#graph-embedding) into an ordered [tournament](#tournament-graph-theory) is half-sparse when the displayed inequality holds for every proper final interval $I$. Reserving two extra tournament vertices allows extension at any outward-oriented leaf: the [median order of a tournament](#median-order-of-a-tournament) supplies at least half of the later vertices as outneighbours of the parent's image, while half-sparsity leaves at least one of them unused. Adding one image while extending every old final interval by two preserves the inequality.

#### Regular tournament

↑ **Parent:** [Tournament (graph theory)](#tournament-graph-theory)

A regular [tournament](#tournament-graph-theory) has equal [outdegree](#outdegree) and indegree at every vertex. On $2k+1$ vertices, label by residues modulo $2k+1$ and direct $i\to j$ when $j-i\in\{1,\ldots,k\}$. This gives an explicit regular tournament. It contains no outward-oriented star with more than $k$ leaves.

### Directed cycle

↑ **Parent:** [Directed graph](#directed-graph)

A closed directed path whose vertices are distinct except for the common start and endpoint is a directed cycle. In a [residual network](flow-network.md#residual-network), augmenting around a directed cycle preserves [flow balance](#flow-balance). A negative total cost on such a cycle gives an improving displacement for a [minimum-cost flow](#minimum-cost-flow-problem).

#### Spanning circuit family

↑ **Parent:** [Directed cycle](#directed-cycle)

A spanning circuit family is a collection of [directed cycles](#directed-cycle) whose union contains every vertex of the [directed graph](#directed-graph). Different circuits may overlap. This is distinct from a [cycle cover of a directed graph](#cycle-cover-of-a-directed-graph), which requires vertex-disjoint cycles.

##### Circuit-cover bound by independence number

↑ **Parent:** [Spanning circuit family](#spanning-circuit-family)

For a nontrivial [strongly connected directed graph](#strong-connectivity), a [coherent cyclic order of a digraph](#coherent-cyclic-order-of-a-digraph) and the [Dilworth theorem](set.md#dilworth-s-theorem) produce a [spanning circuit family](#spanning-circuit-family) with at most its [independence number](#independence-number) circuits. Put a largest consecutive stable block first and duplicate its vertices as sinks. Use forward edges and edges into the sink copies to form an acyclic auxiliary graph. Its reachability order has width equal to the block size. Expand a chain partition to paths, then exchange intersecting path suffixes until the permutation of source-to-sink labels has as many cycles as possible. Paths in the same permutation cycle are disjoint, so identifying copied endpoints produces simple directed circuits. A windmill of directed triangles sharing one vertex shows that the bound is sharp.

### Rooted directed graph

↑ **Parent:** [Directed graph](#directed-graph)

A rooted directed graph has a distinguished root. Root-connectedness means each vertex can be reached by a finite directed path from that root. This is directed reachability, rather than connectedness of the underlying undirected graph.

#### Bisimulation

↑ **Parent:** [Rooted directed graph](#rooted-directed-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bisimulation)

A bisimulation relates the roots of two [rooted directed graphs](#rooted-directed-graph) and matches every successor move in either graph with a successor move in the other leading to related vertices. Multiple successors may be related to the same vertex. This local matching is weaker than graph isomorphism.

##### Bisimulation game

↑ **Parent:** [Bisimulation](#bisimulation)

The Spoiler takes one successor step from the current vertex of either [rooted directed graph](#rooted-directed-graph); the Duplicator must take a matching successor step in the other. The Duplicator wins by never failing at a finite stage, including when the Spoiler cannot move. A winning strategy gives a [bisimulation](#bisimulation) by collecting endpoint pairs of all finite plays consistent with it.

##### Bisimilarity

↑ **Parent:** [Bisimulation](#bisimulation)

Two [rooted directed graphs](#rooted-directed-graph) are bisimilar if some [bisimulation](#bisimulation) relates their roots. A root with one terminal successor is bisimilar to a root with two terminal successors, although the graphs have different sizes.

### Skeleton of a directed graph

↑ **Parent:** [Directed graph](#directed-graph)

The skeleton of a [directed graph](#directed-graph) is the [undirected graph](#undirected-graph) obtained by replacing every directed edge with an undirected edge and forgetting its orientation. In causal structure learning, the [PC algorithm](causal-inference.md#pc-algorithm) first recovers this adjacency structure before learning orientations.

### Cycle cover of a directed graph

↑ **Parent:** [Directed graph](#directed-graph)

A cycle cover of a finite directed graph is a collection of vertex-disjoint directed cycles containing every vertex exactly once. Cycle covers of the weighted directed graph with adjacency matrix $A$ are the terms in the [permanent of a matrix](linear-algebra.md#permanent-mathematics) $\operatorname{perm}A$.

This is a [vertex cycle cover](#vertex-cycle-cover) with the additional requirements of directed cycles and vertex disjointness.

### Directed edge

↑ **Parent:** [Directed graph](#directed-graph)

A directed edge $u\to v$ has an initial vertex $u$ and a terminal vertex $v$.

### Directed walk

↑ **Parent:** [Directed graph](#directed-graph)

A directed walk is a sequence of vertices in which each consecutive pair is joined by a [directed edge](#directed-edge) in the direction traversed.

#### Closed directed walk

↑ **Parent:** [Directed walk](#directed-walk)

A directed walk is closed when its first and last vertices agree.

### Directed path

↑ **Parent:** [Directed graph](#directed-graph)

A directed path follows every edge in its specified direction and visits no vertex more than once.

### Strong connectivity

↑ **Parent:** [Directed graph](#directed-graph)

A directed graph is strongly connected when every vertex is reachable from every other vertex by a [directed path](#directed-path).

### Adjacency matrix of a directed graph

↑ **Parent:** [Directed graph](#directed-graph)

The adjacency matrix of a finite directed graph has entry $A_{ij}$ equal to the number of directed edges from vertex $i$ to vertex $j$. The entry $(A^n)_{ij}$ counts length-$n$ directed walks from $i$ to $j$, so $\operatorname{tr}(A^n)$ counts pointed closed directed walks of length $n$.

## Adjacency matrix

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adjacency_matrix)

The adjacency matrix of a finite simple graph has entry $A_{uv}=1$ when vertices $u,v$ are adjacent and zero otherwise.

For a directed or weighted graph, entries instead record directed adjacency or edge weights.

### Walk count from powers of an adjacency matrix

↑ **Parent:** [Adjacency matrix](#adjacency-matrix)

For every nonnegative integer $k$, the entry $(A^k)_{uv}$ equals the number of length-$k$ walks from $u$ to $v$. This follows by induction, since matrix multiplication appends one adjacent vertex to each walk.

## Distance (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Distance_(graph_theory))

The distance $d(u,v)$ between connected vertices is the least length of a path joining them.

### Average shortest path length

↑ **Parent:** [Distance (graph theory)](#distance-graph-theory)

The [average shortest path length](#average-shortest-path-length) averages [graph distances](#distance-graph-theory) over distinct ordered pairs of [vertices](graph.md#vertex-graph-theory). A nodal value averages distances from one specified [vertex](graph.md#vertex-graph-theory) to all others. Disconnected pairs require a separate convention.

### Path metric

↑ **Parent:** [Distance (graph theory)](#distance-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Path_metric)

Given positive edge lengths $\ell(e)$, the path metric is the infimum of $\sum_{e\in\gamma}\ell(e)$ over paths $\gamma$ joining two vertices.

### Graph diameter

↑ **Parent:** [Distance (graph theory)](#distance-graph-theory)

The diameter of a connected finite graph is the maximum distance between two vertices.

Thus diameter is an extremal statistic of [graph distance](#distance-graph-theory).

#### Linear independence of adjacency powers up to the diameter

↑ **Parent:** [Graph diameter](#graph-diameter)

If a connected graph has adjacency matrix $A$ and diameter $d$, then

$$
I,A,\ldots,A^d
$$

are linearly independent. For the largest index $k$ with a nonzero coefficient, choose vertices at distance $k$; the corresponding entries of all lower powers vanish, while $(A^k)_{uv}>0$ by the [walk count from powers of an adjacency matrix](#walk-count-from-powers-of-an-adjacency-matrix).

## Spectral graph theory

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectral_graph_theory)

[Spectral graph theory](#spectral-graph-theory) studies [graphs](graph.md) through [eigenvalues](linear-operator-theory.md#eigenvalue) and [eigenvectors](linear-operator-theory.md#eigenvector) of associated [matrices](vector-space.md#matrix), including the [adjacency matrix](#adjacency-matrix) and [Laplacian matrix](#laplacian-matrix). A [graph eigenvalue](#graph-eigenvalue) usually refers to the adjacency-matrix spectrum unless another matrix is specified.

### Expander mixing lemma

↑ **Parent:** [Spectral graph theory](#spectral-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Expander_mixing_lemma)

For a $d$-regular undirected [graph](graph.md) whose normalized adjacency [eigenvalues](linear-operator-theory.md#eigenvalue) other than the constant [eigenvalue](linear-operator-theory.md#eigenvalue) have absolute value at most $\rho$, center the indicator vectors of $S,T$. Their constant parts give the expected term $d|S||T|/n$, and the [operator norm](continuous-dual-space.md#operator-norm) on the mean-zero subspace bounds the remaining [inner product](inner-product.md). Here $e(S,T)=\mathbf1_S^TA\mathbf1_T$ counts oriented incidences, so an [edge](#edge-of-a-graph) within $S\cap T$ is counted twice.

### Graph eigenvalue

↑ **Parent:** [Spectral graph theory](#spectral-graph-theory)

The eigenvalues of a finite graph are the eigenvalues of its adjacency matrix.

## Bipartite adjacency matrix

↑ **Parent:** [Graph theory](graph-theory.md)

With the two vertex classes listed consecutively, a bipartite graph has adjacency matrix $\left(\begin{smallmatrix}0&B\\B^T&0\end{smallmatrix}\right)$.

### Perfect matching from a nonzero determinant

↑ **Parent:** [Bipartite adjacency matrix](#bipartite-adjacency-matrix)

If a square bipartite adjacency matrix $B$ has nonzero determinant, some product in its Leibniz expansion is nonzero. Its permutation selects one edge at each vertex and therefore gives a perfect matching.

## Matching (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](matching-graph-theory.md)

## Ramsey theorem

↑ **Parent:** [Graph theory](graph-theory.md)

Every sufficiently large graph contains either a prescribed clique or a prescribed independent set.

### Diagonal Ramsey number

↑ **Parent:** [Ramsey theorem](#ramsey-theorem)

The diagonal Ramsey number $R(t)$ is the least $n$ such that every red-blue edge-colouring of $K_n$ contains a monochromatic $K_t$.

#### Binomial upper bound for a Ramsey number

↑ **Parent:** [Diagonal Ramsey number](#diagonal-ramsey-number)

The off-diagonal recursion

$$
R(s,t)\leq R(s-1,t)+R(s,t-1)
$$

with $R(1,t)=R(s,1)=1$ gives

$$
R(s,t)\leq\binom{s+t-2}{s-1}.
$$

In particular, $R(t)\leq\binom{2t-2}{t-1}<2^{2t}$.

#### Monochromatic-triangle counting formula

↑ **Parent:** [Diagonal Ramsey number](#diagonal-ramsey-number)

In a red-blue [edge colouring](graph-coloring.md#edge-coloring) of $K_n$, let $d_v$ be the red degree of vertex $v$ and let $M$ be the number of [monochromatic](ramsey-theory.md#monochromatic-set) triangles. Every nonmonochromatic triangle has exactly two vertices at which its two incident edges have different colors, so

$$
M=\binom n3-\frac12\sum_v d_v(n-1-d_v).
$$

Since $d_v(n-1-d_v)\leq\lfloor(n-1)^2/4\rfloor$, this identity gives a lower bound for $M$.

### Graph Ramsey number

↑ **Parent:** [Ramsey theorem](#ramsey-theorem)

For a finite graph $G$, its two-colour Ramsey number $R(G)$ is the least $n$ such that every red-blue colouring of $K_n$ contains a monochromatic copy of $G$. It exists because a monochromatic clique on $|V(G)|$ vertices contains a copy of $G$.

#### Triangle-free Ramsey lower bound by alteration

↑ **Parent:** [Graph Ramsey number](#graph-ramsey-number)

Sampling $G(n,p)$ and deleting one vertex per triangle and per independent $t$-set gives $R(3,t)>n-\binom n3p^3-\binom nt(1-p)^{\binom t2}$. Choosing $n$ of order $(t/\log t)^{3/2}$ and $p$ of order $\log t/t$ makes the forbidden configurations inexpensive enough to prove the corresponding lower bound.

#### Off-diagonal graph Ramsey number

↑ **Parent:** [Graph Ramsey number](#graph-ramsey-number)

The Ramsey number $r(G,H)$ is the least $n$ such that every red-blue colouring of $K_n$ contains a red copy of $G$ or a blue copy of $H$.

##### Clique-path Ramsey number

↑ **Parent:** [Off-diagonal graph Ramsey number](#off-diagonal-graph-ramsey-number)

If $P_t$ denotes a path of length $t$, then

$$
r(K_s,P_t)=(s-1)t+1
$$

for $s\geq2$ and $t\geq1$.

#### Ramsey number of a star

↑ **Parent:** [Graph Ramsey number](#graph-ramsey-number)

For the star $K_{1,t}$,

$$
R(K_{1,t})=
\begin{cases}
2t,&t\text{ odd},\\
2t-1,&t\text{ even}.
\end{cases}
$$

The parity distinction follows from the handshake lemma applied to a hypothetical $(t-1)$-regular colour class on $2t-1$ vertices.

#### Paw graph

↑ **Parent:** [Graph Ramsey number](#graph-ramsey-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Paw_graph)

The paw graph is a triangle with one pendant edge.

##### Ramsey number of the paw graph

↑ **Parent:** [Paw graph](#paw-graph)

The paw graph $H$ has $R(H)=7$. A colouring of $K_6$ with two disjoint red triangles and all cross-edges blue avoids a monochromatic paw. In $K_7$, a monochromatic triangle exists; avoiding a paw forces all its edges to the other four vertices into the opposite colour, which then forces those four internal edges into the triangle's colour and creates a paw.

### Uniform hypergraph Ramsey number

↑ **Parent:** [Ramsey theorem](#ramsey-theorem)

The diagonal $r$-uniform hypergraph Ramsey number $R^{(r)}(k)$ is the least $N$ such that every red-blue colouring of the $r$-element subsets of an $N$-element set has a monochromatic $k$-element set.

<h4 id="erdos-hajnal-bound-for-the-three-edge-hypergraph-on-four-vertices">Erdős-Hajnal bound for the three-edge hypergraph on four vertices</h4>

↑ **Parent:** [Uniform hypergraph Ramsey number](#uniform-hypergraph-ramsey-number)

Let $K_4^{(3)-}$ be the three-uniform hypergraph with three of the four possible edges on four vertices. Every $K_4^{(3)-}$-free three-uniform hypergraph on $N$ vertices has an independent set of size at least

$$
c\frac{\log N}{\log\log N}.
$$

Equivalently, $r(K_4^{(3)-},K_k^{(3)})\leq k^{Ck}$.

### Canonical Ramsey theorem

↑ **Parent:** [Ramsey theorem](#ramsey-theorem)

For every colouring of the $r$-element subsets of an infinite set, there is an infinite increasing sequence $X$ and a coordinate set $I\subseteq\{1,\ldots,r\}$ such that two increasing $r$-tuples from $X$ have the same colour exactly when they agree in every coordinate indexed by $I$.

### Partition regular equation

↑ **Parent:** [Ramsey theorem](#ramsey-theorem)

A homogeneous linear equation is partition regular when every finite colouring of the positive integers admits a solution whose coordinates all have one colour.

The equation has [partition regularity](ramsey-theory.md#partition-regular-matrix) when every finite colouring admits such a monochromatic solution.

<h2 id="dirac-s-theorem">Dirac's theorem</h2>

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac's_theorem)

Every graph on $n\ge3$ vertices with minimum degree at least $n/2$ has a Hamilton cycle.

## Longest-path rotation

↑ **Parent:** [Graph theory](graph-theory.md)

If an endpoint of a longest path is adjacent to an internal vertex, replacing the incident path edge by that chord produces another longest path with the same vertex set and a new endpoint. Every neighbour of every endpoint obtained this way must remain on the original path.

This rotation technique is used in arguments surrounding [Pósa's theorem](#posa-s-theorem) and other [Hamiltonian cycle](#hamilton-cycle) criteria.

### Neighbourhood bound for a square-free bipartite graph

↑ **Parent:** [Longest-path rotation](#longest-path-rotation)

Let $A$ be $k$ vertices of a bipartite graph, each of degree at least $k$. If the graph has no $4$-cycle, then $|N(A)|\geq2k-1$. Indeed, any pair in $A$ has at most one common neighbour, so

$$
\sum_{y\in N(A)}\binom{d_A(y)}2\leq\binom k2.
$$

If $|N(A)|\leq2k-2$, Cauchy--Schwarz and $\sum_y d_A(y)\geq k^2$ make the left side strictly larger than $\binom k2$, a contradiction.

## Strongly regular graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strongly_regular_graph)

A strongly regular graph has constant degree and fixed common-neighbour counts for adjacent and nonadjacent vertex pairs.

### Triangle-free graphs with three common neighbours

↑ **Parent:** [Strongly regular graph](#strongly-regular-graph)

For a finite simple graph with at least two vertices, no triangles, and exactly three common neighbours for every nonadjacent pair, the graph is connected. For adjacent vertices $u,v$, the bipartite graph between $N(u)\setminus\{v\}$ and $N(v)\setminus\{u\}$ has degree two at every vertex, forcing $d(u)=d(v)$. Thus the graph is regular. Counting second neighbours gives $3(n-d-1)=d(d-1)$. The nontrivial adjacency eigenvalues are $(-3\pm\sqrt{4d-3})/2$, and the larger-root multiplicity is $[n-1+d^2/\sqrt{4d-3}]/2$. Integrality forces $t=\sqrt{4d-3}$ to be an odd integer dividing $9$, yielding the stated degrees. The complete bipartite graph $K_{3,3}$ realizes degree three. The one-vertex graph is a vacuous exception with degree zero.

### Adjacency-matrix relation for a strongly regular graph

↑ **Parent:** [Strongly regular graph](#strongly-regular-graph)

If a strongly regular graph on $n$ vertices has degree $d$, with $r$ common neighbours for adjacent vertices and $s$ for nonadjacent vertices, then its adjacency matrix satisfies

$$
A^2=(d-s)I+(r-s)A+sJ.
$$

### Three-eigenvalue characterization of a connected strongly regular graph

↑ **Parent:** [Strongly regular graph](#strongly-regular-graph)

A connected regular graph is strongly regular exactly when its adjacency matrix has three distinct eigenvalues, apart from the complete graphs, which have two. The forward direction follows from the [adjacency-matrix relation for a strongly regular graph](#adjacency-matrix-relation-for-a-strongly-regular-graph); conversely, the quadratic polynomial vanishing on the two nonconstant eigenspaces is a scalar multiple of the [all-ones matrix](vector-space.md#all-ones-matrix).

## Moser spindle

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moser_spindle)

The Moser spindle is a seven-vertex unit-distance graph with chromatic number four.

## Probabilistic combinatorics

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](probabilistic-combinatorics.md)

## Random graph

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](random-graph.md)

## Complement graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complement_graph)

The complement of a simple graph has exactly the edges absent from the original graph; a vertex of degree $d$ acquires degree $n-1-d$.

### Simultaneously bipartite graph and complement

↑ **Parent:** [Complement graph](#complement-graph)

If a graph and its [complement graph](#complement-graph) are both [bipartite](bipartite-graph.md), then the graph has at most four vertices. Indeed, each part of a bipartition of the original graph induces a clique in the complement and therefore has at most two vertices. The bound is attained by the four-vertex path, whose complement is another four-vertex path.

## Menger theorem

↑ **Parent:** [Graph theory](graph-theory.md)

The maximum number of disjoint paths joining two vertex sets equals the minimum size of a separating set, with vertex and edge versions according to the chosen notion of disjointness.

### Vertex separator

↑ **Parent:** [Menger theorem](#menger-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vertex_separator)

An $x$-$y$ vertex separator is a set of vertices, excluding $x$ and $y$, whose deletion leaves no path from $x$ to $y$.

### Local connectivity

↑ **Parent:** [Menger theorem](#menger-theorem)

For nonadjacent vertices $a,b$ of a graph $G$, their local connectivity $\kappa(a,b;G)$ is the minimum size of an $a$-$b$ [vertex separator](#vertex-separator). By the [Menger theorem](#menger-theorem), it also equals the maximum number of internally vertex-disjoint $a$-$b$ paths.

### Internally vertex-disjoint paths

↑ **Parent:** [Menger theorem](#menger-theorem)

Paths with common endpoints are internally vertex-disjoint when they share no other vertex.

### Set version of Menger theorem

↑ **Parent:** [Menger theorem](#menger-theorem)

For vertex sets $A,B$, the maximum number of pairwise vertex-disjoint $A$-$B$ paths equals the minimum size of a vertex set meeting every $A$-$B$ path.

#### Fan lemma

↑ **Parent:** [Set version of Menger theorem](#set-version-of-menger-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fan_lemma)

In a $k$-connected graph, for a vertex $x$ and a set $Y$ of at least $k$ other vertices, there are $k$ paths from $x$ to distinct vertices of $Y$ that meet only at $x$. This follows from the [Set version of Menger theorem](#set-version-of-menger-theorem) by separating $x$ from $Y$.

### Linked graph

↑ **Parent:** [Menger theorem](#menger-theorem)

A graph is $k$-linked when any $2k$ distinct vertices paired as $(x_i,y_i)$ can be joined by $k$ mutually vertex-disjoint paths from $x_i$ to $y_i$.

Unlike [vertex connectivity](#vertex-connectivity), linkage specifies all endpoint pairings simultaneously.

#### Four-connected planar obstruction to two-linkage

↑ **Parent:** [Linked graph](#linked-graph)

On vertices $0,\ldots,7$, join cyclic indices differing by one or two modulo eight. The resulting [planar graph](planar-graph.md) has a square face bounded in order by $0,2,4,6$. Deleting at most three vertices cannot disconnect it: each break in the surviving cyclic chain requires two consecutive deleted vertices, and two separate breaks require four deletions. It is therefore four-connected. Disjoint paths joining $0$ to $4$ and $2$ to $6$ would cross in the complementary disk of the square face, contrary to the [Jordan curve theorem](topological-surface.md#jordan-curve-theorem). Thus four-connectivity does not guarantee two-linkage.

#### Rooted dense minor linkage

↑ **Parent:** [Linked graph](#linked-graph)

If a [graph](graph.md) is $2k$-connected and has a [graph minor](graph-minor.md) $H$ satisfying $2\delta(H)\ge |H|+4k-1$, it is $k$-linked. Write $d=|H|-1-\delta(H)$, so $|H|\ge2d+4k+1$. The [rooted branch-set reduction](graph-minor.md#rooted-branch-set-reduction) replaces the minor model by $|H|-k$ disjoint connected sets, the first $2k$ containing any prescribed terminals separately, each missing at most $d$ of the remaining sets. Every prescribed pair then has at least $k+1$ common adjacent unused sets, allowing the $k$ connections to be selected successively. The reduction uses [rooted separations of a graph](#rooted-separation-of-a-graph), contraction of edges outside distinct branch sets, and a final [Hall marriage theorem](matching-graph-theory.md#hall-s-marriage-theorem) matching; the separation condition prevents a contraction from destroying access to the model.

### Vertex connectivity

↑ **Parent:** [Menger theorem](#menger-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vertex_connectivity)

Vertex connectivity $\kappa(G)$ is the smallest number of vertices whose deletion disconnects a nontrivial graph or reduces it to one vertex.

#### Rooted separation of a graph

↑ **Parent:** [Vertex connectivity](#vertex-connectivity)

For a specified [set](set.md) $S$ of [vertices](graph.md#vertex-graph-theory), a rooted separation is a pair $(A,B)$ with $A\cup B=V(G)$, $S\subseteq A$, and no [edges](#edge-of-a-graph) between $A\setminus B$ and $B\setminus A$. Its order is $|A\cap B|$. It avoids a branch set $C$ when $A\cap C=\varnothing$. A graph with [vertex connectivity](#vertex-connectivity) at least $|S|$ has no rooted separation of order below $|S|$ avoiding a nonempty branch set: both sides of such a separation would be nonempty after deleting its separator.

#### k-connected graph

↑ **Parent:** [Vertex connectivity](#vertex-connectivity)

A graph with more than $k$ vertices is $k$-connected when deleting fewer than $k$ vertices always leaves it connected, equivalently when its [vertex connectivity](#vertex-connectivity) is at least $k$.

##### Dirac circumference theorem

↑ **Parent:** [K-connected graph](#k-connected-graph)

A $k$-connected graph has a cycle of length at least $\min\{|G|,2k\}$.

###### Longest-cycle attachment argument

↑ **Parent:** [Dirac circumference theorem](#dirac-circumference-theorem)

A component outside a longest cycle has at least $k$ attachment vertices in a $k$-connected graph, and no two attachments are consecutive, forcing cycle length at least $2k$.

##### 3-connected graph

↑ **Parent:** [K-connected graph](#k-connected-graph)

A graph is 3-connected when it has at least four vertices and remains connected after deletion of any two vertices.

### Edge connectivity

↑ **Parent:** [Menger theorem](#menger-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edge_connectivity)

Edge connectivity $\lambda(G)$ is the smallest number of edges whose deletion disconnects the graph.

### Whitney inequalities for graph connectivity

↑ **Parent:** [Menger theorem](#menger-theorem)

For every nontrivial graph, $\kappa(G)\leq\lambda(G)\leq\delta(G)$.

These compare two numerical invariants of [connectivity](graph.md#connectivity-graph-theory) with the [minimum degree of a graph](#minimum-degree-of-a-graph).

#### Connectivity realization construction

↑ **Parent:** [Whitney inequalities for graph connectivity](#whitney-inequalities-for-graph-connectivity)

Two large cliques joined by a bipartite cross graph with edge count $\ell$ and vertex-cover number $k$ realize edge connectivity $\ell$ and vertex connectivity $k$ while preserving a chosen minimum degree.

## Graph subdivision

↑ **Parent:** [Graph theory](graph-theory.md)

A [graph subdivision](#graph-subdivision) $TH$ replaces each [edge](#edge-of-a-graph) $uv$ of a [simple graph](graph.md#simple-graph) $H$ by a [graph path](#path-in-a-graph) of at least one [edge](#edge-of-a-graph) joining its original endpoints. The original [vertices](graph.md#vertex-graph-theory) are [branch vertices of a graph subdivision](#branch-vertex-of-a-graph-subdivision). The replacement [graph paths](#path-in-a-graph) have pairwise disjoint interiors, contain no [branch vertices of a graph subdivision](#branch-vertex-of-a-graph-subdivision) internally, and together make up the entire new [graph](graph.md). Leaving an [edge](#edge-of-a-graph) unchanged is allowed.[§1.7, printed p. 18: subdivision, branch vertices and subdividing vertices](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview)

For an explicit example, take $H$ with [vertex set](graph.md#vertex-set) $\{A,B,C,D\}$ and [edges](#edge-of-a-graph) $AB,BC,CA,AD$: a [triangle in a graph](graph.md#triangle-in-a-graph) with one attached [leaf of a graph](#leaf-of-a-graph). Replace its [edges](#edge-of-a-graph) by the following [branch paths of a graph subdivision](#branch-path-of-a-graph-subdivision):

$$
P_{AB}=(A,x,B),\qquad P_{BC}=(B,y,z,C),\qquad P_{CA}=(C,A),\qquad P_{AD}=(A,D).
$$

The resulting [graph subdivision](#graph-subdivision) $S$ has [vertex set](graph.md#vertex-set) $\{A,B,C,D,x,y,z\}$ and [edges](#edge-of-a-graph) $Ax,xB,By,yz,zC,CA,AD$. The internal [vertex](graph.md#vertex-graph-theory) sets are $\{x\},\{y,z\},\varnothing,\varnothing$, so disjointness is explicit. The [degrees of vertices](#degree-graph-theory) of $A,B,C,D$ remain $3,2,2,1$, respectively; the three new internal [vertices](graph.md#vertex-graph-theory) each have [degree of a vertex](#degree-graph-theory) two.

<a id="image-a-graph-subdivision-of-a-triangle-in-a-graph-with-an-attached-leaf-of-a-graph-colours-track-the-four-branch-paths-of-a-graph-subdivision"></a>
![](graph-subdivision-triangle-pendant-edge-paths.png)

**[Figure 21](#image-a-graph-subdivision-of-a-triangle-in-a-graph-with-an-attached-leaf-of-a-graph-colours-track-the-four-branch-paths-of-a-graph-subdivision). A graph subdivision of a triangle in a graph with an attached leaf of a graph: colours track the four branch paths of a graph subdivision**.

Adding $m$ internal [vertices](graph.md#vertex-graph-theory) to a finite [graph](graph.md) increases both its [vertex](graph.md#vertex-graph-theory) count and its [edge](#edge-of-a-graph) count by $m$. Here $m=3$, so four [vertices](graph.md#vertex-graph-theory) and four [edges](#edge-of-a-graph) become seven of each; the [graph excess](#graph-excess) is unchanged. Each replacement [graph path](#path-in-a-graph) remains a route between the same junctions. Thus [graph subdivision](#graph-subdivision) preserves whether a [graph](graph.md) is a [planar graph](planar-graph.md): insert intermediate [vertices](graph.md#vertex-graph-theory) along a crossing-free drawing, or trace each replacement [graph path](#path-in-a-graph) as one [edge](#edge-of-a-graph) to recover a drawing of the original [graph](graph.md). Travel times or capacities are separate modelling choices and are not determined by this adjacency construction.

### Branch vertex of a graph subdivision

↑ **Parent:** [Graph subdivision](#graph-subdivision)

A [branch vertex of a graph subdivision](#branch-vertex-of-a-graph-subdivision) is a retained original [vertex](graph.md#vertex-graph-theory) in a specified [graph subdivision](#graph-subdivision). Its [degree of a vertex](#degree-graph-theory) in that [graph subdivision](#graph-subdivision) equals its original [degree of a vertex](#degree-graph-theory). It need not have [degree of a vertex](#degree-graph-theory) at least three: $B,C,D$ in the example are also [branch vertices of a graph subdivision](#branch-vertex-of-a-graph-subdivision). When the target itself has [vertices](graph.md#vertex-graph-theory) of [degree of a vertex](#degree-graph-theory) two, adjacency alone need not identify which [vertices](graph.md#vertex-graph-theory) were original; the specified target mapping supplies that distinction.

### Branch path of a graph subdivision

↑ **Parent:** [Graph subdivision](#graph-subdivision)

A [branch path of a graph subdivision](#branch-path-of-a-graph-subdivision) is the replacement [graph path](#path-in-a-graph) for one original [edge](#edge-of-a-graph). Its endpoints are the corresponding [branch vertices of a graph subdivision](#branch-vertex-of-a-graph-subdivision); its internal [vertices](graph.md#vertex-graph-theory) have [degree of a vertex](#degree-graph-theory) two within the [graph subdivision](#graph-subdivision).

### Complete graph subdivision

↑ **Parent:** [Graph subdivision](#graph-subdivision)

A $TK_r$ is a subdivision of the [complete graph](#complete-graph) $K_r$. Its original complete-graph vertices are branch vertices and its replaced edges are branch paths.

## Bipartite vertex cover

↑ **Parent:** [Graph theory](graph-theory.md)

König's theorem equates the minimum vertex-cover size of a bipartite graph with its maximum matching size.

A bipartite vertex cover is a [vertex cover](#vertex-cover) restricted to a [bipartite graph](bipartite-graph.md); [Kőnig's theorem for bipartite matching](flow-network.md#konig-s-theorem-graph-theory) computes its minimum size.

<h2 id="erdos-gallai-theorem">Erdős-Gallai theorem</h2>

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Erdős–Gallai_theorem)

The [Erdős-Gallai theorem](#erdos-gallai-theorem) characterizes which finite nonincreasing sequences of nonnegative integers form the [degree sequence](#degree-sequence) of a [simple graph](graph.md#simple-graph), using an even total degree and partial-sum inequalities.

## Prism graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prism_graph)

A [prism graph](#prism-graph) joins two copies of a [cycle graph](#cycle-graph) by matching corresponding vertices. The [triangular prism graph](extremal-graph-theory.md#triangular-prism-graph) is the three-cycle case, with six vertices and nine edges.

## Squaregraph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squaregraph)

A [squaregraph](#squaregraph) has a plane embedding in which every bounded face has four sides and every interior vertex has degree at least four. Its outer face may have more than four sides, so this definition differs from a [planar quadrangulation](planar-graph.md#planar-quadrangulation) requiring every face to have degree four.

## Vertex cycle cover

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vertex_cycle_cover)

A [vertex cycle cover](#vertex-cycle-cover) is a collection of cycles whose union contains every vertex of a [graph](graph.md); its cycles can overlap. A [cycle cover of a directed graph](#cycle-cover-of-a-directed-graph) additionally requires directed, vertex-disjoint cycles, and a [spanning circuit family](#spanning-circuit-family) can allow overlaps.

<h2 id="posa-s-theorem">Pósa's theorem</h2>

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pósa's_theorem)

[Pósa's theorem](#posa-s-theorem) gives a sufficient degree-sequence condition for a [Hamiltonian cycle](#hamilton-cycle) in a finite [simple graph](graph.md#simple-graph). [Longest-path rotation](#longest-path-rotation) is a technique used in proving Hamiltonicity results; it is not itself the degree-sequence theorem.

## Pseudoforest

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudoforest)

A [pseudoforest](#pseudoforest) is an [undirected graph](#undirected-graph) in which every [connected component of a graph](graph.md#component-graph-theory) contains at most one [cycle in a graph](#cycle-in-a-graph). Thus each component is a [tree](tree-graph-theory.md) or a [unicyclic component](probabilistic-combinatorics.md#unicyclic-component). A finite tree component has one fewer edge than vertices; a finite unicyclic component has equally many edges and vertices.

## ↑ Ancestors (4)

1. [Foundations of mathematics](foundations-of-mathematics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (6)

- [Graph](graph.md)
- [Graph of a function](function.md#graph-of-a-function)
- [Graph theory](graph-theory.md)
- [Joseph Bernard Kruskal](mathematics.md#joseph-bernard-kruskal)
- [Mark Newman](physicist.md#mark-newman)
- [Ramsey number](ramsey-theory.md#ramsey-number)
