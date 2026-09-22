# Graph theory

↑ **Parent:** [Foundations of mathematics](foundations-of-mathematics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_theory)

[Graph theory](graph-theory.md) studies [vertices](graph.md#vertex-graph-theory) and the [edges](#edge-of-a-graph) connecting them: which [graph paths](#path-in-a-graph) exist, how efficiently we can travel, and which connections are indispensable. A road map becomes a [graph](graph.md) when junctions are [vertices](graph.md#vertex-graph-theory) and road segments are [edges](#edge-of-a-graph); a communications network uses routers and links instead. The drawing helps us see connections, but its apparent lengths need not be the costs being optimized. Record travel times or transmission costs separately in a [weighted graph](markov-process.md#weighted-graph).

The appeal of [graph theory](graph-theory.md) is that one model serves many practical questions. [Graph paths](#path-in-a-graph) describe routes, [connected components of a graph](graph.md#component-graph-theory) identify isolated regions, and [minimum spanning trees](combinatorics.md#minimum-spanning-tree) connect all locations cheaply. The [shortest path problem](#shortest-path-problem) asks a different question: find the cheapest journey between specified locations. Our four-[vertex](graph.md#vertex-graph-theory) example below makes that distinction concrete and shows how the [Dijkstra algorithm](#dijkstra-algorithm) discovers a route without trying every [graph path](#path-in-a-graph).

**Table of contents**

- [Geometric spanner](#geometric-spanner)
- [Graph excess](#graph-excess)
  - [Bicyclic graph](#bicyclic-graph)
    - [Labelled bicyclic graph count](#labelled-bicyclic-graph-count)
    - [Bicyclic kernel classification](#bicyclic-kernel-classification)
- [2-core of a graph](#2-core-of-a-graph)
  - [Graph kernel](#graph-kernel)
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
- [Shortest path problem](#shortest-path-problem)
  - [Label-setting shortest-path algorithm](#label-setting-shortest-path-algorithm)
  - [Bellman inequalities](#bellman-inequalities)
  - [Label-correcting shortest-path algorithm](#label-correcting-shortest-path-algorithm)
  - [Bellman-Ford algorithm](#bellman-ford-algorithm)
  - [Dijkstra algorithm](#dijkstra-algorithm)
    - [Tentative distance](#tentative-distance)
    - [Edge relaxation](#edge-relaxation)
    - [Shortest-path predecessor](#shortest-path-predecessor)
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
- [Graph minor](#graph-minor)
  - [Topological minor](#topological-minor)
  - [Rooted branch-set reduction](#rooted-branch-set-reduction)
  - [Complete graph minor density threshold](#complete-graph-minor-density-threshold)
    - [Dense minor with bounded order and high minimum degree](#dense-minor-with-bounded-order-and-high-minimum-degree)
  - [Branch set of a graph minor](#branch-set-of-a-graph-minor)
    - [Random branch-set construction of a complete graph minor](#random-branch-set-construction-of-a-complete-graph-minor)
  - [Edge contraction](#edge-contraction)
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
- [Graph](graph.md)
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
- [Graph coloring](#graph-coloring)
  - [Proper vertex coloring](#proper-vertex-coloring)
  - [Semi-random palette refinement for triangle-free colouring](#semi-random-palette-refinement-for-triangle-free-colouring)
  - [Colour savings from sparse neighbourhoods](#colour-savings-from-sparse-neighbourhoods)
  - [Coloring entropy weight](#coloring-entropy-weight)
    - [Entropy weight of a graph cover](#entropy-weight-of-a-graph-cover)
  - [Greedy coloring](#greedy-coloring)
    - [Extension of a partial colouring by neighbour-colour savings](#extension-of-a-partial-colouring-by-neighbour-colour-savings)
      - [Neighbour-colour saving](#neighbour-colour-saving)
  - [Three-colourability problem](#three-colourability-problem)
  - [Three-colour clause gadget](#three-colour-clause-gadget)
  - [Boolean-pair colouring gadget](#boolean-pair-colouring-gadget)
  - [Greedy colouring by removing independent sets](#greedy-colouring-by-removing-independent-sets)
  - [Lovász number](#lovasz-number)
    - [Orthonormal representation of a graph](#orthonormal-representation-of-a-graph)
      - [Tensor-product capacity bound from an orthonormal representation](#tensor-product-capacity-bound-from-an-orthonormal-representation)
    - [Complement theta number](#complement-theta-number)
  - [Vector coloring](#vector-coloring)
    - [Strict vector coloring](#strict-vector-coloring)
    - [Random hyperplane rounding](#random-hyperplane-rounding)
  - [Semicoloring](#semicoloring)
    - [Semicoloring by independent hyperplanes](#semicoloring-by-independent-hyperplanes)
  - [Edge coloring](#edge-coloring)
    - [Proper edge coloring](#proper-edge-coloring)
      - [Edge coloring as scheduling](#edge-coloring-as-scheduling)
    - [List edge coloring](#list-edge-coloring)
      - [List-chromatic index](#list-chromatic-index)
        - [Galvin theorem for bipartite list edge coloring](#galvin-theorem-for-bipartite-list-edge-coloring)
    - [Chromatic index](#chromatic-index)
      - [Chromatic index bounds](#chromatic-index-bounds)
    - [Tait coloring](#tait-coloring)
  - [Chromatic number](#chromatic-number)
    - [Chromatic number of Euclidean space](#chromatic-number-of-euclidean-space)
    - [Colour-critical vertex](#colour-critical-vertex)
    - [Mycielskian](#mycielskian)
    - [Graphs of arbitrarily high girth and chromatic number](#graphs-of-arbitrarily-high-girth-and-chromatic-number)
    - [Brooks' theorem](#brooks-theorem)
  - [Edge chromatic number](#edge-chromatic-number)
    - [Vizing's theorem](#vizing-s-theorem)
      - [Vizing fan lemma](#vizing-fan-lemma)
  - [Kempe chain](#kempe-chain)
  - [Chromatic polynomial](#chromatic-polynomial)
    - [Chromatic polynomial determines a Turán graph](#chromatic-polynomial-determines-a-turan-graph)
    - [Deletion-contraction recurrence for the chromatic polynomial](#deletion-contraction-recurrence-for-the-chromatic-polynomial)
    - [Chromatic polynomial after attaching a leaf](#chromatic-polynomial-after-attaching-a-leaf)
- [Independent set (graph theory)](#independent-set-graph-theory)
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
- [Complete graph](#complete-graph)
  - [Clique (graph theory)](#clique-graph-theory)
    - [Maximal clique](#maximal-clique)
    - [Edge-disjoint clique packing](#edge-disjoint-clique-packing)
      - [Clique-packing amplification of moment bounds](#clique-packing-amplification-of-moment-bounds)
      - [Clique conflict graph](#clique-conflict-graph)
    - [Clique number](#clique-number)
  - [Adjacency-matrix quadratic relation for a complete graph](#adjacency-matrix-quadratic-relation-for-a-complete-graph)
- [Complete multipartite graph](#complete-multipartite-graph)
  - [Octahedral graph](#octahedral-graph)
  - [Balancing a multipartite edge-triangle objective](#balancing-a-multipartite-edge-triangle-objective)
  - [Balanced complete multipartite blow-up](#balanced-complete-multipartite-blow-up)
- [Laplacian matrix](#laplacian-matrix)
  - [Weighted graph Laplacian](#weighted-graph-laplacian)
  - [Degree matrix](#degree-matrix)
  - [Graph Laplacian quadratic form](#graph-laplacian-quadratic-form)
  - [Kernel of a graph Laplacian](#kernel-of-a-graph-laplacian)
  - [Diffusion on a graph](#diffusion-on-a-graph)
  - [Laplacian spectrum of a complete graph](#laplacian-spectrum-of-a-complete-graph)
- [Minimum-cost flow problem](#minimum-cost-flow-problem)
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
- [Extremal graph theory](#extremal-graph-theory)
  - [Supersaturation](#supersaturation)
    - [Clique supersaturation by sampling](#clique-supersaturation-by-sampling)
  - [Extremal number](#extremal-number)
    - [Extremal graph for disjoint cliques](#extremal-graph-for-disjoint-cliques)
    - [Monotonicity of the normalized extremal number](#monotonicity-of-the-normalized-extremal-number)
    - [Mantel theorem](#mantel-theorem)
      - [Triangle lower bound one edge above the Mantel threshold](#triangle-lower-bound-one-edge-above-the-mantel-threshold)
  - [Turán's theorem](#turan-s-theorem)
    - [Edit-distance stability for clique-free graphs](#edit-distance-stability-for-clique-free-graphs)
      - [Bipartite stability from few odd cycles](#bipartite-stability-from-few-odd-cycles)
    - [Turán graph](#turan-graph)
      - [Triangle support line between bipartite and tripartite Turan graphs](#triangle-support-line-between-bipartite-and-tripartite-turan-graphs)
    - [Zykov symmetrization](#zykov-symmetrization)
      - [Edge-triangle symmetrization](#edge-triangle-symmetrization)
    - [Quadratic Turan edge bound](#quadratic-turan-edge-bound)
    - [Rhombus-free edge bound](#rhombus-free-edge-bound)
      - [Triangular prism graph](#triangular-prism-graph)
  - [Erdős-Stone theorem](#erdos-stone-theorem)
    - [Logarithmic Erdős-Stone theorem](#logarithmic-erdos-stone-theorem)
      - [Logarithmic clique blow-up from minimum degree](#logarithmic-clique-blow-up-from-minimum-degree)
      - [Random obstruction to larger clique blow-ups](#random-obstruction-to-larger-clique-blow-ups)
    - [High-minimum-degree multipartite stability subgraph](#high-minimum-degree-multipartite-stability-subgraph)
      - [Minimum degree of an extremal forbidden-subgraph graph](#minimum-degree-of-an-extremal-forbidden-subgraph-graph)
  - [Kővári–Sós–Turán theorem](#kovari-sos-turan-theorem)
- [Flow network](#flow-network)
  - [Circulation in a flow network](#circulation-in-a-flow-network)
  - [Vertex capacity](#vertex-capacity)
  - [Maximum flow problem](#maximum-flow-problem)
    - [Sports elimination by maximum flow](#sports-elimination-by-maximum-flow)
    - [Treatment capacity as a sink arc](#treatment-capacity-as-a-sink-arc)
    - [Server connectivity under component failures](#server-connectivity-under-component-failures)
    - [Edmonds–Karp algorithm](#edmonds-karp-algorithm)
    - [Maximum flow with vertex capacities](#maximum-flow-with-vertex-capacities)
      - [Vertex splitting](#vertex-splitting)
  - [Flow network edge capacity](#flow-network-edge-capacity)
  - [Capacity constraint](#capacity-constraint)
  - [Cut of a flow network](#cut-of-a-flow-network)
    - [Minimum cut](#minimum-cut)
      - [Diagonal cut in a nearest-neighbour lattice flow](#diagonal-cut-in-a-nearest-neighbour-lattice-flow)
    - [Cut capacity](#cut-capacity)
  - [Flow](#flow)
    - [Unit flow](#unit-flow)
    - [Divergence of a flow](#divergence-of-a-flow)
      - [Flow conservation](#flow-conservation)
    - [Strength of a flow](#strength-of-a-flow)
    - [Energy of a flow](#energy-of-a-flow)
      - [Finite-energy flow criterion for transience](#finite-energy-flow-criterion-for-transience)
  - [Max-flow min-cut theorem](#max-flow-min-cut-theorem)
    - [Residual reachability certificate for maximum flow](#residual-reachability-certificate-for-maximum-flow)
    - [Uniform capacity perturbation of a flow network](#uniform-capacity-perturbation-of-a-flow-network)
    - [Integral max-flow theorem](#integral-max-flow-theorem)
    - [Kőnig's theorem (graph theory)](#konig-s-theorem-graph-theory)
    - [Residual network](#residual-network)
      - [Residual maximum flow is the remaining optimality gap](#residual-maximum-flow-is-the-remaining-optimality-gap)
      - [Augmenting path](#augmenting-path)
        - [Widest augmenting path](#widest-augmenting-path)
          - [Geometric convergence of widest-path augmentation](#geometric-convergence-of-widest-path-augmentation)
        - [Ford-Fulkerson algorithm](#ford-fulkerson-algorithm)
          - [Integrality of the Ford-Fulkerson algorithm](#integrality-of-the-ford-fulkerson-algorithm)
    - [Parametric maximum flow with one source capacity](#parametric-maximum-flow-with-one-source-capacity)
- [Eulerian graph](#eulerian-graph)
  - [Edge support of a graph](#edge-support-of-a-graph)
  - [Seven Bridges of Königsberg](#seven-bridges-of-konigsberg)
  - [Eulerian trail](#eulerian-trail)
  - [Euler circuit](#euler-circuit)
  - [Euler circuit criterion](#euler-circuit-criterion)
    - [Hierholzer's algorithm](#hierholzer-s-algorithm)
- [Line graph](#line-graph)
  - [Line graph of a regular graph is Eulerian](#line-graph-of-a-regular-graph-is-eulerian)
- [Graph drawing](#graph-drawing)
- [Planar graph](#planar-graph)
  - [Kuratowski's theorem](#kuratowski-s-theorem)
  - [Plane graph](#plane-graph)
    - [Face of a plane graph](#face-of-a-plane-graph)
      - [Outer face](#outer-face)
      - [Facial boundary walk](#facial-boundary-walk)
  - [Honeycomb lattice](#honeycomb-lattice)
    - [Martini lattice](#martini-lattice)
  - [Four color theorem](#four-color-theorem)
  - [Five color theorem](#five-color-theorem)
  - [Planar map](#planar-map)
    - [Face of a planar map](#face-of-a-planar-map)
    - [Rooted planar map](#rooted-planar-map)
    - [Planar quadrangulation](#planar-quadrangulation)
      - [Trivial bijection between planar maps and quadrangulations](#trivial-bijection-between-planar-maps-and-quadrangulations)
  - [Planar dual graph](#planar-dual-graph)
    - [Planar cluster-count identity](#planar-cluster-count-identity)
    - [Dual bond percolation](#dual-bond-percolation)
      - [Three-terminal cell partition duality](#three-terminal-cell-partition-duality)
      - [Dual contour bound for a finite planar cluster](#dual-contour-bound-for-a-finite-planar-cluster)
    - [Planar duality for rectangle crossings](#planar-duality-for-rectangle-crossings)
      - [Exact self-dual rectangle crossing probability](#exact-self-dual-rectangle-crossing-probability)
  - [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph)
    - [Small faces of a spherical polyhedral graph](#small-faces-of-a-spherical-polyhedral-graph)
    - [Planar graph edge bound](#planar-graph-edge-bound)
      - [Bipartite planar graph edge bound](#bipartite-planar-graph-edge-bound)
      - [Nonplanarity by edge counts](#nonplanarity-by-edge-counts)
    - [Planar girth edge bound](#planar-girth-edge-bound)
    - [Triangle-pentagon planar edge bound](#triangle-pentagon-planar-edge-bound)
      - [Icosidodecahedral graph](#icosidodecahedral-graph)
- [Crossing number](#crossing-number)
  - [Crossing lemma](#crossing-lemma)
    - [Crossing lemma for multigraphs](#crossing-lemma-for-multigraphs)
- [Graph neighbourhood](#graph-neighbourhood)
  - [Neighbour of a vertex](#neighbour-of-a-vertex)
  - [Closed graph neighbourhood](#closed-graph-neighbourhood)
  - [External vertex boundary](#external-vertex-boundary)
  - [Common neighbour](#common-neighbour)
- [Degree (graph theory)](#degree-graph-theory)
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
- [Bipartite graph](#bipartite-graph)
  - [Crown graph](#crown-graph)
  - [Biadjacency matrix](#biadjacency-matrix)
  - [Normalized adjacency operator of a bipartite graph](#normalized-adjacency-operator-of-a-bipartite-graph)
  - [Biregular graph](#biregular-graph)
    - [Independent-set bound for biregular graphs](#independent-set-bound-for-biregular-graphs)
    - [Quasirandom bipartite graph](#quasirandom-bipartite-graph)
      - [Spectral discrepancy bound for a biregular graph](#spectral-discrepancy-bound-for-a-biregular-graph)
      - [Centered four-cycle identity for a biregular graph](#centered-four-cycle-identity-for-a-biregular-graph)
  - [Half graph](#half-graph)
    - [Boundary rank obstruction in a half graph](#boundary-rank-obstruction-in-a-half-graph)
  - [Odd-cycle characterization of bipartite graphs](#odd-cycle-characterization-of-bipartite-graphs)
  - [Complete bipartite graph](#complete-bipartite-graph)
    - [Common neighbourhood from bipartite density](#common-neighbourhood-from-bipartite-density)
    - [Star (graph theory)](#star-graph-theory)
  - [Two-colourability criterion for bipartite graphs](#two-colourability-criterion-for-bipartite-graphs)
- [Graph homomorphism](#graph-homomorphism)
  - [Graph embedding](#graph-embedding)
  - [Homomorphism density](#homomorphism-density)
    - [Sidorenko conjecture](#sidorenko-conjecture)
      - [Sidorenko inequality for trees](#sidorenko-inequality-for-trees)
- [Directed graph](#directed-graph)
  - [Kernel-perfect directed graph](#kernel-perfect-directed-graph)
    - [Kernel list-coloring lemma](#kernel-list-coloring-lemma)
  - [Kernel of a directed graph](#kernel-of-a-directed-graph)
  - [Plünnecke graph](#plunnecke-graph)
    - [Weighted cut lemma for commutative graphs](#weighted-cut-lemma-for-commutative-graphs)
    - [Graph magnification ratio](#graph-magnification-ratio)
  - [Coherent cyclic order of a digraph](#coherent-cyclic-order-of-a-digraph)
    - [Cyclic stability of a digraph order](#cyclic-stability-of-a-digraph-order)
  - [Tournament (graph theory)](#tournament-graph-theory)
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
  - [Path metric](#path-metric)
  - [Graph diameter](#graph-diameter)
    - [Linear independence of adjacency powers up to the diameter](#linear-independence-of-adjacency-powers-up-to-the-diameter)
- [Spectral graph theory](#spectral-graph-theory)
  - [Expander mixing lemma](#expander-mixing-lemma)
  - [Graph eigenvalue](#graph-eigenvalue)
- [Bipartite adjacency matrix](#bipartite-adjacency-matrix)
  - [Perfect matching from a nonzero determinant](#perfect-matching-from-a-nonzero-determinant)
- [Matching (graph theory)](#matching-graph-theory)
  - [Stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph)
    - [Mutual-worst edge in stable matchings](#mutual-worst-edge-in-stable-matchings)
    - [Gale-Shapley algorithm](#gale-shapley-algorithm)
  - [Near-perfect matching](#near-perfect-matching)
  - [Matching generating function](#matching-generating-function)
    - [Annealing ratios for a matching generating function](#annealing-ratios-for-a-matching-generating-function)
  - [Augmenting path in a matching](#augmenting-path-in-a-matching)
    - [Short augmenting paths in a dense bipartite graph](#short-augmenting-paths-in-a-dense-bipartite-graph)
  - [Perfect matching](#perfect-matching)
    - [Flexible vertex in a balanced bipartite graph](#flexible-vertex-in-a-balanced-bipartite-graph)
    - [Minimum-weight perfect matching](#minimum-weight-perfect-matching)
    - [One-factorization](#one-factorization)
  - [Maximal matching](#maximal-matching)
  - [Matching number](#matching-number)
  - [Hall's marriage theorem](#hall-s-marriage-theorem)
    - [Random bipartite matching from empty-rectangle exclusion](#random-bipartite-matching-from-empty-rectangle-exclusion)
    - [Hall matching of maximal separated sets](#hall-matching-of-maximal-separated-sets)
    - [Degree-weighted Hall condition](#degree-weighted-hall-condition)
    - [Measurable Hall theorem](#measurable-hall-theorem)
    - [Hall induction through a tight set](#hall-induction-through-a-tight-set)
    - [Regular bipartite graph has a perfect matching](#regular-bipartite-graph-has-a-perfect-matching)
  - [Regular-graph matching bound from unmatched vertices](#regular-graph-matching-bound-from-unmatched-vertices)
    - [Disjoint union of triangles as a sharp matching example](#disjoint-union-of-triangles-as-a-sharp-matching-example)
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
- [Random graph](#random-graph)
  - [Configuration model](#configuration-model)
    - [Bounded-degree pairing avoidance estimate](#bounded-degree-pairing-avoidance-estimate)
    - [Half-edge of a graph](#half-edge-of-a-graph)
  - [Preferential attachment](#preferential-attachment)
    - [Linearized chord diagram model](#linearized-chord-diagram-model)
      - [First-vertex degree in the LCD model](#first-vertex-degree-in-the-lcd-model)
      - [Uniform linearized chord diagram](#uniform-linearized-chord-diagram)
  - [Random k-out graph](#random-k-out-graph)
    - [Connectivity of random k-out graphs](#connectivity-of-random-k-out-graphs)
  - [Rado graph](#rado-graph)
  - [Achlioptas process](#achlioptas-process)
    - [Continuity of fixed-choice percolation](#continuity-of-fixed-choice-percolation)
    - [Persistence of unsampled graph components](#persistence-of-unsampled-graph-components)
    - [Forced merging of large components](#forced-merging-of-large-components)
    - [Component-band vertex count](#component-band-vertex-count)
  - [Simultaneous giant for fixed random-edge choice](#simultaneous-giant-for-fixed-random-edge-choice)
  - [Giant component](#giant-component)
    - [Barely-supercritical largest-component expectation](#barely-supercritical-largest-component-expectation)
    - [Logarithmic-regime giant component](#logarithmic-regime-giant-component)
  - [Isolated vertex](#isolated-vertex)
  - [Erdős-Rényi model](#erdos-renyi-model)
    - [Breadth-first exploration of a binomial random graph](#breadth-first-exploration-of-a-binomial-random-graph)
    - [Uniform random graph process](#uniform-random-graph-process)
      - [Connectivity hitting time equals disappearance of isolated vertices](#connectivity-hitting-time-equals-disappearance-of-isolated-vertices)
      - [Marked-set connectivity threshold](#marked-set-connectivity-threshold)
    - [Tree-component expectation in the Erdős-Rényi model](#tree-component-expectation-in-the-erdos-renyi-model)
      - [Fixed-order tree-component window](#fixed-order-tree-component-window)
    - [Monotone graph property](#monotone-graph-property)
      - [Threshold function for a monotone graph property](#threshold-function-for-a-monotone-graph-property)
      - [Monotone coupling of binomial random graphs](#monotone-coupling-of-binomial-random-graphs)
    - [Sprinkling of a binomial random graph](#sprinkling-of-a-binomial-random-graph)
    - [Isolated vertices in the Erdős-Rényi model](#isolated-vertices-in-the-erdos-renyi-model)
      - [Isolated-vertex threshold in the Erdős-Rényi model](#isolated-vertex-threshold-in-the-erdos-renyi-model)
    - [Connectivity threshold in the Erdős-Rényi model](#connectivity-threshold-in-the-erdos-renyi-model)
      - [Connectivity of a fixed-density binomial random graph](#connectivity-of-a-fixed-density-binomial-random-graph)
      - [Critical-window connectivity probability of a binomial random graph](#critical-window-connectivity-probability-of-a-binomial-random-graph)
    - [Expected subgraph count in the Erdős-Rényi model](#expected-subgraph-count-in-the-erdos-renyi-model)
      - [Sparse clique-count concentration](#sparse-clique-count-concentration)
        - [Pendant extensions of sparse clique copies](#pendant-extensions-of-sparse-clique-copies)
      - [Vertex-disjoint sparse clique copies](#vertex-disjoint-sparse-clique-copies)
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

## Geometric spanner

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_spanner)

A geometric spanner is a [weighted graph](markov-process.md#weighted-graph) on points in [Euclidean space](functional-analysis.md#euclidean-norm), with edge weights equal to their [Euclidean distances](topological-analysis.md#euclidean-distance), in which every pair has a [graph path](#path-in-a-graph) of [length](physics.md#length) at most $t$ times its direct distance. Its [stretch factor](functional-analysis.md#stretch-factor) is the largest ratio $d_G(u,v)/\|u-v\|$, where $d_G$ is shortest-path distance. A square's four perimeter edges, without diagonals, give stretch factor $\sqrt2$: adjacent points have ratio one, and diagonal pairs have route [length](physics.md#length) $2$ instead of $\sqrt2$. The aim is to retain short routes with fewer edges than a [complete graph](#complete-graph). [Gudmundsson, Narasimhan and Smid, Geometric Spanners, §1](https://people.scs.carleton.ca/~michiel/encyc_geometric_spanners.pdf).

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

The 2-core is the unique largest induced [subgraph](#subgraph) with [minimum degree](#minimum-degree-of-a-graph) at least two. It is obtained by repeatedly deleting vertices of degree zero or one. Every subgraph with [minimum degree](#minimum-degree-of-a-graph) two survives each deletion, which proves maximality and order independence. In a connected graph with a nonempty 2-core, the deleted vertices form rooted trees attached individually to the core vertices.

### Graph kernel

↑ **Parent:** [2-core of a graph](#2-core-of-a-graph)

For a connected graph whose [2-core](#2-core-of-a-graph) contains a vertex of degree at least three, suppress each maximal path with degree-two internal vertices to a single edge, allowing its two endpoints to coincide. The resulting [multigraph](graph.md#multigraph), retaining loops and parallel edges, is its kernel. Suppression preserves [graph excess](#graph-excess) and leaves [minimum degree](#minimum-degree-of-a-graph) at least three. A purely cyclic core is a separate unicyclic case; it has no branching vertex to anchor this construction.

## Chordal graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chordal_graph)

A [chordal graph](#chordal-graph) is a finite [simple graph](graph.md#simple-graph) with no [induced cycle](#induced-cycle) of length at least four. Equivalently, every [cycle in a graph](#cycle-in-a-graph) with at least four [vertices](graph.md#vertex-graph-theory) has a chord: an [edge](#edge-of-a-graph) joining two nonconsecutive [vertices](graph.md#vertex-graph-theory) of that [graph cycle](#cycle-in-a-graph). The word "induced" matters: the [induced subgraph](#induced-subgraph) on the chosen [vertices](graph.md#vertex-graph-theory) must contain exactly the cycle's [edges](#edge-of-a-graph), with no chords. Triangles are allowed. This definition concerns adjacency, independently of how the [graph](graph.md) is drawn.

For the square [cycle graph](#cycle-graph) $C_4$, take [vertex set](graph.md#vertex-set) $\{a,b,c,d\}$ and set of [edges](#edge-of-a-graph) $\{ab,bc,cd,da\}$, where $ab$ abbreviates $\{a,b\}$. Its [graph neighbourhoods](#graph-neighbourhood) are $N(a)=N(c)=\{b,d\}$ and $N(b)=N(d)=\{a,c\}$. The square is an [induced cycle](#induced-cycle), so $C_4$ is not a [chordal graph](#chordal-graph). Add the single [edge](#edge-of-a-graph) $ac$: now $N(a)=\{b,c,d\}$, $N(b)=\{a,c\}$, $N(c)=\{a,b,d\}$, and $N(d)=\{a,c\}$. The only possible four-[vertex](graph.md#vertex-graph-theory) [graph cycle](#cycle-in-a-graph) has chord $ac$, so this new [graph](graph.md) is a [chordal graph](#chordal-graph). Its [maximal cliques](#maximal-clique) are exactly $\{a,b,c\}$ and $\{a,c,d\}$.

<a id="image-an-induced-cycle-loses-its-obstruction-when-one-diagonal-is-added-the-resulting-maximal-cliques-form-a-junction-tree"></a>
![](chordal-perfect-elimination-square-cliques.png)

**[Figure 1](#image-an-induced-cycle-loses-its-obstruction-when-one-diagonal-is-added-the-resulting-maximal-cliques-form-a-junction-tree). An induced cycle loses its obstruction when one diagonal is added; the resulting maximal cliques form a junction tree**.

Connect these two [maximal cliques](#maximal-clique) by a single [edge](#edge-of-a-graph) labelled with their intersection $\{a,c\}$. The result is a [junction tree](statistical-model.md#junction-tree), also called a clique tree: its nodes are [maximal cliques](#maximal-clique), and the nodes containing any fixed original [vertex](graph.md#vertex-graph-theory) induce a [connected graph](graph.md#connected-graph) inside the [tree](combinatorics.md#tree-graph-theory). Here $a,c$ occur in both nodes, while $b,d$ each occur in just one. This is the [running intersection property](statistical-model.md#running-intersection-property). More generally, a nonempty [connected graph](graph.md#connected-graph) is a [chordal graph](#chordal-graph) exactly when its [maximal cliques](#maximal-clique) admit such a [tree](combinatorics.md#tree-graph-theory); a disconnected [chordal graph](#chordal-graph) can be represented by one such [tree](combinatorics.md#tree-graph-theory) per [connected component of a graph](graph.md#component-graph-theory).[§3.1–3.2](mathematics-bibliography.md#an-introduction-to-chordal-graphs-and-clique-trees-by-jean-r-s-blair-and-others)

A [chordal graph](#chordal-graph) need not be a [planar graph](#planar-graph): the [complete graph](#complete-graph) $K_5$ is a [chordal graph](#chordal-graph), since every pair of distinct [vertices](graph.md#vertex-graph-theory) is adjacent, but its ten [edges](#edge-of-a-graph) violate the [planar graph edge bound](#planar-graph-edge-bound) $|E|\leq3|V|-6=9$. Conversely, even a plane drawing whose bounded faces are triangles can hide an [induced cycle](#induced-cycle): a [wheel graph](#wheel-graph) with a four-[vertex](graph.md#vertex-graph-theory) rim and a central [vertex](graph.md#vertex-graph-theory) joined to the whole rim still has the rim as an [induced cycle](#induced-cycle). Adding chords to obtain a [chordal graph](#chordal-graph) is called [triangulation of an undirected graph](#triangulation-of-an-undirected-graph); this is an adjacency condition, rather than a requirement about planar faces.

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

**[Figure 2](#image-a-perfect-elimination-ordering-removes-three-overlapping-triangles-without-fill-in-choosing-the-central-vertex-first-adds-three-edges). A perfect elimination ordering removes three overlapping triangles without fill-in; choosing the central vertex first adds three edges**.

To find an ordering, [maximum cardinality search](#maximum-cardinality-search) starts with all scores zero, repeatedly selects an unselected [vertex](graph.md#vertex-graph-theory) of largest score, and increases each unselected [graph neighbour](#neighbour-of-a-vertex)'s score by one. Reverse the selection order to obtain a candidate [perfect elimination ordering](#perfect-elimination-ordering). For the three-triangle [graph](graph.md), one valid selection sequence is $(e,d,c,b,a)$, with scores at selection $0,1,2,2,2$; reversing it gives the displayed deletion order. On a [chordal graph](#chordal-graph) every tie choice works. On an arbitrary [graph](graph.md), test the resulting later [graph neighbourhoods](#graph-neighbourhood) for the [clique](#clique-graph-theory) condition to recognize [chordal graphs](#chordal-graph). Suitable [adjacency lists](computer-science.md#adjacency-list), score buckets and a linear-time verification method give $O(|V|+|E|)$ recognition.[§4.1–4.2; Algorithm 4.2](mathematics-bibliography.md#chordal-graphs-and-semidefinite-optimization-by-lieven-vandenberghe-and-others)

The deletion rule also explains [sparse Gaussian elimination](numerical-analysis.md#sparse-gaussian-elimination). For a symmetric [positive-definite matrix](linear-algebra.md#positive-definite-matrix) whose [matrix graph](numerical-analysis.md#matrix-graph) is $G$, eliminating pivot $v$ applies the [Schur complement](linear-algebra.md#schur-complement) update

$$
a_{uw}\longleftarrow a_{uw}-\frac{a_{uv}a_{vw}}{a_{vv}}.
$$

Only pairs of remaining [graph neighbours](#neighbour-of-a-vertex) of $v$ can acquire new off-diagonal entries. A [perfect elimination ordering](#perfect-elimination-ordering) already has all those [edges](#edge-of-a-graph), so [Cholesky decomposition](linear-algebra.md#cholesky-decomposition) creates no symbolic [fill-in](numerical-analysis.md#fill-in). Positive definiteness ensures nonzero pivots in exact arithmetic. Special numerical cancellation can suppress predicted entries, and floating-point rounding affects their values.[§9.1; equation 9.2; Theorem 9.1](mathematics-bibliography.md#chordal-graphs-and-semidefinite-optimization-by-lieven-vandenberghe-and-others) In the three-triangle [graph](graph.md), deleting $c$ first instead connects every pair in $\{a,b,d,e\}$ and adds exactly $ad,ae,be$. The [graph](graph.md) was already a [chordal graph](#chordal-graph); the extra [fill-in](numerical-analysis.md#fill-in) comes from the ordering.

One further reward is optimal [graph coloring](#graph-coloring). Process a [perfect elimination ordering](#perfect-elimination-ordering) backwards and give each [vertex](graph.md#vertex-graph-theory) the smallest positive color absent from its already colored [graph neighbours](#neighbour-of-a-vertex). Those [graph neighbours](#neighbour-of-a-vertex) form a [clique](#clique-graph-theory), so this [greedy algorithm](computer-science.md#greedy-algorithm) uses at most the [clique number](#clique-number) $\omega(G)$ colors; any [clique](#clique-graph-theory) of that size requires at least that many. In the three-triangle [graph](graph.md), coloring $(e,d,c,b,a)$ gives colors $(1,2,3,1,2)$, so both the [chromatic number](#chromatic-number) and the [clique number](#clique-number) are three. Every [maximal clique](#maximal-clique) also occurs among $\{v_i\}\cup N_i^+$: take its earliest [vertex](graph.md#vertex-graph-theory) and use maximality. The same ordering therefore supports [graph coloring](#graph-coloring), [maximal clique](#maximal-clique) extraction and sparse computation.

Historically, Donald J. Rose, Robert E. Tarjan and George S. Lueker's 1976 paper connected [graph](graph.md) elimination to symmetric [sparse matrices](vector-space.md#sparse-matrix) and gave a search-based $O(|V|+|E|)$ [algorithm](computer-science.md#algorithm) for finding a [perfect elimination ordering](#perfect-elimination-ordering) when one exists. Its abstract distinguishes a minimal elimination ordering from a minimum one: removing avoidable [fill-in](numerical-analysis.md#fill-in) does not by itself minimize the total number of added [edges](#edge-of-a-graph).[pp. 266–283; abstract](mathematics-bibliography.md#algorithmic-aspects-of-vertex-elimination-on-graphs-by-donald-j-rose-and-others)

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

The [shortest path problem](#shortest-path-problem) asks for a [graph path](#path-in-a-graph) from a source [vertex](graph.md#vertex-graph-theory) $s$ to a destination [vertex](graph.md#vertex-graph-theory) $t$ minimizing its total [edge](#edge-of-a-graph) weight. Here $w_e$ is the cost of traversing [edge](#edge-of-a-graph) $e$, and costs add along the [graph path](#path-in-a-graph). If no route exists, its shortest-path distance is $\infty$. With nonnegative [edge](#edge-of-a-graph) weights, deleting [cycles in a graph](#cycle-in-a-graph) from a [walk](#walk-in-a-graph) never increases its cost, so repetitions cannot improve the optimum.

Consider the [undirected graph](#undirected-graph) with [vertex set](graph.md#vertex-set) $V=\{A,B,C,D\}$ and the six [edge](#edge-of-a-graph) weights

$$
w_{AB}=4,\quad w_{AC}=1,\quad w_{CB}=2,\quad w_{BD}=1,\quad w_{CD}=5,\quad w_{AD}=10.
$$

Each [edge](#edge-of-a-graph) can be traversed in either direction at the same cost. The direct [graph path](#path-in-a-graph) $A,D$ costs $10$; $A,B,D$ costs $4+1=5$; $A,C,D$ costs $1+5=6$. The cheapest [graph path](#path-in-a-graph) is $A,C,B,D$, costing $1+2+1=4$. The remaining [graph path](#path-in-a-graph) $A,B,C,D$ costs $11$, exhausting the possibilities without repeated [vertices](graph.md#vertex-graph-theory).

<a id="image-the-shortest-path-problem-three-highlighted-edges-cost-less-than-the-direct-connection"></a>
![](shortest-path-weights.png)

**[Figure 3](#image-the-shortest-path-problem-three-highlighted-edges-cost-less-than-the-direct-connection). The shortest path problem: three highlighted edges cost less than the direct connection**.

Thus fewest [edges](#edge-of-a-graph) and least total cost are different objectives. [Breadth-first search](combinatorics.md#breadth-first-search) minimizes the number of [edges](#edge-of-a-graph), which suffices when every [edge](#edge-of-a-graph) has the same positive cost. Unequal nonnegative costs call for the [Dijkstra algorithm](#dijkstra-algorithm). On a map, weights might be minutes rather than kilometres: a longer-looking route can arrive sooner. This is why a [weighted graph](markov-process.md#weighted-graph) separates the network's connections from what a particular journey costs.

### Label-setting shortest-path algorithm

↑ **Parent:** [Shortest path problem](#shortest-path-problem)

An algorithm that makes each vertex's distance permanent once it is selected. With nonnegative [directed edge](#directed-edge) lengths, the [Dijkstra algorithm](#dijkstra-algorithm) selects the unfinalized vertex with least tentative distance; a shorter route through another unfinalized vertex is impossible because its remaining route has at least that next tentative distance. For an all-to-one problem, incoming [directed edges](#directed-edge) to the selected vertex are relaxed. Negative lengths can invalidate this finalization argument.

### Bellman inequalities

↑ **Parent:** [Shortest path problem](#shortest-path-problem)

The Bellman inequalities turn local [directed edge](#directed-edge) checks into a global certificate for the [shortest path problem](#shortest-path-problem). Here the convention is _all-to-one_: every journey ends at a fixed [vertex](graph.md#vertex-graph-theory) $r$, and $c_{ij}$ is the cost of the original [directed edge](#directed-edge) $i\to j$. Work in a finite [directed graph](#directed-graph) with finite real costs. Write $L_i$ for candidate labels, normalized by $L_r=0$, on the [vertices](graph.md#vertex-graph-theory) that can reach $r$. A feasible potential means precisely that these finite labels satisfy

$$
L_i\le c_{ij}+L_j
$$

for every [directed edge](#directed-edge) within that set. These labels give [lower bounds](set.md#lower-bound-in-a-partially-ordered-set) on costs _to_ $r$. A discovered [directed path](#directed-path) of cost $U_i$ instead gives an [upper bound](set.md#upper-bound-in-a-partially-ordered-set). The following constructed [graph](graph.md) shows both bounds and the exact distances between them; its weights are illustrative costs, not measured travel data.

<a id="image-bellman-inequalities-and-explicit-directed-paths-certify-distances-to-r-from-opposite-sides"></a>
![](edge-relaxation-certificate.png)

**[Figure 4](#image-bellman-inequalities-and-explicit-directed-paths-certify-distances-to-r-from-opposite-sides). Bellman inequalities and explicit directed paths certify distances to $r$ from opposite sides**.

The arrows in the picture point toward the destination, whereas [edge relaxation](#edge-relaxation) propagates an improved label in the opposite direction: an improved $d_j$ can lower $d_i$. In the pictured [graph](graph.md), the [directed paths](#directed-path) from $a$ to $r$ cost $7$, $2+3=5$, and $2-2+4=4$. Thus $\delta(a,r)=4$. The candidate $L=(3,1,3,0)$ in [vertex](graph.md#vertex-graph-theory) order $(a,b,c,r)$ is feasible, but underestimates the exact distances $(4,2,4,0)$. Merely satisfying the [Bellman inequalities](#bellman-inequalities) does not make a candidate exact.

Why do they give [lower bounds](set.md#lower-bound-in-a-partially-ordered-set)? Along any [directed path](#directed-path) $i=v_0\to v_1\to\cdots\to v_k=r$, successive substitution gives

$$
L_i\le\sum_{\ell=0}^{k-1}c_{v_\ell v_{\ell+1}}+L_r=\sum_{\ell=0}^{k-1}c_{v_\ell v_{\ell+1}}.
$$

The same calculation works for a [directed walk](#directed-walk), with repeated [vertices](graph.md#vertex-graph-theory) allowed. Taking the [infimum](real-analysis.md#infimum) of route costs gives $L_i\le\delta(i,r)$. A discovered route gives $\delta(i,r)\le U_i$. If the bounds meet, $L_i=U_i$, they certify an optimum without enumerating routes. Equivalently, check the [Bellman inequalities](#bellman-inequalities) for the proposed distances and exhibit [directed paths](#directed-path) realizing them. The authored [Bellman-Ford algorithm](#bellman-ford-algorithm) implementation checks the corresponding single-source inequalities and equality on recorded route [edges](#edge-of-a-graph); reversing every [directed edge](#directed-edge) gives this all-to-one convention.[Sedgewick and Wayne, BellmanFordSP.java, optimality checks](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/BellmanFordSP.java)

For the exact labels in the picture, the slack $c_{ij}+d_j-d_i$ is respectively $0,3,1,0,0$ on $a\to b$, $a\to r$, $b\to r$, $b\to c$, $c\to r$. Zero slack means equality; the zero-slack [directed path](#directed-path) $a\to b\to c\to r$ realizes the cost $4$. This is the useful beauty of the certificate: a few local [inequalities](arithmetic.md#inequality-mathematics) rule out every cheaper journey, while one explicit journey attains the bound.

Keep unreachable [vertices](graph.md#vertex-graph-theory) separate: $\delta(i,r)=\infty$ when no [directed path](#directed-path) to $r$ exists, and a finite [lower bound](set.md#lower-bound-in-a-partially-ordered-set) alone cannot certify that fact. Extended labels can use $\infty+c=\infty$ for finite $c$, but never compute a slack as $\infty-\infty$. If $i$ can reach a negative-cost [directed cycle](#directed-cycle) and then reach $r$, repeatedly traversing the [directed cycle](#directed-cycle) makes route costs unbounded below: their [infimum](real-analysis.md#infimum) is $-\infty$, with no finite shortest [directed walk](#directed-walk). A finite feasible potential on such a [directed cycle](#directed-cycle) is impossible, since summing its [Bellman inequalities](#bellman-inequalities) would give $0\le\sum c_{ij}<0$. A negative-cost [directed cycle](#directed-cycle) that cannot reach $r$ does not affect distances to $r$. These are statements about unrestricted [directed walks](#directed-walk); requiring a [directed path](#directed-path) with no repeated [vertices](graph.md#vertex-graph-theory) is a different optimization problem when negative-cost [directed cycles](#directed-cycle) exist.[MIT 6.006, Lecture 17, pp. 1 and 5: relevant negative cycles and simple paths](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/5edb13fb34cbe7f4cdccc13d131772e7_MIT6_006F11_lec17.pdf)

For the single-source convention, the same original [directed edge](#directed-edge) $u\to v$ instead gives $L(v)\le L(u)+w_{uv}$ with $L(s)=0$, a [lower bound](set.md#lower-bound-in-a-partially-ordered-set) on distance _from_ $s$. The endpoint carrying the label on the left therefore changes with the direction of the problem.

### Label-correcting shortest-path algorithm

↑ **Parent:** [Shortest path problem](#shortest-path-problem)

An algorithm whose tentative distance labels may be revised repeatedly until all relevant [Bellman inequalities](#bellman-inequalities) hold. [Bellman-Ford algorithm](#bellman-ford-algorithm) uses this approach: a label is an upper bound supplied by a discovered [directed path](#directed-path), and relaxing an [directed edge](#directed-edge) can replace it with a shorter discovered [directed path](#directed-path). A finite label is not declared permanent merely because it has been processed.

### Bellman-Ford algorithm

↑ **Parent:** [Shortest path problem](#shortest-path-problem)

For an all-to-one [shortest path problem](#shortest-path-problem) with root $r$, initialize $d_r^{(0)}=0$ and all other labels to infinity. Set $d_i^{(k)}=\min(d_i^{(k-1)},\min_{(i,j)\in A}\{c_{ij}+d_j^{(k-1)}\})$, keeping the root at zero. Induction identifies the labels with the shortest [directed paths](#directed-path) using at most $k$ [directed edges](#directed-edge). Without a reachable negative [directed cycle](#directed-cycle), $|V|-1$ rounds suffice after removing [directed cycles](#directed-cycle) from a shortest walk. In-place or queue variants repeatedly relax incoming [directed edges](#directed-edge) to an improved label. Labels may decrease multiple times, so this is a [label-correcting shortest-path algorithm](#label-correcting-shortest-path-algorithm).

### Dijkstra algorithm

↑ **Parent:** [Shortest path problem](#shortest-path-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dijkstra's_algorithm)

The [Dijkstra algorithm](#dijkstra-algorithm) solves the single-source [shortest path problem](#shortest-path-problem) in a finite [graph](graph.md) with nonnegative [edge](#edge-of-a-graph) weights, finding distances to all reachable [vertices](graph.md#vertex-graph-theory). Start with [tentative distance](#tentative-distance) $d(A)=0$ and $d(v)=\infty$ elsewhere. Repeatedly choose the unfinalized [vertex](graph.md#vertex-graph-theory) with least [tentative distance](#tentative-distance), declare that label permanent, and perform [edge relaxation](#edge-relaxation) on its outgoing [edges](#edge-of-a-graph). For an [undirected graph](#undirected-graph), inspect both directions. A finite [tentative distance](#tentative-distance) always records the cost of a discovered [graph path](#path-in-a-graph), but can improve before finalization.

In our example, finalizing $A$ discovers $C$ at $1$, $B$ at $4$, and $D$ at $10$. Choose $C$ next: [edge relaxation](#edge-relaxation) through $C$ lowers $B$ to $1+2=3$ and $D$ to $1+5=6$. Choose $B$: [edge relaxation](#edge-relaxation) through $B$ lowers $D$ to $3+1=4$. Finally choose $D$. The permanent distances are therefore $A:0$, $C:1$, $B:3$, $D:4$; the evolving [tentative distances](#tentative-distance) were $B:4\to3$ and $D:10\to6\to4$.

<a id="image-tentative-distances-fall-until-the-dijkstra-algorithm-makes-each-label-permanent"></a>
![](dijkstra-distance-frontier.png)

**[Figure 5](#image-tentative-distances-fall-until-the-dijkstra-algorithm-makes-each-label-permanent). Tentative distances fall until the Dijkstra algorithm makes each label permanent**.

Store a [shortest-path predecessor](#shortest-path-predecessor) whenever [edge relaxation](#edge-relaxation) improves a label. The final table contains enough information to reconstruct routes, rather than merely their costs:

| [Vertex](graph.md#vertex-graph-theory) | Distance from $A$ | [Shortest-path predecessor](#shortest-path-predecessor) | Finalization order |
| --- | --- | --- | --- |
| $A$ | $0$ | None: source | $1$ |
| $C$ | $1$ | $A$ | $2$ |
| $B$ | $3$ | $C$ | $3$ |
| $D$ | $4$ | $B$ | $4$ |

Following [shortest-path predecessors](#shortest-path-predecessor) backwards gives $D,B,C,A$; reversing the order gives $A,C,B,D$. If only this destination matters, stop when $D$ is finalized. Stopping when $D$ is first discovered would incorrectly return $10$. If the smallest remaining [tentative distance](#tentative-distance) is $\infty$, all remaining [vertices](graph.md#vertex-graph-theory) are unreachable.

Why is the permanent choice safe? Suppose the selected [vertex](graph.md#vertex-graph-theory) $u$ had a cheaper [graph path](#path-in-a-graph). Let $y$ be the first unfinalized [vertex](graph.md#vertex-graph-theory) on that [graph path](#path-in-a-graph). Its preceding [vertex](graph.md#vertex-graph-theory) was finalized, so [edge relaxation](#edge-relaxation) has already offered $y$ a label no larger than that prefix's cost. Nonnegative remaining [edge](#edge-of-a-graph) weights make the whole cost at least this prefix's cost; selection gives $d(u)\le d(y)$. A cheaper [graph path](#path-in-a-graph) would contradict these comparisons. Zero weights are allowed; ties can be resolved arbitrarily. This is the reason the [label-setting shortest-path algorithm](#label-setting-shortest-path-algorithm) works, rather than a lucky feature of the drawing.

Negative weights break that reasoning. In a [directed graph](#directed-graph) with $s\to u$ costing $2$, $s\to v$ costing $5$, and $v\to u$ costing $-4$, the [Dijkstra algorithm](#dijkstra-algorithm) would finalize $u$ at $2$ before discovering the cheaper cost $1$. The [Bellman-Ford algorithm](#bellman-ford-algorithm) handles negative [edge](#edge-of-a-graph) weights when no relevant negative [directed cycle](#directed-cycle) exists.

With an [adjacency list](computer-science.md#adjacency-list) and an indexed [binary heap](computer-science.md#binary-heap) implementing a [priority queue](computer-science.md#priority-queue), the [time complexity](computer-science.md#time-complexity) is $O((|V|+|E|)\log |V|)$ for $|V|\ge2$, using [Big O notation](real-analysis.md#big-o-notation). Each [vertex](graph.md#vertex-graph-theory) is extracted at most once, each [edge](#edge-of-a-graph) is inspected once per direction, and each successful [edge relaxation](#edge-relaxation) decreases a heap key in $O(\log |V|)$ time. This assumes constant-cost arithmetic and comparisons; exact computation with very large weights adds their representation cost. The queue uses $O(|V|)$ space beyond the [graph](graph.md). Simply scanning all remaining [vertices](graph.md#vertex-graph-theory) gives $O(|V|^2+|E|)$ instead.[Princeton, DijkstraSP implementation](https://algs4.cs.princeton.edu/44sp/DijkstraSP.java.html)[Princeton, indexed binary heap operations](https://algs4.cs.princeton.edu/code/javadoc/edu/princeton/cs/algs4/IndexMinPQ.html)

The 1959 paper presents the [shortest path problem](#shortest-path-problem) as its second problem, after the [minimum spanning tree](combinatorics.md#minimum-spanning-tree) problem, and grows known shortest routes in increasing distance order.[Dijkstra, A note on two problems in connexion with graphs, pp. 269–271](https://www.cs.yale.edu/homes/lans/readings/routing/dijkstra-routing-1959.pdf) In his later recollection, Dijkstra dated the shortest-route discovery to 1956: a demonstration for the ARMAC computer used a simplified Dutch railway map and printed the route between towns. A practical request became an enduring [algorithm](computer-science.md#algorithm) because the same distance rule applies to any suitable [graph](graph.md).[Dijkstra's recollection, published in 1983](https://garfield.library.upenn.edu/classics1983/A1983QA19900001.pdf)

#### Tentative distance

↑ **Parent:** [Dijkstra algorithm](#dijkstra-algorithm)

A tentative distance $d(v)$ is the cheapest cost so far recorded by a [shortest path problem](#shortest-path-problem) [algorithm](computer-science.md#algorithm). For the single-source convention, initialize $d(s)=0$ and $d(v)=\infty$ elsewhere. Every finite label is the cost of a discovered route from $s$ to $v$, so

$$
\delta(s,v)\le d(v).
$$

It is an [upper bound](set.md#upper-bound-in-a-partially-ordered-set) supplied by an actual route, not a guess that might be too low. The [loop invariant](computer-science.md#loop-invariant) follows directly from [edge relaxation](#edge-relaxation): extending a discovered route to $u$ by $u\to v$ supplies another discovered route. The usual label initialization and this safety property are stated and proved in the authored MIT notes.[MIT 6.006, Lecture 16, p. 1: relaxation safety](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/6277a1f06100c26a7ff21031af6757b5_MIT6_006F11_lec16.pdf)

In the trace under [edge relaxation](#edge-relaxation), $d(t)=10$ first records the direct [directed path](#directed-path) $s\to t$. Later $d(t)=8$ records $s\to a\to t$, and finally $d(t)=3$ records $s\to b\to a\to t$. Each label is a usable route cost, but the first two are not shortest. An infinite [tentative distance](#tentative-distance) means no route has yet been discovered; only a completed search establishes unreachability. The isolated [vertex](graph.md#vertex-graph-theory) $z$ in that example remains at $\infty$.

In a [directed graph](#directed-graph), the discovered route is formally a [directed walk](#directed-walk), which may repeat [vertices](graph.md#vertex-graph-theory); in the pictured acyclic [graph](graph.md) it is always a [directed path](#directed-path). Negative-cost [directed cycles](#directed-cycle) can keep supplying cheaper [directed walks](#directed-walk) without a finite optimum. In the all-to-one convention, the same meaning applies to discovered routes _from_ $i$ _to_ $r$. Do not confuse either version with the [lower bounds](set.md#lower-bound-in-a-partially-ordered-set) supplied by feasible potentials in the [Bellman inequalities](#bellman-inequalities): one records something achievable, the other rules out anything cheaper.

#### Edge relaxation

↑ **Parent:** [Dijkstra algorithm](#dijkstra-algorithm)

Edge relaxation tests whether extending a recorded route by one [directed edge](#directed-edge) improves a [tentative distance](#tentative-distance). For a single source $s$ and an original [directed edge](#directed-edge) $u\to v$ of weight $w_{uv}$, form the candidate $q=d(u)+w_{uv}$. If $d(u)$ is finite and $q<d(v)$, replace $d(v)$ by $q$ and record the [shortest-path predecessor](#shortest-path-predecessor) $\pi(v)=u$. Otherwise leave both unchanged. The [minimum](set.md#minimum-of-a-subset-of-a-total-order) formula in the header gives the resulting label in either case. The authored implementation uses this strict comparison and records the incoming [directed edge](#directed-edge).[Sedgewick and Wayne, DijkstraSP.java, relax method](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/DijkstraSP.java)

<a id="image-edge-relaxation-lowers-discovered-route-costs-including-across-a-negative-weight-directed-edge"></a>
![](edge-relaxation-trace.png)

**[Figure 6](#image-edge-relaxation-lowers-discovered-route-costs-including-across-a-negative-weight-directed-edge). Edge relaxation lowers discovered-route costs, including across a negative-weight directed edge**.

The table lists labels _after_ each specified operation, keeping $d(s)=0$ throughout this constructed acyclic [graph](graph.md). Relaxing $a\to t$ first offers $6+2=8$. Relaxing $b\to a$ then offers $2-1=1$, lowering $a$ from $6$ to $1$; revisiting $a\to t$ now offers $1+2=3$. Finally $b\to t$ offers $2+7=9$, so the label $3$ stays. Changing a label can make a previously checked outgoing [directed edge](#directed-edge) worth checking again. This trace illustrates the operation itself, with a deliberately specified order, rather than a run of the [Dijkstra algorithm](#dijkstra-algorithm).

A single [edge relaxation](#edge-relaxation) does not require nonnegative weights: its candidate is the cost of a real extended [directed walk](#directed-walk), even when the last [directed edge](#directed-edge) has negative weight. Nonnegative weights are needed by the [Dijkstra algorithm](#dijkstra-algorithm) to make its selected minimum [tentative distance](#tentative-distance) permanent. The [Bellman-Ford algorithm](#bellman-ford-algorithm) permits negative weights and revisits labels; its authored implementation also checks for reachable negative-cost [directed cycles](#directed-cycle).[Sedgewick and Wayne, DijkstraSP.java, nonnegative-weight precondition](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/DijkstraSP.java)[Sedgewick and Wayne, BellmanFordSP.java, signed weights and cycle detection](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/BellmanFordSP.java)

For the all-to-one convention of the [Bellman inequalities](#bellman-inequalities), relax the same original [directed edge](#directed-edge) $i\to j$ by $d_i\gets\min\{d_i,c_{ij}+d_j\}$. This prepends $i\to j$ to a discovered route from $j$ to $r$, and improves the tail label $d_i$, not the head label $d_j$. Skip the operation when $d_j=\infty$. In exact arithmetic, a full pass over all relevant [directed edges](#directed-edge) with no improvement establishes all their [Bellman inequalities](#bellman-inequalities); combined with the discovered-route [upper bounds](set.md#upper-bound-in-a-partially-ordered-set), this certifies finite distances. One unsuccessful operation establishes only that this particular candidate did not improve its label at that moment.

#### Shortest-path predecessor

↑ **Parent:** [Dijkstra algorithm](#dijkstra-algorithm)

A shortest-path predecessor $\pi(v)$ records the previous [vertex](graph.md#vertex-graph-theory) on a chosen route from source $s$ to $v$. When [edge relaxation](#edge-relaxation) strictly improves $d(v)$ through $u\to v$, set $\pi(v)=u$. For a [multigraph](graph.md#multigraph), store the actual [directed edge](#directed-edge), since two [edges](#edge-of-a-graph) with the same endpoints can have different weights. Initialize all [vertices](graph.md#vertex-graph-theory), including the source, without a [shortest-path predecessor](#shortest-path-predecessor). The authored implementation reconstructs a route by following these incoming [edges](#edge-of-a-graph) backwards, then reversing their order.[Sedgewick and Wayne, DijkstraSP.java, edgeTo and pathTo](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/DijkstraSP.java)

At the end of the [edge relaxation](#edge-relaxation) trace, $\pi(t)=a$, $\pi(a)=b$, and $\pi(b)=s$. Following them gives $t,a,b,s$, so the forward [directed path](#directed-path) is $s\to b\to a\to t$, of cost $2-1+2=3$. This makes the distance useful: a number tells us the best cost, whereas the [shortest-path predecessors](#shortest-path-predecessor) tell us which connections to take. In the [Dijkstra algorithm](#dijkstra-algorithm), reconstruct a destination's shortest route after its label becomes permanent. In a [label-correcting shortest-path algorithm](#label-correcting-shortest-path-algorithm), wait for convergence and the appropriate negative-cost [directed cycle](#directed-cycle) check. During correction, a predecessor's label may have changed since its child's last update: immediately after $b\to a$ in the trace, the current chain to $t$ costs $3$ although $d(t)$ still records the earlier discovered route of cost $8$.

Strict improvement is a useful guard against [directed cycles](#directed-cycle) in the recorded pointers. Consider $s\to a$ and $s\to b$ of cost zero, followed by $a\to b$ and $b\to a$, also of cost zero. After the first two [edge relaxations](#edge-relaxation), both labels are zero and both [shortest-path predecessors](#shortest-path-predecessor) are $s$. If equality also allows pointer replacement, the last two operations can set $\pi(b)=a$ and $\pi(a)=b$: following pointers loops forever despite correct distance labels. Keeping the old pointer on ties prevents this example; choosing among equal-cost routes requires a separate rule that preserves a route to the source. Strict improvement alone does not protect against reachable negative-cost [directed cycles](#directed-cycle), which can force endless decreases. Equality on recorded [edges](#edge-of-a-graph) plus the [Bellman inequalities](#bellman-inequalities) certifies route costs only when the pointer chains actually terminate at the source.

For all-to-one distances to $r$, record a next [vertex](graph.md#vertex-graph-theory) $j$ whenever relaxing $i\to j$ improves $d_i$. Follow these successors forward in the original [directed graph](#directed-graph) to reach $r$. They are [shortest-path predecessors](#shortest-path-predecessor) when viewed in the reversed [directed graph](#directed-graph); keeping the direction convention explicit prevents returning a route whose arrows point the wrong way.

## Graph property

↑ **Parent:** [Graph theory](graph-theory.md)

A [graph](graph.md) property is a class of finite [graphs](graph.md) closed under isomorphism. Its labelled order-$n$ slice consists of members on [vertex](graph.md#vertex-graph-theory) set $[n]$. Closure under taking arbitrary subgraphs and closure under taking only induced subgraphs lead respectively to [subgraph-closed graph properties](#subgraph-closed-graph-property) and [hereditary graph properties](#hereditary-graph-property).

### Common-center graph property

↑ **Parent:** [Graph property](#graph-property)

All edges of a simple undirected [graph](graph.md) have at least one common endpoint. The empty [graph](graph.md) is included when there is at least one vertex, and isolated vertices are permitted. This is the star predicate with isolated vertices allowed; a connected [star graph](#star-graph-theory) is a special case. Its [decision-tree depth](computer-science.md#decision-tree-depth) is the full number $\binom n2$ of edge bits for $n\geq3$.

#### Certificates for the common-center graph property

↑ **Parent:** [Common-center graph property](#common-center-graph-property)

For $n\geq3$, a full [star graph](#star-graph-theory) requires every nonincident edge to be certified absent, and fixing those bits suffices. Rejection is certified by at most three present edges with empty common intersection; a triangle needs all three. Hence [query certificate complexity](computer-science.md#certificate-complexity-of-a-boolean-function) is $\max\{3,\binom{n-1}{2}\}=\Theta(n^2)$ for this property.

#### Alternating count of common-center graphs

↑ **Parent:** [Common-center graph property](#common-center-graph-property)

For $n\geq3$, count the empty [graph](graph.md) once, all one-edge [graphs](graph.md) once, and each larger accepted [graph](graph.md) under its unique center. The latter weighted contribution is $n(n-2)$, giving $1-\binom n2+n(n-2)$. Its nonzero value proves evasiveness by the [alternating-sum criterion for decision-tree evasiveness](computer-science.md#alternating-sum-criterion-for-decision-tree-evasiveness).

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

Membership is preserved under deleting [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph). This is the decreasing meaning of monotonicity in extremal [graph](graph.md) enumeration; it differs from an increasing [monotone graph property](#monotone-graph-property) used for random-graph thresholds. For a proper unbounded class, its least excluded chromatic number determines the leading quadratic logarithm of its labelled speed.

#### Enumeration of subgraph-closed graph properties

↑ **Parent:** [Subgraph-closed graph property](#subgraph-closed-graph-property)

Here $r+1$ is the least chromatic number of an excluded [graph](graph.md), for a proper unbounded subgraph-closed property. All subgraphs of a balanced [Turán graph](#turan-graph) give the lower bound. For the upper bound, a regularity reduced [graph](graph.md) is clique-free, so its dense pairs have the [Turan theorem](#turan-s-theorem) [edge](#edge-of-a-graph) bound; sparse pairs contribute only small binary entropy and the bounded partition description costs only a linear number of bits.

## Orientation of a graph

↑ **Parent:** [Graph theory](graph-theory.md)

A choice of direction for each edge of an undirected [graph](graph.md), producing a [directed graph](#directed-graph).

### Outdegree orientation criterion

↑ **Parent:** [Orientation of a graph](#orientation-of-a-graph)

A finite undirected [graph](graph.md) can be oriented with [outdegree](#outdegree) at least an integer $k\geq0$ at every vertex if and only if every vertex subset $U$ is incident to at least $k|U|$ distinct edges. The [max-flow min-cut theorem](#max-flow-min-cut-theorem) and [integral max-flow theorem](#integral-max-flow-theorem) prove sufficiency by assigning distinct edges to vertices through an incidence [flow network](#flow-network); each assigned edge is oriented away from that vertex. Necessity follows by counting outgoing edges from $U$.

## Graph intersection

↑ **Parent:** [Graph theory](graph-theory.md)

For two [graphs](graph.md) on the same [vertex set](graph.md#vertex-set), their graph intersection retains exactly the [edges](#edge-of-a-graph) belonging to both.

## Kneser graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kneser_graph)

The Kneser graph has as [vertices](graph.md#vertex-graph-theory) the $k$-element subsets of $[n]$, with an [edge](#edge-of-a-graph) between two exactly when they are disjoint. A [graph colouring](#graph-coloring) of this [graph](graph.md) partitions the $k$-sets into [intersecting families](extremal-set-theory.md#intersecting-family).

<h3 id="lovasz-theorem-on-kneser-graphs">Lovász theorem on Kneser graphs</h3>

↑ **Parent:** [Kneser graph](#kneser-graph)

For integers $n\geq2k\geq2$, the [chromatic number](#chromatic-number) of the [Kneser graph](#kneser-graph) is $n-2k+2$. The upper bound colours by the least element among the first $n-2k+1$ elements, with one final colour for all other sets. The [Gale hemisphere lemma](geometry-and-topology.md#gale-hemisphere-lemma) and the [Lusternik-Schnirelmann-Borsuk theorem](algebraic-topology.md#lusternik-schnirelmann-theorem) give the matching lower bound.

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

The generator computes the [adjacency lists](computer-science.md#adjacency-list) and checks every [vertex](graph.md#vertex-graph-theory) deletion, giving the following complete table:

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

Again the [adjacency lists](computer-science.md#adjacency-list) and all [vertex](graph.md#vertex-graph-theory) deletion counts are computed directly:

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

The beautiful structural consequence is that a [graph](graph.md) splits into [biconnected components](#biconnected-component) joined at [cut vertices](#cut-vertex). Within each nontrivial robust piece, a single [vertex](graph.md#vertex-graph-theory) failure cannot separate the other [vertices](graph.md#vertex-graph-theory); between pieces, the shared [cut vertices](#cut-vertex) reveal the bottlenecks. Also, a [Hamiltonian](classical-mechanics.md#hamiltonian) [graph](graph.md) has no [cut vertex](#cut-vertex): deleting any [vertex](graph.md#vertex-graph-theory) from its [Hamilton cycle](#hamilton-cycle) leaves a [Hamiltonian path](#hamiltonian-path) through all remaining [vertices](graph.md#vertex-graph-theory).

Historically, Tarjan's June 1972 paper developed [depth-first search](computer-science.md#depth-first-search) as a tool for finding [biconnected components](#biconnected-component) in time linear in the numbers of [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph). [Robert Tarjan, Depth-First Search and Linear Graph Algorithms, SIAM Journal on Computing 1(2), 146–160 (1972)](https://epubs.siam.org/doi/10.1137/0201010) In his 1983 recollection, Tarjan credited Hopcroft with the original linear-time [biconnected component](#biconnected-component) [algorithm](computer-science.md#algorithm) during their collaboration beginning in summer 1970, and described the published version as a refinement. The historical lesson is how a carefully organized traversal turns many separate deletion experiments into one computation. [Robert E. Tarjan, Citation Classic recollection (1983)](https://garfield.library.upenn.edu/classics1983/A1983QY47200001.pdf)

### Biconnected component

↑ **Parent:** [Cut vertex](#cut-vertex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Biconnected_component)

A [biconnected component](#biconnected-component) is a maximal connected [subgraph](#subgraph) with no [cut vertex](#cut-vertex) of its own. We use the block convention that also includes each [bridge in a graph](graph.md#bridge-graph-theory) with its two endpoint [vertices](graph.md#vertex-graph-theory), and each isolated [vertex](graph.md#vertex-graph-theory), as a [biconnected component](#biconnected-component). A [biconnected component](#biconnected-component) with at least three [vertices](graph.md#vertex-graph-theory) stays connected after any single [vertex](graph.md#vertex-graph-theory) deletion. Distinct [biconnected components](#biconnected-component) share at most one [vertex](graph.md#vertex-graph-theory); the [vertices](graph.md#vertex-graph-theory) belonging to more than one [biconnected component](#biconnected-component) are exactly the [cut vertices](#cut-vertex). The shared-$A$ example has two [biconnected components](#biconnected-component), its two [triangles in a graph](graph.md#triangle-in-a-graph). The joined-$CD$ example has three: $ABC$, the [bridge in a graph](graph.md#bridge-graph-theory) $CD$ with its endpoints, and $DEF$. The [edges](#edge-of-a-graph) partition into these pieces, while the shared [cut vertices](#cut-vertex) occur in several pieces. [Sedgewick and Wayne, Algorithms, §4.1, biconnected components exercises](https://algs4.cs.princeton.edu/41graph/)

### DFS discovery time

↑ **Parent:** [Cut vertex](#cut-vertex)

The [DFS discovery time](#dfs-discovery-time) of a [vertex](graph.md#vertex-graph-theory) is its first-visit number in [depth-first search](computer-science.md#depth-first-search), assigned by an increasing counter. Discovery [edges](#edge-of-a-graph) form a [rooted tree](combinatorics.md#rooted-tree) in each [connected component of a graph](graph.md#component-graph-theory). For the joined-$CD$ example, starting at $A$ and visiting [graph neighbours](#neighbour-of-a-vertex) in [lexicographic order](extremal-set-theory.md#lexicographic-order) gives first visits $A,B,C,D,E,F$, numbered $1,2,3,4,5,6$; its discovery [edges](#edge-of-a-graph) are $AB,BC,CD,DE,EF$. These numbers encode the chosen traversal, not an invariant of the [graph](graph.md).

### DFS lowpoint

↑ **Parent:** [Cut vertex](#cut-vertex)

For a finite [simple graph](graph.md#simple-graph) that is an [undirected graph](#undirected-graph), the [DFS lowpoint](#dfs-lowpoint) of $v$ is the smallest [DFS discovery time](#dfs-discovery-time) reachable by following zero or more discovery [edges](#edge-of-a-graph) down its [rooted tree](combinatorics.md#rooted-tree), then at most one non-discovery [edge](#edge-of-a-graph) to an ancestor. Staying at $v$ is allowed. Ignore the reverse traversal of the discovery [edge](#edge-of-a-graph) to the [parent in a rooted tree](combinatorics.md#parent-in-a-rooted-tree): it is the same [edge](#edge-of-a-graph), not an escape route. Start with $\operatorname{low}(v)=\operatorname{disc}(v)$. On returning from a [child in a rooted tree](combinatorics.md#child-in-a-rooted-tree) $w$, replace $\operatorname{low}(v)$ by $\min\{\operatorname{low}(v),\operatorname{low}(w)\}$. For a non-discovery [edge](#edge-of-a-graph) from $v$ to an earlier ancestor $a$, replace it by $\min\{\operatorname{low}(v),\operatorname{disc}(a)\}$. This summarizes how far upward the explored branch can reconnect. [Tarjan (1972), §3, LOWPT recurrence, pp. 151–153](https://sites.cs.ucsb.edu/~gilbert/cs240a/notes/TarjanDFS.pdf)

The [cut vertex](#cut-vertex) criterion has a separate case for each [root of a tree](combinatorics.md#root-of-a-tree) in the discovery [forest](combinatorics.md#forest):
- A nonroot [vertex](graph.md#vertex-graph-theory) $u$ is a [cut vertex](#cut-vertex) exactly when some [child in a rooted tree](combinatorics.md#child-in-a-rooted-tree) $w$ satisfies $\operatorname{low}(w)\geq\operatorname{disc}(u)$.
- A [root of a tree](combinatorics.md#root-of-a-tree) is a [cut vertex](#cut-vertex) exactly when it has at least two [children in a rooted tree](combinatorics.md#child-in-a-rooted-tree), counting discovery [edges](#edge-of-a-graph), rather than all [graph neighbours](#neighbour-of-a-vertex).
- A discovery [edge](#edge-of-a-graph) $uw$ is a [bridge in a graph](graph.md#bridge-graph-theory) exactly when $\operatorname{low}(w)>\operatorname{disc}(u)$. A non-discovery [edge](#edge-of-a-graph) is never a [bridge in a graph](graph.md#bridge-graph-theory).

Why does equality matter? If $\operatorname{low}(w)=\operatorname{disc}(u)$, the branch below $w$ can reconnect to $u$, so the discovery [edge](#edge-of-a-graph) $uw$ lies on a [graph cycle](#cycle-in-a-graph) and is not a [bridge in a graph](graph.md#bridge-graph-theory). Deleting the [vertex](graph.md#vertex-graph-theory) $u$ destroys that reconnection too. If $u$ has a [parent in a rooted tree](combinatorics.md#parent-in-a-rooted-tree), the branch is then separated from that [parent in a rooted tree](combinatorics.md#parent-in-a-rooted-tree), explaining the non-strict [cut vertex](#cut-vertex) test. For a [root of a tree](combinatorics.md#root-of-a-tree), there is no earlier side to separate from; distinct discovery branches cannot have an [edge](#edge-of-a-graph) between them, since [depth-first search](computer-science.md#depth-first-search) would have explored them as one branch. This gives the two-[children in a rooted tree](combinatorics.md#child-in-a-rooted-tree) rule. These are proof outlines of the criteria. [Sedgewick and Wayne, Biconnected.java: discovery, lowpoint and root tests](https://algs4.cs.princeton.edu/41graph/Biconnected.java.html)[Sedgewick and Wayne, Algorithms, §4.1: bridge detection](https://algs4.cs.princeton.edu/41graph/)

In the joined-$CD$ example with [DFS discovery times](#dfs-discovery-time) $1,2,3,4,5,6$, the [DFS lowpoints](#dfs-lowpoint) in label order are $1,1,1,4,4,4$. For $C$ and its [child in a rooted tree](combinatorics.md#child-in-a-rooted-tree) $D$, $4>3$: $CD$ is a [bridge in a graph](graph.md#bridge-graph-theory), and $C$ is a [cut vertex](#cut-vertex). For $D$ and its [child in a rooted tree](combinatorics.md#child-in-a-rooted-tree) $E$, $4=4$: $D$ is a [cut vertex](#cut-vertex), although $DE$ is not a [bridge in a graph](graph.md#bridge-graph-theory). The [root of a tree](combinatorics.md#root-of-a-tree) $A$ has only one [child in a rooted tree](combinatorics.md#child-in-a-rooted-tree), $B$, so it is not a [cut vertex](#cut-vertex). In the shared-$A$ example, the [root of a tree](combinatorics.md#root-of-a-tree) $A$ has two [children in a rooted tree](combinatorics.md#child-in-a-rooted-tree), $B$ and $D$, and is a [cut vertex](#cut-vertex), while every [DFS lowpoint](#dfs-lowpoint) is $1$ and no [edge](#edge-of-a-graph) passes the strict [bridge in a graph](graph.md#bridge-graph-theory) test.

Restart [depth-first search](computer-science.md#depth-first-search) at every undiscovered [vertex](graph.md#vertex-graph-theory) to cover a disconnected [graph](graph.md), applying the [root of a tree](combinatorics.md#root-of-a-tree) rule separately in each [connected component of a graph](graph.md#component-graph-theory). With [adjacency lists](computer-science.md#adjacency-list) and constant-cost label operations, computing all [DFS lowpoints](#dfs-lowpoint), [cut vertices](#cut-vertex) and [bridges in a graph](graph.md#bridge-graph-theory) has [time complexity](computer-science.md#time-complexity) $O(|V|+|E|)$ in [Big O notation](real-analysis.md#big-o-notation), because each [vertex](graph.md#vertex-graph-theory) is discovered once and each [edge](#edge-of-a-graph) is inspected twice. The simple parent-skipping rule assumes a [simple graph](graph.md#simple-graph). In a [multigraph](graph.md#multigraph), skip only the actual parent [edge](#edge-of-a-graph), identified individually: a parallel [edge](#edge-of-a-graph) to the same [parent in a rooted tree](combinatorics.md#parent-in-a-rooted-tree) is a valid reconnection and can prevent the first [edge](#edge-of-a-graph) from being a [bridge in a graph](graph.md#bridge-graph-theory). The criteria here concern [undirected graphs](#undirected-graph); a [directed graph](#directed-graph) requires a different connectivity analysis.

## Hypergraph

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](hypergraph.md)

## Walk in a graph

↑ **Parent:** [Graph theory](graph-theory.md)

A [walk](#walk-in-a-graph) records a journey through a [graph](graph.md) as a finite alternating [sequence](real-analysis.md#sequence)

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

Here $AB$ denotes the [unordered pair](set.md#unordered-pair) $\{A,B\}$, and $CA=AC$. Two [triangles in a graph](graph.md#triangle-in-a-graph), $ABC$ and $ADE$, share $A$, with one extra [edge](#edge-of-a-graph) $AF$. These are schematic connections, not measured roads; the highlighted connections in the diagram show which [edges](#edge-of-a-graph) are used, while the numbered [sequence](real-analysis.md#sequence) records their order.

<a id="image-one-constructed-graph-repeated-edges-in-a-walk-repeated-vertices-in-a-trail-and-a-graph-path"></a>
![](walks-trails-closed-walks-route-comparison.png)

**[Figure 9](#image-one-constructed-graph-repeated-edges-in-a-walk-repeated-vertices-in-a-trail-and-a-graph-path). One constructed graph: repeated edges in a walk, repeated vertices in a trail, and a graph path**.

The length-six [walk](#walk-in-a-graph) $B,C,A,B,C,A,F$ uses $BC$ and $CA$ twice, so it is not a [trail](#trail-in-a-graph). The length-six [trail](#trail-in-a-graph) $B,C,A,D,E,A,F$ returns to $A$ but uses six different [edges](#edge-of-a-graph), so it is not a [graph path](#path-in-a-graph). The length-three [graph path](#path-in-a-graph) $B,C,A,F$ repeats neither [vertices](graph.md#vertex-graph-theory) nor [edges](#edge-of-a-graph). Thus

$$
\{\text{graph paths}\}\subsetneq\{\text{trails}\}\subsetneq\{\text{walks}\}
$$

for this particular [graph](graph.md). The restrictions answer different routing questions: revisiting a junction is harmless for many journeys, whereas reusing a serviced road segment can matter for an inspection route. Travel costs require a [weighted graph](markov-process.md#weighted-graph); a [walk](#walk-in-a-graph)'s cost adds the weight of each traversal, even when an [edge](#edge-of-a-graph) is used again.

Every finite [walk](#walk-in-a-graph) from $s$ to $t$ contains a [graph path](#path-in-a-graph) from $s$ to $t$ after deleting detours. For a proof outline, if $v_i=v_j$ with $i<j$, delete the intervening [closed walk](#closed-walk). The retained steps still meet at the same [vertex](graph.md#vertex-graph-theory), and the length strictly decreases. Repeating terminates with no repeated [vertices](graph.md#vertex-graph-theory), or with the zero-length [graph path](#path-in-a-graph) when $s=t$. This explains why [reachability](graph.md#reachability-in-a-graph) can be formulated using either [walks](#walk-in-a-graph) or [graph paths](#path-in-a-graph). With nonnegative [edge](#edge-of-a-graph) weights, deletion also cannot increase cost, connecting the argument to the [shortest path problem](#shortest-path-problem); with negative weights that cost conclusion fails.[Paul Johnson, MAS341, Lecture 3: deleting repeated-vertex detours](https://ptwiddle.github.io/MAS341-Graph-Theory-2017/lecturenotes/lecture3.html)

### Trail in a graph

↑ **Parent:** [Walk in a graph](#walk-in-a-graph)

A [trail](#trail-in-a-graph) is a [walk](#walk-in-a-graph) whose [edge](#edge-of-a-graph) [sequence](real-analysis.md#sequence) $e_1,\ldots,e_m$ has no repetitions. Its [vertices](graph.md#vertex-graph-theory) may repeat, including its first and last [vertices](graph.md#vertex-graph-theory). The zero-length [walk](#walk-in-a-graph) is a [trail](#trail-in-a-graph) because it repeats no [edge](#edge-of-a-graph). Every [graph path](#path-in-a-graph) is a [trail](#trail-in-a-graph), but the converse fails: the [trail](#trail-in-a-graph) in the shared example is

$$
B,BC,C,CA,A,AD,D,DE,E,EA,A,AF,F.
$$

Its six [edges](#edge-of-a-graph) $BC,CA,AD,DE,EA,AF$ are pairwise distinct, although $A$ occurs twice. Visiting a junction again and traversing a road segment again are different events.[Thomas Zaslavsky, Supplementary Notes for Graduate Graph Theory: trails and paths](https://people.math.binghamton.edu/zaslav/Oldcourses/581.S99/notes.html)

In an [undirected graph](#undirected-graph), traversing $AB$ and then $BA$ repeats the same [edge](#edge-of-a-graph); direction of travel does not give it a new identity. In a [multigraph](graph.md#multigraph) with distinct parallel [edges](#edge-of-a-graph) $p,q$ joining $X$ and $Y$, the [closed walk](#closed-walk) $(X,p,Y,q,X)$ is a [trail](#trail-in-a-graph), whereas $(X,p,Y,p,X)$ is not. Both have the same [vertex](graph.md#vertex-graph-theory) [sequence](real-analysis.md#sequence) $X,Y,X$. In a [directed graph](#directed-graph), separate [directed edges](#directed-edge) $X\to Y$ and $Y\to X$ may instead be used once each; record their identities and obey their directions. Thus testing a [trail](#trail-in-a-graph) means checking the actual [edge](#edge-of-a-graph) records, not merely checking consecutive endpoint labels.

For a finite [graph](graph.md), a [trail](#trail-in-a-graph) has length at most $|E|$; unrestricted [walks](#walk-in-a-graph) can have arbitrarily large length whenever a positive-length [closed walk](#closed-walk) exists, since it can be repeated. An [Eulerian trail](#eulerian-trail) is the special [trail](#trail-in-a-graph) that uses every [edge](#edge-of-a-graph), so its length is exactly $|E|$. Our length-six [trail](#trail-in-a-graph) omits $AB$ and is therefore not an [Eulerian trail](#eulerian-trail). In a road-inspection model, a [trail](#trail-in-a-graph) describes servicing its selected segments once while allowing returns to junctions; requiring service of every segment leads to the [Eulerian trail](#eulerian-trail) question. If extra travel between serviced segments is necessary, the complete journey can be a [walk](#walk-in-a-graph) even when each segment is serviced only once. This distinction keeps the service requirement separate from the route actually travelled.

### Closed walk

↑ **Parent:** [Walk in a graph](#walk-in-a-graph)

A [closed walk](#closed-walk) is a [walk](#walk-in-a-graph) with equal endpoint [vertices](graph.md#vertex-graph-theory), $v_m=v_0$. Under our convention this includes the zero-length [walk](#walk-in-a-graph) $(v)$; returning after traversing at least one [edge](#edge-of-a-graph) requires $m>0$. Closure imposes no other restriction on repeated [vertices](graph.md#vertex-graph-theory) or [edges](#edge-of-a-graph). In a [directed graph](#directed-graph), a [closed directed walk](#closed-directed-walk) must also follow every [directed edge](#directed-edge) in its permitted direction.[Lehman, Leighton and Meyer, Mathematics for Computer Science, §§9.2 and 11.8.1: closed walks](mathematics-bibliography.md#mathematics-for-computer-science-by-eric-lehman-and-others)

<a id="image-returning-to-a-backtracking-closed-walk-closed-trail-with-a-repeated-internal-vertex-and-graph-cycle"></a>
![](walks-trails-closed-walks-return-comparison.png)

**[Figure 10](#image-returning-to-a-backtracking-closed-walk-closed-trail-with-a-repeated-internal-vertex-and-graph-cycle). Returning to $A$: backtracking closed walk, closed trail with a repeated internal vertex, and graph cycle**.

In the shared [simple graph](graph.md#simple-graph), $A,F,A$ is a length-two [closed walk](#closed-walk) that immediately backtracks along $AF$. It is not a [trail](#trail-in-a-graph), since $AF$ is used twice, and it is not a [graph cycle](#cycle-in-a-graph). The length-six [closed walk](#closed-walk) $A,B,C,A,D,E,A$ is a [trail](#trail-in-a-graph), since its six [edges](#edge-of-a-graph) are distinct, but is not a [graph cycle](#cycle-in-a-graph): it returns to $A$ midway through the journey. The length-three [closed walk](#closed-walk) $A,B,C,A$ is a [graph cycle](#cycle-in-a-graph), with all [vertices](graph.md#vertex-graph-theory) distinct apart from the required endpoint repetition. In a [simple graph](graph.md#simple-graph) that is an [undirected graph](#undirected-graph), a [graph cycle](#cycle-in-a-graph) has length at least three; the two-step backtrack is excluded.[Lehman, Leighton and Meyer, Mathematics for Computer Science, §11.8.1: cycles and backtracking](mathematics-bibliography.md#mathematics-for-computer-science-by-eric-lehman-and-others)

A positive-length [closed walk](#closed-walk) therefore need not reveal a [graph cycle](#cycle-in-a-graph): even a [tree](combinatorics.md#tree-graph-theory) permits an out-and-back journey on an [edge](#edge-of-a-graph). A positive-length closed [trail](#trail-in-a-graph) in a [simple graph](graph.md#simple-graph) does contain a [graph cycle](#cycle-in-a-graph). For a proof outline, choose a shortest positive-length consecutive portion of the [trail](#trail-in-a-graph) whose endpoint [vertices](graph.md#vertex-graph-theory) coincide. It cannot repeat an internal [vertex](graph.md#vertex-graph-theory), since that would give a shorter such portion; it cannot have length one or two because [self-loops](graph.md#loop-graph-theory) and repeated [edges](#edge-of-a-graph) are excluded. It is consequently a [graph cycle](#cycle-in-a-graph). Cutting it out leaves another closed [trail](#trail-in-a-graph), possibly of length zero, so repetition partitions the original [edges](#edge-of-a-graph) into [graph cycles](#cycle-in-a-graph). In our six-step example these are the two [triangles in a graph](graph.md#triangle-in-a-graph). A closed [trail](#trail-in-a-graph) using every [edge](#edge-of-a-graph) would be an [Euler circuit](#euler-circuit); here $AF$ is omitted.

Counting return journeys makes [closed walks](#closed-walk) useful even when they repeat [edges](#edge-of-a-graph). For a finite [simple graph](graph.md#simple-graph) with [adjacency matrix](#adjacency-matrix) $M$, the [walk count from powers of an adjacency matrix](#walk-count-from-powers-of-an-adjacency-matrix) gives $(M^k)_{uv}$ length-$k$ [walks](#walk-in-a-graph) from $u$ to $v$, for every [nonnegative integer](arithmetic.md#natural-number) $k$. A proof outline is that [matrix multiplication](vector-space.md#matrix-multiplication) appends one allowed step, summing over the previous endpoint; $M^0$ is the [identity matrix](vector-space.md#identity-matrix), recording the unique zero-length [walk](#walk-in-a-graph) at each [vertex](graph.md#vertex-graph-theory). Consequently

$$
(M^k)_{vv}=\#\{\text{length-}k\text{ closed walks starting at }v\},\qquad \operatorname{tr}(M^k)=\sum_{v\in V}(M^k)_{vv}.
$$

The [trace](linear-algebra.md#matrix-trace) counts [closed walks](#closed-walk) with a specified starting [vertex](graph.md#vertex-graph-theory) and traversal order, not distinct [graph cycles](#cycle-in-a-graph). These formulas use adjacency entries, not arbitrary travel costs in a [weighted graph](markov-process.md#weighted-graph).[Alexander Wolitzky, Graph Theory and Social Networks, slides 9–10: powers of adjacency matrices](https://ocw.mit.edu/courses/14-15-networks-spring-2022/mit14_15s22_lec2.pdf)

In our example, $(M^2)_{AA}=5$: the five length-two [closed walks](#closed-walk) are $A,B,A$, $A,C,A$, $A,D,A$, $A,E,A$, and $A,F,A$. Also $(M^3)_{AA}=4$, going round either [triangle in a graph](graph.md#triangle-in-a-graph) in either direction, and $\operatorname{tr}(M^3)=12$: each of the two [triangles in a graph](graph.md#triangle-in-a-graph) supplies three choices of starting [vertex](graph.md#vertex-graph-theory) and two directions. These exact counts for the constructed [graph](graph.md) illustrate why return counts and [graph cycle](#cycle-in-a-graph) counts differ.

A [closed walk](#closed-walk) naturally models a delivery or inspection journey that returns to its depot. Repeated [vertices](graph.md#vertex-graph-theory) let it combine several excursions; repeated [edges](#edge-of-a-graph) let it serve a dead end and return. For an [Euclidean travelling salesman tour](mathematical-optimization.md#euclidean-travelling-salesman-tour), one can first construct a [closed walk](#closed-walk) visiting all locations and then use the [triangle inequality](topological-analysis.md#triangle-inequality) to shortcut repeated visits without increasing total length. That argument assumes direct travel between the retained locations is permitted, as in a [complete graph](#complete-graph) weighted by [Euclidean distance](topological-analysis.md#euclidean-distance); an arbitrary road network need not contain those shortcut [edges](#edge-of-a-graph).

## Undirected graph

↑ **Parent:** [Graph theory](graph-theory.md)

An undirected [graph](graph.md) has edges that are unordered pairs of vertices. In a simple undirected graph there are no loops or multiple edges. The [skeleton of a directed graph](#skeleton-of-a-directed-graph) forgets the directions of its edges and is an undirected graph.

## Graph minor

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_minor)

A [graph minor](#graph-minor) compresses connected regions of a [graph](graph.md) into single [vertices](graph.md#vertex-graph-theory) while retaining selected connections between them. For finite [simple graphs](graph.md#simple-graph), $H\preccurlyeq G$ means that some sequence of deleting [vertices](graph.md#vertex-graph-theory), deleting [edges](#edge-of-a-graph), and performing [edge contractions](#edge-contraction) produces $H$ up to [graph isomorphism](graph.md#graph-isomorphism). Deleting a [vertex](graph.md#vertex-graph-theory) also deletes all its incident [edges](#edge-of-a-graph); deleting an [edge](#edge-of-a-graph) leaves its endpoints. The [edge contraction](#edge-contraction) convention here removes resulting [self-loops](graph.md#loop-graph-theory) and duplicate [edges](#edge-of-a-graph).[The Basics (author-hosted chapter preview)](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview)

For an exact small example, let $G$ be the [cycle graph](#cycle-graph) $C_4$ with [vertices](graph.md#vertex-graph-theory) $u,v,a,b$ and [edges](#edge-of-a-graph) $uv,va,ab,bu$. Contract $uv$ to a new [vertex](graph.md#vertex-graph-theory) $w$. The surviving [edges](#edge-of-a-graph) are $wa,ab,bw$, giving the [complete graph](#complete-graph) $K_3$. Thus $K_3\preccurlyeq C_4$, although $C_4$ has no [triangle in a graph](graph.md#triangle-in-a-graph) as a [subgraph](#subgraph). The [branch sets of a graph minor](#branch-set-of-a-graph-minor) are $\{u,v\},\{a\},\{b\}$, with the original [edges](#edge-of-a-graph) $va,ab,bu$ witnessing all three required adjacencies. The first panel of the [edge contraction](#edge-contraction) diagram shows this operation.

A [subgraph](#subgraph) uses existing [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph); a [topological minor](#topological-minor) permits a [graph subdivision](#graph-subdivision) of the target as a [subgraph](#subgraph), so target [edges](#edge-of-a-graph) become [graph paths](#path-in-a-graph) with mutually disjoint interiors and no target [vertex](graph.md#vertex-graph-theory) in an interior. An ordinary [graph minor](#graph-minor) permits whole connected [branch sets of a graph minor](#branch-set-of-a-graph-minor) in place of target [vertices](graph.md#vertex-graph-theory). Every [topological minor](#topological-minor) is a [graph minor](#graph-minor), by contracting the replacement [graph paths](#path-in-a-graph).[Proposition 1.7.3(i)](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview)

The converse fails. Take the [tree](combinatorics.md#tree-graph-theory) with [edges](#edge-of-a-graph) $uv,ua,ub,vc,vd$. Contracting $uv$ gives the [star graph](#star-graph-theory) $K_{1,4}$. Yet the original [tree](combinatorics.md#tree-graph-theory) has [maximum degree](#maximum-degree) three, whereas every [graph subdivision](#graph-subdivision) of $K_{1,4}$ retains a centre of [degree of a vertex](#degree-graph-theory) four. Hence $K_{1,4}$ is a [graph minor](#graph-minor) but not a [topological minor](#topological-minor) of this [tree](combinatorics.md#tree-graph-theory). The difference is that a connected [branch set of a graph minor](#branch-set-of-a-graph-minor) may gather connections incident to several original [vertices](graph.md#vertex-graph-theory).

The counts of [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph) never increase under these operations. However, the $C_4$ example shows that being a [bipartite graph](#bipartite-graph) is not preserved: its [graph minor](#graph-minor) $K_3$ contains an [odd cycle](#odd-cycle). Its [chromatic number](#chromatic-number) also increases from two to three. A [connected graph](graph.md#connected-graph) stays connected under an [edge contraction](#edge-contraction), because the image of each [graph path](#path-in-a-graph) still connects its endpoints, but deletion can disconnect it. Thus one must check the particular [graph property](#graph-property) before treating it as preserved by taking [graph minors](#graph-minor).

Being a [planar graph](#planar-graph) is preserved: in a crossing-free drawing, shrink a contracted [edge](#edge-of-a-graph) and bring its incident [edges](#edge-of-a-graph) into the merged [vertex](graph.md#vertex-graph-theory); deletion merely removes parts of the drawing. This makes a nonplanar [graph minor](#graph-minor) a certificate that the original [graph](graph.md) is nonplanar. More strongly, for a finite [simple graph](graph.md#simple-graph), being a [planar graph](#planar-graph) is equivalent to having neither the [complete graph](#complete-graph) $K_5$ nor the [complete bipartite graph](#complete-bipartite-graph) $K_{3,3}$ as a [graph minor](#graph-minor). Finding the corresponding [branch sets of a graph minor](#branch-set-of-a-graph-minor) settles nonplanarity even when no literal $K_5$ or $K_{3,3}$ [subgraph](#subgraph) is present. The converse is a substantial theorem, rather than a consequence of preservation alone.[Theorem 4.4.6, equivalence of planarity and exclusion of K5 and K3,3 minors](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/planar-graphs-author-hosted-chapter-preview)

### Topological minor

↑ **Parent:** [Graph minor](#graph-minor)

A [topological minor](#topological-minor) records a network pattern whose [vertices](graph.md#vertex-graph-theory) remain individual junctions but whose [edges](#edge-of-a-graph) may become longer routes. For finite [simple graphs](graph.md#simple-graph), $H\preccurlyeq_{\mathrm{top}}G$ means that $G$ contains a [subgraph](#subgraph) that is a [graph subdivision](#graph-subdivision) of $H$ up to [graph isomorphism](graph.md#graph-isomorphism). Equivalently, choose distinct [branch vertices of a graph subdivision](#branch-vertex-of-a-graph-subdivision) $b_v\in V(G)$ for $v\in V(H)$ and a [graph path](#path-in-a-graph) $P_{uv}$ from $b_u$ to $b_v$ for every $uv\in E(H)$. These are [internally vertex-disjoint paths](#internally-vertex-disjoint-paths), and no internal [vertex](graph.md#vertex-graph-theory) of any $P_{uv}$ is a [branch vertex of a graph subdivision](#branch-vertex-of-a-graph-subdivision). Only endpoints corresponding to a shared target [vertex](graph.md#vertex-graph-theory) may be shared.[§1.7, printed p. 18: subdivisions; printed p. 21: topological-minor embeddings](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview)

The [graph subdivision](#graph-subdivision) example below replaces two [edges](#edge-of-a-graph) of a [triangle in a graph](graph.md#triangle-in-a-graph) by routes of two and three [edges](#edge-of-a-graph) while retaining its attached [leaf of a graph](#leaf-of-a-graph). If the host [graph](graph.md) also contains an extra [edge](#edge-of-a-graph) $BD$, the same routes still witness a [topological minor](#topological-minor): delete $BD$ when selecting the [subgraph](#subgraph). An [induced subgraph](#induced-subgraph) is not required. However, routes that merely connect the right pairs are insufficient: using a [branch vertex of a graph subdivision](#branch-vertex-of-a-graph-subdivision) as an intermediate junction, or making two routes share an internal [vertex](graph.md#vertex-graph-theory), can change the local network structure.

Every [topological minor](#topological-minor) is a [graph minor](#graph-minor). In each [branch path of a graph subdivision](#branch-path-of-a-graph-subdivision), contract all but one [edge](#edge-of-a-graph); the disjoint interiors let this shorten each route without merging distinct [branch vertices of a graph subdivision](#branch-vertex-of-a-graph-subdivision). This recovers $H$ after deleting unused [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph).[Proposition 1.7.3(i), printed p. 21](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview) The converse fails because an ordinary [branch set of a graph minor](#branch-set-of-a-graph-minor) can gather several junctions into one.

For the [tree](combinatorics.md#tree-graph-theory) $T$ with [vertices](graph.md#vertex-graph-theory) $u,v,a,b,c,d$ and [edges](#edge-of-a-graph) $uv,ua,ub,vc,vd$, contracting $uv$ produces a [star graph](#star-graph-theory) $K_{1,4}$: the [branch sets of a graph minor](#branch-set-of-a-graph-minor) are $\{u,v\},\{a\},\{b\},\{c\},\{d\}$. Both $u,v$ have [degree of a vertex](#degree-graph-theory) three; each of the other four [vertices](graph.md#vertex-graph-theory) is a [leaf of a graph](#leaf-of-a-graph) with [degree of a vertex](#degree-graph-theory) one. The new centre $w$ has four distinct [graph neighbours](#neighbour-of-a-vertex) $a,b,c,d$; its [degree of a vertex](#degree-graph-theory) is $3+3-2=4$, in agreement with the [edge contraction](#edge-contraction) formula.

<a id="image-a-graph-minor-can-combine-two-junctions-contracting-uv-creates-a-star-graph-with-a-centre-of-degree-of-a-vertex-four"></a>
![](topological-minor-tree-contraction-degree-obstruction.png)

**[Figure 11](#image-a-graph-minor-can-combine-two-junctions-contracting-uv-creates-a-star-graph-with-a-centre-of-degree-of-a-vertex-four). A graph minor can combine two junctions: contracting $uv$ creates a star graph with a centre of degree of a vertex four**.

Yet $K_{1,4}$ is not a [topological minor](#topological-minor) of $T$. In a [graph subdivision](#graph-subdivision) of $K_{1,4}$, four [branch paths of a graph subdivision](#branch-path-of-a-graph-subdivision) must leave the centre through four different [edges](#edge-of-a-graph); sharing their first internal [vertex](graph.md#vertex-graph-theory) would violate internal disjointness. Thus any host needs a [vertex](graph.md#vertex-graph-theory) of [degree of a vertex](#degree-graph-theory) at least four, whereas $\Delta(T)=3$. More generally, $H\preccurlyeq_{\mathrm{top}}G$ implies $\Delta(H)\leq\Delta(G)$, where $\Delta$ is the [maximum degree of a graph](#maximum-degree-of-a-graph). This bound concerns the host [graph](graph.md); extra unused [edges](#edge-of-a-graph) may make its [branch vertices of a graph subdivision](#branch-vertex-of-a-graph-subdivision) have larger [degrees of vertices](#degree-graph-theory) than their target counterparts.

This distinction matters when a network's individual junctions have a limited number of connections: replacing a connection by a route preserves the number of routes meeting at each chosen junction, while contracting a connected region can combine connections from separate junctions. It also explains why a small nonplanar pattern can hide inside long routes. By [Kuratowski's theorem](#kuratowski-s-theorem), a finite [simple graph](graph.md#simple-graph) is a [planar graph](#planar-graph) exactly when it has neither the [complete graph](#complete-graph) $K_5$ nor the [complete bipartite graph](#complete-bipartite-graph) $K_{3,3}$ as a [topological minor](#topological-minor). The obstruction is a [graph subdivision](#graph-subdivision) inside the network, regardless of the number of intermediate [vertices](graph.md#vertex-graph-theory).

### Rooted branch-set reduction

↑ **Parent:** [Graph minor](#graph-minor)

Let $q\ge2$ be even, let $S=\{x_1,\ldots,x_q\}$, and suppose a [graph](graph.md) has $h$ disjoint nonempty [vertex](graph.md#vertex-graph-theory) [sets](set.md) $C_1,\ldots,C_h$, where $h\ge d+3q/2$. Suppose each $G[C_i]$ is connected or every one of its [graph components](graph.md#component-graph-theory) meets $S$, and each $C_i$ is adjacent to all but at most $d$ of the other $C_j$ not meeting $S$. Assume also that no [rooted separation of a graph](#rooted-separation-of-a-graph) of order below $q$ avoids $d+1$ of these [sets](set.md). Then there are $m=h-q/2$ disjoint connected [vertex](graph.md#vertex-graph-theory) [sets](set.md) $D_1,\ldots,D_m$ such that $x_i\in D_i$ for $1\le i\le q$ and each of these first $q$ [sets](set.md) is adjacent to all but at most $d$ of $D_{q+1},\ldots,D_m$.

Here adjacency of [sets](set.md) means existence of an [edge](#edge-of-a-graph) between them. A [rooted separation of a graph](#rooted-separation-of-a-graph) is $(A,B)$ with $A\cup B=V(G)$, $S\subseteq A$, no [edges](#edge-of-a-graph) between $A\setminus B$ and $B\setminus A$, and order $|A\cap B|$. It avoids $C_i$ when $A\cap C_i=\varnothing$. We prove the reduction by [induction](foundations-of-mathematics.md#mathematical-induction), first on the [vertex](graph.md#vertex-graph-theory) count and then on the [edge](#edge-of-a-graph) count; any counterexample chosen minimal in this ordering will be impossible.

We may delete [edges](#edge-of-a-graph) joining two [vertices](graph.md#vertex-graph-theory) of $S$. They cannot affect [rooted separations of a graph](#rooted-separation-of-a-graph), since $S$ lies wholly on the first side. Within a branch [set](set.md), their deletion can only split a [graph component](graph.md#component-graph-theory) into [graph components](graph.md#component-graph-theory) each containing an endpoint in $S$, so the branch-set hypothesis also persists. An isolated [vertex](graph.md#vertex-graph-theory) outside $S$ and all branch [sets](set.md) can be deleted. An isolated [vertex](graph.md#vertex-graph-theory) $v\in S$ is also impossible, since $(S,V(G)\setminus\{v\})$ has order $q-1$ and avoids at least $h-q\ge d+q/2\ge d+1$ [sets](set.md). Thus in a minimal counterexample $S$ is independent, and every isolated [vertex](graph.md#vertex-graph-theory) outside $S$ belongs to a singleton branch [set](set.md).

Consider a [rooted separation of a graph](#rooted-separation-of-a-graph) $(A,B)$ of order exactly $q$ avoiding at least $d+1$ branch [sets](set.md), and put $S'=A\cap B$. Restrict to $G'=G[B]-E(G[S'])$ and $C'_i=C_i\cap B$. Each $C'_i$ is nonempty: any $C_i$ not itself avoided is adjacent to at least one of the $d+1$ avoided [sets](set.md), and the endpoint of such an [edge](#edge-of-a-graph) in $C_i$ must lie in $B$. If a [graph component](graph.md#component-graph-theory) of $G'[C'_i]$ misses $S'$, it lies in $B\setminus A$ and is a whole [graph component](graph.md#component-graph-theory) of $G[C_i]$, with no [vertex](graph.md#vertex-graph-theory) of $S$. The original hypothesis then forces $G[C_i]$ to be connected and $C'_i=C_i$, entirely outside $A$. Thus each restricted [set](set.md) is connected or all its [graph components](graph.md#component-graph-theory) meet $S'$. In particular every $C'_j$ missing $S'$ equals an original [set](set.md) outside $A$, so all its required adjacencies from $C'_i$ persist.

A [rooted separation of a graph](#rooted-separation-of-a-graph) $(A',B')$ of $G'$ avoiding $d+1$ restricted [sets](set.md) lifts to $(A\cup A',B')$ in $G$, of the same order: an avoided restricted [set](set.md) misses $S'$, hence is an original [set](set.md) outside $A$. The [edges](#edge-of-a-graph) removed inside $S'$ do not obstruct lifting, since $S'\subseteq A'$. This proves the required separation hypothesis for $G'$. If $G'$ is smaller, [induction](foundations-of-mathematics.md#mathematical-induction) gives the desired connected [sets](set.md) rooted at $S'$. Moreover $G[A]$ has $q$ disjoint [graph paths](#path-in-a-graph) from $S$ to $S'$, by the [Menger theorem](#menger-theorem). Indeed a separator of smaller order between these [sets](set.md) would give a [rooted separation of a graph](#rooted-separation-of-a-graph) of $G$ of smaller order still avoiding those $d+1$ original [sets](set.md). Truncate the [graph paths](#path-in-a-graph) at their first visits to $S'$, label their endpoints accordingly, and adjoin each [graph path](#path-in-a-graph) to the corresponding rooted connected [set](set.md). They meet $B$ only in their distinct endpoints, so this gives the desired [sets](set.md) for $G$, a contradiction. Consequently in a minimal counterexample every such separation of order $q$ has $B=V(G)$ and $A=S$, an [independent set](#independent-set-graph-theory).

Now contract any [edge](#edge-of-a-graph) whose endpoints do not belong to two different branch [sets](set.md). Its endpoints cannot both lie in $S$, so the image of $S$ still has size $q$. The branch-set conditions persist. If the contraction created a forbidden [rooted separation of a graph](#rooted-separation-of-a-graph) of order below $q$, its lift would have order below $q$, except possibly when the contracted [vertex](graph.md#vertex-graph-theory) lies in its separator. In that case the lifted order increases by one and is at most $q$. Equality would put the contracted [edge](#edge-of-a-graph) inside $A$, contradicting the just-proved independence of $A$ for an order-$q$ separation avoiding $d+1$ [sets](set.md). Thus the separation hypothesis also persists. Applying [induction](foundations-of-mathematics.md#mathematical-induction) in the contracted [graph](graph.md) and expanding the contracted [vertex](graph.md#vertex-graph-theory) would produce the required disjoint connected [sets](set.md). Hence **every [edge](#edge-of-a-graph) in a minimal counterexample joins two different branch [sets](set.md)**.

Every [vertex](graph.md#vertex-graph-theory) outside the branch [sets](set.md) would be isolated, since every [edge](#edge-of-a-graph) joins two branch [sets](set.md); such an isolated [vertex](graph.md#vertex-graph-theory) could be deleted. Thus the branch [sets](set.md) cover the [graph](graph.md). Each nonsingleton branch [set](set.md) is therefore an [independent set](#independent-set-graph-theory), and all its [vertices](graph.md#vertex-graph-theory) belong to $S$, because each of its singleton [graph components](graph.md#component-graph-theory) must meet $S$. Let $C$ be the union of the nonsingleton branch [sets](set.md), and write $c=|C|\le q$. There is a [matching in a graph](#matching-graph-theory) from $C$ into $V(G)\setminus S$. Otherwise the [Hall marriage theorem](#hall-s-marriage-theorem) gives $X\subseteq C$ with neighbourhood $Y\subseteq V(G)\setminus S$ satisfying $|Y|<|X|$. Since $S$ is independent, $(S\cup Y,V(G)\setminus X)$ is a [rooted separation of a graph](#rooted-separation-of-a-graph) of order $q-|X|+|Y|<q$. It avoids every singleton branch [set](set.md) outside $S\cup Y$, of which there are at least

$$
|V(G)|-q-|Y|\ge |V(G)|-q-c+1\ge h-\frac c2-q+1\ge h-\frac{3q}2+1\ge d+1.
$$

The penultimate counting bound uses that the nonsingleton [sets](set.md) number at most $c/2$, so $|V(G)|-c\ge h-c/2$. This contradicts the separation hypothesis.

Use that [matching in a graph](#matching-graph-theory) to make a two-vertex connected [set](set.md) for each terminal in $C$; terminals outside $C$ remain singleton [sets](set.md). There are at least

$$
|V(G)|-q-c\ge h-\frac{3q}2=m-q
$$

unused [vertices](graph.md#vertex-graph-theory), all singleton original branch [sets](set.md). Choose $m-q$ of them for the remaining $D_i$. Every rooted $D_i$ contains a singleton original branch [set](set.md): either its terminal, or its terminal's matched [neighbour](#neighbour-of-a-vertex). That singleton misses at most $d$ of the selected nonterminal singleton [sets](set.md). This constructs the desired family and completes the proof.

### Complete graph minor density threshold

↑ **Parent:** [Graph minor](#graph-minor)

The complete graph minor density threshold is

$$
c(t)=\inf\{c:\text{every nonempty finite graph }G\text{ with }e(G)\geq c|G|\text{ has a }K_t\text{ minor}\}.
$$

The density here is [edge](#edge-of-a-graph) count divided by order, half the average [degree of a vertex](#degree-graph-theory). For large $t$, this threshold has order $t\sqrt{\log t}$, with the logarithm taken to base $e$.

#### Dense minor with bounded order and high minimum degree

↑ **Parent:** [Complete graph minor density threshold](#complete-graph-minor-density-threshold)

For each positive integer $k$, a nonempty [graph](graph.md) satisfying $e(G)\geq11k|G|$ has a [graph minor](#graph-minor) $H$ satisfying

$$
|H|\leq11k+2,\qquad 2\delta(H)\geq |H|+4k-1.
$$

The density hypothesis is a lower bound. Reversing its inequality would be false for an edgeless [graph](graph.md). This auxiliary lemma can be used to establish a $7t\sqrt{\log t}$ upper bound for the [complete graph minor density threshold](#complete-graph-minor-density-threshold).

### Branch set of a graph minor

↑ **Parent:** [Graph minor](#graph-minor)

A [branch set of a graph minor](#branch-set-of-a-graph-minor) is the connected region representing one target [vertex](graph.md#vertex-graph-theory). For finite [simple graphs](graph.md#simple-graph) $G$ and $H$, a witness to $H\preccurlyeq G$ assigns a nonempty [set](set.md) $B_x\subseteq V(G)$ to each $x\in V(H)$, such that the [sets](set.md) are pairwise disjoint, each [induced subgraph](#induced-subgraph) $G[B_x]$ is a [connected graph](graph.md#connected-graph), and every $xy\in E(H)$ has a witnessing [edge](#edge-of-a-graph) of $G$ between $B_x$ and $B_y$. Extra [edges](#edge-of-a-graph) between [branch sets of a graph minor](#branch-set-of-a-graph-minor) are allowed: they can be deleted. Unused [vertices](graph.md#vertex-graph-theory) are also allowed.[Minor Containment and Disjoint Paths in almost-linear time by Tuukka Korhonen and others](mathematics-bibliography.md#minor-containment-and-disjoint-paths-in-almost-linear-time-by-tuukka-korhonen-and-others)

<a id="image-connected-branch-sets-of-a-graph-minor-and-their-witnessing-edges-with-an-optional-edge-deletion"></a>
![](graph-minor-connected-branch-set-adjacency.png)

**[Figure 12](#image-connected-branch-sets-of-a-graph-minor-and-their-witnessing-edges-with-an-optional-edge-deletion). Connected branch sets of a graph minor and their witnessing edges, with an optional edge deletion**.

In the diagram, the host [graph](graph.md) has [vertex set](graph.md#vertex-set) $\{1,2,3,4,5,6\}$ and [edges](#edge-of-a-graph)

$$
12,\ 34,\ 56,\ 23,\ 45,\ 61,\ 24.
$$

Choose $B_A=\{1,2\}$, $B_B=\{3,4\}$, and $B_C=\{5,6\}$. Their internal [edges](#edge-of-a-graph) $12,34,56$ establish connectedness. The [edges](#edge-of-a-graph) $23,45,61$ witness $AB,BC,CA$, respectively, so they form a model of the [complete graph](#complete-graph) $K_3$. The additional [edge](#edge-of-a-graph) $24$ also joins $B_A$ to $B_B$; it supplies another witness for the same target [edge](#edge-of-a-graph), not a fourth target [edge](#edge-of-a-graph). Contracting $12,34,56$ and merging duplicate [edges](#edge-of-a-graph) gives exactly $\{AB,BC,CA\}$.

The same [branch sets of a graph minor](#branch-set-of-a-graph-minor) also witness the [path graph](#path-graph) $A,B,C$: retain the witnesses $23,45$, and delete $61$ to remove the unwanted $AC$ adjacency. This demonstrates why the definition requires an [edge](#edge-of-a-graph) for every target adjacency, without forbidding other adjacencies in the host [graph](graph.md). For a [complete graph](#complete-graph) $K_t$, there are no unwanted pairs: its model consists of $t$ disjoint connected [branch sets of a graph minor](#branch-set-of-a-graph-minor) with an [edge](#edge-of-a-graph) between every pair.

To turn a model into an operation sequence, keep a [spanning tree](combinatorics.md#spanning-tree) inside each $G[B_x]$, keep one witnessing [edge](#edge-of-a-graph) for each [edge](#edge-of-a-graph) of $H$, and delete all other [edges](#edge-of-a-graph) and unused [vertices](graph.md#vertex-graph-theory). Contract each chosen [spanning tree](combinatorics.md#spanning-tree) to one [vertex](graph.md#vertex-graph-theory). Disjointness prevents two target [vertices](graph.md#vertex-graph-theory) from merging; connectedness provides the [edge contractions](#edge-contraction) that merge each individual region. Conversely, track the original [vertices](graph.md#vertex-graph-theory) merged into every surviving [vertex](graph.md#vertex-graph-theory) during a deletion-and-[edge contraction](#edge-contraction) sequence. They form disjoint connected [branch sets of a graph minor](#branch-set-of-a-graph-minor), and each surviving [edge](#edge-of-a-graph) comes from an original [edge](#edge-of-a-graph) between its two regions. A list of these regions, their connecting [trees](combinatorics.md#tree-graph-theory), and their witnessing [edges](#edge-of-a-graph) therefore gives a directly checkable certificate.

#### Random branch-set construction of a complete graph minor

↑ **Parent:** [Branch set of a graph minor](#branch-set-of-a-graph-minor)

In a dense [graph](graph.md) with many [common neighbours](#common-neighbour) for every pair of [vertices](graph.md#vertex-graph-theory), choose disjoint random small sets. A set is good if few [vertices](graph.md#vertex-graph-theory) have no neighbour in it. The [Markov inequality](probability-inequality.md#markov-s-inequality) controls the number of bad sets, and random sampling makes almost every pair of good sets adjacent. Add unused [common neighbours](#common-neighbour) to connect each set and to repair the remaining missing adjacencies. If the number of used [vertices](graph.md#vertex-graph-theory) stays below every common-neighbour count, this constructs disjoint [branch sets of a graph minor](#branch-set-of-a-graph-minor) representing a large [complete graph](#complete-graph).

### Edge contraction

↑ **Parent:** [Graph minor](#graph-minor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edge_contraction)

An [edge contraction](#edge-contraction) merges the two endpoints of an existing [edge](#edge-of-a-graph). For a finite [simple graph](graph.md#simple-graph) $G$ and $e=uv$, replace $u,v$ by a new [vertex](graph.md#vertex-graph-theory) $w$. Retain every [edge](#edge-of-a-graph) with neither endpoint in $\{u,v\}$, and join $w$ to every member of

$$
N_{G/e}(w)=(N_G(u)\cup N_G(v))\setminus\{u,v\}.
$$

Here $N_G(u)$ and $N_G(v)$ denote the original open [graph neighbourhoods](#graph-neighbourhood), and $N_{G/e}(w)$ is the new [graph neighbourhood](#graph-neighbourhood). Remove the [self-loop](graph.md#loop-graph-theory) arising from $uv$ and merge duplicate [edges](#edge-of-a-graph), so the result $G/e$ is again a [simple graph](graph.md#simple-graph). This is not deletion of $uv$, which keeps both original [vertices](graph.md#vertex-graph-theory).[The Basics (author-hosted chapter preview)](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview)

<a id="image-edge-contraction-of-a-four-cycle-and-a-triangle-in-a-graph-common-neighbours-determine-the-lost-edge-count"></a>
![](graph-edge-contraction-common-neighbour-count.png)

**[Figure 13](#image-edge-contraction-of-a-four-cycle-and-a-triangle-in-a-graph-common-neighbours-determine-the-lost-edge-count). Edge contraction of a four-cycle and a triangle in a graph: common neighbours determine the lost edge count**.

The left example contracts $uv$ in the [cycle graph](#cycle-graph) $C_4$ to give $\{wa,ab,bw\}$. Its endpoints have no [common neighbours](#common-neighbour), so four [edges](#edge-of-a-graph) become three. The right example contracts $uv$ in the [triangle in a graph](graph.md#triangle-in-a-graph) with [edges](#edge-of-a-graph) $uv,ua,va$. Its endpoints have the single [common neighbour](#common-neighbour) $a$, so the two [edges](#edge-of-a-graph) $ua,va$ become one [edge](#edge-of-a-graph) $wa$: three [edges](#edge-of-a-graph) become one.

For any such [edge contraction](#edge-contraction), the exact counts are

$$
|V(G/e)|=|V(G)|-1,\qquad |E(G/e)|=|E(G)|-1-|N_G(u)\cap N_G(v)|.
$$

The contracted [edge](#edge-of-a-graph) accounts for one loss. Each [common neighbour](#common-neighbour) $z$ contributes exactly one further loss, since $uz,vz$ become a single [edge](#edge-of-a-graph) $wz$. All other [edges](#edge-of-a-graph) correspond one-to-one to surviving [edges](#edge-of-a-graph). In particular the new [degree of a vertex](#degree-graph-theory) is

$$
\deg_{G/e}(w)=\deg_G(u)+\deg_G(v)-2-|N_G(u)\cap N_G(v)|.
$$

These formulas depend on simplifying to a [simple graph](graph.md#simple-graph); a [multigraph](graph.md#multigraph) convention that retains duplicate [edges](#edge-of-a-graph) has different counts. In the six-[vertex](graph.md#vertex-graph-theory) [branch set of a graph minor](#branch-set-of-a-graph-minor) diagram, contracting $12$ loses one [edge](#edge-of-a-graph), contracting the resulting $34$ loses two because of its [common neighbour](#common-neighbour) $A$, and contracting $56$ loses one. Hence its seven [edges](#edge-of-a-graph) become the three [edges](#edge-of-a-graph) of $K_3$: $7-1-2-1=3$.

An [edge contraction](#edge-contraction) can increase a [degree of a vertex](#degree-graph-theory) even while decreasing both total counts. For example, contracting $uv$ in the [tree](combinatorics.md#tree-graph-theory) with [edges](#edge-of-a-graph) $uv,ua,ub,vc,vd$ merges two [vertices](graph.md#vertex-graph-theory) of [degree of a vertex](#degree-graph-theory) three into one of [degree of a vertex](#degree-graph-theory) four. This is the mechanism behind the distinction between a [graph minor](#graph-minor) and a [topological minor](#topological-minor).

## Vertex cover

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vertex_cover)

A [vertex cover](#vertex-cover) chooses [vertices](graph.md#vertex-graph-theory) that collectively touch every [edge](#edge-of-a-graph) of a [graph](graph.md). Think of placing monitors at junctions: if a monitor watches every connection incident to its junction, a [vertex cover](#vertex-cover) watches all connections. The [minimum vertex cover](#minimum-vertex-cover) asks how few monitors suffice. This is a model of covering connections through their endpoints, rather than of monitoring distances in the drawing.

For a finite [simple graph](graph.md#simple-graph) $G=(V,E)$, a [vertex cover](#vertex-cover) is a [subset](set.md#subset) $C\subseteq V$ satisfying

$$
\{u,v\}\in E\Longrightarrow u\in C\ \text{or}\ v\in C.
$$

Both endpoints may be selected; the condition requires at least one. An [isolated vertex](#isolated-vertex) covers no [edge](#edge-of-a-graph), so a [minimum vertex cover](#minimum-vertex-cover) never needs it.[Diestel, Graph Theory, fourth electronic edition, Section 2.1, definition of vertex cover](https://diestel-graph-theory.com/Sample.pdf)

Take the [cycle graph](#cycle-graph) $C_5$ with [vertices](graph.md#vertex-graph-theory) $0,1,2,3,4$ and [edges](#edge-of-a-graph) $01,12,23,34,40$. The [set](set.md) $C=\{1,3,4\}$ is a [vertex cover](#vertex-cover): [vertex](graph.md#vertex-graph-theory) $1$ covers $01$ and $12$, [vertex](graph.md#vertex-graph-theory) $3$ covers $23$ and $34$, and [vertex](graph.md#vertex-graph-theory) $4$ covers $40$ as well as $34$. In particular, the closing [edge](#edge-of-a-graph) $40$ is covered even though [vertex](graph.md#vertex-graph-theory) $0$ is unselected.

The unselected [vertices](graph.md#vertex-graph-theory) $I=V\setminus C=\{0,2\}$ form an [independent set](#independent-set-graph-theory). This is the key connection: an [edge](#edge-of-a-graph) missed by $C$ would have both endpoints in $I$, precisely what an [independent set](#independent-set-graph-theory) forbids. For every [subset](set.md#subset) $C\subseteq V$,

$$
C\text{ is a vertex cover}\quad\Longleftrightarrow\quad V\setminus C\text{ is an independent set}.
$$

Here $V\setminus C$ is the [complement of a set](set.md#complement-of-a-set) within $V$; the [graph](graph.md) itself keeps all its [edges](#edge-of-a-graph). The [complement graph](#complement-graph) is a different construction.[Barak, Introduction to Theoretical Computer Science, Chapter 14, vertex-cover exercise](https://introtcs.org/public/lec_12_NP.html)

<a id="image-a-minimum-vertex-cover-and-its-maximum-independent-complement-on-the-same-five-cycle"></a>
![](vertex-cover-independent-complement.png)

**[Figure 14](#image-a-minimum-vertex-cover-and-its-maximum-independent-complement-on-the-same-five-cycle). A minimum vertex cover and its maximum independent complement on the same five-cycle**.

The endpoints of any [maximal matching](#maximal-matching) form a [vertex cover](#vertex-cover): an [edge](#edge-of-a-graph) avoiding all endpoints would enlarge that [matching in a graph](#matching-graph-theory). Consequently a [graph](graph.md) with no [matching in a graph](#matching-graph-theory) of size $s$ has a [vertex cover](#vertex-cover) of size at most $2(s-1)$. This supplies a convenient [vertex cover](#vertex-cover), but it need not be a [minimum vertex cover](#minimum-vertex-cover).

### Minimum vertex cover

↑ **Parent:** [Vertex cover](#vertex-cover)

A [minimum vertex cover](#minimum-vertex-cover) is a [vertex cover](#vertex-cover) of smallest [cardinality](set-theory.md#cardinality) among all [vertex covers](#vertex-cover) of the same finite [simple graph](graph.md#simple-graph). The optimum size is the [vertex cover number](#vertex-cover-number). By the [complement of a set](set.md#complement-of-a-set) correspondence, a [minimum vertex cover](#minimum-vertex-cover) leaves a largest possible [independent set](#independent-set-graph-theory) unselected.

Minimum size is stronger than merely being unable to remove a selected [vertex](graph.md#vertex-graph-theory). In the [star graph](#star-graph-theory) $K_{1,3}$, the three leaves form a [vertex cover](#vertex-cover) from which no [vertex](graph.md#vertex-graph-theory) can be removed: each leaf covers its own [edge](#edge-of-a-graph). Nevertheless, the centre alone is a [minimum vertex cover](#minimum-vertex-cover) of size one. Such an inclusion-minimal [vertex cover](#vertex-cover) can therefore be much larger than a [minimum vertex cover](#minimum-vertex-cover).

#### Vertex cover number

↑ **Parent:** [Minimum vertex cover](#minimum-vertex-cover)

The [vertex cover number](#vertex-cover-number) records the size of a [minimum vertex cover](#minimum-vertex-cover):

$$
\tau(G)=\min\{|C|:C\subseteq V(G),\ C\text{ is a vertex cover of }G\}.
$$

The [vertex cover number](#vertex-cover-number) is a number, while a [minimum vertex cover](#minimum-vertex-cover) is a [set](set.md) attaining it. For the [cycle graph](#cycle-graph) $C_5$, the [independence number](#independence-number) is $2$, so the complement correspondence gives $\tau(C_5)=5-2=3$. The [vertex cover](#vertex-cover) $\{1,3,4\}$ above attains this size.

Every [matching in a graph](#matching-graph-theory) gives a lower bound on the [vertex cover number](#vertex-cover-number). Its [edges](#edge-of-a-graph) have no shared endpoints, so covering each selected [edge](#edge-of-a-graph) requires a different [vertex](graph.md#vertex-graph-theory). Thus, for any [matching in a graph](#matching-graph-theory) $M$ and any [vertex cover](#vertex-cover) $C$,

$$
|M|\leq |C|,\qquad \nu(G)\leq\tau(G),
$$

where $\nu(G)$ is the [matching number](#matching-number). Exhibiting a [matching in a graph](#matching-graph-theory) and a [vertex cover](#vertex-cover) of the same size certifies that both are optimum. [Kőnig's theorem for bipartite matching](#konig-s-theorem-graph-theory) says that every finite [bipartite graph](#bipartite-graph) admits this equality: $\nu(G)=\tau(G)$.[Diestel, Graph Theory, Section 2.1, Theorem 2.1.1 and its lower-bound argument](https://diestel-graph-theory.com/Sample.pdf)

For the [complete bipartite graph](#complete-bipartite-graph) $K_{2,3}$, let the left [vertices](graph.md#vertex-graph-theory) be $L=\{a,b\}$ and the right [vertices](graph.md#vertex-graph-theory) be $R=\{x,y,z\}$. All six [edges](#edge-of-a-graph) join $L$ to $R$. Selecting $C=L$ covers every [edge](#edge-of-a-graph); selecting $M=\{ax,by\}$ gives a [matching in a graph](#matching-graph-theory) of size two. The lower bound and this [vertex cover](#vertex-cover) give $2\leq\tau(K_{2,3})\leq2$, so $\tau(K_{2,3})=\nu(K_{2,3})=2$. The remaining [vertices](graph.md#vertex-graph-theory) $R$ form a largest [independent set](#independent-set-graph-theory) of size three. Crossings of drawn [edges](#edge-of-a-graph) are not extra [vertices](graph.md#vertex-graph-theory).

<a id="image-two-disjoint-matching-edges-certify-that-the-two-left-vertices-are-a-minimum-cover-of-k₂-₃"></a>
![](bipartite-matching-cover-certificate.png)

**[Figure 15](#image-two-disjoint-matching-edges-certify-that-the-two-left-vertices-are-a-minimum-cover-of-k₂-₃). Two disjoint matching edges certify that the two left vertices are a minimum cover of K₂,₃**.

The [bipartite graph](#bipartite-graph) hypothesis matters. In a [triangle in a graph](graph.md#triangle-in-a-graph), any two [vertices](graph.md#vertex-graph-theory) form a [minimum vertex cover](#minimum-vertex-cover), while any two [edges](#edge-of-a-graph) share an endpoint. Hence $\tau(K_3)=2$ and $\nu(K_3)=1$. Similarly, the [cycle graph](#cycle-graph) $C_5$ has $\tau(C_5)=3$ and $\nu(C_5)=2$. The inequality for the [matching number](#matching-number) remains valid, but equality can fail.

### 3-SAT reduction to vertex cover

↑ **Parent:** [Vertex cover](#vertex-cover)

A [polynomial-time many-one reduction](computer-science.md#polynomial-time-many-one-reduction) represents each variable by an adjacent literal pair and each clause by a [triangle in a graph](graph.md#triangle-in-a-graph). Connect each occurrence vertex to its corresponding literal vertex. A [vertex cover](#vertex-cover) of size $n+2m$ must choose one literal vertex per variable and two vertices per clause, and its omitted clause vertex forces a true literal. Conversely a satisfying [Boolean valuation](mathematical-logic.md#boolean-valuation) supplies such a cover. This establishes [NP-hardness](computer-science.md#np-hardness) of the vertex-cover decision problem from [3-SAT](computer-science.md#3-sat).

## Binomial random graph

↑ **Parent:** [Graph theory](graph-theory.md)

The binomial random graph $G(n,p)$ has vertex set $\{1,\ldots,n\}$ and includes each of the $\binom n2$ possible edges independently with probability $p$.

### Poisson threshold for vertices lying in no triangle

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

For a fixed set of $r$ vertices, exclude all triangles meeting that set. Their total expectation is $r\log(n/c)+o(1)$. Distinct triangle pairs sharing an edge contribute $O_r(n^3p^5)=o(1)$ to the [Janson dependency sum](probability-inequality.md#janson-dependency-sum). [Harris' inequality](probability-inequality.md#harris-inequality) and [Janson inequality](probability-inequality.md#janson-inequality) bound the avoidance probability between matching exponentials, giving $(c/n)^r(1+o(1))$. The [factorial-moment criterion for Poisson convergence](markov-process.md#factorial-moment-criterion-for-poisson-convergence) then gives the displayed law.

### Deferred edge exposure in greedy independent-set colouring

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

Construct an [independent set](#independent-set-graph-theory) by choosing a candidate vertex, exposing only its incident edges, and retaining its non-neighbours as candidates. Once the chosen independent set is removed, every exposed edge has a removed endpoint. Thus the remaining internal edges still have their independent original laws, conditional on the revealed history. This special exposure rule permits fresh-binomial estimates for successive classes; an arbitrary adaptively selected vertex subset does not have that property.

### Strictly balanced graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

A finite [graph](graph.md) $H$ with at least one [edge](#edge-of-a-graph) is strictly balanced when every proper nonempty [subgraph](#subgraph) $F$ has smaller edge-to-vertex ratio. It is connected and has no isolated [vertices](graph.md#vertex-graph-theory): otherwise a component of at least the average density, or deletion of isolated [vertices](graph.md#vertex-graph-theory), violates the inequality. The density condition suppresses overlapping copies at the sparse appearance scale.

#### Poisson limit for strictly balanced subgraph counts

↑ **Parent:** [Strictly balanced graph](#strictly-balanced-graph)

Here $v,e,a$ are the numbers of [vertices](graph.md#vertex-graph-theory), [edges](#edge-of-a-graph) and [graph automorphisms](graph.md#graph-automorphism) of $H$. Vertex-disjoint ordered $r$-tuples contribute $(n)_{rv}p^{re}/a^r\to(c^e/a)^r$ to the [factorial moment](markov-process.md#factorial-moment). Adding a copy overlapping the previous union in $f$ [vertices](graph.md#vertex-graph-theory) and $g$ [edges](#edge-of-a-graph) changes the power of $n$ by $-f+(v/e)g\le0$, strictly when the intersection is a proper nonempty [subgraph](#subgraph). The first overlap is strict because $H$ is connected and the previous copies are disjoint. Finitely many overlap types therefore contribute $o(1)$. The [factorial-moment criterion for Poisson convergence](markov-process.md#factorial-moment-criterion-for-poisson-convergence) gives the result.

### Missing common-neighbour count in a binomial random graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

Let $X$ count unordered [vertex](graph.md#vertex-graph-theory) pairs with no [common neighbour](#common-neighbour) in a [binomial random graph](#binomial-random-graph). Each other [vertex](graph.md#vertex-graph-theory) provides the required pair of [edges](#edge-of-a-graph) independently, with success probability $p^2$. A fixed pair has no common neighbour with probability $(1-p^2)^{n-2}$. Summing its indicators gives the displayed [expectation](probability-theory.md#expected-value).

#### Diameter bound for a fixed-density binomial random graph

↑ **Parent:** [Missing common-neighbour count in a binomial random graph](#missing-common-neighbour-count-in-a-binomial-random-graph)

For fixed $0<p<1$, the [missing common-neighbour count in a binomial random graph](#missing-common-neighbour-count-in-a-binomial-random-graph) has [expectation](probability-theory.md#expected-value) tending to zero. The [Markov inequality](probability-inequality.md#markov-s-inequality) therefore shows that every pair has a [common neighbour](#common-neighbour) with probability tending to one. On that event every [graph distance](#distance-graph-theory) is at most two, so the [graph](graph.md) is [connected](geometry-and-topology.md#connected-space) and its [graph diameter](#graph-diameter) is at most two.

### Chromatic number of a binomial random graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

For a fixed probability strictly between zero and one, the largest independent set has leading size $2\log_{1/(1-p)}n$, giving a lower bound for colouring. The matching upper bound uses [independent sets in every large subset of a dense random graph](#independent-sets-in-every-large-subset-of-a-dense-random-graph), then repeatedly colours and removes such sets. A sufficiently strong probability estimate makes the failure contribution negligible for the expectation.

#### Independent sets in every large subset of a dense random graph

↑ **Parent:** [Chromatic number of a binomial random graph](#chromatic-number-of-a-binomial-random-graph)

For fixed $p$ and $\gamma>0$, [Janson inequality](probability-inequality.md#janson-inequality) bounds the failure probability for a given large [vertex](graph.md#vertex-graph-theory) subset by $\exp(-c|U|^2/(\log n)^4)$. A union bound over all at most $2^n$ subsets still tends to zero. This uniform statement is essential because [vertex](graph.md#vertex-graph-theory) sets left by a greedy colouring procedure depend on the [graph](graph.md); one cannot assume each adaptively chosen remainder is an independent fresh random [graph](graph.md).

### Vertex exposure for chromatic number

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

Group random [edges](#edge-of-a-graph) by their larger endpoint. These independent coordinates each change [edges](#edge-of-a-graph) incident to only one [vertex](graph.md#vertex-graph-theory). Removing that [vertex](graph.md#vertex-graph-theory) leaves the same [graph](graph.md) under any two outcomes, so their [chromatic numbers](#chromatic-number) differ by at most one. The [McDiarmid inequality](probability-inequality.md#mcdiarmid-s-inequality) with $n$ coordinate ranges of length one gives the displayed concentration bound.

### Chromatic number of the half-density binomial random graph

↑ **Parent:** [Binomial random graph](#binomial-random-graph)

For the [binomial random graph](#binomial-random-graph) $G(n,1/2)$, the [chromatic number](#chromatic-number) is $(1+o(1))n/(2\log_2n)$ [with high probability](probabilistic-combinatorics.md#with-high-probability). A [first moment method](probability-inequality.md#first-moment-method) bounds the [independence number](#independence-number) above. [Edge-disjoint clique packing](#edge-disjoint-clique-packing) in the [complement graph](#complement-graph), followed by an [edge-exposure martingale](martingale.md#edge-exposure-martingale) and a [union bound](probability-inequality.md#boole-s-inequality) over moderately large [vertex](graph.md#vertex-graph-theory) sets, supplies [independent sets](#independent-set-graph-theory) for [greedy colouring by removing independent sets](#greedy-colouring-by-removing-independent-sets).

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

If $np\to0$, the [triangle count in a binomial random graph](#triangle-count-in-a-binomial-random-graph) has [expectation](probability-theory.md#expected-value) at most $(np)^3/6\to0$, so the [Markov inequality](probability-inequality.md#markov-s-inequality) shows there are no [triangles in a graph](graph.md#triangle-in-a-graph) with probability tending to one. If $np\to\infty$, the [triangle variance in a binomial random graph](#triangle-variance-in-a-binomial-random-graph) divided by the squared mean is $O((np)^{-3})+O((n^2p)^{-1})\to0$. The [second moment method](probability-inequality.md#second-moment-method) then gives at least one [triangle in a graph](graph.md#triangle-in-a-graph) with probability tending to one. At the intermediate scale $np\to c\in(0,\infty)$, a nontrivial [Poisson limit for triangles in a binomial random graph](#poisson-limit-for-triangles-in-a-binomial-random-graph) describes the count.

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

## Graph

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](graph.md)

## Graph coloring

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_coloring)

A [graph coloring](#graph-coloring) assigns labels called colours to elements of a [graph](graph.md), subject to specified constraints. Here we focus on [proper vertex colouring](#proper-vertex-coloring) of a [simple graph](graph.md#simple-graph) $G=(V,E)$: it is an [undirected graph](#undirected-graph) with a [finite set](set.md#finite-set) of [vertices](graph.md#vertex-graph-theory), and a colouring with at most $k$ colours is a [function](function.md)

$$
c:V\to\{1,\ldots,k\},\qquad \{u,v\}\in E\Longrightarrow c(u)\ne c(v).
$$

The colour labels need not be visual colours: they can represent time slots or resources. Unused labels are allowed. Properness concerns [graph adjacency](graph.md#graph-adjacency), so moving [vertices](graph.md#vertex-graph-theory) in a drawing does not change whether the [graph coloring](#graph-coloring) is valid.[MIT, Graphs and Coloring, Section 2.1](https://ocw.mit.edu/courses/6-1200j-mathematics-for-computer-science-spring-2024/mit6_1200j_s24_lec11.pdf)

Each [colour class](ramsey-theory.md#colour-class) $c^{-1}(i)$ is an [independent set](#independent-set-graph-theory): no [edge](#edge-of-a-graph) has both endpoints in it. Conversely, a [set partition](combinatorics.md#set-partition) of $V$ into [independent sets](#independent-set-graph-theory) gives a proper [graph coloring](#graph-coloring) by assigning one colour to each part. Thus [graph coloring](#graph-coloring) groups mutually compatible objects, and its [chromatic number](#chromatic-number) asks for the fewest such groups.

For an illustrative scheduling model, let each [vertex](graph.md#vertex-graph-theory) represent an activity of equal duration and each [edge](#edge-of-a-graph) represent a pair that cannot occur in the same time slot. A proper [graph coloring](#graph-coloring) is then a schedule respecting those pairwise conflicts. If the conflicts form a [cycle graph](#cycle-graph) $C_4$ with [edges](#edge-of-a-graph) $12,23,34,41$, activities $1,3$ can share one slot and $2,4$ another. This model assumes interchangeable slots and includes only the pairwise conflicts encoded by the [graph](graph.md).[Leighton, MIT Graph Theory and Coloring, transcript pages 8–10](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/1ccaf180bcd244fddd32e60789fa922f_h9wxtqoa1jY.pdf)

The word "colouring" also occurs in [edge coloring](#edge-coloring), which requires different colours on [edges](#edge-of-a-graph) sharing an endpoint. The [chromatic number](#chromatic-number) discussed here always refers to [proper vertex colouring](#proper-vertex-coloring).

### Proper vertex coloring

↑ **Parent:** [Graph coloring](#graph-coloring)

A proper vertex coloring assigns labels to the [vertices](graph.md#vertex-graph-theory) of a [graph](graph.md) so that [vertices](graph.md#vertex-graph-theory) joined by an [edge](#edge-of-a-graph) have different labels. Each [colour class](ramsey-theory.md#colour-class) is an [independent set](#independent-set-graph-theory). The [chromatic number](#chromatic-number) is the least number of labels needed for this form of [graph coloring](#graph-coloring).

### Semi-random palette refinement for triangle-free colouring

↑ **Parent:** [Graph coloring](#graph-coloring)

Maintain lists of available colours, tentatively colour small random portions, erase conflicts and prune colours used by neighbours. In a [triangle-free graph](graph.md#triangle-free-graph), a vertex's neighbours form an [independent set](#independent-set-graph-theory), which enables local estimates. Track list size and average remaining neighbour congestion per colour; prune unusually congested colours before the next round. Concentration and the [Lovász local lemma](probabilistic-combinatorics.md#lovasz-local-lemma) preserve these invariants until lists have enough slack for completion. Tracking averages matters because triangle-free graphs can still contain many four-cycles and need not have uniform per-colour congestion.

### Colour savings from sparse neighbourhoods

↑ **Parent:** [Graph coloring](#graph-coloring)

If each neighbourhood misses a fixed positive fraction of the possible pairs at a large degree bound, randomly assign about half that many colours and erase vertices with monochromatic incident edges. A nonadjacent neighbour pair can share a retained colour, giving a [neighbour-colour saving](#neighbour-colour-saving). Write the number of successful repeated colours as a difference of two [certifiable functions](probability-inequality.md#certifiable-function): colours with a nonadjacent pair, minus those for which a neighbour loses that colour. Both change by at most two under one-coordinate changes and have constant-size certificates. [Talagrand's convex distance inequality](probability-inequality.md#talagrand-s-convex-distance-inequality) and the [Lovász local lemma](probabilistic-combinatorics.md#lovasz-local-lemma) make their linear expected saving simultaneous at all high-degree vertices; low-degree vertices have slack already. This yields a colouring using a fixed positive fraction fewer than the degree bound.

### Coloring entropy weight

↑ **Parent:** [Graph coloring](#graph-coloring)

For a uniformly chosen vertex $Z$, minimize the [information entropy](information-theory.md#information-entropy) of its color over proper colorings. Multiply by the number of vertices to define this weight. Minimizing the color entropy gives the strongest contribution from that graph in the [entropy weight of a graph cover](#entropy-weight-of-a-graph-cover) inequality.

#### Entropy weight of a graph cover

↑ **Parent:** [Coloring entropy weight](#coloring-entropy-weight)

If graphs $G_i$ cover the edges of an $n$-vertex graph with [independence number](#independence-number) at most $\alpha$, their coloring entropy weights satisfy the displayed bound. A random vertex's color is recorded in every covering graph containing it; independent dummy colors with matching marginal laws fill the other positions. Conditional on all recorded colors, compatible vertices form an [independent set](#independent-set-graph-theory), leaving conditional entropy at most $\log_2\alpha$. The [mutual information](information-theory.md#mutual-information) carried by the colors is at most $n^{-1}\sum_iw(G_i)$, proving the bound.

### Greedy coloring

↑ **Parent:** [Graph coloring](#graph-coloring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Greedy_coloring)

For a finite [simple graph](graph.md#simple-graph), choose an order of its [vertices](graph.md#vertex-graph-theory) and process them one at a time. Give each [vertex](graph.md#vertex-graph-theory) the smallest positive colour label not already used by its coloured neighbours, and keep all earlier assignments. This is [greedy coloring](#greedy-coloring): each step makes a locally available choice. The resulting [graph coloring](#graph-coloring) is proper because, for each [edge](#edge-of-a-graph), its later endpoint avoids the colour of its earlier endpoint.[Leighton, MIT Graph Theory and Coloring, transcript pages 12–13](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/1ccaf180bcd244fddd32e60789fa922f_h9wxtqoa1jY.pdf)

If the [maximum degree of a graph](#maximum-degree-of-a-graph) is $\Delta(G)$, a [vertex](graph.md#vertex-graph-theory) has at most $\Delta(G)$ previously coloured neighbours, forbidding at most that many distinct colours. At least one label among $1,\ldots,\Delta(G)+1$ remains available. Consequently every order gives

$$
\chi(G)\leq\text{number of colours used by greedy colouring}\leq\Delta(G)+1.
$$

This is an upper bound, not a promise that [greedy coloring](#greedy-coloring) attains the [chromatic number](#chromatic-number).[MIT, Graphs and Coloring, Theorem 2](https://ocw.mit.edu/courses/6-1200j-mathematics-for-computer-science-spring-2024/mit6_1200j_s24_lec11.pdf)

<a id="image-two-orders-for-greedy-coloring-of-the-same-path-graph-p-4"></a>
![](greedy-coloring-order.png)

**[Figure 16](#image-two-orders-for-greedy-coloring-of-the-same-path-graph-p-4). Two orders for greedy coloring of the same path graph $P_4$**. The [edges](#edge-of-a-graph) are $12,23,34$ in both drawings. Each dot shows its assigned colour number, with the [vertex](graph.md#vertex-graph-theory) label above and its processing step below. The order $1,2,3,4$ uses two colours; the order $1,4,2,3$ uses three.

Consider the [path graph](#path-graph) $P_4$ with [edges](#edge-of-a-graph) $12,23,34$. In the order $1,2,3,4$, [greedy coloring](#greedy-coloring) assigns the colours $1,2,1,2$ respectively. In the order $1,4,2,3$, it assigns colours $1,1,2,3$ in processing order: [vertices](graph.md#vertex-graph-theory) $1,4$ both get colour $1$, then [vertex](graph.md#vertex-graph-theory) $2$ gets colour $2$, and finally [vertex](graph.md#vertex-graph-theory) $3$ sees colours $2$ and $1$ at its two neighbours and must take colour $3$. Written in [vertex](graph.md#vertex-graph-theory) order $1,2,3,4$, this second colouring is $1,2,3,1$.

The [path graph](#path-graph) has [chromatic number](#chromatic-number) two: the first assignment achieves two colours, and any [edge](#edge-of-a-graph) rules out one. Its [maximum degree of a graph](#maximum-degree-of-a-graph) is two, so three colours in the second assignment still satisfy the bound. The extra colour comes entirely from the processing order. The [crown graph](#crown-graph) gives a larger family where a poor order can make [greedy coloring](#greedy-coloring) use arbitrarily many colours although the [chromatic number](#chromatic-number) remains two.

#### Extension of a partial colouring by neighbour-colour savings

↑ **Parent:** [Greedy coloring](#greedy-coloring)

In a proper partial [graph coloring](#graph-coloring), let $R_v$ count coloured neighbours and $D_v$ count their distinct colours. The saving $S_v=R_v-D_v$ leaves $K-D_v$ available colours for only $d(v)-R_v$ initially uncoloured neighbours. If the displayed inequality holds at every vertex, ordinary greedy completion succeeds. Each additionally coloured neighbour removes at most one available colour while also reducing the number of uncoloured neighbours by one.

##### Neighbour-colour saving

↑ **Parent:** [Extension of a partial colouring by neighbour-colour savings](#extension-of-a-partial-colouring-by-neighbour-colour-savings)

The number of coloured neighbours of $v$ minus the number of distinct colours on those neighbours. Repeated colours among pairwise nonadjacent neighbours reduce the number of unavailable colours without increasing the number of neighbours still to colour.

### Three-colourability problem

↑ **Parent:** [Graph coloring](#graph-coloring)

This [decision problem](computer-science.md#decision-problem) asks whether a finite [undirected graph](#undirected-graph) has a [graph colouring](#graph-coloring) with three colours. It is [NP-complete](computer-science.md#np-completeness): a colouring certifies membership in [NP](computer-science.md#np-complexity), while [3-SAT](computer-science.md#3-sat) reduces using [Boolean-pair colouring gadgets](#boolean-pair-colouring-gadget) and [three-colour clause gadgets](#three-colour-clause-gadget).

### Three-colour clause gadget

↑ **Parent:** [Graph coloring](#graph-coloring)

Take auxiliary [graph triangles](graph.md#triangle-in-a-graph) $a,b,c$ and $d,t,e$, join $a$ to $d$, and add edges $bx,cy,ez$. When $t$ has colour $T$ and the inputs $x,y,z$ have colours in $\{T,F\}$, this graph admits an extension to a [graph colouring](#graph-coloring) with three colours exactly when at least one input is $T$. All-false inputs force $a=d=F$, contradicting their edge. Conversely, use $(a,b,c,d,e)=(T,F,B,F,B)$ if $x=T$, $(T,B,F,F,B)$ if $x=F,y=T$, and $(F,T,B,B,F)$ if $x=y=F,z=T$. The extension property is necessary for both directions of a [polynomial-time many-one reduction](computer-science.md#polynomial-time-many-one-reduction).

### Boolean-pair colouring gadget

↑ **Parent:** [Graph coloring](#graph-coloring)

Two [graph triangles](graph.md#triangle-in-a-graph) sharing a vertex $B$ force their two opposite edges to use the same two colours in a [graph colouring](#graph-coloring) with three colours. A palette [graph triangle](graph.md#triangle-in-a-graph) $T,F,B$ and another [graph triangle](graph.md#triangle-in-a-graph) $u,\bar u,B$ therefore force the literal pair to have opposite Boolean colours. This gadget is used in a reduction from [3-SAT](computer-science.md#3-sat) to the [three-colourability problem](#three-colourability-problem).

### Greedy colouring by removing independent sets

↑ **Parent:** [Graph coloring](#graph-coloring)

If every [vertex](graph.md#vertex-graph-theory) subset of size at least $m$ contains an [independent set](#independent-set-graph-theory) of size $r$, repeatedly colour and remove an $r$-element [independent set](#independent-set-graph-theory) while at least $m$ [vertices](graph.md#vertex-graph-theory) remain. Giving each remaining [vertex](graph.md#vertex-graph-theory) its own colour uses at most $|V|/r+m$ colours.

<h3 id="lovasz-number">Lovász number</h3>

↑ **Parent:** [Graph coloring](#graph-coloring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lovász_number)

The Lovász number of a finite simple [graph](graph.md) is the [semidefinite program](convex-optimization.md#semidefinite-programming) value

$$
\vartheta(G)=\max\{\operatorname{tr}(JB):B\succeq0,\ \operatorname{tr}B=1,\ B_{ij}=0\text{ for }ij\in E(G)\},
$$

where $J$ is the [all-ones matrix](vector-space.md#all-ones-matrix). Its value on the [complement graph](#complement-graph) gives a lower bound for the [chromatic number](#chromatic-number).

#### Orthonormal representation of a graph

↑ **Parent:** [Lovász number](#lovasz-number)

Assign a real unit vector $u_v$ to each graph vertex, with $u_v\perp u_w$ whenever distinct vertices are nonadjacent. A handle is a further unit vector $h$. In the handle formulation of the [Lovász number](#lovasz-number), one minimizes $\max_v|h\cdot u_v|^{-2}$ over representations and handles. Orthonormal here does not mean every pair of assigned vectors is orthogonal.

##### Tensor-product capacity bound from an orthonormal representation

↑ **Parent:** [Orthonormal representation of a graph](#orthonormal-representation-of-a-graph)

Tensor products of the assigned vectors represent strong graph powers, and tensor products of the handle have squared inner products equal to products of the original ones. The vectors assigned to an independent set are orthonormal. [Bessel inequality](hilbert-space.md#bessel-s-inequality) then bounds its size by the largest inverse squared handle inner product. Taking roots and minimizing proves $c(G)\leq\vartheta(G)$.

#### Complement theta number

↑ **Parent:** [Lovász number](#lovasz-number)

For a finite simple [graph](graph.md) with at least one vertex, the complement theta number has the equivalent [semidefinite program](convex-optimization.md#semidefinite-programming) formulations

$$
\bar\vartheta(G)=\min\left\{t:
\begin{pmatrix}t&\mathbf1^T\\\mathbf1&Z\end{pmatrix}\succeq0,
\ Z_{ii}=1,\ Z_{ij}=0\text{ for }ij\in E(G)\right\}
$$

and

$$
\bar\vartheta(G)=\min\{t:U\succeq0,\ U_{ii}=t-1,\ U_{ij}=-1\text{ for }ij\in E(G)\}.
$$

The [Schur complement](linear-algebra.md#schur-complement) and $U=tZ-J$ prove the equivalence; any feasible $t$ is at least one, so division by $t$ is valid. For a [graph](graph.md) with an edge, $U/(t-1)$ is the [Gram matrix](linear-algebra.md#gram-matrix) of a [strict vector coloring](#strict-vector-coloring). Consequently $\bar\vartheta(G)$ is the strict vector chromatic number, and an ordinary $k$-[graph colouring](#graph-coloring) gives $\bar\vartheta(G)\leq k$ by assigning the colors the vertices of a [regular simplex](algebraic-topology.md#regular-simplex).

### Vector coloring

↑ **Parent:** [Graph coloring](#graph-coloring)

A vector $k$-coloring, for $k>1$, assigns a [unit vector](vector-space.md#unit-vector) $v_i$ to each [vertex](graph.md#vertex-graph-theory) of a [graph](graph.md), such that $\langle v_i,v_j\rangle\leq-1/(k-1)$ on every [edge](#edge-of-a-graph). A [graph colouring](#graph-coloring) with $k$ colors gives a vector $k$-coloring by placing the colors at the vertices of a [regular simplex](algebraic-topology.md#regular-simplex). The [Gram matrix](linear-algebra.md#gram-matrix) of these [vectors](vector-space.md#vector) allows [semidefinite programming](convex-optimization.md#semidefinite-programming) to search for such a representation.

#### Strict vector coloring

↑ **Parent:** [Vector coloring](#vector-coloring)

A strict vector $k$-coloring requires equality $\langle v_i,v_j\rangle=-1/(k-1)$ on every [edge](#edge-of-a-graph). The least admissible $k$ is the [complement theta number](#complement-theta-number) for a [graph](graph.md) with an edge. Allowing merely an inequality defines the potentially smaller vector chromatic number.

#### Random hyperplane rounding

↑ **Parent:** [Vector coloring](#vector-coloring)

For [unit vectors](vector-space.md#unit-vector) $u,v$ and a random normal $a$ with independent [standard normal distribution](probability-theory.md#standard-normal-distribution) coordinates,

$$
\mathbb P\{\operatorname{sign}\langle a,u\rangle\ne\operatorname{sign}\langle a,v\rangle\}
=\frac{\arccos\langle u,v\rangle}{\pi}.
$$

The [Gaussian distribution](probability-theory.md#normal-distribution) is invariant under [orthogonal transformations](linear-algebra.md#orthogonal-transformation). Projecting onto the [plane](geometry-and-topology.md#plane) spanned by $u,v$ therefore gives a uniformly distributed direction. If the angle between $u,v$ is $\theta$, the sign-disagreement directions form two sectors of total angle $2\theta$ out of $2\pi$. The endpoint cases $u=v$ and $u=-v$ give probabilities zero and one directly.

### Semicoloring

↑ **Parent:** [Graph coloring](#graph-coloring)

A $k$-semicoloring of a finite [graph](graph.md) assigns one of $k$ colors to every [vertex](graph.md#vertex-graph-theory) and is a proper [graph colouring](#graph-coloring) on an [induced subgraph](#induced-subgraph) containing at least half the [vertices](graph.md#vertex-graph-theory). This is weaker than a proper coloring of the whole [graph](graph.md), and is useful as an intermediate step in a [randomized algorithm](computer-science.md#randomized-algorithm).

#### Semicoloring by independent hyperplanes

↑ **Parent:** [Semicoloring](#semicoloring)

Suppose a [graph](graph.md) with $n$ [vertices](graph.md#vertex-graph-theory) and $m>0$ [edges](#edge-of-a-graph) has a [vector coloring](#vector-coloring) with adjacent inner products at most $-1/2$. Take $r$ independent copies of [random hyperplane rounding](#random-hyperplane-rounding) and use the $r$ signs as a color. Each [edge](#edge-of-a-graph) remains monochromatic with probability at most $3^{-r}$, so the expected number $B$ of monochromatic [edges](#edge-of-a-graph) is at most $m3^{-r}$ by [linearity of expectation](probability-theory.md#linearity-of-expectation).

Choose $r=\max\{0,\lceil\log_3(4m/n)\rceil\}$. Then [Markov inequality](probability-inequality.md#markov-s-inequality) gives $\mathbb P(B>n/2)\leq1/2$. On success, delete one endpoint of every monochromatic [edge](#edge-of-a-graph). This [random alteration method](probabilistic-combinatorics.md#random-alteration-method) leaves at least $n/2$ [vertices](graph.md#vertex-graph-theory) properly colored with

$$
k=2^r=O\left(\max\{1,(m/n)^{\log_3 2}\}\right)=O(n^{\log_3 2}).
$$

The removed [vertices](graph.md#vertex-graph-theory) can retain their original colors, as the [semicoloring](#semicoloring) only requires the retained [induced subgraph](#induced-subgraph) to be proper. A failed draw can be detected and repeated, with at most two trials on average. The case $m=0$ needs just one color. This is the elementary independent-hyperplane construction in [Karger, Motwani and Sudan's paper on approximate graph coloring](https://arxiv.org/abs/cs/9812008).

### Edge coloring

↑ **Parent:** [Graph coloring](#graph-coloring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edge_coloring)

An [edge colouring](#edge-coloring) assigns a label called a colour to every [edge of a graph](#edge-of-a-graph): it is a [function](function.md) $c:E(G)\to\{1,\ldots,k\}$. Here this definition allows arbitrary assignments. Two [edges](#edge-of-a-graph) sharing a [vertex](graph.md#vertex-graph-theory) may receive the same colour. A [proper edge colouring](#proper-edge-coloring) imposes the additional condition that such [edges](#edge-of-a-graph) receive different colours. Some textbooks use "[edge colouring](#edge-coloring)" as shorthand for this proper version; check the convention before applying a theorem.[Line graphs and edge coloring, slide 1: arbitrary labeling versus proper edge coloring](mathematics-bibliography.md#line-graphs-and-edge-coloring)

The distinction matters in [Ramsey theory](ramsey-theory.md). In a red-blue [edge colouring](#edge-coloring) of a [complete graph](#complete-graph), a [triangle in a graph](graph.md#triangle-in-a-graph) is monochromatic when its three [edges](#edge-of-a-graph) have the same colour. These are arbitrary [edge colourings](#edge-coloring): forbidding equal colours on [edges](#edge-of-a-graph) sharing a [vertex](graph.md#vertex-graph-theory) would forbid the very monochromatic [triangles in a graph](graph.md#triangle-in-a-graph) being sought. For example, assigning red to every [edge](#edge-of-a-graph) of $K_3$ is a valid arbitrary [edge colouring](#edge-coloring), although it is not a [proper edge colouring](#proper-edge-coloring). Colour labels can also stand for time slots: then [proper edge colouring](#proper-edge-coloring) turns incompatible jobs into separate rounds.

#### Proper edge coloring

↑ **Parent:** [Edge coloring](#edge-coloring)

A [proper edge colouring](#proper-edge-coloring) gives different labels to any two distinct [edges](#edge-of-a-graph) sharing a [vertex](graph.md#vertex-graph-theory). We work with finite [undirected graphs](#undirected-graph) without [self-loops](graph.md#loop-graph-theory); distinct parallel [edges](#edge-of-a-graph) in a [multigraph](graph.md#multigraph) must also have different colours. For a [simple graph](graph.md#simple-graph), whose [edges](#edge-of-a-graph) are two-element [sets](set.md), the condition is

$$
e\ne f,\quad e\cap f\ne\varnothing\quad\Longrightarrow\quad c(e)\ne c(f).
$$

Every [colour class](ramsey-theory.md#colour-class) $M_i=\{e\in E(G):c(e)=i\}$ is a [matching in a graph](#matching-graph-theory). Conversely, a [set partition](combinatorics.md#set-partition) of the [edges](#edge-of-a-graph) into [matchings in a graph](#matching-graph-theory) supplies a [proper edge colouring](#proper-edge-coloring). Thus minimizing colours means grouping all the [edges](#edge-of-a-graph) into as few [matchings in a graph](#matching-graph-theory) as possible.

The [line graph](#line-graph) makes the relationship with [proper vertex colouring](#proper-vertex-coloring) explicit: replace each original [edge](#edge-of-a-graph) by a [vertex](graph.md#vertex-graph-theory), joining two new [vertices](graph.md#vertex-graph-theory) exactly when their original [edges](#edge-of-a-graph) share an endpoint. A [proper edge colouring](#proper-edge-coloring) of $G$ becomes a [proper vertex colouring](#proper-vertex-coloring) of its [line graph](#line-graph) $L(G)$, so $\chi\prime(G)=\chi(L(G))$. For a [multigraph](graph.md#multigraph), retain a distinct new [vertex](graph.md#vertex-graph-theory) for each parallel [edge](#edge-of-a-graph).[Line graphs and edge coloring, slide 1: line graph identity](mathematics-bibliography.md#line-graphs-and-edge-coloring)

##### Edge coloring as scheduling

↑ **Parent:** [Proper edge coloring](#proper-edge-coloring)

Suppose each job occupies two distinct resources for one whole slot, and each resource can serve at most one job in that slot. Make resources [vertices](graph.md#vertex-graph-theory) and jobs [edges](#edge-of-a-graph). Two jobs conflict exactly when their [edges](#edge-of-a-graph) share a [vertex](graph.md#vertex-graph-theory), so a valid schedule is a [proper edge colouring](#proper-edge-coloring). Each slot is a [matching in a graph](#matching-graph-theory); the [chromatic index](#chromatic-index) is the minimum number of slots. The colour labels specify the slots, rather than physical colours. This model assumes all jobs are available initially, with equal duration, interchangeable slots and no additional conflicts. The school-timetable motivation in [Graph Theory by Reinhard Diestel](mathematics-bibliography.md#graph-theory-by-reinhard-diestel) (author-hosted Colouring preview, opening paragraphs, pp. 123–124) uses this resource-pair interpretation.

Here is a complete example. Two technicians $A,B$ must each use three instruments $X,Y,Z$ once. Each job needs its technician and its instrument simultaneously. The six jobs are the [edges](#edge-of-a-graph) of the [complete bipartite graph](#complete-bipartite-graph) $K_{2,3}$:

$$
E=\{AX,AY,AZ,BX,BY,BZ\},\qquad
M_1=\{AX,BY\},\quad M_2=\{AY,BZ\},\quad M_3=\{AZ,BX\}.
$$

Within each $M_i$, the two jobs use different technicians and different instruments, so $M_i$ is a [matching in a graph](#matching-graph-theory). The three [matchings in a graph](#matching-graph-theory) together cover every job exactly once. Technician $A$ has three jobs, so fewer than three slots cannot suffice; the displayed schedule uses three. This is an optimal [proper edge colouring](#proper-edge-coloring) with [chromatic index](#chromatic-index) three, witnessed by both a schedule and a resource-workload lower bound.

<a id="image-six-jobs-on-a-complete-bipartite-graph-become-three-scheduling-slots-each-a-matching-in-a-graph"></a>
![](edge-coloring-bipartite-job-slots.png)

**[Figure 17](#image-six-jobs-on-a-complete-bipartite-graph-become-three-scheduling-slots-each-a-matching-in-a-graph). Six jobs on a complete bipartite graph become three scheduling slots, each a matching in a graph**. The [vertices](graph.md#vertex-graph-theory) are resources, and each numbered [edge](#edge-of-a-graph) is one job. The slot table uses the same colour labels as the [proper edge colouring](#proper-edge-coloring). A technician or instrument appears at most once within a column. Crossings of drawn [edges](#edge-of-a-graph) introduce no resource and no conflict.

Repeated jobs requiring the same resource pair become distinct parallel [edges](#edge-of-a-graph) of a [multigraph](graph.md#multigraph), rather than one [edge](#edge-of-a-graph). Additional restrictions change the problem: prescribed allowed slots lead to [list edge coloring](#list-edge-coloring), while unequal durations, deadlines, or jobs needing more than two resources require a richer [scheduling](mathematical-optimization.md#scheduling) model. Selecting a largest [matching in a graph](#matching-graph-theory) solves a single-round question; a shortest complete schedule must organize all jobs across rounds.

#### List edge coloring

↑ **Parent:** [Edge coloring](#edge-coloring)

Each [edge](#edge-of-a-graph) has a list of allowed colors; a list edge coloring chooses an allowed color on each edge, giving different colors to incident edges. The [list-chromatic index](#list-chromatic-index) is the uniform list-size threshold guaranteeing success.

##### List-chromatic index

↑ **Parent:** [List edge coloring](#list-edge-coloring)

The list-chromatic index is the least integer $q$ such that every assignment of at least $q$ allowed colors to each [edge](#edge-of-a-graph) admits a [list edge coloring](#list-edge-coloring). Uniform identical lists show it is at least the [chromatic index](#chromatic-index). The [Galvin theorem for bipartite list edge coloring](#galvin-theorem-for-bipartite-list-edge-coloring) gives equality for [bipartite graphs](#bipartite-graph).

###### Galvin theorem for bipartite list edge coloring

↑ **Parent:** [List-chromatic index](#list-chromatic-index)

A [bipartite graph](#bipartite-graph) has equal [list-chromatic index](#list-chromatic-index), [chromatic index](#chromatic-index) and [maximum degree of a graph](#maximum-degree-of-a-graph) $\Delta$. Start with a proper $\Delta$-[edge coloring](#edge-coloring). Orient its [line graph](#line-graph) toward smaller colors at one part and toward larger colors at the other. An edge of color $c$ has at most $(c-1)+(\Delta-c)=\Delta-1$ outgoing neighbours. Every induced orientation has a [digraph kernel](#kernel-of-a-directed-graph) obtained from a [stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph) with those preferences. Apply the [kernel list-coloring lemma](#kernel-list-coloring-lemma).

#### Chromatic index

↑ **Parent:** [Edge coloring](#edge-coloring)

The [chromatic index](#chromatic-index) $\chi\prime(G)$, also called the [edge chromatic number](#edge-chromatic-number), is the least number of labels in a [proper edge colouring](#proper-edge-coloring) of a finite [undirected graph](#undirected-graph) without [self-loops](graph.md#loop-graph-theory). Equivalently, it is the smallest number of [matchings in a graph](#matching-graph-theory) whose [set partition](combinatorics.md#set-partition) covers all the [edges](#edge-of-a-graph). We take $\chi\prime(G)=0$ when there are no [edges](#edge-of-a-graph). For an arbitrary [edge colouring](#edge-coloring), one colour always suffices whenever an [edge](#edge-of-a-graph) exists, so properness is essential to this definition. The [chromatic number](#chromatic-number) $\chi(G)$ instead colours [vertices](graph.md#vertex-graph-theory).[Colouring, author-hosted chapter preview, p. 124: chromatic index and line graph](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

To establish an exact [chromatic index](#chromatic-index), supply both a [proper edge colouring](#proper-edge-coloring) and a reason that fewer colours cannot work. Every [edge](#edge-of-a-graph) at a fixed [vertex](graph.md#vertex-graph-theory) must have its own colour, giving the lower bound $\chi\prime(G)\geq\Delta(G)$, where $\Delta(G)$ is the [maximum degree of a graph](#maximum-degree-of-a-graph). The bound need not be attained: it counts a single resource's workload, while conflicts can also accumulate around a [graph cycle](#cycle-in-a-graph).

<a id="image-worked-proper-edge-colourings-a-triangle-in-a-graph-needs-three-colours-while-an-even-cycle-graph-needs-two"></a>
![](edge-coloring-triangle-even-cycle.png)

**[Figure 18](#image-worked-proper-edge-colourings-a-triangle-in-a-graph-needs-three-colours-while-an-even-cycle-graph-needs-two). Worked proper edge colourings: a triangle in a graph needs three colours, while an even cycle graph needs two**. Numbers beside [edges](#edge-of-a-graph) are colour labels; letters at dots are [vertices](graph.md#vertex-graph-theory). Both [graphs](graph.md) have [maximum degree of a graph](#maximum-degree-of-a-graph) two. The [triangle in a graph](graph.md#triangle-in-a-graph) has three pairwise conflicting [edges](#edge-of-a-graph), while opposite [edges](#edge-of-a-graph) of the square can share a colour.

For the [triangle in a graph](graph.md#triangle-in-a-graph) $K_3$ with [edges](#edge-of-a-graph) $ab,bc,ca$, every pair of [edges](#edge-of-a-graph) shares a [vertex](graph.md#vertex-graph-theory), so all three require different labels. The assignment $c(ab)=1,c(bc)=2,c(ca)=3$ works, proving $\chi\prime(K_3)=3$ although $\Delta(K_3)=2$. In its [line graph](#line-graph), those three [edges](#edge-of-a-graph) become a three-[vertex](graph.md#vertex-graph-theory) [clique](#clique-graph-theory). Treating this as three pair-resource jobs makes the obstruction tangible: each resource has only two jobs, but every pair of jobs conflicts, so no slot can contain two jobs.

For the square [cycle graph](#cycle-graph) $C_4$ with [edges](#edge-of-a-graph) $ab,bc,cd,da$, use $c(ab)=c(cd)=1$ and $c(bc)=c(da)=2$. Each [colour class](ramsey-theory.md#colour-class) is a [matching in a graph](#matching-graph-theory), and each [vertex](graph.md#vertex-graph-theory) has one [edge](#edge-of-a-graph) of each colour. Since $\Delta(C_4)=2$, this proves $\chi\prime(C_4)=2$. More generally, alternation closes on any even [cycle graph](#cycle-graph) $C_{2m}$, $m\geq2$. On an [odd cycle](#odd-cycle) $C_{2m+1}$, $m\geq1$, two-colour alternation would make the last and first [edges](#edge-of-a-graph) share a colour at their common [vertex](graph.md#vertex-graph-theory); a third colour on the last [edge](#edge-of-a-graph) suffices. Thus even [cycle graphs](#cycle-graph) have [chromatic index](#chromatic-index) two and odd [cycle graphs](#cycle-graph) have [chromatic index](#chromatic-index) three. These exact examples show why [maximum degree of a graph](#maximum-degree-of-a-graph) alone does not determine the answer.

##### Chromatic index bounds

↑ **Parent:** [Chromatic index](#chromatic-index)

For every finite [simple graph](graph.md#simple-graph), [Vizing's theorem](#vizing-s-theorem) gives

$$
\Delta(G)\leq\chi\prime(G)\leq\Delta(G)+1.
$$

Here $\Delta(G)$ is the [maximum degree of a graph](#maximum-degree-of-a-graph), taken as zero when there are no [vertices](graph.md#vertex-graph-theory). A [bipartite graph](#bipartite-graph) has the stronger equality $\chi\prime(G)=\Delta(G)$. The six-job [complete bipartite graph](#complete-bipartite-graph) above attains this lower bound, while the [triangle in a graph](graph.md#triangle-in-a-graph) attains the extra-colour alternative. The simple-[graph](graph.md) restriction in the upper bound matters.[Colouring, author-hosted chapter preview, §5.3, p. 132: Proposition 5.3.1 and Theorem 5.3.2](mathematics-bibliography.md#graph-theory-by-reinhard-diestel)

The [bipartite graph](#bipartite-graph) equality still holds for finite loopless [multigraphs](graph.md#multigraph), with parallel [edges](#edge-of-a-graph) counted separately in each [vertex degree](#degree-graph-theory). For instance, $r$ parallel jobs between two resources need exactly $r$ slots: every pair conflicts, and $\Delta=\chi\prime=r$. For a general finite loopless [multigraph](graph.md#multigraph), however, the [simple graph](graph.md#simple-graph) upper bound can fail. Put two parallel [edges](#edge-of-a-graph) on each side of a [triangle in a graph](graph.md#triangle-in-a-graph). All six [edges](#edge-of-a-graph) pairwise share a [vertex](graph.md#vertex-graph-theory), so each needs its own colour; every [vertex](graph.md#vertex-graph-theory) has [degree of a vertex](#degree-graph-theory) four. Consequently $\chi\prime=6>\Delta+1=5$. A multiplicity-aware bound is $\chi\prime(G)\leq\Delta(G)+\mu(G)$, where $\mu(G)$ is the largest number of parallel [edges](#edge-of-a-graph) between a pair of [vertices](graph.md#vertex-graph-theory). The doubled [triangle in a graph](graph.md#triangle-in-a-graph) has $\mu=2$ and attains that bound. These statements exclude [self-loops](graph.md#loop-graph-theory); the two-distinct-resource scheduling model excludes them too.[Line graphs and edge coloring, slide 2: bipartite multigraph equality, multiplicity bound and fat triangle](mathematics-bibliography.md#line-graphs-and-edge-coloring)

For historical orientation, [Graph Theory by Reinhard Diestel](mathematics-bibliography.md#graph-theory-by-reinhard-diestel) (Colouring preview, §5.3, p. 132) dates the bipartite equality to 1916 and [Vizing's theorem](#vizing-s-theorem) to 1964. These are textbook attributions; the original papers have not been inspected here. The results state existence of optimal or nearly optimal [proper edge colourings](#proper-edge-coloring), rather than saying that arbitrary greedy choices will find them. The [list-chromatic index](#list-chromatic-index) asks the further question of success for every sufficiently large family of allowed-colour lists.

#### Tait coloring

↑ **Parent:** [Edge coloring](#edge-coloring)

A proper three-color [edge coloring](#edge-coloring) of a [cubic graph](graph.md#cubic-graph). Label its colors by the nonzero elements of $\mathbb F_2^2$: the incident colors at each [vertex](graph.md#vertex-graph-theory) then sum to zero. On a planar map without [bridges in a graph](graph.md#bridge-graph-theory), integrating these labels on the [dual graph](graph.md#dual-graph) gives a four-color face coloring. On a [torus](topology.md#torus), a nonzero period can obstruct this integration.

### Chromatic number

↑ **Parent:** [Graph coloring](#graph-coloring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chromatic_number)

For a nonempty finite [simple graph](graph.md#simple-graph) $G$, the [chromatic number](#chromatic-number) $\chi(G)$ is the least positive [integer](number-theory.md#integer) $k$ for which $G$ has a proper vertex [graph coloring](#graph-coloring) with at most $k$ colours. To establish an exact [chromatic number](#chromatic-number), give a colouring using that many colours and explain why fewer cannot suffice. A colouring alone gives only an upper bound.[Lehman, Leighton and Meyer, Mathematics for Computer Science, Definition 11.7.1](mathematics-bibliography.md#mathematics-for-computer-science-by-eric-lehman-and-others)

<a id="image-optimal-graph-colorings-of-the-cycle-graphs-c-3-c-4-c-5"></a>
![](graph-coloring-cycle-examples.png)

**[Figure 19](#image-optimal-graph-colorings-of-the-cycle-graphs-c-3-c-4-c-5). Optimal graph colorings of the cycle graphs $C_3,C_4,C_5$**. Numbers inside dots are colour labels, and labels outside are [vertices](graph.md#vertex-graph-theory). The [cycle graph](#cycle-graph) $C_4$ alternates two colours. The [odd cycles](#odd-cycle) $C_3,C_5$ need three, although $C_5$ is a [triangle-free graph](graph.md#triangle-free-graph).

These small [graphs](graph.md) show why the [chromatic number](#chromatic-number) measures more than the presence of [triangles in a graph](graph.md#triangle-in-a-graph):

- The [cycle graph](#cycle-graph) $C_3$, also the [complete graph](#complete-graph) $K_3$, has [chromatic number](#chromatic-number) three. Every pair of [vertices](graph.md#vertex-graph-theory) is adjacent, so three distinct colours are necessary and sufficient.
- The [cycle graph](#cycle-graph) $C_4$ has [chromatic number](#chromatic-number) two. Around the [graph cycle](#cycle-in-a-graph), the assignment $1,2,1,2$ is proper, and a single colour would violate every [edge](#edge-of-a-graph).
- The [cycle graph](#cycle-graph) $C_5$ has [chromatic number](#chromatic-number) three. With two colours, alternation around the [graph cycle](#cycle-in-a-graph) would force the first and fifth [vertices](graph.md#vertex-graph-theory) to have the same colour despite their joining [edge](#edge-of-a-graph). The assignment $1,2,1,2,3$ works. Thus a [triangle-free graph](graph.md#triangle-free-graph) can still require more than two colours.
- The [complete graph](#complete-graph) $K_n$ has [chromatic number](#chromatic-number) $n$: all $n$ [vertices](graph.md#vertex-graph-theory) are pairwise adjacent, so each must have its own colour.[Meyer, MIT Graph Coloring, slides 18–19](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2005/5926091844fc3d60fa18eb75c9a2bc03_slides5w.pdf)

For a [cycle graph](#cycle-graph) of even length, alternating two colours closes consistently; for an [odd cycle](#odd-cycle), it does not, and a third colour on the final [vertex](graph.md#vertex-graph-theory) suffices. More generally, the [two-colourability criterion for bipartite graphs](#two-colourability-criterion-for-bipartite-graphs) says that $\chi(G)\leq2$ exactly when $G$ is a [bipartite graph](#bipartite-graph), and the [odd-cycle characterization of bipartite graphs](#odd-cycle-characterization-of-bipartite-graphs) identifies the obstruction as an [odd cycle](#odd-cycle). A nonempty [graph](graph.md) with no [edges](#edge-of-a-graph) has [chromatic number](#chromatic-number) one; a [bipartite graph](#bipartite-graph) with at least one [edge](#edge-of-a-graph) has [chromatic number](#chromatic-number) exactly two.

In the pairwise-conflict scheduling model of [graph coloring](#graph-coloring), $\chi(G)$ is the least number of interchangeable slots needed. This turns a drawing into an optimization question: how many groups of compatible activities are unavoidable? [Greedy coloring](#greedy-coloring) constructs a valid grouping quickly, but its number of colours can exceed the [chromatic number](#chromatic-number).

#### Chromatic number of Euclidean space

↑ **Parent:** [Chromatic number](#chromatic-number)

This is the least number of colors needed to color all points of [Euclidean space](functional-analysis.md#euclidean-norm) so that points at [Euclidean distance](topological-analysis.md#euclidean-distance) one receive different colors. Any finite unit-distance graph embedded in the space gives a lower bound. If $p$ is prime, the characteristic vectors of all $(2p-1)$-subsets of $[4p-1]$, divided by $\sqrt{2p}$, give such a graph: its edges are exactly pairs intersecting in $p-1$ points. The [prime-power modular intersection bound](extremal-set-theory.md#prime-power-modular-intersection-bound) bounds an independent set by $\binom{4p-1}{p-1}$, and hence gives $\chi(\mathbb R^{4p-1})\geq\binom{4p-1}{2p-1}/\binom{4p-1}{p-1}$.

#### Colour-critical vertex

↑ **Parent:** [Chromatic number](#chromatic-number)

A vertex $v$ is colour-critical if deleting it lowers the [chromatic number](#chromatic-number) by one. If $\chi(F)=r+1$ and $\chi(F-v)=r$, an embedding of $F-v$ into a complete $r$-partite graph inside one neighbourhood extends to an embedding of $F$. This supplies maximum-degree obstructions in [extremal graph theory](#extremal-graph-theory).

#### Mycielskian

↑ **Parent:** [Chromatic number](#chromatic-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mycielskian)

The Mycielski construction replaces a graph $G$ with a graph $\mu(G)$ having one shadow vertex for each original vertex and one further vertex adjacent to every shadow. It satisfies

$$
\chi(\mu(G))=\chi(G)+1
$$

and preserves triangle-freeness. Iterating it from the five-cycle gives triangle-free graphs of arbitrarily large chromatic number.

#### Graphs of arbitrarily high girth and chromatic number

↑ **Parent:** [Chromatic number](#chromatic-number)

For every $g,k\geq3$, there is a finite graph with no cycle of length at most $g$ and with chromatic number at least $k$. A probabilistic proof samples a sparse binomial random graph, observes that it has few short cycles and no large independent set, and deletes one vertex from every short cycle.

#### Brooks' theorem

↑ **Parent:** [Chromatic number](#chromatic-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brooks'_theorem)

A connected graph of maximum degree $\Delta$ has chromatic number at most $\Delta$ unless it is a complete graph or an odd cycle.

### Edge chromatic number

↑ **Parent:** [Graph coloring](#graph-coloring)

The edge chromatic number is the least number of colours required to colour edges so that incident edges receive different colours.

<h4 id="vizing-s-theorem">Vizing's theorem</h4>

↑ **Parent:** [Edge chromatic number](#edge-chromatic-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vizing's_theorem)

Every finite simple graph of maximum degree $\Delta$ has edge chromatic number $\Delta$ or $\Delta+1$.

##### Vizing fan lemma

↑ **Parent:** [Vizing's theorem](#vizing-s-theorem)

In a partial proper edge colouring with one uncoloured edge incident with a vertex $x$, a Vizing fan is a sequence of neighbours of $x$ whose incident edge colours are missing at earlier fan vertices. With one more colour than the maximum degree, fan rotations and a two-colour [Kempe chain](#kempe-chain) free one common colour at the endpoints of the uncoloured edge.

### Kempe chain

↑ **Parent:** [Graph coloring](#graph-coloring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kempe_chain)

For two colours in a proper graph colouring, a Kempe chain is a connected component of the subgraph using only those colours. Interchanging the two colours throughout one component preserves properness.

### Chromatic polynomial

↑ **Parent:** [Graph coloring](#graph-coloring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chromatic_polynomial)

The chromatic polynomial turns a [graph coloring](#graph-coloring) problem into a counting problem: **how many choices remain when adjacent [vertices](graph.md#vertex-graph-theory) must have different colours?** For a finite [simple graph](graph.md#simple-graph) $G$ and a positive [integer](number-theory.md#integer) $t$, $P_G(t)$ is the number of [proper vertex colorings](#proper-vertex-coloring) using a fixed, distinguished palette of $t$ colours. A colouring need not use every available colour, and exchanging two palette colours generally gives a different colouring. Although $P_G$ is a [polynomial](polynomial.md), its values at arbitrary noninteger arguments are not counts of colourings.

Consider the three-vertex [path graph](#path-graph) $A$--$B$--$C$. Choose $A$ in $t$ ways, then $B$ in $t-1$ ways, then $C$ in $t-1$ ways: $A$ and $C$ may agree because they are not adjacent. The [multiplication principle](combinatorics.md#rule-of-product) gives

$$
P_{P_3}(t)=t(t-1)^2=t^3-2t^2+t.
$$

Adding the [edge](#edge-of-a-graph) $AC$ makes the three-vertex [complete graph](#complete-graph) $K_3$. Now $C$ must avoid both preceding colours, so

$$
P_{K_3}(t)=t(t-1)(t-2)=t^3-3t^2+2t.
$$

With three available colours, the [path graph](#path-graph) has **12 colourings**, whereas the triangle has **6**. With two colours the counts are $2$ and $0$: the extra constraint makes the triangle impossible to colour.

<a id="image-all-twelve-proper-colourings-of-a-three-vertex-path-using-a-three-colour-palette"></a>
![](chromatic-polynomial-path-colorings.png)

**[Figure 20](#image-all-twelve-proper-colourings-of-a-three-vertex-path-using-a-three-colour-palette). All twelve proper colourings of a three-vertex path using a three-colour palette**.

For a nonempty [graph](graph.md), the [chromatic number](#chromatic-number) records only the first positive [integer](number-theory.md#integer) $t$ for which $P_G(t)>0$. The [chromatic polynomial](#chromatic-polynomial) also counts the choices for every larger palette. For the path the [chromatic number](#chromatic-number) is $2$, and for the triangle it is $3$. Counting assignments also gives a useful interpretation for scheduling: if adjacent [vertices](graph.md#vertex-graph-theory) represent tasks that must use different slots, the [chromatic polynomial](#chromatic-polynomial) counts the valid assignments to $t$ named slots. Adding a conflict [edge](#edge-of-a-graph) can only remove assignments.

The [chromatic polynomial](#chromatic-polynomial) also remembers some of the graph's structure. For a [simple graph](graph.md#simple-graph) with $n\geq 1$ [vertices](graph.md#vertex-graph-theory) and $m$ [edges](#edge-of-a-graph), its leading terms are $t^n-mt^{n-1}$; its [degree of a polynomial](polynomial.md#degree-of-a-polynomial) gives the number of [vertices](graph.md#vertex-graph-theory), and its next coefficient gives the number of [edges](#edge-of-a-graph). It does not determine the graph completely. A four-vertex [path graph](#path-graph) and a four-vertex [star graph](#star-graph-theory) are not related by a [graph isomorphism](graph.md#graph-isomorphism), but both are [trees](combinatorics.md#tree-graph-theory) and have [chromatic polynomial](#chromatic-polynomial) $t(t-1)^3$.

The early connection to map colouring appears in George D. Birkhoff's article [A Determinant Formula for the Number of Ways of Coloring a Map, Annals of Mathematics 14 (1912–1913), pp. 42–46](https://www.jstor.org/stable/1967597). For a derivation of the counting recurrence and its leading coefficients, see [Paul Johnson's MAS 341 lecture on chromatic polynomials](https://ptwiddle.github.io/MAS341-Graph-Theory-2017/lecturenotes/lecturex9.html).

<h4 id="chromatic-polynomial-determines-a-turan-graph">Chromatic polynomial determines a Turán graph</h4>

↑ **Parent:** [Chromatic polynomial](#chromatic-polynomial)

If a simple graph has the same [chromatic polynomial](#chromatic-polynomial) as the [Turán graph](#turan-graph) $T_r(n)$, it has the same number of vertices and edges, and the same [chromatic number](#chromatic-number) $r$. It is therefore $K_{r+1}$-free and attains equality in [Turán's theorem](#turan-s-theorem). The equality case forces it to be isomorphic to $T_r(n)$.

#### Deletion-contraction recurrence for the chromatic polynomial

↑ **Parent:** [Chromatic polynomial](#chromatic-polynomial)

Deleting an edge removes one colour constraint. [Edge contraction](#edge-contraction) describes exactly the newly admitted colourings that violate that constraint. If $e$ joins distinct [vertices](graph.md#vertex-graph-theory) $u,v$ of a [simple graph](graph.md#simple-graph) $G$, write $G-e$ for the [graph](graph.md) with that [edge](#edge-of-a-graph) deleted and $G/e$ for the [graph](graph.md) with $u,v$ identified and $e$ removed. Parallel edges produced by the contraction may be reduced to one edge, since they impose the same condition on a [proper vertex coloring](#proper-vertex-coloring). Then

$$
P_G(t)=P_{G-e}(t)-P_{G/e}(t).
$$

To see why, divide the [proper vertex colorings](#proper-vertex-coloring) of $G-e$ into two classes. Those with different colours at $u,v$ are exactly the colourings of $G$. Those with equal colours at $u,v$ correspond one-to-one to colourings of $G/e$: the merged [vertex](graph.md#vertex-graph-theory) receives their common colour. Subtracting the second class leaves the first.

For the triangle, delete $AC$ to get a three-vertex [path graph](#path-graph), or contract $AC$ to get two [vertices](graph.md#vertex-graph-theory) joined by an [edge](#edge-of-a-graph) after removing the redundant parallel edge. Consequently,

$$
P_{K_3}(t)=t(t-1)^2-t(t-1)=t(t-1)(t-2).
$$

At $t=3$, this says **$6=12-6$**. Of the twelve path colourings pictured above, six give $A,C$ the same colour; these are precisely the ones ruled out when we restore $AC$.

<a id="image-deleting-and-contracting-a-triangle-edge-separates-the-allowed-and-newly-forbidden-colourings"></a>
![](chromatic-polynomial-deletion-contraction.png)

**[Figure 21](#image-deleting-and-contracting-a-triangle-edge-separates-the-allowed-and-newly-forbidden-colourings). Deleting and contracting a triangle edge separates the allowed and newly forbidden colourings**.

This recurrence is useful because it reduces a constrained counting problem to smaller [graphs](graph.md). A [graph](graph.md) on $n$ [vertices](graph.md#vertex-graph-theory) with no [edges](#edge-of-a-graph) has $P_G(t)=t^n$, since every [vertex](graph.md#vertex-graph-theory) chooses its colour independently. Repeated [edge](#edge-of-a-graph) deletion and [edge contraction](#edge-contraction) reduce to this case and show that the counting function is a [polynomial](polynomial.md). The same recurrence gives its leading coefficients. The method is conceptually simple, although the number of recursive cases can still grow rapidly.

#### Chromatic polynomial after attaching a leaf

↑ **Parent:** [Chromatic polynomial](#chromatic-polynomial)

Attaching a new [vertex](graph.md#vertex-graph-theory) that is a [leaf of a graph](#leaf-of-a-graph) multiplies the [chromatic polynomial](#chromatic-polynomial) by $t-1$: after colouring the old graph, the new [vertex](graph.md#vertex-graph-theory) may receive any colour except its neighbour's. Starting with one [vertex](graph.md#vertex-graph-theory) and repeatedly adding a [leaf of a graph](#leaf-of-a-graph) constructs any finite [tree](combinatorics.md#tree-graph-theory). Thus a [tree](combinatorics.md#tree-graph-theory) with $n\geq 1$ [vertices](graph.md#vertex-graph-theory) has

$$
P_T(t)=t(t-1)^{n-1}.
$$

In contrast, every pair of [vertices](graph.md#vertex-graph-theory) in a [complete graph](#complete-graph) must receive different colours, so the [multiplication principle](combinatorics.md#rule-of-product) gives the [falling factorial](combinatorics.md#falling-factorial)

$$
P_{K_n}(t)=t(t-1)\cdots(t-n+1).
$$

For positive [integers](number-theory.md#integer) $t<n$ this product vanishes, expressing the impossibility of assigning distinct colours to all $n$ [vertices](graph.md#vertex-graph-theory).

## Independent set (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Independent_set_(graph_theory))

An [independent set](#independent-set-graph-theory) selects mutually compatible objects when an [edge](#edge-of-a-graph) of a [graph](graph.md) represents a conflict. For example, if [vertices](graph.md#vertex-graph-theory) are activities and [edges](#edge-of-a-graph) join activities that cannot occur together, an [independent set](#independent-set-graph-theory) is a collection that can share one time slot. Finding the largest such collection is measured by the [independence number](#independence-number).[Barak, Introduction to Theoretical Computer Science, Chapter 14, The independent set problem](https://introtcs.org/public/lec_12_NP.html)

In a finite [simple graph](graph.md#simple-graph) $G=(V,E)$, an [independent set](#independent-set-graph-theory) is a [subset](set.md#subset) $I\subseteq V$ with no [edge](#edge-of-a-graph) joining two selected [vertices](graph.md#vertex-graph-theory):

$$
u,v\in I,\ u\ne v\Longrightarrow\{u,v\}\notin E.
$$

The empty [set](set.md) and every singleton [set](set.md) are [independent sets](#independent-set-graph-theory). In the [cycle graph](#cycle-graph) $C_5$ drawn under [vertex cover](#vertex-cover), $\{0,2\}$ is an [independent set](#independent-set-graph-theory), but $\{0,4\}$ is not: the closing [edge](#edge-of-a-graph) $40$ joins those two [vertices](graph.md#vertex-graph-theory). Choosing nonconsecutive labels is insufficient unless the wraparound [edge](#edge-of-a-graph) is checked.

An [independent set](#independent-set-graph-theory) of maximum size has [cardinality](set-theory.md#cardinality) equal to the [independence number](#independence-number). Being unable to add another [vertex](graph.md#vertex-graph-theory) only makes an [independent set](#independent-set-graph-theory) inclusion-maximal. In the [star graph](#star-graph-theory) $K_{1,3}$, the centre alone is inclusion-maximal, since it is adjacent to every leaf, but the three leaves form a larger [independent set](#independent-set-graph-theory). This distinction mirrors the difference between an inclusion-minimal [vertex cover](#vertex-cover) and a [minimum vertex cover](#minimum-vertex-cover).

Every [independent set](#independent-set-graph-theory) $I$ has a [vertex cover](#vertex-cover) $V\setminus I$ as its [complement of a set](set.md#complement-of-a-set); a largest [independent set](#independent-set-graph-theory) has a [minimum vertex cover](#minimum-vertex-cover) as its complement. In every [proper vertex colouring](#proper-vertex-coloring), each [colour class](ramsey-theory.md#colour-class) is an [independent set](#independent-set-graph-theory), so [graph coloring](#graph-coloring) partitions the [vertices](graph.md#vertex-graph-theory) into mutually compatible groups.

### Independent transversal

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

For a [graph](graph.md) whose vertices are partitioned into parts, an independent transversal is an [independent set](#independent-set-graph-theory) containing exactly one vertex from each part. If a cycle's parts each have twelve vertices, choose one vertex uniformly and independently per part. A cycle edge joining distinct parts is selected at both ends with [probability](probability-theory.md#probability) $1/144$. Each [event](probability-theory.md#event) depends on at most $47$ others, since each part meets at most $24$ cycle edges. The [Lovász local lemma](probabilistic-combinatorics.md#lovasz-local-lemma) applies because $48e/144<1$, proving existence for an arbitrary such partition.

### Degree-ordered independent-set entropy bound

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

Order vertices by nonincreasing positive degrees $d_i$, and let $b_i$ count preceding neighbors. The [Madiman-Tetali inequality](information-theory.md#madiman-tetali-entropy-inequality) applied to preceding-neighbor sets and $b_i$ copies of singleton $i$ bounds the entropy of a uniformly chosen [independent set](#independent-set-graph-theory). In each local term, all-zero neighbor assignment permits two choices at $i$, while every other assignment permits at most one. The maximum-entropy bound gives $\log_2(2^{b_i+1}-1)$ for that term. Complete bipartite graphs $K_{d,d}$ attain equality when one part is ordered before the other.

### Independence number

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Independence_number)

The [independence number](#independence-number) is the largest [cardinality](set-theory.md#cardinality) of an [independent set](#independent-set-graph-theory) in a finite [simple graph](graph.md#simple-graph):

$$
\alpha(G)=\max\{|I|:I\subseteq V(G),\ I\text{ is an independent set of }G\}.
$$

It answers "how many mutually compatible objects can be selected at once?", while the [chromatic number](#chromatic-number) asks how many compatible groups are needed for all the [vertices](graph.md#vertex-graph-theory). Diestel uses this notation for a largest [independent set](#independent-set-graph-theory).[Diestel, Graph Theory, Chapter 2, Exercise 23](https://diestel-graph-theory.com/Sample.pdf)

For the [cycle graph](#cycle-graph) $C_5$, the [independent set](#independent-set-graph-theory) $\{0,2\}$ shows that $\alpha(C_5)\geq2$. Three selected [vertices](graph.md#vertex-graph-theory) would require at least three unselected [vertices](graph.md#vertex-graph-theory) separating them around the [cycle graph](#cycle-graph), which has only five [vertices](graph.md#vertex-graph-theory). Thus $\alpha(C_5)=2$. There are five largest [independent sets](#independent-set-graph-theory), obtained by rotating $\{0,2\}$ around the [cycle graph](#cycle-graph), and five corresponding [minimum vertex covers](#minimum-vertex-cover).

For the [complete bipartite graph](#complete-bipartite-graph) $K_{2,3}$, an [independent set](#independent-set-graph-theory) cannot contain a [vertex](graph.md#vertex-graph-theory) from each side, since every such pair is joined by an [edge](#edge-of-a-graph). The larger side has three [vertices](graph.md#vertex-graph-theory), so $\alpha(K_{2,3})=3$. A [triangle in a graph](graph.md#triangle-in-a-graph) has [independence number](#independence-number) one. A [graph](graph.md) with no [edges](#edge-of-a-graph) and $n$ [vertices](graph.md#vertex-graph-theory) has [independence number](#independence-number) $n$, including $\alpha(G)=0$ when $n=0$.

The complement correspondence between [vertex covers](#vertex-cover) and [independent sets](#independent-set-graph-theory) gives, with $n=|V(G)|$,

$$
\tau(G)+\alpha(G)=n.
$$

Every extra [vertex](graph.md#vertex-graph-theory) that can be left in an [independent set](#independent-set-graph-theory) is one fewer [vertex](graph.md#vertex-graph-theory) needed in a [minimum vertex cover](#minimum-vertex-cover). This identity holds for all finite [simple graphs](graph.md#simple-graph), including the [triangle in a graph](graph.md#triangle-in-a-graph) and the [cycle graph](#cycle-graph) $C_5$; it does not require the [bipartite graph](#bipartite-graph) hypothesis of [Kőnig's theorem for bipartite matching](#konig-s-theorem-graph-theory).

For a nonempty [graph](graph.md), every [colour class](ramsey-theory.md#colour-class) of a [proper vertex colouring](#proper-vertex-coloring) contains at most $\alpha(G)$ [vertices](graph.md#vertex-graph-theory). Counting all the [vertices](graph.md#vertex-graph-theory) therefore gives

$$
\chi(G)\geq\frac{|V(G)|}{\alpha(G)}.
$$

Since the [chromatic number](#chromatic-number) is an [integer](number-theory.md#integer), the bound rounds up: for the [cycle graph](#cycle-graph) $C_5$, $\chi(C_5)\geq\lceil5/2\rceil=3$. It is attained by assigning colour $A$ to $0,2$, colour $B$ to $1,3$, and colour $C$ to $4$. All five [edges](#edge-of-a-graph), including $40$, have differently coloured endpoints.

#### Caro-Wei bound

↑ **Parent:** [Independence number](#independence-number)

For a finite simple [graph](graph.md), $\alpha(G)\geq\sum_{v\in V(G)}1/(1+\deg v)\geq |V(G)|^2/(|V(G)|+2|E(G)|)$. Randomly order its [vertices](graph.md#vertex-graph-theory) and retain each [vertex](graph.md#vertex-graph-theory) preceding all its [graph neighbours](#neighbour-of-a-vertex). This gives an [independent set](#independent-set-graph-theory) with the first expression as its [expected value](probability-theory.md#expected-value). The second inequality is the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality).

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

A [graph ray](#ray-in-a-graph) is an infinite [sequence](real-analysis.md#sequence) $v_0,v_1,\ldots$ of distinct [graph vertices](graph.md#vertex-graph-theory) with an [edge](#edge-of-a-graph) between consecutive [graph vertices](graph.md#vertex-graph-theory). Every infinite connected [locally finite graph](#locally-finite-graph) contains a [graph ray](#ray-in-a-graph) from each [graph vertex](graph.md#vertex-graph-theory), by the [König infinity lemma](combinatorics.md#konig-s-lemma) applied to its finite self-avoiding [graph paths](#path-in-a-graph). An open [graph ray](#ray-in-a-graph) witnesses an infinite [percolation cluster](bond-percolation.md#percolation-cluster).

### Path graph

↑ **Parent:** [Path in a graph](#path-in-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Path_graph)

A path graph $P_n$ has $n$ vertices in a single chain and $n-1$ edges. Its endpoint [graph distance](#distance-graph-theory) is $n-1$ and, with unit resistances, its endpoint [effective resistance](markov-process.md#effective-resistance) is also $n-1$.

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

An odd cycle is a [cycle in a graph](#cycle-in-a-graph) with an [odd number](number-theory.md#odd-number) of edges.

#### Cycle graph

↑ **Parent:** [Cycle in a graph](#cycle-in-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cycle_graph)

The cycle graph $C_n$ has vertices $v_1,\ldots,v_n$ and edges $v_iv_{i+1}$, with indices read cyclically.

##### Wheel graph

↑ **Parent:** [Cycle graph](#cycle-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wheel_graph)

A wheel graph is the [join of graphs](#join-graph-theory) of a [cycle graph](#cycle-graph) and a single [vertex](graph.md#vertex-graph-theory). Every wheel with a rim of at least three [vertices](graph.md#vertex-graph-theory) has a $K_4$ [graph minor](#graph-minor): partition the rim into three nonempty consecutive connected sets and use its centre as the fourth [branch set of a graph minor](#branch-set-of-a-graph-minor).

##### Hamilton cycle

↑ **Parent:** [Cycle graph](#cycle-graph)

A [Hamilton cycle](#hamilton-cycle), also called a [Hamiltonian cycle](#hamilton-cycle), is a [cycle in a graph](#cycle-in-a-graph) containing every [vertex](graph.md#vertex-graph-theory) of the [graph](graph.md). Here the convention is a finite [simple graph](graph.md#simple-graph) whose [edges](#edge-of-a-graph) are undirected, with $n=|V|\geq3$. A traversal is a [sequence](real-analysis.md#sequence)

$$
v_0,v_1,\ldots,v_{n-1},v_n=v_0,
$$

where $v_0,\ldots,v_{n-1}$ are all the distinct [vertices](graph.md#vertex-graph-theory) and $\{v_i,v_{i+1}\}\in E$ for $0\leq i<n$. Thus "once" means once before the closing return: the start appears again at the end, and there are exactly $n$ traversed [edges](#edge-of-a-graph). The [graph](graph.md) may contain additional unused [edges](#edge-of-a-graph).[Diestel, Graph Theory, Chapter 10, opening paragraph, printed p. 323: Hamilton cycles, Hamilton paths, and the contrast with Euler tours](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/hamilton-cycles)

A [Hamiltonian path](#hamiltonian-path) visits all [vertices](graph.md#vertex-graph-theory) once without requiring a return. Removing an [edge](#edge-of-a-graph) from a [Hamilton cycle](#hamilton-cycle) gives a [Hamiltonian path](#hamiltonian-path); a particular [Hamiltonian path](#hamiltonian-path) closes only if its endpoints are adjacent. An [Euler circuit](#euler-circuit) instead traverses every [edge](#edge-of-a-graph) exactly once and can revisit [vertices](graph.md#vertex-graph-theory) midway. The two requirements are independent, as these original labelled examples show.

<a id="hamilton-euler-vertex-edge-comparison"></a>
![](hamilton-euler-vertex-edge-comparison.png)

**[Figure 22](#hamilton-euler-vertex-edge-comparison). Two graphs separate Hamilton cycle vertex coverage from Euler circuit edge coverage; arrows mark traversal order, not directed edges**.

For the [complete graph](#complete-graph) $K_4$, use $V=\{A,B,C,D\}$ and $E=\{AB,AC,AD,BC,BD,CD\}$, where $AB$ abbreviates the unordered pair $\{A,B\}$. The route $A,B,C,D,A$ is a [Hamilton cycle](#hamilton-cycle): it visits every [vertex](graph.md#vertex-graph-theory) and uses four of the six [edges](#edge-of-a-graph), omitting $AC$ and $BD$. It is not an [Euler circuit](#euler-circuit), and the [graph](graph.md) admits no [Euler circuit](#euler-circuit) at all: every [vertex degree](#degree-graph-theory) is three, contradicting the [Euler circuit criterion](#euler-circuit-criterion). The crossing of the drawn diagonals is not another [vertex](graph.md#vertex-graph-theory).

Conversely, take two [triangles in a graph](graph.md#triangle-in-a-graph) sharing only $X$, with $V=\{X,A,B,C,D\}$ and $E=\{XA,AB,BX,XC,CD,DX\}$. The route $X,A,B,X,C,D,X$ is an [Euler circuit](#euler-circuit), using all six [edges](#edge-of-a-graph) once; the [vertex degrees](#degree-graph-theory) are $4,2,2,2,2$. It cannot be a [Hamilton cycle](#hamilton-cycle), since $X$ occurs midway as well as at the start and end. More strongly, no [Hamilton cycle](#hamilton-cycle) exists: $X$ is a [cut vertex](#cut-vertex), and deleting it leaves the two separate [edges](#edge-of-a-graph) $AB$ and $CD$. Nevertheless, $A,B,X,C,D$ is a [Hamiltonian path](#hamiltonian-path), whose endpoints are not adjacent.

###### Hamiltonian graph

↑ **Parent:** [Hamilton cycle](#hamilton-cycle)

A [Hamiltonian graph](#hamiltonian-graph) is a [graph](graph.md) containing a [Hamilton cycle](#hamilton-cycle). This describes existence of a spanning [graph cycle](#cycle-in-a-graph), rather than requiring every [edge](#edge-of-a-graph) of the [graph](graph.md) to belong to that [graph cycle](#cycle-in-a-graph). In the finite [simple graph](graph.md#simple-graph) convention, $K_n$ is a [Hamiltonian graph](#hamiltonian-graph) for $n\geq3$, because any ordering of its [vertices](graph.md#vertex-graph-theory) closes using available [edges](#edge-of-a-graph).

###### Necessary conditions for a Hamilton cycle

↑ **Parent:** [Hamilton cycle](#hamilton-cycle)

A [Hamiltonian graph](#hamiltonian-graph) must be a [connected graph](graph.md#connected-graph) and have [minimum degree](#minimum-degree-of-a-graph) $\delta(G)\geq2$: each [vertex](graph.md#vertex-graph-theory) has two distinct neighbours on its [Hamilton cycle](#hamilton-cycle). It also has no [cut vertex](#cut-vertex). Indeed, deleting any [vertex](graph.md#vertex-graph-theory) from the [Hamilton cycle](#hamilton-cycle) leaves a [graph path](#path-in-a-graph) through every remaining [vertex](graph.md#vertex-graph-theory), so the remaining [graph](graph.md) is connected. These are quick ways to rule out a [Hamilton cycle](#hamilton-cycle).[Diestel, Graph Theory, §10.1, printed pp. 323–324: necessary minimum degree two and 2-connectivity](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/hamilton-cycles)

Even these conditions together are not sufficient: the [complete bipartite graph](#complete-bipartite-graph) $K_{2,3}$ is connected, has [minimum degree](#minimum-degree-of-a-graph) two and no [cut vertex](#cut-vertex), but has no [Hamilton cycle](#hamilton-cycle). Every [graph cycle](#cycle-in-a-graph) in a [bipartite graph](#bipartite-graph) alternates between its two parts, using equally many [vertices](graph.md#vertex-graph-theory) from each; it cannot use all two and all three.

In the other direction, [Dirac's theorem](#dirac-s-theorem) gives a sufficient condition: a finite [simple graph](graph.md#simple-graph) with $n\geq3$ and $\delta(G)\geq n/2$ has a [Hamilton cycle](#hamilton-cycle). Failure of this inequality proves nothing by itself: the [cycle graph](#cycle-graph) $C_5$ has a [Hamilton cycle](#hamilton-cycle) despite $\delta(C_5)=2<5/2$.[Diestel, Graph Theory, §10.1, Theorem 10.1.1, printed p. 324](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/hamilton-cycles)

###### Weighted Hamilton cycle

↑ **Parent:** [Hamilton cycle](#hamilton-cycle)

A [weighted Hamilton cycle](#weighted-hamilton-cycle) is a [Hamilton cycle](#hamilton-cycle) in a [weighted graph](markov-process.md#weighted-graph), with cost equal to the sum of its traversed [edge](#edge-of-a-graph) weights. Here weights represent symmetric nonnegative costs, rather than conductances. Asking whether a [Hamilton cycle](#hamilton-cycle) exists is a feasibility question; asking for the cheapest one is an instance of the [travelling salesman problem](mathematical-optimization.md#travelling-salesman-problem). A [complete graph](#complete-graph) supplies every possible connection between distinct [vertices](graph.md#vertex-graph-theory), making feasibility automatic for $n\geq3$, while choosing the cheapest visiting order remains a separate [mathematical optimization](mathematical-optimization.md) problem.

<a id="weighted-hamilton-cycle-four-vertex-tours"></a>
![](weighted-hamilton-cycle-four-vertex-tours.png)

**[Figure 23](#weighted-hamilton-cycle-four-vertex-tours). A fictitious weighted graph on four vertices: its three Hamilton cycles, identified under reversal and cyclic rotation, have costs 14, 19 and 21**.

Assign the [complete graph](#complete-graph) $K_4$ the symmetric [edge](#edge-of-a-graph) costs $w_{AB}=2$, $w_{BC}=3$, $w_{CD}=4$, $w_{AD}=5$, $w_{AC}=6$ and $w_{BD}=7$, in arbitrary units. Fix the start at $A$ and identify each [Hamilton cycle](#hamilton-cycle) with its reverse. The three possibilities are

$$
\begin{aligned}
A,B,C,D,A &: 2+3+4+5=14,\\
A,B,D,C,A &: 2+7+4+6=19,\\
A,C,B,D,A &: 6+3+7+5=21.
\end{aligned}
$$

These exhaust the possibilities: the [permutations](combinatorics.md#permutation) of the other three [vertices](graph.md#vertex-graph-theory) give $3!=6$ orders, paired into three reversals. Hence the perimeter tour really is optimal for this toy instance. The diagram's geometric lengths are not costs, and no [triangle inequality](topological-analysis.md#triangle-inequality) is assumed.

The usefulness of this model is to distinguish visiting required sites from covering required connections. If tasks are assigned to [vertices](graph.md#vertex-graph-theory) and the route must return after one visit to each, a [weighted Hamilton cycle](#weighted-hamilton-cycle) captures the ordering requirement. If the job instead requires each [edge](#edge-of-a-graph) once, the relevant object is an [Euler circuit](#euler-circuit). The [shortest path problem](#shortest-path-problem) asks only for a cheapest route between specified endpoints. A 1954 primary research paper gave a concrete motivation for the [travelling salesman problem](mathematical-optimization.md#travelling-salesman-problem): certify that a particular tour through 49 cities has minimum road-distance cost.[Solution of a Large-Scale Traveling-Salesman Problem by G. Dantzig, R. Fulkerson and S. Johnson, abstract; Journal of the Operations Research Society of America 2(4), pp. 393–410 (1954)](mathematics-bibliography.md#solution-of-a-large-scale-traveling-salesman-problem-by-george-b-dantzig-and-others)

These are abstract route models. If a cost stands for a whole [graph path](#path-in-a-graph) through an underlying network, travelling between consecutive task [vertices](graph.md#vertex-graph-theory) can pass through intermediate network [vertices](graph.md#vertex-graph-theory) more than once. One visit per task therefore does not imply one visit per physical junction. One-way connections require a [directed graph](#directed-graph); changing costs or extra timing constraints require a richer model than the fixed symmetric toy instance.

###### Icosian game

↑ **Parent:** [Hamilton cycle](#hamilton-cycle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Icosian_game)

The [Icosian game](#icosian-game) made the [vertex](graph.md#vertex-graph-theory)-visit puzzle tangible. The report of its 1857 presentation describes a plane projection of a regular [dodecahedron](geometry-and-topology.md#dodecahedron), with holes at the [vertices](graph.md#vertex-graph-theory) for ivory pins. The Trinity College Dublin archive connects this game with the search for closed routes visiting each [vertex](graph.md#vertex-graph-theory) exactly once. This puzzle supplies a historical illustration of the [Hamilton cycle](#hamilton-cycle) requirement.[The Icosian Calculus, Hamilton papers archive: opening historical introduction and quoted report of the 1857 British Association presentation: dodecahedron projection and ivory pins](mathematics-bibliography.md#the-icosian-calculus-hamilton-papers-archive)

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

## Complete graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_graph)

The complete graph $K_r$ has $r$ vertices and every possible edge between distinct vertices.

### Clique (graph theory)

↑ **Parent:** [Complete graph](#complete-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clique_(graph_theory))

A clique in a graph is a vertex set whose induced subgraph is complete. A copy of $K_r$ is therefore an $r$-vertex clique.

#### Maximal clique

↑ **Parent:** [Clique (graph theory)](#clique-graph-theory)

A maximal clique is a [clique](#clique-graph-theory) not strictly contained in another clique. This is distinct from a largest clique, whose size equals the [clique number](#clique-number). In a triangulated [probabilistic graphical model](statistical-model.md#probabilistic-graphical-model), maximal cliques are the natural nodes of a [junction tree](statistical-model.md#junction-tree).

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

The maximum number of vertices in a [clique](#clique-graph-theory) of a [graph](graph.md). If the graph contains $K_k$ and no $K_{k+1}$, its clique number is exactly $k$, since every larger [clique](#clique-graph-theory) contains a $(k+1)$-[clique](#clique-graph-theory).

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

The octahedral graph is the [graph](graph.md) obtained from $K_6$ by removing a [perfect matching](#perfect-matching); equivalently it is $K_{2,2,2}$. Its [chromatic number](#chromatic-number) is three, and it contains two vertex-disjoint [triangles in a graph](graph.md#triangle-in-a-graph). A [complete bipartite graph](#complete-bipartite-graph) with a single additional internal edge cannot contain it: every triangle in that host uses the additional edge.

### Balancing a multipartite edge-triangle objective

↑ **Parent:** [Complete multipartite graph](#complete-multipartite-graph)

With two part sizes of fixed sum and all other sizes fixed, this objective has form constant plus $(1-cB)a_ia_j$, where $B$ is the sum of the other sizes. A nonpositive coefficient permits merging the pair, while a positive coefficient favours balancing it. Choose an optimum with fewest nonzero parts: all remaining coefficients are positive, and the integer sizes differ by at most one. For real sizes they are exactly equal. This explains extremizers among [Turán graphs](#turan-graph).

### Balanced complete multipartite blow-up

↑ **Parent:** [Complete multipartite graph](#complete-multipartite-graph)

The balanced complete multipartite blow-up $K_r(t)$ replaces each [vertex](graph.md#vertex-graph-theory) of the [complete graph](#complete-graph) $K_r$ by an [independent set](#independent-set-graph-theory) of $t$ [vertices](graph.md#vertex-graph-theory), placing every possible [edge](#edge-of-a-graph) between different sets and none inside a set. Every fixed [graph](graph.md) of [chromatic number](#chromatic-number) at most $r$ embeds into $K_r(t)$ for sufficiently large $t$.

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

The constant [eigenvector](linear-operator-theory.md#eigenvector) has [eigenvalue](linear-operator-theory.md#eigenvalue) zero; the other two describe progressively stronger neighbour disagreement. Dividing these [eigenvectors](linear-operator-theory.md#eigenvector) by $\sqrt3,\sqrt2,\sqrt6$, respectively, gives an [orthonormal basis](linear-algebra.md#orthonormal-basis). The four-[vertex](graph.md#vertex-graph-theory) [cycle graph](#cycle-graph) is already worked out under [circulant matrix](linear-algebra.md#circulant-matrix), where [Fourier diagonalization of a circulant matrix](linear-algebra.md#fourier-diagonalization-of-a-circulant-matrix) gives its [eigenvalues](linear-operator-theory.md#eigenvalue).

Every formula here uses $L=D-A$ without degree normalization. For comparison, Chung's treatment uses the degree-scaled [matrix](vector-space.md#matrix) $D^{-1/2}LD^{-1/2}$, with a convention for isolated [vertices](graph.md#vertex-graph-theory); its [eigenvalues](linear-operator-theory.md#eigenvalue) must not be substituted into the examples here.[Chung, Lectures on Spectral Graph Theory, Section 1.2](https://www.math.ucsd.edu/~fan/cbms.pdf)

### Weighted graph Laplacian

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

For a finite [undirected graph](#undirected-graph) without [self-loops](graph.md#loop-graph-theory), give each [edge](#edge-of-a-graph) a symmetric nonnegative weight $w_{ij}=w_{ji}$. In the [weighted graph](markov-process.md#weighted-graph), set $(A_w)_{ij}=w_{ij}$ for an [edge](#edge-of-a-graph) and zero otherwise, and $(D_w)_{ii}=\sum_jw_{ij}$ with all other entries zero. The [Weighted graph Laplacian](#weighted-graph-laplacian) is

$$
L_w=D_w-A_w,\qquad
(L_wx)_i=\sum_jw_{ij}(x_i-x_j),\qquad
x^TL_wx=\sum_{\{i,j\}\in E}w_{ij}(x_i-x_j)^2.
$$

Each [edge](#edge-of-a-graph) appears once in the [quadratic form](linear-algebra.md#quadratic-form). For the [path graph](#path-graph) $A-B-C$ with weights $w_{AB}=2$ and $w_{BC}=3$,

$$
L_w=\begin{pmatrix}2&-2&0\\-2&5&-3\\0&-3&3\end{pmatrix},\qquad
x=\begin{pmatrix}2\\0\\-1\end{pmatrix},\qquad
x^TL_wx=2(2-0)^2+3(0-(-1))^2=11.
$$

The [Weighted graph Laplacian](#weighted-graph-laplacian) is still a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix). Its [kernel](linear-algebra.md#kernel-of-a-linear-map) consists of [vectors](vector-space.md#vector) constant on each [connected component of a graph](graph.md#component-graph-theory) after zero-weight [edges](#edge-of-a-graph) are removed: an [edge](#edge-of-a-graph) of weight zero imposes no constraint. In an [electrical network](markov-process.md#electrical-network), taking the weights to be [electrical conductances](electromagnetism.md#electrical-conductance) makes $x^TL_wx$ the total power dissipated by [Joule heating](electromagnetism.md#joule-heating) when $x$ gives the [voltages](markov-process.md#voltage) at the [vertices](graph.md#vertex-graph-theory). This physical interpretation explains why stronger connections penalize disagreement more heavily.[Spielman, Spectral Graph Theory, Section 16.3.2: resistor networks](https://www.cs.yale.edu/homes/spielman/PAPERS/SGTChapter.pdf)

### Degree matrix

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

The [degree matrix](#degree-matrix) is the [diagonal matrix](linear-algebra.md#diagonal-matrix) whose $i$th diagonal entry is the [degree of a vertex](#degree-graph-theory) $i$. For a finite [simple graph](graph.md#simple-graph), $d_i=\sum_jA_{ij}$, where $A$ is its [adjacency matrix](#adjacency-matrix). For a [Weighted graph Laplacian](#weighted-graph-laplacian), use the sum of incident [edge](#edge-of-a-graph) weights instead of the number of incident [edges](#edge-of-a-graph).

### Graph Laplacian quadratic form

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

Assign a real value $x_i$ to each [vertex](graph.md#vertex-graph-theory). The [Graph Laplacian quadratic form](#graph-laplacian-quadratic-form) measures disagreement across [edges](#edge-of-a-graph):

$$
x^TLx=\sum_{\{i,j\}\in E}(x_i-x_j)^2\geq0.
$$

This makes the [Graph Laplacian](#laplacian-matrix) a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix). The [energy](classical-mechanics.md#energy) is small when neighbours have similar values, even if distant [vertices](graph.md#vertex-graph-theory) have very different values; it depends on connections rather than where the [graph](graph.md) is drawn. In the three-[vertex](graph.md#vertex-graph-theory) [path graph](#path-graph), take $x=(2,0,-1)^T$. Then

$$
Lx=(2,-1,-1)^T,\qquad
x^TLx=2\cdot2+0\cdot(-1)+(-1)\cdot(-1)=5,
$$

and the two [edges](#edge-of-a-graph) contribute $(2-0)^2=4$ and $(0-(-1))^2=1$.

<a id="image-edge-disagreement-and-eigenvectors-of-the-three-vertex-path-laplacian"></a>
![](graph-laplacian-edge-energy.png)

**[Figure 24](#image-edge-disagreement-and-eigenvectors-of-the-three-vertex-path-laplacian). Edge disagreement and eigenvectors of the three-vertex path Laplacian**.

For a short proof, expand $x^T(D-A)x$. Each [edge](#edge-of-a-graph) contributes $x_i^2+x_j^2$ through the [degree matrix](#degree-matrix) and $-2x_ix_j$ through the [adjacency matrix](#adjacency-matrix), yielding $(x_i-x_j)^2$. The sum over unordered [edges](#edge-of-a-graph) has no factor $1/2$; a sum over all ordered pairs does:

$$
x^TLx=\frac12\sum_{i,j}A_{ij}(x_i-x_j)^2.
$$

Equivalently, let $B$ be an [oriented incidence matrix](graph.md#oriented-incidence-matrix), with one row per [edge](#edge-of-a-graph). Then $Bx$ records endpoint differences and $L=B^TB$, independently of the chosen orientations. This translates a local comparison into a global [quadratic form](linear-algebra.md#quadratic-form) and makes its nonnegativity visible.

### Kernel of a graph Laplacian

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

The [kernel](linear-algebra.md#kernel-of-a-linear-map) of the [Graph Laplacian](#laplacian-matrix) consists exactly of [vectors](vector-space.md#vector) constant on each [connected component of a graph](graph.md#component-graph-theory). Indeed, $Lx=0$ implies $x^TLx=0$, so the [Graph Laplacian quadratic form](#graph-laplacian-quadratic-form) forces equality at the endpoints of every [edge](#edge-of-a-graph); equality then propagates along [graph paths](#path-in-a-graph). Conversely, these equalities make every entry of $Lx$ zero. Thus the [dimension](vector-space.md#dimension-vector-space) of the [kernel](linear-algebra.md#kernel-of-a-linear-map), equivalently the multiplicity of the zero [eigenvalue](linear-operator-theory.md#eigenvalue), counts the [connected components of a graph](graph.md#component-graph-theory).

For the disconnected [graph](graph.md) with just two [edges](#edge-of-a-graph), $AB$ and $CD$, in order $A,B,C,D$,

$$
L=\begin{pmatrix}1&-1&0&0\\-1&1&0&0\\0&0&1&-1\\0&0&-1&1\end{pmatrix},\qquad
\ker L=\operatorname{span}\left\{\begin{pmatrix}1\\1\\0\\0\end{pmatrix},\begin{pmatrix}0\\0\\1\\1\end{pmatrix}\right\}.
$$

The two displayed [vectors](vector-space.md#vector) form a [basis](vector-space.md#basis) of the [kernel](linear-algebra.md#kernel-of-a-linear-map). The other two [eigenvectors](linear-operator-theory.md#eigenvector) $(1,-1,0,0)^T$ and $(0,0,1,-1)^T$ each have [eigenvalue](linear-operator-theory.md#eigenvalue) two, so the full list of [eigenvalues](linear-operator-theory.md#eigenvalue), including multiplicities, is $0,0,2,2$. Separate [connected components of a graph](graph.md#component-graph-theory) allow independent constant levels; a single global constant is only one of these possibilities.

<a id="image-two-disconnected-edges-give-two-independent-zero-eigenvectors"></a>
![](graph-laplacian-connected-components.png)

**[Figure 25](#image-two-disconnected-edges-give-two-independent-zero-eigenvectors). Two disconnected edges give two independent zero eigenvectors**.

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

More generally, an [eigenvector](linear-operator-theory.md#eigenvector) with [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda$ decays by $e^{-\lambda t}$. The [spectral theorem for real symmetric matrices](linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) supplies an [orthonormal basis](linear-algebra.md#orthonormal-basis) of these [eigenvectors](linear-operator-theory.md#eigenvector), and the [kernel of a graph Laplacian](#kernel-of-a-graph-laplacian) identifies the surviving terms. On a nonempty [connected graph](graph.md#connected-graph),

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

### Two-resource path packing as minimum-cost circulation

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

Consider nonnegative route variables with constraints $u\leq a$, $v\leq b$, $v+w\leq c$, $w+z\leq d$, and a linear reward $p_u u+p_v v+p_w w+p_z z$. It is a [minimum-cost flow](#minimum-cost-flow-problem) problem: use arcs $s\to t$ of capacity $a$ and cost $-p_u$, $s\to L$ of capacity $c$ and cost zero, $L\to t$ of capacity $b$ and cost $-p_v$, $L\to R$ of unlimited capacity and cost $-p_w$, $s\to R$ of unlimited capacity and cost $-p_z$, and $R\to t$ of capacity $d$ and cost zero. Close the network by an unlimited zero-cost arc $t\to s$. The four forward path flows are exactly $u,v,w,z$, so conservation gives the resource constraints. This reduction does not assert that general multi-commodity flow is ordinary minimum-cost flow.

### Feasible flow

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

A feasible flow satisfies every [flow balance](#flow-balance) and every capacity interval of a network problem. Feasibility is distinct from optimality: [capacitated flow optimality conditions](#capacitated-flow-optimality-conditions) additionally certify that no allowed balanced flow displacement reduces the cost. With only one independent [graph cycle](#cycle-in-a-graph), every balanced flow is determined by a single cycle parameter, and its feasible set is the intersection of the induced parameter intervals.

### Capacitated flow optimality conditions

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

For positive capacities and a feasible flow, optimality is equivalent to [network dual potentials](#network-dual-potential) for which the [network reduced cost](#network-reduced-cost) is nonnegative at a lower bound, zero in the interior, and nonpositive at an upper bound. These signs make every feasible displacement nonnegative in total cost. They are also equivalent to absence of negative-cost cycles in the [residual network](#residual-network). A zero-capacity edge is fixed and imposes no reduced-cost sign condition.

### Flow balance

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

A flow balance prescribes net outgoing minus incoming flow at a vertex. Positive $b_i$ is supply and negative $b_i$ is demand; zero is ordinary [flow conservation](#flow-conservation). Summing all balances requires total supply to equal total demand. In a [directed graph](#directed-graph), these equations are represented by the [oriented incidence matrix](graph.md#oriented-incidence-matrix).

### Uncapacitated minimum-cost flow

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

An uncapacitated [minimum-cost flow](#minimum-cost-flow-problem) has nonnegative edge flows without finite upper capacities. The [flow balances](#flow-balance) prescribe net supply at each vertex. For the [oriented incidence matrix](graph.md#oriented-incidence-matrix) convention with tail $+1$ and head $-1$, vertex [network dual potentials](#network-dual-potential) have [network reduced costs](#network-reduced-cost) $c_{ij}-\pi_i+\pi_j$. Nonnegative [network reduced costs](#network-reduced-cost) and [complementary slackness](mathematical-optimization.md#complementary-slackness) certify a feasible optimum. A feasible negative-cost directed cycle makes the problem unbounded below.

#### Network dual potential

↑ **Parent:** [Uncapacitated minimum-cost flow](#uncapacitated-minimum-cost-flow)

A vertex potential in the dual of an [uncapacitated minimum-cost flow](#uncapacitated-minimum-cost-flow) yields the edge inequalities $\pi_i-\pi_j\leq c_{ij}$. Its objective is $\sum_i\pi_i b_i$. Adding a common constant leaves all [network reduced costs](#network-reduced-cost) and the objective unchanged when total net supply is zero. Potentials tight on a [spanning tree](combinatorics.md#spanning-tree) are fixed up to this common constant.

##### Dual network potentials from shortest-path distances

↑ **Parent:** [Network dual potential](#network-dual-potential)

In a directed network with no negative-cost directed cycle, add a source having zero-cost arcs to all vertices and compute shortest-path distances $d_i$. The inequalities $d_j\le d_i+c_{ij}$ make $\pi_i=-d_i$ dual feasible for [uncapacitated minimum-cost flow](#uncapacitated-minimum-cost-flow). Shortest-path tree arcs are tight. An arbitrary spanning tree also fixes tight candidate potentials up to a constant, but it does not guarantee the non-tree inequalities; these must be checked.

##### Network reduced cost

↑ **Parent:** [Network dual potential](#network-dual-potential)

With the tail-positive incidence convention, a network edge's reduced cost is $r_{ij}=c_{ij}-\pi_i+\pi_j$. For [uncapacitated minimum-cost flow](#uncapacitated-minimum-cost-flow), dual feasibility requires $r_{ij}\geq0$ and [complementary slackness](mathematical-optimization.md#complementary-slackness) requires $f_{ij}r_{ij}=0$. A negative non-tree reduced cost identifies an improving [graph cycle](#cycle-in-a-graph) pivot in the [network simplex algorithm](#network-simplex-algorithm). This sign convention differs from the row-column potentials of a [transportation problem](mathematical-optimization.md#transportation-problem).

### Network simplex algorithm

↑ **Parent:** [Minimum-cost flow problem](#minimum-cost-flow-problem)

The network simplex algorithm specializes the [simplex algorithm](numerical-analysis.md#simplex-algorithm) to network flows. A basis is represented by a spanning tree with nonbasic flows at their bounds; potentials give [reduced costs](mathematical-optimization.md#reduced-cost), and entering arcs produce cycle pivots. [Degeneracy in linear programming](mathematical-optimization.md#degeneracy-in-linear-programming) is particularly common in assignment instances.

#### Network simplex tree basis

↑ **Parent:** [Network simplex algorithm](#network-simplex-algorithm)

For a connected capacitated [minimum-cost flow](#minimum-cost-flow-problem) network, a [spanning tree](combinatorics.md#spanning-tree) supplies basic flow variables. Every non-tree edge is fixed at its lower or upper bound. [Flow balance](#flow-balance) determines the tree flows; these must also obey [capacity constraints](#capacity-constraint). An entering edge creates one cycle, and adjusting flow on that cycle preserves balance until a bound is hit and an edge leaves the tree.

## Extremal graph theory

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Extremal_graph_theory)

### Supersaturation

↑ **Parent:** [Extremal graph theory](#extremal-graph-theory)

Supersaturation strengthens an extremal existence theorem by forcing many copies of a forbidden graph when the edge count exceeds its extremal threshold by a fixed density. For a fixed clique, the [Erdős-Stone theorem](#erdos-stone-theorem) and averaging over bounded-size random vertex subsets give a positive multiple of $n^{|V(F)|}$ copies.

#### Clique supersaturation by sampling

↑ **Parent:** [Supersaturation](#supersaturation)

Choose a fixed sample size $m$ for which the normalized [Turan theorem](#turan-s-theorem) bound lies below the given density by a positive margin. The expected [edge](#edge-of-a-graph) count in a random $m$-vertex subset then forces a positive proportion of subsets to contain a forbidden-size [clique](#clique-graph-theory). Each [clique](#clique-graph-theory) belongs to a known number of subsets, so double counting gives a positive constant times $n^{r+1}$ [cliques](#clique-graph-theory).

### Extremal number

↑ **Parent:** [Extremal graph theory](#extremal-graph-theory)

The extremal number $\operatorname{ex}(n,H)$ is the largest number of edges in an $n$-vertex graph containing no subgraph isomorphic to $H$.

#### Extremal graph for disjoint cliques

↑ **Parent:** [Extremal number](#extremal-number)

For fixed positive integers $r,s$ and sufficiently large $n$, the unique extremal [graph](graph.md) forbidding $s$ vertex-disjoint copies of the [complete graph](#complete-graph) $K_{r+1}$ is the [join of graphs](#join-graph-theory) $K_{s-1}+T_r(n-s+1)$, up to [isomorphic graphs](graph.md#graph-isomorphism). Each forbidden [clique](#clique-graph-theory) would require a distinct [vertex](graph.md#vertex-graph-theory) of $K_{s-1}$.

#### Monotonicity of the normalized extremal number

↑ **Parent:** [Extremal number](#extremal-number)

For every fixed graph $H$, the sequence

$$
\frac{\operatorname{ex}(n,H)}{\binom n2}
$$

is nonincreasing once $n\geq2$. Indeed, choose a uniformly random $m$-vertex [induced subgraph](#induced-subgraph) of an extremal $H$-free graph on $n$ vertices. It remains $H$-free and has expected edge count

$$
\operatorname{ex}(n,H)\frac{\binom m2}{\binom n2},
$$

which cannot exceed $\operatorname{ex}(m,H)$.

#### Mantel theorem

↑ **Parent:** [Extremal number](#extremal-number)

Every triangle-free graph on $n$ vertices has at most $\lfloor n^2/4\rfloor$ edges.

This is the triangle-free case of [Turán's theorem](#turan-s-theorem).

##### Triangle lower bound one edge above the Mantel threshold

↑ **Parent:** [Mantel theorem](#mantel-theorem)

Every graph on $2n$ vertices with at least $n^2+1$ edges contains at least $n$ triangles. An induction deletes the endpoints of an edge lying in no triangle; if every edge lies in a triangle, the [edge-triangle incidence bound](graph.md#edge-triangle-incidence-bound) is already sufficient.

<h3 id="turan-s-theorem">Turán's theorem</h3>

↑ **Parent:** [Extremal graph theory](#extremal-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turán's_theorem)

Among $n$-vertex graphs containing no $K_{r+1}$, the maximum number of edges is attained by the complete $r$-partite graph whose part sizes differ by at most one, denoted $T_r(n)$.

#### Edit-distance stability for clique-free graphs

↑ **Parent:** [Turán's theorem](#turan-s-theorem)

A clique-free [graph](graph.md) near the [Turan theorem](#turan-s-theorem) [edge](#edge-of-a-graph) bound is close to a complete multipartite [graph](graph.md). Choose a maximum-degree [vertex](graph.md#vertex-graph-theory), split its neighbourhood from the remaining [vertices](graph.md#vertex-graph-theory), and apply induction inside the neighbourhood. The degree bound implies that missing cross [edges](#edge-of-a-graph) are at least twice the number of [edges](#edge-of-a-graph) inside the remaining class. This inequality controls all three types of edits and gives the constant three.

##### Bipartite stability from few odd cycles

↑ **Parent:** [Edit-distance stability for clique-free graphs](#edit-distance-stability-for-clique-free-graphs)

Fix an odd cycle length. If the [graph](graph.md) has [edge](#edge-of-a-graph) density at least $1/2-\epsilon$ and sufficiently few copies of that cycle, [odd-cycle copies from positive triangle density](probabilistic-combinatorics.md#odd-cycle-copies-from-positive-triangle-density) forces few [triangles in a graph](graph.md#triangle-in-a-graph). The [triangle removal lemma](probabilistic-combinatorics.md#triangle-removal-lemma) deletes at most $\epsilon\binom n2$ [edges](#edge-of-a-graph), after which the clique-free edit bound applies with two parts. Absorbing its linear rounding error into the density margin gives the displayed bound for large order.

<h4 id="turan-graph">Turán graph</h4>

↑ **Parent:** [Turán's theorem](#turan-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turán_graph)

The Turan graph $T_r(n)$ is the [complete multipartite graph](#complete-multipartite-graph) on $n$ vertices with $r$ parts whose sizes differ by at most one.

##### Triangle support line between bipartite and tripartite Turan graphs

↑ **Parent:** [Turán graph](#turan-graph)

For $n\geq3$, put $e_i=e(T_i(n))$, $t_3=k_3(T_3(n))$, and $c_n=(e_3-e_2)/t_3$. Every [graph](graph.md) on $n$ [vertices](graph.md#vertex-graph-theory) satisfies

$$
e(G)-c_n k_3(G)\leq e_2.
$$

Thus an [edge](#edge-of-a-graph) count $e_2+\theta(e_3-e_2)$ forces at least $\theta t_3$ [triangles in a graph](graph.md#triangle-in-a-graph). This is an exact finite bound, with the rounding in the [Turán graph](#turan-graph) retained. To prove it, use [edge-triangle symmetrization](#edge-triangle-symmetrization). The inequality $c_n\geq2/n$ allows merging the two smallest classes when there are at least four classes. With three classes, fixing the middle class makes the objective affine in the product of the other two sizes; either merge them or balance them. Only $T_2(n)$ and $T_3(n)$ need remain.

#### Zykov symmetrization

↑ **Parent:** [Turán's theorem](#turan-s-theorem)

Zykov symmetrization replaces one of two nonadjacent vertices by a clone of the other. Cloning the vertex of larger degree does not decrease the edge count and does not create a larger clique. Iteration reduces the extremal problem for clique-free graphs to complete multipartite graphs.

##### Edge-triangle symmetrization

↑ **Parent:** [Zykov symmetrization](#zykov-symmetrization)

For each real $c$, some maximizer of $e(G)-c k_3(G)$ among [graphs](graph.md) on $n$ [vertices](graph.md#vertex-graph-theory) is [complete multipartite graph](#complete-multipartite-graph). Among maximizers maximize $\sum_v d(v)^2$. Cloning either of two nonadjacent [vertices](graph.md#vertex-graph-theory) preserves the objective, since maximality forces their local contributions $d(v)-c e(G[N(v)])$ to agree. If their [vertex neighbourhoods](graph.md#vertex-neighbourhood) differ, the sum of the two changes in the squared-[degree of a vertex](#degree-graph-theory) objective is twice the size of their symmetric difference, a contradiction. Nonadjacency therefore partitions the [vertices](graph.md#vertex-graph-theory) into classes with identical [vertex neighbourhoods](graph.md#vertex-neighbourhood).

#### Quadratic Turan edge bound

↑ **Parent:** [Turán's theorem](#turan-s-theorem)

Every $n$-vertex graph containing no $K_{r+1}$ satisfies

$$
e(G)\leq\left(1-\frac1r\right)\frac{n^2}{2}.
$$

#### Rhombus-free edge bound

↑ **Parent:** [Turán's theorem](#turan-s-theorem)

A graph-theoretic rhombus is two triangles sharing an edge. Every rhombus-free graph on $n\geq4$ vertices has at most

$$
e(T_2(n))=\left\lfloor\frac{n^2}{4}\right\rfloor
$$

edges. If the graph is triangle-free this is Turán's theorem. Otherwise remove a triangle: every remaining vertex has at most one neighbor in it, and induction bounds the edge count by  
$\lfloor(n-3)^2/4\rfloor+n\leq\lfloor n^2/4\rfloor$.

##### Triangular prism graph

↑ **Parent:** [Rhombus-free edge bound](#rhombus-free-edge-bound)

The triangular prism has six vertices and nine edges. Each edge lies in at most one triangle, so it has no rhombus; its two triangles show that it is not $K_{3,3}=T_2(6)$.

This is the [prism graph](#prism-graph) built from two triangles.

<h3 id="erdos-stone-theorem">Erdős-Stone theorem</h3>

↑ **Parent:** [Extremal graph theory](#extremal-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Erdős-Stone_theorem)

For every graph $H$ with chromatic number $r+1$,

$$
\operatorname{ex}(n,H)=\left(1-\frac1r+o(1)\right)\binom n2.
$$

<h4 id="logarithmic-erdos-stone-theorem">Logarithmic Erdős-Stone theorem</h4>

↑ **Parent:** [Erdős-Stone theorem](#erdos-stone-theorem)

An [edge](#edge-of-a-graph) density exceeding the [Turan theorem](#turan-s-theorem) threshold for $K_{r+1}$ by a fixed positive amount forces a balanced $K_{r+1}(t)$ subgraph with logarithmic part size. Combine [clique supersaturation by sampling](#clique-supersaturation-by-sampling) with the [dense clique family blow-up lemma](graph.md#dense-clique-family-blow-up-lemma). Dense binomial random [graphs](graph.md) show that the logarithmic order is optimal for a uniform density guarantee.

##### Logarithmic clique blow-up from minimum degree

↑ **Parent:** [Logarithmic Erdős-Stone theorem](#logarithmic-erdos-stone-theorem)

A fixed positive excess over the [Turan theorem](#turan-s-theorem) threshold forces logarithmic balanced [complete multipartite graphs](#complete-multipartite-graph). There is an elementary induction using [common neighbourhood from bipartite density](#common-neighbourhood-from-bipartite-density): first obtain a logarithmic $r$-partite subgraph from the induction hypothesis, and select disjoint transversal $r$-cliques in it. Each such clique has at least $r\varepsilon n$ [common neighbours](#common-neighbour), by the [union bound](probability-inequality.md#boole-s-inequality) on non-neighbour sets. Apply the bipartite common-neighbour count to these cliques as left-side objects. Their selected union and a large common neighbourhood form the extra part.

##### Random obstruction to larger clique blow-ups

↑ **Parent:** [Logarithmic Erdős-Stone theorem](#logarithmic-erdos-stone-theorem)

In a [binomial random graph](#binomial-random-graph) with fixed [edge](#edge-of-a-graph) probability below one, the displayed first-moment bound tends to zero for $t=C\log n$ and sufficiently large fixed $C$. At the same time the [edge](#edge-of-a-graph) density concentrates near $p$. Thus a positive fixed density cannot force balanced complete multipartite subgraphs whose part size grows faster than logarithmically.

#### High-minimum-degree multipartite stability subgraph

↑ **Parent:** [Erdős-Stone theorem](#erdos-stone-theorem)

For fixed positive integers $r,t$, a [graph](graph.md) $G$ on $n$ [vertices](graph.md#vertex-graph-theory) with $e(G)=(1-1/r+o(1))n^2/2$ and no [balanced complete multipartite blow-up](#balanced-complete-multipartite-blow-up) $K_{r+1}(t)$ contains an $r$-partite [subgraph](#subgraph) $H$ with $n-o(n)$ [vertices](graph.md#vertex-graph-theory), balanced classes of size $n/r+o(n)$, and [minimum degree of a graph](#minimum-degree-of-a-graph) $\delta(H)=(1-1/r+o(1))n$.

One proof first removes a vanishing fraction of [vertices](graph.md#vertex-graph-theory) of low [degree of a vertex](#degree-graph-theory), finds a slowly growing $K_r(L)$ by the [Erdős-Stone theorem](#erdos-stone-theorem), and assigns almost every remaining [vertex](graph.md#vertex-graph-theory) to a root class in which it has fewer than $t$ [neighbours of a vertex](#neighbour-of-a-vertex). After discarding a further vanishing fraction, a $K_{t,t}$ inside an assigned class would extend to $K_{r+1}(t)$ using the root classes. Thus internal [edges](#edge-of-a-graph) and missing cross-class [edges](#edge-of-a-graph) both number $o(n^2)$. Removing the [vertices](graph.md#vertex-graph-theory) with unusually many missing cross-class [edges](#edge-of-a-graph) gives the stated [minimum degree of a graph](#minimum-degree-of-a-graph).

##### Minimum degree of an extremal forbidden-subgraph graph

↑ **Parent:** [High-minimum-degree multipartite stability subgraph](#high-minimum-degree-multipartite-stability-subgraph)

If a fixed [graph](graph.md) $F$ has [chromatic number](#chromatic-number) $r+1$, every extremal $F$-free [graph](graph.md) $G$ on $n$ [vertices](graph.md#vertex-graph-theory) has [minimum degree of a graph](#minimum-degree-of-a-graph) $(1-1/r+o(1))n$. Use a [high-minimum-degree multipartite stability subgraph](#high-minimum-degree-multipartite-stability-subgraph) $H$: replacing any [vertex](graph.md#vertex-graph-theory) by one adjacent to all but one class of $H$ preserves $F$-freeness. Any supposed new copy of $F$ can replace the new [vertex](graph.md#vertex-graph-theory) by an unused [common neighbour](#common-neighbour) in the omitted class. Extremality therefore gives the lower bound on every [degree of a vertex](#degree-graph-theory); the [Erdős-Stone theorem](#erdos-stone-theorem) gives the upper bound on the average [degree of a vertex](#degree-graph-theory).

<h3 id="kovari-sos-turan-theorem">Kővári–Sós–Turán theorem</h3>

↑ **Parent:** [Extremal graph theory](#extremal-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kővári–Sós–Turán_theorem)

For each fixed positive integer $t$,

$$
\operatorname{ex}(n,K_{t,t})=O\left(n^{2-1/t}\right).
$$

The standard proof counts $t$-element subsets of [graph neighbourhoods](#graph-neighbourhood) in a bipartite subgraph. If one side has degrees $d_y$, the absence of $K_{t,t}$ gives

$$
\sum_y\binom{d_y}{t}\leq(t-1)\binom nt.
$$

[convexity](real-analysis.md#convex-function) then bounds the number of edges.

## Flow network

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flow_network)

A [flow network](#flow-network) is a [directed graph](#directed-graph) $G=(V,E)$ with distinct source and sink [vertices](graph.md#vertex-graph-theory) $s,t$ and a nonnegative [flow network edge capacity](#flow-network-edge-capacity) $c_{uv}$ on each directed [edge](#edge-of-a-graph) $(u,v)$. In the finite setting here, every [flow network edge capacity](#flow-network-edge-capacity) is a finite real number. A [feasible flow](#feasible-flow) assigns a nonnegative amount $f_{uv}$ to each original directed [edge](#edge-of-a-graph), satisfies the [capacity constraints](#capacity-constraint), and obeys [flow conservation](#flow-conservation) at every other [vertex](graph.md#vertex-graph-theory):

$$
0\leq f_{uv}\leq c_{uv},\qquad
\sum_{u:(u,v)\in E}f_{uv}=\sum_{w:(v,w)\in E}f_{vw}\quad(v\notin\{s,t\}).
$$

These are nonnegative arc amounts. The antisymmetric convention in [flow](#flow) instead records net amounts $\theta_{uv}=f_{uv}-f_{vu}$, taking a missing arc amount as zero. The two conventions express the same [flow conservation](#flow-conservation); keeping them distinct makes backward [residual network](#residual-network) [edges](#edge-of-a-graph) easier to interpret.

Think of [vertices](graph.md#vertex-graph-theory) as routers, directed [edges](#edge-of-a-graph) as communication links, [flow network edge capacities](#flow-network-edge-capacity) as available bandwidth, and [flow](#flow) as a steady transmission rate. An intermediate router can distribute incoming traffic among outgoing links, but [flow conservation](#flow-conservation) prevents it from creating traffic. The [maximum flow problem](#maximum-flow-problem) asks how much total traffic can pass from $s$ to $t$, allowing several [graph paths](#path-in-a-graph) to share the work. The same [flow network](#flow-network) language models transportation and abstract resource allocation.[Goemans, Network flows, introduction and maximum flow formulation](https://ocw.mit.edu/courses/6-854j-advanced-algorithms-fall-2008/4064d889e5033a9915327a777d12b592_notes_flow.pdf)

Our running [flow network](#flow-network) has [vertices](graph.md#vertex-graph-theory) $V=\{s,a,b,t\}$ and exactly five directed [edges](#edge-of-a-graph), with [flow network edge capacities](#flow-network-edge-capacity)

$$
(c_{sa},c_{sb},c_{ab},c_{at},c_{bt})=(3,2,1,2,3).
$$

The cross [edge](#edge-of-a-graph) $a\to b$ lets traffic entering $a$ use spare capacity on $b\to t$. With this [edge](#edge-of-a-graph) removed, the two separate [graph paths](#path-in-a-graph) can carry only $\min(3,2)+\min(2,3)=4$; including it will let the [maximum flow](#maximum-flow-problem) reach $5$. Thus a link's usefulness depends on the rest of the [flow network](#flow-network), rather than just its own [flow network edge capacity](#flow-network-edge-capacity).

### Circulation in a flow network

↑ **Parent:** [Flow network](#flow-network)

A [network circulation](#circulation-in-a-flow-network) is a [flow](#flow) with zero net supply at every vertex. A feasible residual [network circulation](#circulation-in-a-flow-network) changes one feasible flow into another with the same prescribed supplies. It decomposes into directed cycles, giving the negative-cycle optimality test for [minimum-cost flow](#minimum-cost-flow-problem).

### Vertex capacity

↑ **Parent:** [Flow network](#flow-network)

An internal vertex capacity bounds the total [flow](#flow) through that vertex, equivalently its total inflow or outflow by [flow conservation](#flow-conservation). Replace the vertex by an input and output vertex, direct incoming edges to the input and outgoing edges from the output, and connect input to output with an edge of the vertex capacity. This converts the constraint into an ordinary [flow network edge capacity](#flow-network-edge-capacity).

### Maximum flow problem

↑ **Parent:** [Flow network](#flow-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_flow_problem)

The [maximum flow problem](#maximum-flow-problem) maximises the [strength of a flow](#strength-of-a-flow) from a source to a sink subject to [flow conservation](#flow-conservation) and [flow network edge capacities](#flow-network-edge-capacity). For the nonnegative arc amounts used in [flow network](#flow-network), its objective is net outflow from the source:

$$
|f|=\sum_{v:(s,v)\in E}f_{sv}-\sum_{u:(u,s)\in E}f_{us}
=\sum_{u:(u,t)\in E}f_{ut}-\sum_{v:(t,v)\in E}f_{tv}.
$$

The equality follows by summing [flow conservation](#flow-conservation) over all internal [vertices](graph.md#vertex-graph-theory). Incoming source [flow](#flow) must be subtracted: merely circulating traffic through $s$ does not deliver more to $t$. The [max-flow min-cut theorem](#max-flow-min-cut-theorem) identifies the optimum with the least [cut capacity](#cut-capacity) of a [cut of a flow network](#cut-of-a-flow-network). A [feasible flow](#feasible-flow) and a [cut of a flow network](#cut-of-a-flow-network) of equal value certify optimality without requiring a particular choice of [augmenting paths](#augmenting-path).

For the five-[edge](#edge-of-a-graph) [flow network](#flow-network) with [flow network edge capacities](#flow-network-edge-capacity) $(3,2,1,2,3)$, take

$$
(f_{sa},f_{sb},f_{ab},f_{at},f_{bt})=(3,2,1,2,3).
$$

Every [capacity constraint](#capacity-constraint) holds with equality. [Flow conservation](#flow-conservation) at $a$ is $3=1+2$, and at $b$ it is $2+1=3$. The [strength of a flow](#strength-of-a-flow) is $|f|=3+2=5$, also $2+3=5$ entering $t$. This [flow](#flow) consists of $2$ units on the [graph path](#path-in-a-graph) $s\to a\to t$, $2$ on $s\to b\to t$, and $1$ on $s\to a\to b\to t$. The [cut of a flow network](#cut-of-a-flow-network) with source side $\{s\}$ has [cut capacity](#cut-capacity) $3+2=5$, so no [feasible flow](#feasible-flow) can do better.

Even a seemingly poor first [augmenting path](#augmenting-path) $s\to a\to b\to t$, carrying $1$, does not cause failure in this example. It leaves [residual network](#residual-network) capacity $2$ along $s\to a\to t$ and $2$ along $s\to b\to t$. These two subsequent [augmenting paths](#augmenting-path) yield values $1$, $3$, and $5$, and produce exactly the [flow](#flow) above. Backward [residual network](#residual-network) [edges](#edge-of-a-graph) become essential in the unit-capacity example under [residual network](#residual-network), where this same first choice blocks every unused forward route.

Discrete assignment is another reason to study [maximum flow](#maximum-flow-problem). Put unit-capacity [edges](#edge-of-a-graph) from $s$ to job [vertices](graph.md#vertex-graph-theory), from each job to eligible worker [vertices](graph.md#vertex-graph-theory), and from workers to $t$. An integral [flow](#flow) selects a [matching in a graph](#matching-graph-theory): each job and worker participates at most once, and the [strength of a flow](#strength-of-a-flow) counts assigned jobs. The [integral max-flow theorem](#integral-max-flow-theorem) therefore turns maximum cardinality assignment into [maximum flow](#maximum-flow-problem). Minimizing assignment costs is the related [assignment problem](mathematical-optimization.md#assignment-problem), modeled by [minimum-cost flow](#minimum-cost-flow-problem).[Goemans, Network flows, assignment formulation](https://ocw.mit.edu/courses/6-854j-advanced-algorithms-fall-2008/4064d889e5033a9915327a777d12b592_notes_flow.pdf)

#### Sports elimination by maximum flow

↑ **Parent:** [Maximum flow problem](#maximum-flow-problem)

For a league in which every remaining game gives exactly one win, first give the target team all its remaining wins, obtaining $W$. Make a node for each unordered pair of other teams, with source capacity equal to their remaining games. Route each game-node flow to one of its two teams, and cap the team's total additional wins at $W-w_i-1$ for a strict target victory. A negative cap immediately rules out success. Otherwise an integral [maximum flow](#maximum-flow-problem) saturating every game-source arc specifies the winners of all games and proves feasibility. Each actual game is counted once; duplicating ordered pairs changes the problem.

#### Treatment capacity as a sink arc

↑ **Parent:** [Maximum flow problem](#maximum-flow-problem)

In a [flow network](#flow-network) for treatment facilities, the amount treated at a facility is represented by a directed arc from it to the sink, with that arc's capacity equal to its treatment limit. Untreated fluid may pass through the facility independently of how much is treated there. Thus the treatment limit is not a bound on total incoming flow. [Flow conservation](#flow-conservation) at a facility equates incoming flow with outgoing untreated flow plus its sink-arc flow.

#### Server connectivity under component failures

↑ **Parent:** [Maximum flow problem](#maximum-flow-problem)

To find the smallest link failure set separating a client from every server, add a common sink with sufficiently large-capacity server arcs and give original links unit capacities in both directions. The [max-flow min-cut theorem](#max-flow-min-cut-theorem) identifies the minimum failure count $\lambda$. Unit-capacity [vertex splitting](#vertex-splitting) also charges intermediary node failures. The network tolerates fewer than $\lambda$ failures and fails for some set of $\lambda$ failures. This concerns connection to at least one server, not separate connectivity to each server.

<h4 id="edmonds-karp-algorithm">Edmonds–Karp algorithm</h4>

↑ **Parent:** [Maximum flow problem](#maximum-flow-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edmonds–Karp_algorithm)

This [maximum flow](#maximum-flow-problem) algorithm repeatedly augments along a shortest residual path found by [breadth-first search](combinatorics.md#breadth-first-search). Residual distances from the source never decrease. If the same arc becomes saturated again after being restored by a reverse augmentation, the distance to its tail has increased by at least two. Thus each arc is critical only $O(|V|)$ times, yielding $O(|V||E|)$ augmentations. Each search costs $O(|E|)$, so the total time is $O(|V||E|^2)$. Termination with no residual source-sink path supplies a [max-flow min-cut theorem](#max-flow-min-cut-theorem) certificate.

#### Maximum flow with vertex capacities

↑ **Parent:** [Maximum flow problem](#maximum-flow-problem)

The [maximum flow problem](#maximum-flow-problem) with internal [vertex capacities](#vertex-capacity) reduces to the usual edge-capacitated problem by splitting each constrained vertex into input and output copies. The connecting edge carries its entire through-flow. Feasible flows correspond under this construction, preserving the source-to-sink value; the [Ford-Fulkerson algorithm](#ford-fulkerson-algorithm) and [max-flow min-cut theorem](#max-flow-min-cut-theorem) therefore apply to the transformed network.

##### Vertex splitting

↑ **Parent:** [Maximum flow with vertex capacities](#maximum-flow-with-vertex-capacities)

Replace a vertex $v$ by $v_{\rm in},v_{\rm out}$ and an arc between them carrying its vertex capacity. Incoming arcs enter $v_{\rm in}$ and outgoing arcs leave $v_{\rm out}$. A path must cross that internal arc to use the vertex. This converts node-capacitated [maximum flow](#maximum-flow-problem) to an ordinary [flow network](#flow-network). For undirected mixed-failure cuts, normalize the source side so $v_{\rm out}$ inside implies $v_{\rm in}$ inside; then each original link contributes at most one crossing orientation.

### Flow network edge capacity

↑ **Parent:** [Flow network](#flow-network)

A directed edge capacity is the upper bound $c_{ij}\geq0$ on the feasible nonnegative [flow](#flow) through that edge. In a [residual network](#residual-network), its forward residual capacity is $c_{ij}-f_{ij}$ and its backward residual capacity is $f_{ij}$. Increasing every edge capacity need not increase the [maximum flow](#maximum-flow-problem) by that same amount, because a [cut of a flow network](#cut-of-a-flow-network) can contain several edges.

### Capacity constraint

↑ **Parent:** [Flow network](#flow-network)

If a directed edge $e$ has capacity $c(e)$, a feasible flow satisfies $0\leq f(e)\leq c(e)$. In an antisymmetric-flow convention, this is encoded together with the residual capacity of the reverse orientation.

### Cut of a flow network

↑ **Parent:** [Flow network](#flow-network)

An source-to-sink cut is a partition $(A,V\setminus A)$ with the source in $A$ and the sink outside $A$. Its capacity is the sum of the capacities of directed edges leaving $A$.

#### Minimum cut

↑ **Parent:** [Cut of a flow network](#cut-of-a-flow-network)

A [cut of a flow network](#cut-of-a-flow-network) of minimum [cut capacity](#cut-capacity) among cuts separating the prescribed source and sink. The [max-flow min-cut theorem](#max-flow-min-cut-theorem) identifies this capacity with the maximum possible [flow](#flow) value.

##### Diagonal cut in a nearest-neighbour lattice flow

↑ **Parent:** [Minimum cut](#minimum-cut)

On $\{0,\ldots,m\}^2$, give an adjacent edge capacity equal to the larger endpoint distance $|i_1-i_2|$ from the diagonal. The set $S=\{i_1<i_2\}$ has $2m$ outgoing edges: two at each interior diagonal vertex and one at each endpoint. Every such edge has capacity one. Thus any [flow](#flow) from above to below the diagonal is at most $2m$; a feasible path decomposition attaining this value certifies optimality by [weak duality](mathematical-optimization.md#weak-duality).

#### Cut capacity

↑ **Parent:** [Cut of a flow network](#cut-of-a-flow-network)

The sum of arc capacities directed from the source side to the sink side of a [cut of a flow network](#cut-of-a-flow-network).

### Flow

↑ **Parent:** [Flow network](#flow-network)

A flow is an antisymmetric function on directed edges whose [divergence of a flow](#divergence-of-a-flow) vanishes away from designated sources and sinks.

#### Unit flow

↑ **Parent:** [Flow](#flow)

A unit flow from $a$ to $b$ is an antisymmetric [flow](#flow) with net outward [strength of a flow](#strength-of-a-flow) one at $a$, net inward strength one at $b$, and zero [divergence of a flow](#divergence-of-a-flow) elsewhere. For a unit flow to infinity, only the finite source has nonzero divergence.

#### Divergence of a flow

↑ **Parent:** [Flow](#flow)

The divergence of a flow at a vertex is its total outward flow. Flow conservation means that this divergence vanishes at every interior vertex.

##### Flow conservation

↑ **Parent:** [Divergence of a flow](#divergence-of-a-flow)

Flow conservation requires total inflow to equal total outflow at every vertex other than the source and sink, equivalently $\operatorname{div}f=0$ there.

#### Strength of a flow

↑ **Parent:** [Flow](#flow)

The strength of a source-to-sink flow is the net amount leaving the source, equivalently the net amount entering the sink.

#### Energy of a flow

↑ **Parent:** [Flow](#flow)

For unit edge resistances, the energy of a flow is

$$
\mathcal E(\theta)=\sum_e\theta(e)^2,
$$

where every unoriented edge is counted once.

##### Finite-energy flow criterion for transience

↑ **Parent:** [Energy of a flow](#energy-of-a-flow)

An infinite locally finite connected graph is a [transient graph](markov-process.md#transient-graph) exactly when it supports a unit flow from a vertex to infinity with finite [energy of a flow](#energy-of-a-flow).

### Max-flow min-cut theorem

↑ **Parent:** [Flow network](#flow-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Max-flow_min-cut_theorem)

For a finite [flow network](#flow-network) with finite nonnegative real [flow network edge capacities](#flow-network-edge-capacity), the greatest [strength of a flow](#strength-of-a-flow) of a [feasible flow](#feasible-flow) equals the least [cut capacity](#cut-capacity) of a source-to-sink [cut of a flow network](#cut-of-a-flow-network):

$$
\max_{f\text{ feasible}}|f|
=\min_{S\subseteq V:\,s\in S,\,t\notin S}
\sum_{(u,v)\in E:\,u\in S,\,v\notin S}c_{uv}.
$$

For a [maximum flow](#maximum-flow-problem), the [vertices](graph.md#vertex-graph-theory) reachable from the source in the [residual network](#residual-network) define a [minimum cut](#minimum-cut) whose outgoing original [edges](#edge-of-a-graph) are saturated and whose incoming original [edges](#edge-of-a-graph) carry zero [flow](#flow).[Karger, MIT 6.854 Notes 6, maximum-flow optimality conditions](https://courses.csail.mit.edu/6.854/21/Notes/n06-flow.html)

Why is a [cut of a flow network](#cut-of-a-flow-network) an upper bound? Sum [flow conservation](#flow-conservation) on its source side $S$. Internal [edge](#edge-of-a-graph) contributions cancel, leaving

$$
|f|=\sum_{(u,v)\in E:\,u\in S,\,v\notin S}f_{uv}
-\sum_{(u,v)\in E:\,u\notin S,\,v\in S}f_{uv}
\leq\sum_{(u,v)\in E:\,u\in S,\,v\notin S}c_{uv}
=c(S,V\setminus S).
$$

Only directed [edges](#edge-of-a-graph) leaving $S$ contribute to [cut capacity](#cut-capacity). Directed [edges](#edge-of-a-graph) entering $S$ are subtracted in net [flow](#flow), so adding their capacities to the upper bound would lose the intended bottleneck. This inequality is [weak duality](mathematical-optimization.md#weak-duality); the theorem says the bound is attained, an instance of [strong duality](mathematical-optimization.md#strong-duality). Its beauty is that a routing plan and a separating boundary independently witness each other's optimality.

In the running [flow network](#flow-network), the two internal [vertices](graph.md#vertex-graph-theory) give four possible source sides. For $S=\{s\}$, the [cut capacity](#cut-capacity) is $c_{sa}+c_{sb}=3+2=5$. For $S=\{s,a\}$ it is $c_{sb}+c_{ab}+c_{at}=2+1+2=5$. For $S=\{s,b\}$ it is $c_{sa}+c_{bt}=3+3=6$; the incoming [edge](#edge-of-a-graph) $a\to b$ contributes nothing to that [cut capacity](#cut-capacity). Finally, $S=\{s,a,b\}$ gives $c_{at}+c_{bt}=2+3=5$. Thus the [minimum cut](#minimum-cut) has [cut capacity](#cut-capacity) $5$, matching the explicitly computed [maximum flow](#maximum-flow-problem).

<a id="image-maximum-flow-of-value-five-and-two-minimum-cut-certificates"></a>
![](max-flow-cut-certificate.png)

**[Figure 26](#image-maximum-flow-of-value-five-and-two-minimum-cut-certificates). Maximum flow of value five and two minimum-cut certificates**. Labels show flow/capacity on each directed edge. The shaded source sides give cuts of capacities three plus two and two plus one plus two, both equal to the flow value.

Ford and Fulkerson's 1956 paper opens with a railway-capacity question attributed there to T. Harris and proves a minimal-cut theorem as Theorem 1. Its original formulation uses [graph paths](#path-in-a-graph) carrying nonnegative amounts; the [residual reachability certificate for maximum flow](#residual-reachability-certificate-for-maximum-flow) below gives the finite directed [flow network](#flow-network) proof used here.[Ford and Fulkerson, Maximal Flow Through a Network, Canadian Journal of Mathematics 8 (1956), pp. 399–404](https://doi.org/10.4153/CJM-1956-045-5)

#### Residual reachability certificate for maximum flow

↑ **Parent:** [Max-flow min-cut theorem](#max-flow-min-cut-theorem)

In a finite [flow network](#flow-network), a [maximum flow](#maximum-flow-problem) exists because the [feasible flow](#feasible-flow) set contains the zero [flow](#flow) and is a [compact set](topology.md#compact-space): the [capacity constraints](#capacity-constraint) bound every coordinate, and they and [flow conservation](#flow-conservation) define a [closed set](topology.md#closed-set). The [strength of a flow](#strength-of-a-flow) is a [continuous function](calculus.md#continuous-function), so the [extreme value theorem](real-analysis.md#extreme-value-theorem) gives an attained maximum. An [augmenting path](#augmenting-path) in the [residual network](#residual-network) would permit positive augmentation, contradicting maximality. The source-reachable [vertices](graph.md#vertex-graph-theory) in the [residual network](#residual-network) therefore define a [cut of a flow network](#cut-of-a-flow-network) whose outgoing original [edges](#edge-of-a-graph) are saturated and incoming original [edges](#edge-of-a-graph) carry zero [flow](#flow). [Flow conservation](#flow-conservation) makes the [strength of a flow](#strength-of-a-flow) equal to this [cut capacity](#cut-capacity), proving the [max-flow min-cut theorem](#max-flow-min-cut-theorem).

Existence and [strong duality](mathematical-optimization.md#strong-duality) for finite real [flow network edge capacities](#flow-network-edge-capacity) do not imply finite termination for every choice of [augmenting paths](#augmenting-path) in the [Ford-Fulkerson algorithm](#ford-fulkerson-algorithm). With irrational capacities, some choices can continue forever. With integer capacities, [Integrality of the Ford-Fulkerson algorithm](#integrality-of-the-ford-fulkerson-algorithm) instead forces finite termination; rational capacities reduce to that case by a common denominator. Choosing shortest [augmenting paths](#augmenting-path) as in the [Edmonds–Karp algorithm](#edmonds-karp-algorithm) avoids dependence on capacity magnitudes.[Karger, MIT 6.854 Notes 6, section 2.1, rational and real capacities](https://courses.csail.mit.edu/6.854/21/Notes/n06-flow.html)

#### Uniform capacity perturbation of a flow network

↑ **Parent:** [Max-flow min-cut theorem](#max-flow-min-cut-theorem)

If every directed edge capacity increases by $\varepsilon$, a [cut of a flow network](#cut-of-a-flow-network) with $m(S)$ outgoing edges gains $\varepsilon m(S)$. By the [max-flow min-cut theorem](#max-flow-min-cut-theorem), the new [maximum flow](#maximum-flow-problem) value is

$$
v(\varepsilon)=\min_{S:s\in S,\,t\notin S}\bigl(c(S)+\varepsilon m(S)\bigr).
$$

For a finite [flow network](#flow-network), this is a nondecreasing concave piecewise-linear function, and its active cut can change as $\varepsilon$ varies. Two unit-capacity edge-disjoint two-edge source-to-sink paths gain $2\varepsilon$, refuting an invariably exact $\varepsilon$ increase. If there is a directed source-to-sink path, every cut has at least one outgoing edge and the increase is at least $\varepsilon$; without a path it can be zero.

#### Integral max-flow theorem

↑ **Parent:** [Max-flow min-cut theorem](#max-flow-min-cut-theorem)

A flow network with integer capacities has a maximum flow whose value on every edge is an integer. The augmenting-path algorithm proves this because every augmentation preserves integrality.

<h4 id="konig-s-theorem-graph-theory">Kőnig's theorem (graph theory)</h4>

↑ **Parent:** [Max-flow min-cut theorem](#max-flow-min-cut-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kőnig's_theorem_(graph_theory))

In a finite bipartite graph, the maximum size of a matching equals the minimum size of a vertex cover. It follows by representing matching as an integral flow and vertex covers as finite-capacity cuts.

#### Residual network

↑ **Parent:** [Max-flow min-cut theorem](#max-flow-min-cut-theorem)

For a [feasible flow](#feasible-flow) $f$, each original directed [edge](#edge-of-a-graph) $u\to v$ supplies a forward [residual network](#residual-network) [edge](#edge-of-a-graph) of capacity $c_{uv}-f_{uv}$ and a backward one $v\to u$ of capacity $f_{uv}$; zero-capacity residual [edges](#edge-of-a-graph) may be omitted. The forward [edge](#edge-of-a-graph) permits an increase, while the backward [edge](#edge-of-a-graph) permits cancellation of existing [flow](#flow). In particular, backward residual capacity is the amount already sent, rather than unused original capacity. If both original orientations exist, keep their residual contributions separate, or add capacities for contributions with the same direction. An [augmenting path](#augmenting-path) uses these permitted changes while preserving [flow conservation](#flow-conservation) and the [capacity constraints](#capacity-constraint).

To see why cancellation matters, give all five directed [edges](#edge-of-a-graph) $s\to a$, $s\to b$, $a\to b$, $a\to t$, $b\to t$ unit [flow network edge capacities](#flow-network-edge-capacity). Starting from zero [flow](#flow), an [augmenting path](#augmenting-path) $s\to a\to b\to t$ carrying $1$ yields

$$
(f_{sa},f_{sb},f_{ab},f_{at},f_{bt})=(1,0,1,0,1),\qquad |f|=1.
$$

The remaining unused original [edges](#edge-of-a-graph) are $s\to b$ and $a\to t$, which do not form a source-to-sink [graph path](#path-in-a-graph). However, the backward residual [edge](#edge-of-a-graph) $b\to a$ has capacity $f_{ab}=1$. Consequently the [residual network](#residual-network) contains the [augmenting path](#augmenting-path) $s\to b\to a\to t$, with residual capacities $1,1,1$.

Augment by $1$: increase $f_{sb}$ and $f_{at}$ from $0$ to $1$, and decrease $f_{ab}$ from $1$ to $0$. The result is

$$
(f_{sa},f_{sb},f_{ab},f_{at},f_{bt})=(1,1,0,1,1),\qquad |f|=2.
$$

Now [flow conservation](#flow-conservation) is $1=0+1$ at $a$ and $1+0=1$ at $b$. The final [flow](#flow) sends one unit along each of $s\to a\to t$ and $s\to b\to t$. The [cut of a flow network](#cut-of-a-flow-network) $S=\{s\}$ has [cut capacity](#cut-capacity) $1+1=2$, proving this is a [maximum flow](#maximum-flow-problem). Traversing $b\to a$ in the [residual network](#residual-network) revised the earlier routing decision; it did not send actual traffic along a nonexistent original [edge](#edge-of-a-graph).

<a id="image-backward-residual-capacity-reroutes-the-first-unit-of-flow"></a>
![](residual-flow-rerouting.png)

**[Figure 27](#image-backward-residual-capacity-reroutes-the-first-unit-of-flow). Backward residual capacity reroutes the first unit of flow**. Before: one unit follows s to a to b to t. Middle: the residual augmenting path s to b to a to t cancels flow on a to b. After: two units use the separate paths, and the middle original edge carries zero flow.

##### Residual maximum flow is the remaining optimality gap

↑ **Parent:** [Residual network](#residual-network)

For an undirected capacitated network, write the net edge flow as $y_{ij}=-y_{ji}$, and the directed residual capacity as $c_{ij}-y_{ij}$. On every source–sink cut, residual capacity is the original cut capacity minus the current net flow value $f$. Taking the minimum over cuts and applying the [max-flow min-cut theorem](#max-flow-min-cut-theorem) to each network gives the displayed remaining-flow identity.

##### Augmenting path

↑ **Parent:** [Residual network](#residual-network)

An [augmenting path](#augmenting-path) is a source-to-sink [graph path](#path-in-a-graph) $P$ of positive capacities in the [residual network](#residual-network). Its bottleneck is $\Delta=\min_{e\in P}c_f(e)>0$. Add $\Delta$ to original [flow](#flow) on forward residual [edges](#edge-of-a-graph) and subtract $\Delta$ on backward residual [edges](#edge-of-a-graph). Each internal [vertex](graph.md#vertex-graph-theory) still satisfies [flow conservation](#flow-conservation), and the bottleneck guarantees every [capacity constraint](#capacity-constraint). The resulting [feasible flow](#feasible-flow) has [strength of a flow](#strength-of-a-flow) $|f|+\Delta$. In the unit-capacity [residual network](#residual-network) example, $\Delta=1$, and the subtraction on $a\to b$ is precisely what allows the value to rise from $1$ to $2$.

###### Widest augmenting path

↑ **Parent:** [Augmenting path](#augmenting-path)

An [augmenting path](#augmenting-path) maximizing the possible increase in flow, namely its smallest [residual network](#residual-network) edge capacity. If the remaining maximum flow is $F>0$ and the original undirected network has $m$ edges, a path has bottleneck at least $F/m$. Otherwise the vertices reachable through arcs of capacity at least $F/m$ define a cut of capacity strictly less than $F$, contradicting the [max-flow min-cut theorem](#max-flow-min-cut-theorem). Only one directed arc per original crossing edge contributes to that cut.

###### Geometric convergence of widest-path augmentation

↑ **Parent:** [Widest augmenting path](#widest-augmenting-path)

Starting from zero flow, a [widest augmenting path](#widest-augmenting-path) increases the current flow by at least $F_k/m$, where $F_k$ is its remaining optimality gap. Therefore $F_{k+1}\leq(1-1/m)F_k$. Integer capacities keep this gap integer, so a gap below one is zero. The method takes $O(m\log f^*)$ augmentations for $f^*\geq2$, or uniformly $O(m\log(1+f^*))$; zero maximum flow requires no augmentation.

###### Ford-Fulkerson algorithm

↑ **Parent:** [Augmenting path](#augmenting-path)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ford-Fulkerson_algorithm)

The Ford-Fulkerson algorithm repeatedly augments a feasible flow along an [augmenting path](#augmenting-path). When no such path remains, the source-reachable vertices in the [residual network](#residual-network) define a cut of capacity equal to the flow value, proving optimality by the [max-flow min-cut theorem](#max-flow-min-cut-theorem).

###### Integrality of the Ford-Fulkerson algorithm

↑ **Parent:** [Ford-Fulkerson algorithm](#ford-fulkerson-algorithm)

Starting from the zero flow with integer capacities, every residual capacity and every augmenting bottleneck is an integer. Each augmentation therefore preserves integer edge flows and raises the flow value by at least one. Since the value is bounded by the total capacity leaving the source, the algorithm terminates after finitely many augmentations with an integral maximum flow.

#### Parametric maximum flow with one source capacity

↑ **Parent:** [Max-flow min-cut theorem](#max-flow-min-cut-theorem)

If one edge leaving the source has capacity $x$, every cut capacity is affine in $x$ with coefficient zero or one. In the 2024 Cambridge Part IB example, cuts of capacities $x+5$ and $14$ are both sharp, giving

$$
\delta^*(x)=\min\{x+5,14\}.
$$

## Eulerian graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eulerian_graph)

An [Eulerian graph](#eulerian-graph) has an [Euler circuit](#euler-circuit): a closed [trail](#trail-in-a-graph) traversing every [edge](#edge-of-a-graph) exactly once. Here the [graph](graph.md) is a finite [undirected graph](#undirected-graph), possibly a [multigraph](graph.md#multigraph) with [self-loops](graph.md#loop-graph-theory). Parallel [edges](#edge-of-a-graph) retain distinct identities, and each [self-loop](graph.md#loop-graph-theory) contributes two to its [vertex degree](#degree-graph-theory). Repeated [vertices](graph.md#vertex-graph-theory) are allowed. This models inspecting every road segment once, even when a junction must be revisited.

For a nonempty set of [edges](#edge-of-a-graph), the [Euler circuit criterion](#euler-circuit-criterion) requires a [connected graph](graph.md#connected-graph) only on the [edge support of a graph](#edge-support-of-a-graph): [isolated vertices](#isolated-vertex) impose no travel requirement. A single [vertex](graph.md#vertex-graph-theory) with a [self-loop](graph.md#loop-graph-theory) and two [vertices](graph.md#vertex-graph-theory) joined by two parallel [edges](#edge-of-a-graph) are both [Eulerian graphs](#eulerian-graph). Neither requires three [vertices](graph.md#vertex-graph-theory). With no [edges](#edge-of-a-graph) and at least one [vertex](graph.md#vertex-graph-theory), we allow the zero-length [trail](#trail-in-a-graph) at that [vertex](graph.md#vertex-graph-theory) as an [Euler circuit](#euler-circuit); the [graph](graph.md) with no [vertices](graph.md#vertex-graph-theory) has no such [walk](#walk-in-a-graph).

The motivating [Seven Bridges of Königsberg](#seven-bridges-of-konigsberg) problem asks for an [Eulerian trail](#eulerian-trail), which need not return to its starting [vertex](graph.md#vertex-graph-theory). In [Leonhard Euler](mathematics.md#leonhard-euler)'s [Solutio problematis ad geometriam situs pertinentis by Leonhard Euler](mathematics-bibliography.md#solutio-problematis-ad-geometriam-situs-pertinentis-by-leonhard-euler), §2 poses the bridge-crossing question and §§4–6 encode land regions by letters. The river's shape drops out: only the connections matter. The paper was written in 1735 and published in 1741, according to the Euler Archive; the journal volume carries the nominal year 1736.[Euler Archive, E53: Solutio problematis ad geometriam situs pertinentis](mathematics-bibliography.md#euler-archive-e53-solutio-problematis-ad-geometriam-situs-pertinentis)

### Edge support of a graph

↑ **Parent:** [Eulerian graph](#eulerian-graph)

For a finite undirected [multigraph](graph.md#multigraph) $G=(V,E)$, its [edge support of a graph](#edge-support-of-a-graph) is the [subgraph](#subgraph) $G_+=(V_+,E)$ with $V_+=\{v\in V:\deg(v)>0\}$. It removes exactly the [isolated vertices](#isolated-vertex), retaining every [edge](#edge-of-a-graph), including [self-loops](graph.md#loop-graph-theory) and parallel [edges](#edge-of-a-graph). When $E\ne\varnothing$, connectivity of this [subgraph](#subgraph) is the relevant condition for an [Eulerian trail](#eulerian-trail) or [Euler circuit](#euler-circuit).

<h3 id="seven-bridges-of-konigsberg">Seven Bridges of Königsberg</h3>

↑ **Parent:** [Eulerian graph](#eulerian-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seven_Bridges_of_Königsberg)

Model the four land regions by [vertices](graph.md#vertex-graph-theory) $A,B,C,D$ and the seven bridges by distinct [edges](#edge-of-a-graph): two $AB$, two $AC$, and one each of $AD,BD,CD$. Their [vertex degrees](#degree-graph-theory) are $(5,3,3,3)$. [Leonhard Euler](mathematics.md#leonhard-euler)'s paper records these connections in §6 and the obstruction in §9; §20 states the zero-or-two odd-region rule. Four odd [vertex degrees](#degree-graph-theory) exclude an [Eulerian trail](#eulerian-trail), even if returning to the starting [vertex](graph.md#vertex-graph-theory) is optional.[§§6, 9, 20](mathematics-bibliography.md#solutio-problematis-ad-geometriam-situs-pertinentis-by-leonhard-euler)

### Eulerian trail

↑ **Parent:** [Eulerian graph](#eulerian-graph)

An [Eulerian trail](#eulerian-trail), also called an [Eulerian path](#eulerian-trail), is a [trail in a graph](#trail-in-a-graph) traversing every [edge](#edge-of-a-graph) exactly once. The name [Eulerian path](#eulerian-trail) does not require a [graph path](#path-in-a-graph): [vertices](graph.md#vertex-graph-theory) may repeat. A [Hamiltonian path](#hamiltonian-path) instead visits every [vertex](graph.md#vertex-graph-theory) exactly once, and may omit [edges](#edge-of-a-graph). An [Eulerian trail](#eulerian-trail) may omit [isolated vertices](#isolated-vertex), so these are different coverage requirements.

For a finite undirected [multigraph](graph.md#multigraph) with at least one [edge](#edge-of-a-graph), allowing [self-loops](graph.md#loop-graph-theory), an [Eulerian trail](#eulerian-trail) exists exactly when the [edge support of a graph](#edge-support-of-a-graph) is a [connected graph](graph.md#connected-graph) and there are zero or two [vertices](graph.md#vertex-graph-theory) of odd [vertex degree](#degree-graph-theory). In the two-odd-[vertex](graph.md#vertex-graph-theory) case they must be the two distinct endpoints; in the zero-odd-[vertex](graph.md#vertex-graph-theory) case every [Eulerian trail](#eulerian-trail) is an [Euler circuit](#euler-circuit). Count a [self-loop](graph.md#loop-graph-theory) twice in the [vertex degree](#degree-graph-theory) but once in the [trail](#trail-in-a-graph), and count each parallel [edge](#edge-of-a-graph) separately.[pp. 1–3, Theorem 1.1.2 and the note about isolated vertices](mathematics-bibliography.md#math-530-graph-theory-combinatorial-mathematics-i-spring-2023/math-530-spring-2023-lecture-6-multigraphs-and-digraphs)

The [parity](quantum-mechanics.md#parity) obstruction is local: each intermediate visit pairs an arriving [edge](#edge-of-a-graph) with a departing [edge](#edge-of-a-graph). Only the distinct endpoints can have an unpaired incidence. The [handshaking lemma](combinatorics.md#degree-sum-formula), $\sum_{v\in V}\deg(v)=2|E|$, also shows that the number of [vertices](graph.md#vertex-graph-theory) with odd [vertex degree](#degree-graph-theory) is even. Sufficiency in the two-endpoint case reduces to the [Euler circuit criterion](#euler-circuit-criterion): add one extra [edge](#edge-of-a-graph) between the odd [vertices](graph.md#vertex-graph-theory), construct an [Euler circuit](#euler-circuit), rotate its record to start with the extra [edge](#edge-of-a-graph), then delete that [edge](#edge-of-a-graph). The remaining [trail](#trail-in-a-graph) has the required endpoints.

For the [Seven Bridges of Königsberg](#seven-bridges-of-konigsberg) [multigraph](graph.md#multigraph), the [vertex degrees](#degree-graph-theory) at $A,B,C,D$ are $(5,3,3,3)$, so no [Eulerian trail](#eulerian-trail) exists. Remove the unique [edge](#edge-of-a-graph) $AD$: the [vertex degrees](#degree-graph-theory) become $(4,3,3,2)$, and a six-[edge](#edge-of-a-graph) [Eulerian trail](#eulerian-trail) runs from $B$ to $C$. Label the parallel [edges](#edge-of-a-graph) $p_1,p_2$ between $A,B$ and $q_1,q_2$ between $A,C$; label $BD$ by $r$ and $CD$ by $s$. A complete record is $B,p_1,A,q_1,C,s,D,r,B,p_2,A,q_2,C$. It revisits $A,B,C$ while using every remaining [edge](#edge-of-a-graph) once.

<a id="image-four-odd-vertex-degrees-forbid-an-eulerian-trail-two-allow-distinct-endpoints-zero-allow-an-euler-circuit"></a>
![](eulerian-degree-parity-multigraphs.png)

**[Figure 28](#image-four-odd-vertex-degrees-forbid-an-eulerian-trail-two-allow-distinct-endpoints-zero-allow-an-euler-circuit). Four odd vertex degrees forbid an Eulerian trail; two allow distinct endpoints; zero allow an Euler circuit**.

### Euler circuit

↑ **Parent:** [Eulerian graph](#eulerian-graph)

An [Euler circuit](#euler-circuit), also called an [Euler tour](#euler-circuit), is an [Eulerian trail](#eulerian-trail) whose final [vertex](graph.md#vertex-graph-theory) equals its initial [vertex](graph.md#vertex-graph-theory). Its length is $|E|$. It can revisit other [vertices](graph.md#vertex-graph-theory), unlike a [Hamiltonian cycle](#hamilton-cycle), which visits each [vertex](graph.md#vertex-graph-theory) once before returning to the start. For a finite undirected [multigraph](graph.md#multigraph) with at least one [edge](#edge-of-a-graph), an [Euler circuit](#euler-circuit) exists exactly when the [edge support of a graph](#edge-support-of-a-graph) is a [connected graph](graph.md#connected-graph) and every [vertex degree](#degree-graph-theory) is even.

For example, let $p,q$ be distinct parallel [edges](#edge-of-a-graph) joining $A,B$, let $\ell$ be a [self-loop](graph.md#loop-graph-theory) at $A$, and add an [isolated vertex](#isolated-vertex) $Z$. Then $(\deg(A),\deg(B),\deg(Z))=(4,2,0)$, and $A,\ell,A,p,B,q,A$ is an [Euler tour](#euler-circuit). The [self-loop](graph.md#loop-graph-theory) supplies one traversal and two incidences; $Z$ need not be visited. Replacing $p,q$ by a single [edge](#edge-of-a-graph) changes both [vertex degrees](#degree-graph-theory) to odd numbers and removes the possibility of an [Euler circuit](#euler-circuit). Thus collapsing parallel [edges](#edge-of-a-graph) can change the answer.

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

**[Figure 29](#image-hierholzer-s-algorithm-inserts-one-closed-trail-into-another-at-their-shared-vertex-using-each-of-six-edges-exactly-once). Hierholzer's algorithm inserts one closed trail into another at their shared vertex, using each of six edges exactly once**.

In the drawing, arrows indicate the chosen traversal direction along undirected [edges](#edge-of-a-graph). The first closed [trail](#trail-in-a-graph) uses $AB,BC,CA$ and the second uses $AD,DE,EA$. Insert the second at the final occurrence of $A$ in $A,B,C,A$, giving $A,B,C,A,D,E,A$. A reader can check consecutive endpoints, closure, and the six distinct [edges](#edge-of-a-graph) directly. With [multigraphs](graph.md#multigraph), perform the same check on [edge](#edge-of-a-graph) identities, since endpoint pairs alone cannot distinguish parallel [edges](#edge-of-a-graph).

<h4 id="hierholzer-s-algorithm">Hierholzer's algorithm</h4>

↑ **Parent:** [Euler circuit criterion](#euler-circuit-criterion)

[Hierholzer's algorithm](#hierholzer-s-algorithm) constructs an [Euler circuit](#euler-circuit) by growing closed [trails](#trail-in-a-graph) along unused [edges](#edge-of-a-graph) and splicing them at shared [vertices](graph.md#vertex-graph-theory), as in the [Euler circuit criterion](#euler-circuit-criterion). Each [edge](#edge-of-a-graph) must have a distinct record. An implementation using [adjacency lists](computer-science.md#adjacency-list), a [stack](computer-science.md#stack-data-structure), and a used flag for each [edge](#edge-of-a-graph) runs in $O(|V|+|E|)$ time, including the connectivity and [vertex degree](#degree-graph-theory) checks. Store both incidences of a [self-loop](graph.md#loop-graph-theory), while marking its single [edge](#edge-of-a-graph) record used only once.

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
ⓦ [Wiki](https://en.wikipedia.org/wiki/Planar_graph)

A [planar graph](#planar-graph) admits at least one [graph drawing](#graph-drawing) in which [edges](#edge-of-a-graph) meet only at common endpoints. This is a property of the abstract [graph](graph.md), not a requirement on every [graph drawing](#graph-drawing). A [plane graph](#plane-graph) specifies one such drawing.[Planar Graphs; Bipartite Matching, slides lec 5f.3 and 5f.12](mathematics-bibliography.md#planar-graphs-bipartite-matching-by-albert-r-meyer-6-042j-lecture-5f)

For example, the [complete graph](#complete-graph) $K_4$ joins every pair of four [vertices](graph.md#vertex-graph-theory), giving six [edges](#edge-of-a-graph). Put its [vertices](graph.md#vertex-graph-theory) at the corners of a square and its diagonals cross. Instead put $A,B,C$ at the corners of a [triangle](geometry-and-topology.md#triangle) and $D$ inside it: the same six [edges](#edge-of-a-graph) $AB,AC,BC,AD,BD,CD$ now meet only at their endpoints. The first [graph drawing](#graph-drawing) obscures planarity; the second proves it. In particular, its [crossing number](#crossing-number) is zero.

<a id="complete-four-vertex-graph-crossing-and-plane-drawings"></a>
![](complete-four-vertex-graph-crossing-and-plane-drawings.png)

**[Figure 30](#complete-four-vertex-graph-crossing-and-plane-drawings). The same complete graph on four vertices drawn with a crossing and with four faces**.

The distinction matters whenever connections must fit on one surface without intersecting. A failed [graph drawing](#graph-drawing) may only need rearrangement, whereas [nonplanarity by edge counts](#nonplanarity-by-edge-counts) proves that every rearrangement fails.

<h3 id="kuratowski-s-theorem">Kuratowski's theorem</h3>

↑ **Parent:** [Planar graph](#planar-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kuratowski's_theorem)

A finite [simple graph](graph.md#simple-graph) is a [planar graph](#planar-graph) if and only if it contains no [graph subdivision](#graph-subdivision) of the [complete graph](#complete-graph) $K_5$ or the [complete bipartite graph](#complete-bipartite-graph) $K_{3,3}$ as a [subgraph](#subgraph); equivalently, neither is a [topological minor](#topological-minor). The easy direction follows by tracing each replacement [graph path](#path-in-a-graph) as one drawn [edge](#edge-of-a-graph). The converse asserts that every failure of planarity contains one of these two patterns.[§4.4, Theorem 4.4.6(iii), printed p. 111](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/planar-graphs-author-hosted-chapter-preview)

[Graph Theory by Reinhard Diestel](mathematics-bibliography.md#graph-theory-by-reinhard-diestel) (Planar Graphs preview, §4.4, Theorem 4.4.6, printed p. 111) dates [Kuratowski's theorem](#kuratowski-s-theorem) to 1930 and the equivalent [graph minor](#graph-minor) characterization to 1937. These dates are that textbook's historical attribution.

### Plane graph

↑ **Parent:** [Planar graph](#planar-graph)

A [plane graph](#plane-graph) is a [planar graph](#planar-graph) with a specified [graph drawing](#graph-drawing) whose [edges](#edge-of-a-graph) meet only at common endpoints, also called an embedding in the [Euclidean plane](geometry-and-topology.md#euclidean-plane). Its [faces of a plane graph](#face-of-a-plane-graph) and [facial boundary walks](#facial-boundary-walk) refer to that embedding. This geometric use of embedding differs from a [graph embedding](#graph-embedding), which maps one abstract [graph](graph.md) into another.

#### Face of a plane graph

↑ **Parent:** [Plane graph](#plane-graph)

A [face of a plane graph](#face-of-a-plane-graph) is a [connected component](geometry-and-topology.md#connected-component) of the [Euclidean plane](geometry-and-topology.md#euclidean-plane) after removing the drawn [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph). Count the [outer face](#outer-face) too. This is the plane counterpart of a [face of a planar map](#face-of-a-planar-map) on the [sphere](geometry-and-topology.md#sphere).[Planar Graphs; Bipartite Matching, slide lec 5f.6, including the outer face](mathematics-bibliography.md#planar-graphs-bipartite-matching-by-albert-r-meyer-6-042j-lecture-5f)

##### Outer face

↑ **Parent:** [Face of a plane graph](#face-of-a-plane-graph)

The [outer face](#outer-face) is the unique unbounded [face of a plane graph](#face-of-a-plane-graph) for a finite [plane graph](#plane-graph). It counts once even though it surrounds the whole [graph drawing](#graph-drawing). A [tree](combinatorics.md#tree-graph-theory) has only this [face of a plane graph](#face-of-a-plane-graph).

##### Facial boundary walk

↑ **Parent:** [Face of a plane graph](#face-of-a-plane-graph)

For a finite [connected graph](graph.md#connected-graph) embedded as a [plane graph](#plane-graph), follow the [edges](#edge-of-a-graph) around a [face of a plane graph](#face-of-a-plane-graph) to obtain a [closed walk](#closed-walk). Count traversals, not distinct [edges](#edge-of-a-graph): a [bridge in a graph](graph.md#bridge-graph-theory) occurs twice along one [facial boundary walk](#facial-boundary-walk). Each [edge](#edge-of-a-graph) contributes two sides in total.[Mathematics for Computer Science, §12.4, Lemma 12.4.1, printed p. 485](mathematics-bibliography.md#mathematics-for-computer-science-by-eric-lehman-and-others)

For the three-[vertex](graph.md#vertex-graph-theory) [graph path](#path-in-a-graph) $A-B-C$, the only [facial boundary walk](#facial-boundary-walk) is $A,B,C,B,A$, of length four. Both [edges](#edge-of-a-graph) are [bridges in a graph](graph.md#bridge-graph-theory); neither is a [graph cycle](#cycle-in-a-graph). Thus a [facial boundary walk](#facial-boundary-walk) need not be a [graph cycle](#cycle-in-a-graph).

### Honeycomb lattice

↑ **Parent:** [Planar graph](#planar-graph)

The honeycomb lattice is the periodic degree-three [planar graph](#planar-graph) consisting of the vertices and edges of a regular hexagonal tiling. It has two vertex classes; every edge joins opposite classes. Its [planar dual graph](#planar-dual-graph) is the [triangular lattice](graph.md#triangular-lattice).

#### Martini lattice

↑ **Parent:** [Honeycomb lattice](#honeycomb-lattice)

The martini lattice is obtained from the [honeycomb lattice](#honeycomb-lattice) by replacing every vertex in one of its two vertex classes by a triangle, attaching its three former incident bonds to the triangle's three vertices. It is a periodic degree-three [planar graph](#planar-graph), with triangular faces and nine-sided faces. Each decorated vertex and its incident bonds is a three-terminal cell with three internal triangle bonds and three terminal spokes. Its independent [bond percolation](bond-percolation.md) threshold is $1/\sqrt2$, as follows from [three-terminal cell partition duality](#three-terminal-cell-partition-duality).

### Four color theorem

↑ **Parent:** [Planar graph](#planar-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Four_color_theorem)

Every finite [planar graph](#planar-graph) has [chromatic number](#chromatic-number) at most four. This stronger theorem is distinct from the elementary [five colour theorem](#five-color-theorem); the latter's [Kempe chain](#kempe-chain) proof does not prove this assertion.

### Five color theorem

↑ **Parent:** [Planar graph](#planar-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Five_color_theorem)

Every finite [planar graph](#planar-graph) admits a proper vertex coloring with at most five colors. [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph) supplies a vertex of degree at most five. Inductively color its deletion. The only obstruction is five differently colored neighbours in cyclic order. If opposite neighbours 1 and 3 are in different two-color components, interchange one component. If they are connected, planarity prevents opposite neighbours 2 and 4 from being connected in their two-color subgraph, and that interchange frees a color instead. This is a [Kempe chain](#kempe-chain) proof.

### Planar map

↑ **Parent:** [Planar graph](#planar-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Planar_map)

A planar map is a [planar graph](#planar-graph) together with a fixed embedding in the [sphere](geometry-and-topology.md#sphere), considered up to orientation-preserving homeomorphism. A rooted planar map has a distinguished oriented edge, which removes most embedding symmetries.

#### Face of a planar map

↑ **Parent:** [Planar map](#planar-map)

A face of a planar map is a connected component of the complement of its embedded graph. Its degree is the number of edge incidences around its boundary, counted with multiplicity, and the sum of all face degrees is twice the number of edges.

#### Rooted planar map

↑ **Parent:** [Planar map](#planar-map)

A rooted planar map is a [planar map](#planar-map) with a distinguished oriented edge called its root edge. Its tail is the root vertex, and the face on a chosen side of the edge may be designated as the root face.

#### Planar quadrangulation

↑ **Parent:** [Planar map](#planar-map)

A planar quadrangulation is a [planar map](#planar-map) in which every face has degree four, with incidences counted with multiplicity. A pointed quadrangulation additionally has a distinguished vertex.

A [squaregraph](#squaregraph) has separate conditions on bounded faces and interior vertex degrees; its outer face need not be quadrilateral.

##### Trivial bijection between planar maps and quadrangulations

↑ **Parent:** [Planar quadrangulation](#planar-quadrangulation)

The trivial bijection sends a rooted [planar map](#planar-map) with $n$ edges to a rooted [planar quadrangulation](#planar-quadrangulation) with $n$ faces. Put one new vertex in each face and, in each corner, connect that face vertex to the incident original vertex. Each original edge then lies inside one quadrangular face; deleting the original edges gives the quadrangulation. The face bipartition recovers the original vertices and hence the inverse map.

### Planar dual graph

↑ **Parent:** [Planar graph](#planar-graph)

A planar dual graph has one vertex in each face of a fixed planar embedding and one dual edge crossing each primal edge.

This is the planar-embedding case of a [dual graph](graph.md#dual-graph).

#### Planar cluster-count identity

↑ **Parent:** [Planar dual graph](#planar-dual-graph)

For a fixed finite plane graph, the complementary dual configuration opens a dual edge exactly when its primal edge is closed. Its components correspond to faces of the spanning open primal graph. The componentwise [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph) gives the displayed identity. The outer face and isolated primal vertices are included; the identity also handles disconnected graphs, bridges and loops.

#### Dual bond percolation

↑ **Parent:** [Planar dual graph](#planar-dual-graph)

In planar [bond percolation](bond-percolation.md), declare a dual edge open exactly when the primal edge it crosses is closed. Independent primal parameter $p$ then gives independent dual parameter $1-p$.

##### Three-terminal cell partition duality

↑ **Parent:** [Dual bond percolation](#dual-bond-percolation)

A planar finite network with three boundary terminals induces one of five connection partitions: all three connected, all three separate, or one connected pair and an isolated third terminal. Put three dual terminals on the intervening boundary arcs. Passing to the [planar dual graph](#planar-dual-graph) interchanges the all-connected and all-separate partitions and permutes the three pair partitions. If the network is symmetric under all terminal permutations, equality $P_3=P_0$ of the first two probabilities makes its whole partition law dual-invariant. Independent cells on a self-dual triangular terminal arrangement then give identical primal and dual coarse connection laws. Infinite connectivity is preserved because cells are uniformly finite. For a [martini lattice](#martini-lattice) cell with six independent bonds of common parameter $p$, $P_3=3p^5-2p^6$ and $P_3-P_0=(2p^2-1)(p^4-3p^3+2p^2+1)$. The unique zero in $[0,1]$ is $1/\sqrt2$.

##### Dual contour bound for a finite planar cluster

↑ **Parent:** [Dual bond percolation](#dual-bond-percolation)

In [bond percolation](bond-percolation.md) on the square lattice, the outer boundary of a finite [percolation cluster](bond-percolation.md#percolation-cluster), after filling its holes, consists of closed bonds. Their crossing edges in the [planar dual graph](#planar-dual-graph) form a connected enclosing contour, and hence belong to a single [dual bond percolation](#dual-bond-percolation) cluster $K$. If $|K|=m$, both its coordinate widths are at most $m-1$, so the enclosed primal cluster contains at most $m^2$ vertices. A contour enclosing the origin also places every vertex of $K$ within distance $m+1$ of the origin. An exponential volume tail for the subcritical [dual bond percolation](#dual-bond-percolation) clusters thus gives a bound $Ce^{-c\sqrt n}$ for a finite primal cluster of size at least $n$.

#### Planar duality for rectangle crossings

↑ **Parent:** [Planar dual graph](#planar-dual-graph)

For a rectangle in a planar lattice, exactly one of an open primal left-to-right crossing and a closed dual top-to-bottom crossing occurs.

##### Exact self-dual rectangle crossing probability

↑ **Parent:** [Planar duality for rectangle crossings](#planar-duality-for-rectangle-crossings)

For the lattice rectangle with [graph vertices](graph.md#vertex-graph-theory) $\{0,\ldots,n\}\times\{0,\ldots,n-1\}$, let $H_n$ be an open left-to-right crossing. Its complementary event is a closed dual top-to-bottom crossing. The dual crossing rectangle has width $n-1$ and height $n$, so rotation and translation identify it with the original rectangle. Boundary [edges](#edge-of-a-graph) along the starting and ending sides do not affect the crossing event. At $p=1/2$ the primal and dual [edge](#edge-of-a-graph) states have identical laws, hence

$$
\mathbb P_{1/2}(H_n)=1-\mathbb P_{1/2}(H_n)=\frac12.
$$

The one-unit adjustment in the side lengths makes the symmetry exact rather than an informal assertion about a finite [graph vertex](graph.md#vertex-graph-theory) square.

### Euler formula for a connected planar graph

↑ **Parent:** [Planar graph](#planar-graph)

For a finite [connected graph](graph.md#connected-graph) with at least one [vertex](graph.md#vertex-graph-theory), embedded as a [plane graph](#plane-graph), let $n$ count [vertices](graph.md#vertex-graph-theory), $m$ count [edges](#edge-of-a-graph), and $f$ count [faces of a plane graph](#face-of-a-plane-graph), including the [outer face](#outer-face). Then

$$
n-m+f=2.
$$

The hypotheses refer to an actual embedding; regions in a crossing-filled [graph drawing](#graph-drawing) do not supply its $f$.[Planar Graphs; Bipartite Matching, slides lec 5f.14–5f.15](mathematics-bibliography.md#planar-graphs-bipartite-matching-by-albert-r-meyer-6-042j-lecture-5f)

In the [plane graph](#plane-graph) $K_4$ pictured above, three bounded [faces of a plane graph](#face-of-a-plane-graph) and the [outer face](#outer-face) give $4-6+4=2$. A square [cycle graph](#cycle-graph) gives $4-4+2=2$, while the [graph path](#path-in-a-graph) $A-B-C$ gives $3-2+1=2$. Changing a crossing into a new [vertex](graph.md#vertex-graph-theory) changes the [graph](graph.md): the square-and-diagonals drawing then has five [vertices](graph.md#vertex-graph-theory), eight [edges](#edge-of-a-graph), and five [faces of a plane graph](#face-of-a-plane-graph), giving $5-8+5=2$.

A proof outline deletes [edges](#edge-of-a-graph) on [graph cycles](#cycle-in-a-graph). Each deletion preserves the [connected graph](graph.md#connected-graph) and merges two [faces of a plane graph](#face-of-a-plane-graph), leaving $n-m+f$ unchanged. Eventually a [tree](combinatorics.md#tree-graph-theory) remains, with $m=n-1$ and $f=1$. Adding the point at infinity identifies the plane picture with a [sphere](geometry-and-topology.md#sphere); the value two agrees with its [Euler characteristic](homology.md#euler-characteristic) and the [cell-count formula for Euler characteristic](homology.md#cell-count-formula-for-euler-characteristic).

#### Small faces of a spherical polyhedral graph

↑ **Parent:** [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph)

For a connected cellular spherical [planar graph](#planar-graph) with vertex degrees at least three and face sizes at least three, degree/face double counting and the [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph) give $\sum_n(6-n)F_n=12+\sum_m(2m-6)V_m\ge12$. The left side is at most $3(F_3+F_4+F_5)$, proving the displayed bound. In particular a convex polyhedron has at least four faces of size at most five.

#### Planar graph edge bound

↑ **Parent:** [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph)

A finite [simple graph](graph.md#simple-graph) that is a [connected graph](graph.md#connected-graph) and a [planar graph](#planar-graph), with $n\geq3$ [vertices](graph.md#vertex-graph-theory) and $m$ [edges](#edge-of-a-graph), satisfies $m\leq3n-6$. Choose a [plane graph](#plane-graph): each [facial boundary walk](#facial-boundary-walk) has length at least three, so $3f\leq2m$. Substitute $f=2-n+m$ from the [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph).[Mathematics for Computer Science, §12.4, Lemma 12.4.2 and Theorem 12.4.3, printed pp. 485–486](mathematics-bibliography.md#mathematics-for-computer-science-by-eric-lehman-and-others)

The [complete graph](#complete-graph) $K_4$ attains equality: $6=3\cdot4-6$. The bound also holds for a disconnected finite [simple graph](graph.md#simple-graph) that is a [planar graph](#planar-graph) with $n\geq3$: place its [connected components of a graph](graph.md#component-graph-theory) in disjoint regions and join them with new [bridges in a graph](graph.md#bridge-graph-theory), then apply the connected bound.

##### Bipartite planar graph edge bound

↑ **Parent:** [Planar graph edge bound](#planar-graph-edge-bound)

If a finite [simple graph](graph.md#simple-graph) is a [connected graph](graph.md#connected-graph), a [bipartite graph](#bipartite-graph), and a [planar graph](#planar-graph), with $n\geq3$ [vertices](graph.md#vertex-graph-theory), then $m\leq2n-4$. Every [facial boundary walk](#facial-boundary-walk) has even length and length at least three, hence at least four. Thus $4f\leq2m$; substitute the [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph).[Mathematics for Computer Science, §12.5, Lemma 12.5.2 and Theorem 12.5.3, printed pp. 486–487](mathematics-bibliography.md#mathematics-for-computer-science-by-eric-lehman-and-others)

The square [cycle graph](#cycle-graph) attains equality: $4=2\cdot4-4$. The three-[vertex](graph.md#vertex-graph-theory) [graph path](#path-in-a-graph) also attains equality: $2=2\cdot3-4$. Its repeated [bridges in a graph](graph.md#bridge-graph-theory) illustrate why counting [facial boundary walk](#facial-boundary-walk) length correctly matters. Neither bound applies unchanged to a [multigraph](graph.md#multigraph): two [vertices](graph.md#vertex-graph-theory) may support arbitrarily many parallel [edges](#edge-of-a-graph) in a [plane graph](#plane-graph).

##### Nonplanarity by edge counts

↑ **Parent:** [Planar graph edge bound](#planar-graph-edge-bound)

The [complete graph](#complete-graph) $K_5$ has $n=5$ and $m=\binom52=10$, exceeding the [planar graph edge bound](#planar-graph-edge-bound) $3\cdot5-6=9$. Therefore it is not a [planar graph](#planar-graph). The [complete bipartite graph](#complete-bipartite-graph) $K_{3,3}$ has $n=6$ and $m=3\cdot3=9$. The general bound allows twelve [edges](#edge-of-a-graph), but the [bipartite planar graph edge bound](#bipartite-planar-graph-edge-bound) allows only eight, proving nonplanarity.

<a id="plane-graph-face-counts-and-edge-obstructions"></a>
![](plane-graph-face-counts-and-edge-obstructions.png)

**[Figure 31](#plane-graph-face-counts-and-edge-obstructions). Actual plane-graph face counts compared with impossible face counts for the two complete-graph obstructions**.

These are necessary bounds, not a complete planarity test. For an original counterexample, subdivide every [edge](#edge-of-a-graph) of $K_{3,3}$ once. The resulting [simple graph](graph.md#simple-graph) is a [connected graph](graph.md#connected-graph) with $n=15$, $m=18$, and is [bipartite](#bipartite-graph): put all original [vertices](graph.md#vertex-graph-theory) in one part and all nine new [vertices](graph.md#vertex-graph-theory) in the other. Both inequalities hold, $18\leq39$ and $18\leq26$. Nevertheless, a crossing-free [graph drawing](#graph-drawing) would let us trace each two-[edge](#edge-of-a-graph) [graph path](#path-in-a-graph) as one curve, producing an impossible embedding of $K_{3,3}$. The [graph subdivision](#graph-subdivision) preserves this obstruction. [Kuratowski's theorem](#kuratowski-s-theorem) supplies a stronger characterization than these counts.

#### Planar girth edge bound

↑ **Parent:** [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph)

If every face of a connected planar graph has size at least $g>2$, double-counting edge-face incidences and using Euler's formula gives

$$
e\leq\frac{g(n-2)}{g-2}.
$$

#### Triangle-pentagon planar edge bound

↑ **Parent:** [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph)

Let a connected bridgeless planar graph have $n\ge4$ vertices, $e$ edges, no four-cycle, and $t$ triangular faces. If no edge borders two triangular faces, then

$$
2e\ge3t+5(f-t),
\qquad e\ge3t,
$$

so $f\le8e/15$. The [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph) then gives

$$
e\le\frac{15(n-2)}7.
$$

##### Icosidodecahedral graph

↑ **Parent:** [Triangle-pentagon planar edge bound](#triangle-pentagon-planar-edge-bound)

The icosidodecahedral graph is the skeleton of the [icosidodecahedron](geometry-and-topology.md#icosidodecahedron). It has 30 vertices, 60 edges, 20 triangular faces, and 12 pentagonal faces. Every edge separates a triangle from a pentagon, so it attains equality in the [triangle-pentagon planar edge bound](#triangle-pentagon-planar-edge-bound).

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

Here a loopless [multigraph](graph.md#multigraph) has $v$ [vertices](graph.md#vertex-graph-theory), $e$ [edges](#edge-of-a-graph), and at most $\mu$ parallel [edges](#edge-of-a-graph) per pair. In a minimum-crossing drawing, crossings between incident [edges](#edge-of-a-graph) can be removed by exchanging their initial segments, so every crossing involves four distinct [vertices](graph.md#vertex-graph-theory). For each parallel class choose an [edge](#edge-of-a-graph) with probability $1/\mu$ per [edge](#edge-of-a-graph), with the remaining probability choosing none. Retain [vertices](graph.md#vertex-graph-theory) independently with probability $p$. The sampled [simple graph](graph.md#simple-graph) has expected [edge](#edge-of-a-graph) count $p^2e/\mu$, expected [vertex](graph.md#vertex-graph-theory) count $pv$, and expected crossing count $p^4\operatorname{cr}(G)/\mu^2$. Deleting one [edge](#edge-of-a-graph) per crossing and using the [planar graph edge bound](#planar-graph-edge-bound) gives $p^4\operatorname{cr}(G)/\mu^2\geq p^2e/\mu-3pv$. Choose $p=4\mu v/e$.

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

Let $p$ be [prime](number-theory.md#prime-number) and set $s=2p-2$. If a [bipartite graph](#bipartite-graph) has edge-disjoint [perfect matchings](#perfect-matching) $M_0,\ldots,M_{\sigma-1}$ on nested nonempty [vertex](graph.md#vertex-graph-theory) sets, and $|V(M_{i+s})|>s|V(M_i)|/(s+1)$, then the union of $s+1$ consecutive [matchings in a graph](#matching-graph-theory) has maximum degree at most $2p-1$ and more than $(p-1)|V(M_i)|$ [edges](#edge-of-a-graph). The [prime-regular subgraph from Boolean polynomial constraints](combinatorics.md#prime-regular-subgraph-from-boolean-polynomial-constraints) gives a $p$-regular subgraph. Its [perfect matching](#perfect-matching) decomposition gives a $k$-regular subgraph for every $k\leq p$. If none exists, every $s$ steps shrink the [vertex](graph.md#vertex-graph-theory) set by factor at most $s/(s+1)$, bounding $\sigma$ by a constant times $\log n$.

#### Short-cycle expectation in a uniform regular graph

↑ **Parent:** [Regular graph](#regular-graph)

For fixed $r,\ell\geq3$ and $rn$ even, a prescribed [graph cycle](#cycle-in-a-graph) in the [configuration model](#configuration-model) has two ordered distinct half-edges at each of its vertices. Therefore its expected count is $(n)_\ell[r(r-1)]^\ell/[2\ell\prod_{j=0}^{\ell-1}(rn-2j-1)]$. Conditioning on the chosen cycle leaves degrees $r-2$ at its vertices and $r$ elsewhere; forbid further edges along that cycle. The [bounded-degree pairing avoidance estimate](#bounded-degree-pairing-avoidance-estimate) changes by $o(1)$, so the simplicity probability conditional on the cycle divided by the unconditional probability tends to one. The displayed expectation therefore holds for the uniform [simple graph](graph.md#simple-graph), not just the unconditioned pairing model.

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

An exhaustion of a countable [graph](graph.md) is an increasing [sequence](real-analysis.md#sequence) of finite connected [graph vertex](graph.md#vertex-graph-theory) sets whose union is the whole [graph vertex](graph.md#vertex-graph-theory) set. In a [locally finite graph](#locally-finite-graph), every prescribed finite [graph path](#path-in-a-graph) together with all [graph neighbours](#neighbour-of-a-vertex) of its visited [graph vertices](graph.md#vertex-graph-theory) lies in a sufficiently large exhaustion set. This permits coupling finite-volume and infinite-volume [simple random walks](markov-process.md#simple-random-walk) up to a finite stopping time.

## Cut (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cut_(graph_theory))

A cut is a partition $V=A\sqcup B$ of the vertex set. Its size is the number of edges with one endpoint in each part.

### Edge cutset

↑ **Parent:** [Cut (graph theory)](#cut-graph-theory)

An edge cutset separating two vertices is a set of edges whose removal leaves no [path in a graph](#path-in-a-graph) between those vertices. For a vertex set containing exactly one of the two vertices, its [edge boundary](combinatorics.md#edge-boundary-in-a-graph) is such a cutset.

### Maximum cut

↑ **Parent:** [Cut (graph theory)](#cut-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_cut)

A maximum cut has greatest size among all cuts of a finite graph.

### Random cut lower bound

↑ **Parent:** [Cut (graph theory)](#cut-graph-theory)

Every finite graph with $m$ edges has a [cut of a graph](#cut-graph-theory) of size at least $m/2$, and hence a spanning [bipartite graph](#bipartite-graph) with at least $m/2$ edges. Put each vertex independently on either side with equal probability. Every edge crosses with probability $1/2$, so [linearity of expectation](probability-theory.md#linearity-of-expectation) gives expected cut size $m/2$.

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

and apply [linearity of expectation](probability-theory.md#linearity-of-expectation).

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
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bipartite_graph)

A [bipartite graph](#bipartite-graph) separates its [vertices](graph.md#vertex-graph-theory) into two [independent sets](#independent-set-graph-theory): every [edge](#edge-of-a-graph) goes from one part to the other. Here $G=(V,E)$ is a finite [simple graph](graph.md#simple-graph) and an [undirected graph](#undirected-graph), with no [self-loops](graph.md#loop-graph-theory) and no repeated [edges](#edge-of-a-graph). The two parts $X,Y\subseteq V$ satisfy

$$
X\cap Y=\varnothing,\qquad X\cup Y=V,\qquad \{u,v\}\in E\Longrightarrow (u\in X,\ v\in Y)\ \text{or}\ (u\in Y,\ v\in X).
$$

Thus neither part contains an [edge](#edge-of-a-graph). The parts need not have equal sizes, and some pairs across them may have no [edge](#edge-of-a-graph); requiring every cross pair gives a [complete bipartite graph](#complete-bipartite-graph). The [independent set](#independent-set-graph-theory) and cross-[edge](#edge-of-a-graph) definitions are equivalent.[Section 1.1, printed p. 3, independent vertices; Section 1.6, printed p. 17, bipartite and complete multipartite graphs](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview)

For example, the six-[vertex](graph.md#vertex-graph-theory) [cycle graph](#cycle-graph) $C_6$ with [edges](#edge-of-a-graph) $12,23,34,45,56,61$ has parts $X=\{1,3,5\}$ and $Y=\{2,4,6\}$. Drawing the same [graph](graph.md) as a hexagon or in two columns changes neither its [edges](#edge-of-a-graph) nor its [bipartite](#bipartite-graph) property. An extra [isolated vertex](#isolated-vertex) $z$ can go in either part.

<a id="bipartite-graph-independent-parts"></a>
![](bipartite-graph-independent-parts.png)

**[Figure 32](#bipartite-graph-independent-parts). The same six-cycle and isolated vertex drawn as a cycle and as two independent parts**.

We allow either part to be empty. Consequently a [graph](graph.md) with no [edges](#edge-of-a-graph) is [bipartite](#bipartite-graph), even when $V=\varnothing$; choose $X=V$, $Y=\varnothing$. Here "two colours" means two colours are available, with no requirement to use both. This convention explicitly includes the empty case, whereas definitions requiring two nonempty classes need an exception. For several [connected components of a graph](graph.md#component-graph-theory), choose the two parts separately in each [graph component](graph.md#component-graph-theory) and take their [unions](set.md#set-union). In a nonempty [connected graph](graph.md#connected-graph) that is [bipartite](#bipartite-graph), fixing one [vertex](graph.md#vertex-graph-theory)'s colour forces all others along [graph paths](#path-in-a-graph), so its two-colour assignment is unique up to swapping the colours. Each [graph component](graph.md#component-graph-theory), including an [isolated vertex](#isolated-vertex), can be swapped independently.

The [two-colourability criterion for bipartite graphs](#two-colourability-criterion-for-bipartite-graphs) identifies these parts with the colour classes of a [proper vertex colouring](#proper-vertex-coloring): assign colour $0$ to $X$ and colour $1$ to $Y$, so adjacent [vertices](graph.md#vertex-graph-theory) have different colours. More surprisingly, the [odd-cycle characterization of bipartite graphs](#odd-cycle-characterization-of-bipartite-graphs) turns a global requirement into one precise obstruction:

$$
G\text{ is bipartite}\quad\Longleftrightarrow\quad G\text{ contains no odd cycle}.
$$

This statement is for the finite [undirected graph](#undirected-graph) and [simple graph](graph.md#simple-graph) model above; a [graph cycle](#cycle-in-a-graph) has distinct [vertices](graph.md#vertex-graph-theory) except for the repeated starting [vertex](graph.md#vertex-graph-theory). Along a [graph cycle](#cycle-in-a-graph) in a [bipartite graph](#bipartite-graph), colours alternate, so returning to the starting colour takes an [even number](number-theory.md#even-number) of [edges](#edge-of-a-graph). Therefore any [odd cycle](#odd-cycle), whether or not other [edges](#edge-of-a-graph) join its [vertices](graph.md#vertex-graph-theory), prevents a [bipartite](#bipartite-graph) split.[Section 1.6, Proposition 1.6.1 and proof, printed pp. 17–18](mathematics-bibliography.md#graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview)

[Breadth-first search](combinatorics.md#breadth-first-search) supplies the converse constructively. Start an uncoloured [vertex](graph.md#vertex-graph-theory) $s$ with colour $0$, and use a [FIFO queue](computer-science.md#fifo-queue) to explore its [graph component](graph.md#component-graph-theory). When an [edge](#edge-of-a-graph) $uv$ first discovers $v$, give $v$ the opposite colour to $u$, record $u$ as its [parent in a rooted tree](combinatorics.md#parent-in-a-rooted-tree), and enqueue $v$. If both endpoints of any scanned [edge](#edge-of-a-graph) already have the same colour, stop with a conflict. Restart from an uncoloured [vertex](graph.md#vertex-graph-theory) until every [graph component](graph.md#component-graph-theory) has been examined. If no conflict occurs, all [edges](#edge-of-a-graph) cross the two colour classes, which are the required [independent sets](#independent-set-graph-theory).[BipartiteX.java](mathematics-bibliography.md#algorithms-4th-edition-by-robert-sedgewick-and-others/bipartitex-java)

A conflict also explains the failure. In the [rooted tree](combinatorics.md#rooted-tree) produced by [breadth-first search](combinatorics.md#breadth-first-search), let $d(v)$ be the [graph distance](#distance-graph-theory) from $s$. The colour of $v$ is its distance's [integer parity](number-theory.md#parity-mathematics). An [edge](#edge-of-a-graph) $uv$ in an [undirected graph](#undirected-graph) satisfies $|d(u)-d(v)|\leq1$, so equal colours force $d(u)=d(v)$. Follow the two parent chains upward to their [lowest common ancestor](combinatorics.md#lowest-common-ancestor) $w$, discard the shared [graph path](#path-in-a-graph) from $s$ to $w$, and join the remaining two [graph paths](#path-in-a-graph) with the conflict [edge](#edge-of-a-graph) $uv$. The result is a genuine [graph cycle](#cycle-in-a-graph) with

$$
\bigl(d(u)-d(w)\bigr)+\bigl(d(v)-d(w)\bigr)+1=2\bigl(d(u)-d(w)\bigr)+1
$$

[edges](#edge-of-a-graph), an [odd integer](number-theory.md#odd-integer). The two branches have no shared [vertices](graph.md#vertex-graph-theory) except $w$, so this is more than a [closed walk](#closed-walk). This [odd cycle](#odd-cycle) is a certificate that anyone can check directly, using only its listed [vertices](graph.md#vertex-graph-theory) and [edges](#edge-of-a-graph).

<a id="bipartite-graph-odd-cycle-certificate"></a>
![](bipartite-graph-odd-cycle-certificate.png)

**[Figure 33](#bipartite-graph-odd-cycle-certificate). A BFS colour conflict closes a five-cycle; the shared root path is excluded from the certificate**.

In the example, [breadth-first search](combinatorics.md#breadth-first-search) from $s$ gives $d(w)=1$, $d(a)=d(b)=2$, and $d(u)=d(v)=3$. The conflict [edge](#edge-of-a-graph) $uv$ closes the [odd cycle](#odd-cycle) $w,a,u,v,b,w$, with five [edges](#edge-of-a-graph). The common [edge](#edge-of-a-graph) $sw$ is excluded. Thus the same procedure returns either two [independent sets](#independent-set-graph-theory) covering $V$, or an explicit [odd cycle](#odd-cycle). With [adjacency lists](computer-science.md#adjacency-list) and constant-time [FIFO queue](computer-science.md#fifo-queue) operations, its [time complexity](computer-science.md#time-complexity) is $O(|V|+|E|)$ in [Big O notation](real-analysis.md#big-o-notation), with $O(|V|)$ additional storage.[BipartiteX.java](mathematics-bibliography.md#algorithms-4th-edition-by-robert-sedgewick-and-others/bipartitex-java)

The two parts often have a practical meaning: workers and jobs, with an [edge](#edge-of-a-graph) exactly when a worker can perform a job. A [matching in a graph](#matching-graph-theory) chooses compatible worker–job pairs with no reused endpoint; merely being [bipartite](#bipartite-graph) does not guarantee enough compatible pairs. [Hall's marriage theorem](#hall-s-marriage-theorem) characterizes when every worker can be matched, and the [assignment problem](mathematical-optimization.md#assignment-problem) adds costs to seek an optimal assignment. These connections make the [bipartite](#bipartite-graph) structure useful after recognition, as the starting point for selecting [edges](#edge-of-a-graph) under constraints.

### Crown graph

↑ **Parent:** [Bipartite graph](#bipartite-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crown_graph)

A crown graph is a [complete bipartite graph](#complete-bipartite-graph) with a perfect matching removed. For $n\geq2$ it has [chromatic number](#chromatic-number) two, but [greedy coloring](#greedy-coloring) in the order $a_1,b_1,a_2,b_2,\ldots,a_n,b_n$ uses $n$ colors: the matched pair gets the same new color, and every subsequent pair sees all earlier colors.

### Biadjacency matrix

↑ **Parent:** [Bipartite graph](#bipartite-graph)

For a [bipartite graph](#bipartite-graph) with ordered parts $X,Y$, its biadjacency matrix has rows indexed by $X$ and columns indexed by $Y$, with entry one for an [edge](#edge-of-a-graph) and zero otherwise. It has size $|X|$ by $|Y|$, rather than the square full [bipartite adjacency matrix](#bipartite-adjacency-matrix) on $X\sqcup Y$, which is the block [matrix](vector-space.md#matrix) $\left(\begin{smallmatrix}0&M\\M^{\mathsf T}&0\end{smallmatrix}\right)$. Its [singular values](linear-algebra.md#singular-value) describe the [normalized adjacency operator of a bipartite graph](#normalized-adjacency-operator-of-a-bipartite-graph) after division by $\sqrt{|X||Y|}$.

### Normalized adjacency operator of a bipartite graph

↑ **Parent:** [Bipartite graph](#bipartite-graph)

Equip the function spaces of the two nonempty parts of a [bipartite graph](#bipartite-graph) with uniform [inner products](linear-algebra.md#inner-product). Its normalized adjacency operator is $(\theta_Gv)(x)=\mathbb E_yG(x,y)v(y)$. In orthonormal coordinate [bases](vector-space.md#basis), its matrix is $G/\sqrt{|X||Y|}$, not the unscaled adjacency matrix. For a [biregular graph](#biregular-graph) of [edge density of a bipartite graph](probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) $\gamma$, constant functions give a largest [singular value](linear-algebra.md#singular-value) $\gamma$, and the remaining [singular values](linear-algebra.md#singular-value) belong to the centered kernel $G-\gamma$.

### Biregular graph

↑ **Parent:** [Bipartite graph](#bipartite-graph)

A biregular graph is a [bipartite graph](#bipartite-graph) whose vertices have constant degree on each part separately. The two degree constants can differ. If its parts are $X,Y$ and its [edge density of a bipartite graph](probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) is $\gamma$, the two degrees are $\gamma|Y|$ and $\gamma|X|$. Thus its adjacency function has constant row and column averages $\gamma$.

#### Independent-set bound for biregular graphs

↑ **Parent:** [Biregular graph](#biregular-graph)

For a [biregular graph](#biregular-graph) with $m$ left vertices of degree $r$ and $n$ right vertices of degree $s$, let $X$ be the indicator vector of a uniformly selected [independent set](#independent-set-graph-theory). Use base-two [information entropy](information-theory.md#information-entropy). [Shearer inequality](information-theory.md#shearer-s-inequality) gives $H(X_U)\leq r^{-1}\sum_{w\in W}H(X_{N(w)})$. Conditional on $X_U$, each right vertex with an empty selected neighbourhood is an independent fair binary choice, and the other right vertices are forbidden. Writing $q_w=\mathbb P(X_{N(w)}=0)$ gives $H(X)\leq r^{-1}\sum_w[H(X_{N(w)})+rq_w]$. For the $2^s$ neighbourhood patterns, assign weight $2^r$ to the zero pattern and weight one to all others. [Jensen's inequality](real-analysis.md#jensen-s-inequality) implies $H(Y)+rq_w\leq\log_2(2^r+2^s-1)$. Since $n/r=m/s$, the bound follows from $H(X)=\log_2i(G)$. If $s$ divides $m$, the disjoint union of $m/s$ copies of the [complete bipartite graph](#complete-bipartite-graph) $K_{s,r}$ attains equality: each component has $2^s+2^r-1$ [independent sets](#independent-set-graph-theory).

#### Quasirandom bipartite graph

↑ **Parent:** [Biregular graph](#biregular-graph)

For a [biregular graph](#biregular-graph) of [edge density of a bipartite graph](probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) $\gamma$, small rectangular discrepancy, a [box norm](additive-combinatorics.md#box-norm) fourth power close to $\gamma^4$, and a small second [singular value](linear-algebra.md#singular-value) of the [normalized adjacency operator of a bipartite graph](#normalized-adjacency-operator-of-a-bipartite-graph) are equivalent notions of quasirandomness, with quantitative bounds independent of the part sizes. Centering the adjacency function removes the constant singular component.

##### Spectral discrepancy bound for a biregular graph

↑ **Parent:** [Quasirandom bipartite graph](#quasirandom-bipartite-graph)

Let $H=M-\delta J$ be the centered [biadjacency matrix](#biadjacency-matrix) of an equal-part [biregular graph](#biregular-graph), and put $s=\|H\|_{\mathrm{op}}$. For subsets $A,B$ of the two parts, their edge discrepancy is $\mathbf1_A^{\mathsf T}H\mathbf1_B$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) proves the displayed bound. If the part size is $n$, centering the two [indicator vectors](measure-theory.md#indicator-vector) improves it to $s n\sqrt{\alpha(1-\alpha)\beta(1-\beta)}$. The [centered four-cycle identity for a biregular graph](#centered-four-cycle-identity-for-a-biregular-graph) shows that $t_4(G)\leq\delta^4(1+c^4)$ implies $s\leq c\delta n$ for $c\geq0$.

##### Centered four-cycle identity for a biregular graph

↑ **Parent:** [Quasirandom bipartite graph](#quasirandom-bipartite-graph)

For an equal-part [biregular graph](#biregular-graph) with part size $n$ and degree $\delta n$, let $M$ be its [biadjacency matrix](#biadjacency-matrix) and $H=M-\delta J$, where $J$ is the all-ones [matrix](vector-space.md#matrix). The constant row and column sums make $H$ annihilate constants on both sides. Since $MM^{\mathsf T}=\delta^2nJ+HH^{\mathsf T}$ and the two summands have zero products, their squared [matrix trace](linear-algebra.md#matrix-trace) splits as displayed. The [bipartite four-cycle density](probabilistic-combinatorics.md#bipartite-four-cycle-density) counts the squared [matrix trace](linear-algebra.md#matrix-trace) of $MM^{\mathsf T}$ divided by $n^4$.

### Half graph

↑ **Parent:** [Bipartite graph](#bipartite-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Half_graph)

A half graph has two [vertex](graph.md#vertex-graph-theory) classes $X=\{x_1,\ldots,x_n\}$ and $Y=\{y_1,\ldots,y_n\}$, with $x_i$ adjacent to $y_j$ exactly when $i\leq j$. Its nested [vertex neighbourhoods](graph.md#vertex-neighbourhood) give a useful obstruction to partitions in which every pair is a [regular pair of vertex sets](probabilistic-combinatorics.md#regular-pair-of-vertex-sets).

#### Boundary rank obstruction in a half graph

↑ **Parent:** [Half graph](#half-graph)

Partition both sides of a [half graph](#half-graph) into classes of size at least $100$. A class of size $s$ has at most $2\lceil s/10\rceil$ elements with fewer than $s/10$ class elements on one side in the underlying order. If there are $k_X$ and $k_Y$ classes, the union of these boundary elements has size at most $2n/5+2(k_X+k_Y)\leq11n/25$. Some index $m$ is therefore away from both boundaries. The class containing $m$ on each side has at least one tenth of its points strictly above $m$ and strictly below $m$. Choosing lower $X$ points with upper $Y$ points, or upper $X$ points with lower $Y$ points, yields [edge density of a bipartite graph](probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) values one and zero. Both cannot be within $1/10$ of the same class-pair [edge density of a bipartite graph](probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph), so that pair is not a $1/10$-[regular pair of vertex sets](probabilistic-combinatorics.md#regular-pair-of-vertex-sets).

### Odd-cycle characterization of bipartite graphs

↑ **Parent:** [Bipartite graph](#bipartite-graph)

A graph is [bipartite](#bipartite-graph) if and only if it contains no [odd cycle](#odd-cycle). One direction follows because every cycle alternates between the two vertex classes. For the converse, in each [connected component of a graph](graph.md#component-graph-theory) choose a root and partition the vertices according to the parity of their [graph distance](#distance-graph-theory) from it. An edge joining equal parities would close an odd cycle, so every edge crosses the partition.

### Complete bipartite graph

↑ **Parent:** [Bipartite graph](#bipartite-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_bipartite_graph)

The complete bipartite graph $K_{r,s}$ has vertex classes of sizes $r$ and $s$ and contains all $rs$ edges between the classes.

#### Common neighbourhood from bipartite density

↑ **Parent:** [Complete bipartite graph](#complete-bipartite-graph)

If a [bipartite graph](#bipartite-graph) with class sizes $m,N$ has at least $\beta mN$ [edges](#edge-of-a-graph), double count pairs consisting of an $s$-set in the first class and a common neighbour in the second. Convexity of binomial coefficients gives some $S$ with $|N(S)|\ge N\binom{\lfloor\beta m\rfloor}s/\binom ms$. When $s\le\beta m/2$, the quotient is at least $(\beta/2)^s$. This turns density into a large complete bipartite subgraph.

#### Star (graph theory)

↑ **Parent:** [Complete bipartite graph](#complete-bipartite-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Star_(graph_theory))

A star graph is the [complete bipartite graph](#complete-bipartite-graph) with one centre and $m$ leaves. Any pair of its [edges](#edge-of-a-graph) meet at the centre.

### Two-colourability criterion for bipartite graphs

↑ **Parent:** [Bipartite graph](#bipartite-graph)

A finite graph is [bipartite](#bipartite-graph) exactly when it has a proper colouring with two colours. Equivalently,

$$
P_G(2)>0
$$

for its [chromatic polynomial](#chromatic-polynomial).

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

The Sidorenko conjecture states that every [bipartite graph](#bipartite-graph) $H$ satisfies

$$
t(H,G)\geq t(K_2,G)^{|E(H)|}
$$

for every bipartite host graph $G$. Thus a random map is at least as likely to preserve every edge as the heuristic that treats the edge constraints independently predicts.

##### Sidorenko inequality for trees

↑ **Parent:** [Sidorenko conjecture](#sidorenko-conjecture)

Every [tree](combinatorics.md#tree-graph-theory) $T$ satisfies the [Sidorenko conjecture](#sidorenko-conjecture). If a bipartite host graph has edge density $\alpha$, then a uniformly random bipartition-respecting map from a $k$-vertex tree into the host is a [graph homomorphism](#graph-homomorphism) with probability at least $\alpha^{k-1}$.

## Directed graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Directed_graph)

A directed graph consists of [vertices](graph.md#vertex-graph-theory) joined by oriented edges.

### Kernel-perfect directed graph

↑ **Parent:** [Directed graph](#directed-graph)

A [digraph kernel](#kernel-of-a-directed-graph) is an [independent set](#independent-set-graph-theory) $K$ of [vertices](graph.md#vertex-graph-theory) such that each vertex outside $K$ has a [directed edge](#directed-edge) from itself to a vertex in $K$. A [directed graph](#directed-graph) is kernel-perfect if every [induced subgraph](#induced-subgraph) has a [digraph kernel](#kernel-of-a-directed-graph). Preference orientations of the [line graph](#line-graph) of a [bipartite graph](#bipartite-graph) are kernel-perfect: a [stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph) is independent in the line graph, and stability supplies the required outgoing edge at every unmatched edge.

#### Kernel list-coloring lemma

↑ **Parent:** [Kernel-perfect directed graph](#kernel-perfect-directed-graph)

In a [kernel-perfect directed graph](#kernel-perfect-directed-graph), lists of size at least $d^+(v)+1$ admit a proper [graph coloring](#graph-coloring). Choose a color $a$ and a [digraph kernel](#kernel-of-a-directed-graph) in the subgraph on vertices whose lists contain $a$. Color that kernel $a$, delete it, and remove $a$ from the remaining lists. Every vertex losing a color also loses an outgoing neighbour; hence the inequality persists. Induction on the [vertex](graph.md#vertex-graph-theory) count finishes the proof.

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

A closed directed path whose vertices are distinct except for the common start and endpoint is a directed cycle. In a [residual network](#residual-network), augmenting around a directed cycle preserves [flow balance](#flow-balance). A negative total cost on such a cycle gives an improving displacement for a [minimum-cost flow](#minimum-cost-flow-problem).

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

For a $d$-regular undirected [graph](graph.md) whose normalized adjacency [eigenvalues](linear-operator-theory.md#eigenvalue) other than the constant [eigenvalue](linear-operator-theory.md#eigenvalue) have absolute value at most $\rho$, center the indicator vectors of $S,T$. Their constant parts give the expected term $d|S||T|/n$, and the [operator norm](continuous-dual-space.md#operator-norm) on the mean-zero subspace bounds the remaining [inner product](linear-algebra.md#inner-product). Here $e(S,T)=\mathbf1_S^TA\mathbf1_T$ counts oriented incidences, so an [edge](#edge-of-a-graph) within $S\cap T$ is counted twice.

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
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matching_(graph_theory))

A matching is a set of edges with no shared endpoints. It saturates a vertex set when every vertex in that set is incident to one of its edges.

### Stable matching in a bipartite graph

↑ **Parent:** [Matching (graph theory)](#matching-graph-theory)

Give each [vertex](graph.md#vertex-graph-theory) a strict ordering of its [neighbours of a vertex](#neighbour-of-a-vertex), all preferred to being unmatched. A [matching in a graph](#matching-graph-theory) is stable if no unused [edge](#edge-of-a-graph) has both endpoints preferring each other to their current partners, with an unmatched endpoint willing to accept any neighbour. The [Gale-Shapley algorithm](#gale-shapley-algorithm) produces a stable matching even when the two parts have unequal sizes and some pairs are unacceptable.

#### Mutual-worst edge in stable matchings

↑ **Parent:** [Stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph)

If the endpoints of an [edge](#edge-of-a-graph) rank one another last and one [stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph) contains that edge, every stable matching contains it. In the symmetric difference of two stable matchings, preference comparisons propagate along alternating paths: if a vertex prefers its new partner, that partner must prefer its old partner to avoid blocking the old matching. An alternating path cannot end unmatched on the preferred side, so the component is an alternating cycle, on which the two parts prefer opposite matchings. A mutual-worst edge absent from the new matching would make both its endpoints prefer the new matching, contradicting this propagation.

#### Gale-Shapley algorithm

↑ **Parent:** [Stable matching in a bipartite graph](#stable-matching-in-a-bipartite-graph)

An unmatched vertex in the proposing part proposes to its best untried neighbour. The receiving vertex keeps its preferred proposal, rejecting any other. There are at most as many proposals as [edges](#edge-of-a-graph), so this terminates. A rejected proposer can never become preferable to the receiver's final partner, since the receiver's held partner only improves. An edge never proposed along cannot block either: its proposer finishes with a better partner or has exhausted all choices. Thus the final [matching in a graph](#matching-graph-theory) is stable.

### Near-perfect matching

↑ **Parent:** [Matching (graph theory)](#matching-graph-theory)

In a [graph](graph.md) with $2n$ [vertices](graph.md#vertex-graph-theory), a near-perfect [matching in a graph](#matching-graph-theory) has $n-1$ [edges](#edge-of-a-graph) and exactly two unmatched [vertices](graph.md#vertex-graph-theory).

### Matching generating function

↑ **Parent:** [Matching (graph theory)](#matching-graph-theory)

The coefficient $m_k$ counts [matchings in a graph](#matching-graph-theory) with $k$ [edges](#edge-of-a-graph). For a [bipartite graph](#bipartite-graph) with $n$ [vertices](graph.md#vertex-graph-theory) on each side, $m_n$ counts [perfect matchings](#perfect-matching) and equals the [permanent of a matrix](linear-algebra.md#permanent-mathematics) of its bipartite adjacency [matrix](vector-space.md#matrix). Positive activity $\lambda$ makes $Z_G$ the normalizing constant of the [weighted matching Markov chain](markov-process.md#weighted-matching-markov-chain).

#### Annealing ratios for a matching generating function

↑ **Parent:** [Matching generating function](#matching-generating-function)

For $0<a\leq b$, expand the [expectation](probability-theory.md#expected-value) under the [weighted matching Markov chain](markov-process.md#weighted-matching-markov-chain) stationary weights to obtain the displayed identity. If the largest [matching in a graph](#matching-graph-theory) has $n$ [edges](#edge-of-a-graph) and $b/a\leq1+1/n$, the observable lies in $[1,e]$. Its sample mean has controlled error by the [Hoeffding inequality](probability-inequality.md#hoeffding-inequality). A product of $J$ ratios, each estimated to relative accuracy $O(\varepsilon/J)$, approximates the full ratio to relative accuracy $O(\varepsilon)$.

### Augmenting path in a matching

↑ **Parent:** [Matching (graph theory)](#matching-graph-theory)

An augmenting path alternates between edges outside and inside a [matching in a graph](#matching-graph-theory) and joins two unmatched endpoints. Flipping its edges increases the matching size by one. In an assignment equality graph it moves toward a [perfect matching](#perfect-matching) while preserving zero [reduced costs](mathematical-optimization.md#reduced-cost) on matched edges.

#### Short augmenting paths in a dense bipartite graph

↑ **Parent:** [Augmenting path in a matching](#augmenting-path-in-a-matching)

The two sides have $n$ [vertices](graph.md#vertex-graph-theory) each. Given a nonperfect [matching in a graph](#matching-graph-theory), choose unmatched [vertices](graph.md#vertex-graph-theory) $u,v$ on opposite sides. An unmatched [neighbour](#neighbour-of-a-vertex) of either supplies a one-edge [augmenting path in a matching](#augmenting-path-in-a-matching). Otherwise their [neighbours](#neighbour-of-a-vertex) are matched; the matched left [vertices](graph.md#vertex-graph-theory) corresponding to $N(u)$ and the set $N(v)$ have total size greater than $n$, so they intersect. This supplies the alternating [path in a graph](#path-in-a-graph) $u,b,a,v$ with $ab$ in the [matching in a graph](#matching-graph-theory). Repeated augmentation produces a [perfect matching](#perfect-matching).

Choose such an augmentation deterministically. Its reverse is specified by at most four [vertices](graph.md#vertex-graph-theory), giving at most $2n^4$ preimages for a [matching in a graph](#matching-graph-theory) of the next size. Thus the [matching generating function](#matching-generating-function) coefficients satisfy $m_k\leq2n^4m_{k+1}$.

### Perfect matching

↑ **Parent:** [Matching (graph theory)](#matching-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_matching)

A [perfect matching](#perfect-matching) is a [matching in a graph](#matching-graph-theory) that covers every [vertex](graph.md#vertex-graph-theory) exactly once. Its [edges](#edge-of-a-graph) have no shared endpoints, and every [vertex](graph.md#vertex-graph-theory) is an endpoint of one selected [edge](#edge-of-a-graph). It is useful when a collection must be divided into disjoint pairs with no element left over.

In a [bipartite graph](#bipartite-graph) with equally many [vertices](graph.md#vertex-graph-theory) on its two sides, a [perfect matching](#perfect-matching) can assign every person one allowed job and every job one person. The example under [permanent of a matrix](linear-algebra.md#permanent-mathematics) has three people and three jobs, with exactly three valid assignments. The blue [edges](#edge-of-a-graph) below show those three [perfect matchings](#perfect-matching); a crossing in the drawing is not an extra [vertex](graph.md#vertex-graph-theory).

<a id="image-three-perfect-matchings-pair-every-person-vertex-with-one-job-vertex-along-allowed-edges"></a>
![](permanent-perfect-matching-assignments.png)

**[Figure 34](#image-three-perfect-matchings-pair-every-person-vertex-with-one-job-vertex-along-allowed-edges). Three perfect matchings pair every person vertex with one job vertex along allowed edges**.

Every selected [edge](#edge-of-a-graph) covers two [vertices](graph.md#vertex-graph-theory), so a [graph](graph.md) with an [odd integer](number-theory.md#odd-integer) number of [vertices](graph.md#vertex-graph-theory) has no [perfect matching](#perfect-matching). An [even integer](number-theory.md#even-number) number is necessary but does not guarantee existence: an [isolated vertex](#isolated-vertex) cannot be covered. A [perfect matching](#perfect-matching) also need not be unique. For example, the [complete bipartite graph](#complete-bipartite-graph) $K_{2,2}$ has two [perfect matchings](#perfect-matching), corresponding to the two ways of assigning two people to two jobs.

Counting all [perfect matchings](#perfect-matching) is a different question from finding one. For a zero-one [biadjacency matrix](#biadjacency-matrix) of a balanced [bipartite graph](#bipartite-graph), the count is its [permanent of a matrix](linear-algebra.md#permanent-mathematics). The [nonzero determinant criterion for a perfect matching](#perfect-matching-from-a-nonzero-determinant) supplies an existence test, but cancellation means that a zero [determinant](linear-algebra.md#determinant) does not rule one out.

#### Flexible vertex in a balanced bipartite graph

↑ **Parent:** [Perfect matching](#perfect-matching)

A vertex on one side of a balanced [bipartite graph](#bipartite-graph) is flexible if every incident edge lies in a [perfect matching](#perfect-matching). The strict [Hall marriage theorem](#hall-s-marriage-theorem) inequalities for nonempty proper subsets imply flexibility of every vertex: after forcing an edge, removal of its ends loses at most one neighbour from each remaining set. If a perfect matching exists without the strict condition, choose a minimal nonempty tight set. Its induced balanced graph has the strict condition internally, and each internal matching extends using the original matching outside that set. Thus at least one flexible vertex always exists.

#### Minimum-weight perfect matching

↑ **Parent:** [Perfect matching](#perfect-matching)

A minimum-weight [perfect matching](#perfect-matching) pairs every vertex exactly once while minimizing total edge weight. General weighted [perfect matching](#perfect-matching) has polynomial-time algorithms. In the [Christofides algorithm](mathematical-optimization.md#christofides-algorithm), it corrects precisely the odd-degree vertices of a [minimum spanning tree](combinatorics.md#minimum-spanning-tree). Alternating edges of a cyclic order on an even number of vertices give two [perfect matchings](#perfect-matching); the cheaper one costs at most half that cycle's cost.

#### One-factorization

↑ **Parent:** [Perfect matching](#perfect-matching)

A one-factorization partitions every edge of a graph into [perfect matchings](#perfect-matching). Each matching uses every vertex exactly once. A [total of synthemes](combinatorics.md#total-of-synthemes) is precisely a one-factorization of the complete graph on six points.

### Maximal matching

↑ **Parent:** [Matching (graph theory)](#matching-graph-theory)

A matching is maximal when no edge can be added to it, and maximum when no matching has more edges. Every maximum matching is maximal, and the unmatched vertices of a maximal matching form an independent set.

Maximality is a property of a [matching in a graph](#matching-graph-theory), distinct from maximum cardinality.

### Matching number

↑ **Parent:** [Matching (graph theory)](#matching-graph-theory)

The matching number $\nu(G)$ is the largest number of edges in a matching of $G$.

The matching number $\nu(G)$ is the maximum cardinality of a [matching in a graph](#matching-graph-theory).

<h3 id="hall-s-marriage-theorem">Hall's marriage theorem</h3>

↑ **Parent:** [Matching (graph theory)](#matching-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hall's_marriage_theorem)

A bipartite graph has a matching saturating $X$ exactly when $|N(S)|\ge|S|$ for every $S\subseteq X$.

#### Random bipartite matching from empty-rectangle exclusion

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

In the equal-part random [bipartite graph](#bipartite-graph) with fixed edge probability $0<p<1$, rule out empty rectangles of side $\lceil\sqrt n\rceil$ and vertices with at least $n-\lceil\sqrt n\rceil$ nonneighbors. A union bound gives the displayed asymptotic estimate. Small vertex sets satisfy Hall's condition by the degree bound; intermediate sets do so because their omitted-neighbor rectangle would contain a forbidden square; large sets meet every vertex in the other part. Thus [Hall's marriage theorem](#hall-s-marriage-theorem) gives a perfect matching asymptotically almost surely. This does not mean probability one at any finite size.

#### Hall matching of maximal separated sets

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

Two maximum-[cardinality](set-theory.md#cardinality) $\varepsilon$-separated subsets $A,B$ of a [compact metric space](topological-analysis.md#compact-metric-space) have a bijection that moves each point by less than $\varepsilon$. Join $a$ to $b$ when their distance is below $\varepsilon$. If $S\subseteq A$ had fewer than $|S|$ neighbours, replacing these neighbours in $B$ by $S$ would create a larger separated set. The [Hall marriage theorem](#hall-s-marriage-theorem) therefore supplies a [perfect matching](#perfect-matching). This allows empirical averages on a compact [isometry group](riemannian-geometry.md#isometry-group) to be made approximately invariant without assuming a prior [Haar measure](measure-theory.md#haar-measure) construction.

#### Degree-weighted Hall condition

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

In a finite bipartite graph, suppose every left vertex has positive degree and each edge joins vertices with $d(x)\geq d(y)$ from left to right. Then $|N(A)|\geq\sum_{x\in A}\sum_{y\sim x}1/d(y)\geq|A|$, so a matching covers the left side.

#### Measurable Hall theorem

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

For finitely many [Lebesgue measurable sets](measure-theory.md#lebesgue-measurable-set) $A_i\subseteq[0,1]$ and nonnegative demands $b_i$, pairwise disjoint measurable [subsets](set.md#subset) $B_i\subseteq A_i$ with $\lambda(B_i)=b_i$ exist exactly when $\lambda(\bigcup_{i\in I}A_i)\geq\sum_{i\in I}b_i$ for every index [subset](set.md#subset) $I$. Necessity is additivity and monotonicity of [Lebesgue measure](measure-theory.md#lebesgue-measure). For sufficiency, partition the [set union](set.md#set-union) into membership cells $E_J$, send flow from a source through demand vertices $i$ to cells with $i\in J$, then to a sink. Source capacities are $b_i$, cell capacities are $\lambda(E_J)$, and intermediate capacities are $D=\sum_i b_i$. Every [cut of a flow network](#cut-of-a-flow-network) has capacity at least $D$ by the assumed inequalities. The [max-flow min-cut theorem](#max-flow-min-cut-theorem) provides the allocations, and [divisibility of Lebesgue measure](measure-theory.md#divisibility-of-lebesgue-measure) turns each cell allocation into disjoint pieces. If $D=0$, all $B_i$ can simply be empty.

#### Hall induction through a tight set

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

For Hall's theorem, either every proper nonempty set has one excess neighbour and one deletes an arbitrary edge's endpoints, or a tight set $S$ with $|N(S)|=|S|$ splits the problem into the induced graph on $S\cup N(S)$ and its complement.

#### Regular bipartite graph has a perfect matching

↑ **Parent:** [Hall's marriage theorem](#hall-s-marriage-theorem)

In a $k$-regular bipartite graph, edge counting gives equal vertex-class sizes and $k|S|\leq k|N(S)|$. Hall's theorem therefore supplies a perfect matching.

### Regular-graph matching bound from unmatched vertices

↑ **Parent:** [Matching (graph theory)](#matching-graph-theory)

If a $k$-regular graph on $n$ vertices has a maximum matching of size $m$, its unmatched vertices are independent. Counting their incident edges gives $k(n-2m)\leq2(k-1)m$, and hence $m\geq kn/(4k-2)$.

#### Disjoint union of triangles as a sharp matching example

↑ **Parent:** [Regular-graph matching bound from unmatched vertices](#regular-graph-matching-bound-from-unmatched-vertices)

The disjoint union of $r$ triangles is $2$-regular on $3r$ vertices and has matching number $r$, attaining the regular-graph lower bound $n/3$.

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

In a red-blue [edge colouring](#edge-coloring) of $K_n$, let $d_v$ be the red degree of vertex $v$ and let $M$ be the number of [monochromatic](ramsey-theory.md#monochromatic-set) triangles. Every nonmonochromatic triangle has exactly two vertices at which its two incident edges have different colors, so

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

## Random graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_graph)

A random graph is a graph sampled from a probability distribution on graphs.

### Configuration model

↑ **Parent:** [Random graph](#random-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Configuration_model)

For a prescribed [degree sequence](#degree-sequence) with even sum $M=\sum_i d_i$, attach $d_i$ labelled [half-edges](#half-edge-of-a-graph) to [vertex](graph.md#vertex-graph-theory) $i$ and choose a uniform [perfect matching](#perfect-matching) of the $M$ half-edges. Each pair becomes an [edge](#edge-of-a-graph), giving a [multigraph](graph.md#multigraph) that may have [self-loops](graph.md#loop-graph-theory) or parallel edges. The number of pairings is $M!/[2^{M/2}(M/2)!]$. Every [simple graph](graph.md#simple-graph) with that degree sequence has exactly $\prod_i d_i!$ pairing representations, so conditioning on simplicity produces the uniform simple-graph model.

#### Bounded-degree pairing avoidance estimate

↑ **Parent:** [Configuration model](#configuration-model)

For bounded [vertex degrees](#degree-graph-theory), total degree $M\to\infty$, and a forbidden graph $G_0$ of bounded [maximum degree](#maximum-degree), put $\lambda=M^{-1}\sum_i d_i(d_i-1)$ and $\mu=M^{-1}\sum_{ij\in E(G_0)}d_i d_j$. Count prescribed loop pairs, double-edge pairs, and forbidden-edge pairs in the [configuration model](#configuration-model). Their means are respectively $\lambda/2+o(1)$, $\lambda^2/4+o(1)$, and $\mu+o(1)$. A fixed collection of $t$ disjoint prescribed pairs occurs with probability $[(M-1)(M-3)\cdots(M-2t+1)]^{-1}$. Bounded degrees make intersecting bad configurations contribute $O(M^{-1})$ to each fixed [factorial moment](markov-process.md#factorial-moment). Thus the total bad-pattern count has factorial moments $(\lambda/2+\lambda^2/4+\mu)^j+o(1)$. The [Bonferroni inequalities](combinatorics.md#bonferroni-inequalities) and uniformly bounded means give the displayed zero-pattern probability, without requiring the parameters to converge.

#### Half-edge of a graph

↑ **Parent:** [Configuration model](#configuration-model)

A half-edge records an incidence of an [edge](#edge-of-a-graph) at a [vertex](graph.md#vertex-graph-theory). Two half-edges form each edge, including two incidences at the same vertex for a [self-loop](graph.md#loop-graph-theory). In the [configuration model](#configuration-model) these incidences are individually labelled before random pairing.

### Preferential attachment

↑ **Parent:** [Random graph](#random-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Preferential_attachment)

In preferential attachment, new [edges](#edge-of-a-graph) favour existing [vertices](graph.md#vertex-graph-theory) in proportion to a prescribed attractiveness, often their current [degree of a vertex](#degree-graph-theory). A complete model must specify initial conditions, [self-loop](graph.md#loop-graph-theory) conventions and the normalization at each attachment. These details matter for the [vertex degree](#degree-graph-theory) distribution of the earliest [vertices](graph.md#vertex-graph-theory).

#### Linearized chord diagram model

↑ **Parent:** [Preferential attachment](#preferential-attachment)

Start with one [self-loop](graph.md#loop-graph-theory), and at step $t$ add one [vertex](graph.md#vertex-graph-theory) and one [edge](#edge-of-a-graph). An old [vertex](graph.md#vertex-graph-theory) $i$ is chosen with [probability](probability-theory.md#probability) $d_i(t-1)/(2t-1)$, and the new [vertex](graph.md#vertex-graph-theory) is chosen with [probability](probability-theory.md#probability) $1/(2t-1)$, producing a [self-loop](graph.md#loop-graph-theory). [Self-loops](graph.md#loop-graph-theory) contribute two to the [degree of a vertex](#degree-graph-theory). There are $n$ [edges](#edge-of-a-graph) and total [vertex degree](#degree-graph-theory) $2n$ at time $n$. This exact normalization is distinct from treating the total [vertex degree](#degree-graph-theory) as the number of [edges](#edge-of-a-graph).

##### First-vertex degree in the LCD model

↑ **Parent:** [Linearized chord diagram model](#linearized-chord-diagram-model)

In a [uniform linearized chord diagram](#uniform-linearized-chord-diagram), $\Pr(\sqrt nR_1\ge x)=(1-x^2/n)^n\to e^{-x^2}$. Conditional on the right endpoints, $d_1(n)=2+\sum_{i=2}^n\mathbf1_{\{L_i\le R_1\}}$, with [independent](random-variable.md#independent-random-variables) success [probabilities](probability-theory.md#probability) $R_1/R_i$. A [Chernoff bound](probability-inequality.md#chernoff-bound) gives $R_i=(1+o(1))\sqrt{i/n}$ uniformly for $i\ge n^{1/10}$. The early indicators are $o(\sqrt n)$, and the remaining conditional [mean](probability-theory.md#expected-value) is $(2+o(1))nR_1$. Their conditional [variance](variance.md) is $O_{\mathbb P}(\sqrt n)$. Hence $d_1(n)/\sqrt n-2\sqrt nR_1\to0$ in [probability](probability-theory.md#probability), proving the displayed tail limit. A [self-loop](graph.md#loop-graph-theory)'s contribution is included in the constant two.

##### Uniform linearized chord diagram

↑ **Parent:** [Linearized chord diagram model](#linearized-chord-diagram-model)

Pair $2n$ linearly ordered endpoints uniformly. Each pair is a chord; its larger endpoint ends a [vertex](graph.md#vertex-graph-theory) block, with all endpoints after the previous right endpoint merged into that [vertex](graph.md#vertex-graph-theory). Orient the chord from its right-endpoint block to its left-endpoint block. Removing the last endpoint and its mate leaves a uniform smaller pairing. Reinserting the mate into one of $2n-1$ equally likely gaps chooses an existing block proportionally to its endpoint count, or the final gap creates a [self-loop](graph.md#loop-graph-theory). This proves equivalence with the [linearized chord diagram model](#linearized-chord-diagram-model).

An equivalent continuous representation draws $n$ [independent](random-variable.md#independent-random-variables) pairs of [independent](random-variable.md#independent-random-variables) uniform points on $[0,1]$, orders the pairs by their maxima $R_1<\cdots<R_n$, and calls their minima $L_i$. The $R_i^2$ are [uniform order statistics](probability-theory.md#uniform-order-statistic); conditional on all the $R_i$, the $L_i$ are [independent](random-variable.md#independent-random-variables) uniform points on $[0,R_i]$.

### Random k-out graph

↑ **Parent:** [Random graph](#random-graph)

Each [vertex](graph.md#vertex-graph-theory) independently chooses $k$ distinct other [vertices](graph.md#vertex-graph-theory) uniformly, and an undirected [edge](#edge-of-a-graph) exists when either endpoint chooses the other. This has dependent undirected [edges](#edge-of-a-graph) and is not a [binomial random graph](#binomial-random-graph). Coupling the choices as the first $k$ entries of [independent](random-variable.md#independent-random-variables) random permutations makes the [graphs](graph.md) increasing in $k$.

#### Connectivity of random k-out graphs

↑ **Parent:** [Random k-out graph](#random-k-out-graph)

For $k=2$, a disconnected [graph](graph.md) has a component of size $3\le s\le n/2$. The [probability](probability-theory.md#probability) that a fixed $s$-set has no crossing [edge](#edge-of-a-graph) is at most $(s/n)^{2s}(1-s/n)^{2(n-s)}$. The [union bound](probability-inequality.md#boole-s-inequality) and $\binom ns\le(n/s)^s[n/(n-s)]^{n-s}$ bound the failure [probability](probability-theory.md#probability) by $\sum_{s=3}^{\lfloor n/2\rfloor}(s/n)^s=o(1)$. Split this sum at $\sqrt n$. The [random k-out graph](#random-k-out-graph) coupling extends the result to every fixed $k\ge2$.

### Rado graph

↑ **Parent:** [Random graph](#random-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rado_graph)

The Rado graph is the unique countably infinite [graph](graph.md) with the two-uniform [hypergraph extension property](hypergraph.md#hypergraph-extension-property). Equivalently, for any disjoint finite vertex sets $U,W$, some new vertex is adjacent to every member of $U$ and no member of $W$. The [back-and-forth method](foundations-of-mathematics.md#back-and-forth-method) proves uniqueness. Independent edge sampling on the [natural numbers](arithmetic.md#natural-number) with any fixed $p\in(0,1)$ produces this graph [almost surely](convergence-of-random-variables.md#almost-sure-convergence). It contains both edges and nonedges and therefore is not a [complete graph](#complete-graph). Its first-order axioms constitute the [theory of the random graph](foundations-of-mathematics.md#theory-of-the-random-graph).

### Achlioptas process

↑ **Parent:** [Random graph](#random-graph)

At each step offer a fixed number of independent uniform candidate [edges](#edge-of-a-graph) on a fixed vertex set, and let a rule select one. The standard two-choice model offers two candidates. The rule may depend on the entire previously exposed history. Repeated already present [edges](#edge-of-a-graph) make no change in the independent-candidate version; another usual version offers only absent [edges](#edge-of-a-graph). The [forced merging of large components](#forced-merging-of-large-components) and [persistence of unsampled graph components](#persistence-of-unsampled-graph-components) apply to both over a linear number of steps. Fixed choice is essential in the [continuity of fixed-choice percolation](#continuity-of-fixed-choice-percolation) argument.

#### Continuity of fixed-choice percolation

↑ **Parent:** [Achlioptas process](#achlioptas-process)

A fixed-choice [Achlioptas process](#achlioptas-process) cannot have its [largest component of a graph](graph.md#largest-component-of-a-graph) jump from $o(n)$ to a fixed positive fraction of $n$ within $o(n)$ steps, [with high probability](probabilistic-combinatorics.md#with-high-probability). The proof combines [forced merging of large components](#forced-merging-of-large-components) and [persistence of unsampled graph components](#persistence-of-unsampled-graph-components). An assumed jump forces positive vertex mass in each band $[k,Dk)$ slightly before the jump: insufficient smaller components can feed the final large component, while enough components above $Dk$ would merge too early. Persistence carries a fixed positive amount of each band to a common time. Taking sufficiently many disjoint bands with $k=1,D,D^2,\ldots$ then counts more than $n$ [vertices](graph.md#vertex-graph-theory). The number of offered candidates is fixed throughout this argument. Riordan and Warnke establish this obstruction and broader continuity results in [their original research paper](https://arxiv.org/abs/1102.5306).

#### Persistence of unsampled graph components

↑ **Parent:** [Achlioptas process](#achlioptas-process)

Fix positive $\alpha$, $D\geq2$ and $B>0$. Suppose a size band $[k,Dk)$ of an [Achlioptas process](#achlioptas-process) contains at least $\alpha n$ [vertices](graph.md#vertex-graph-theory) at time $m$. For every fixed $k$, at least $\beta n$ of those [vertices](graph.md#vertex-graph-theory) remain in unchanged [graph components](graph.md#component-graph-theory) throughout the next $T=\lceil Bn/k\rceil$ steps, [with high probability](probabilistic-combinatorics.md#with-high-probability), where one may take $\beta=\alpha e^{-16BD}/4$. This is a deliberately nonoptimal positive constant.

For independent uniform candidate [edges](#edge-of-a-graph), an initial [graph component](graph.md#component-graph-theory) with $w<Dk$ [vertices](graph.md#vertex-graph-theory) is untouched if none of the $2T$ candidate [edges](#edge-of-a-graph) meets it. A uniform [edge](#edge-of-a-graph) hits it with [probability](probability-theory.md#probability) at most $3w/n$. For sufficiently large $n$, $(1-3w/n)^{2T}\geq e^{-16BD}$, so the [expected value](probability-theory.md#expected-value) of the untouched vertex mass $Y$ is at least $\alpha e^{-16BD}n$. Replacing one row of two candidate [edges](#edge-of-a-graph) can change $Y$ by at most $8Dk$, because only the initial [graph components](graph.md#component-graph-theory) hit by an old or new endpoint can change status. The [McDiarmid inequality](probability-inequality.md#mcdiarmid-s-inequality) therefore makes $Y\geq\alpha e^{-16BD}n/2$ except on an event of [probability](probability-theory.md#probability) $e^{-c n/k}$, for a positive constant $c$ depending only on $\alpha,B,D$. An untouched [graph component](graph.md#component-graph-theory) stays unchanged whichever offered [edge](#edge-of-a-graph) is selected.

For candidates restricted to absent [edges](#edge-of-a-graph), generate each by an independent uniform proposal stream and reject already present [edges](#edge-of-a-graph). During any interval of $O(n)$ steps with $O(n)$ present [edges](#edge-of-a-graph), each proposal has rejection [probability](probability-theory.md#probability) $O(1/n)$ conditional on the past. The number of rejections is at most $O(\log n)$ except on an event of [probability](probability-theory.md#probability) smaller than any inverse power of $n$: if there were $r$ rejections among $2T+r$ proposals, a [union bound](probability-inequality.md#boole-s-inequality) over their positions bounds this by $\binom{2T+r}r(C/n)^r$. The first $2T$ proposals are independent and give the previous untouched-mass estimate. Extra proposals can touch at most $2r$ additional initial [graph components](graph.md#component-graph-theory), losing only $O(Dk\log n)=o(n)$ [vertices](graph.md#vertex-graph-theory) for fixed $k$. This leaves the stated $\beta n$ bound. A [union bound](probability-inequality.md#boole-s-inequality) makes these estimates simultaneous over starting times $m\leq3n$. They hold through the entire interval, so deterministic or random stopping times within it are allowed.

#### Forced merging of large components

↑ **Parent:** [Achlioptas process](#achlioptas-process)

For the two-choice [Achlioptas process](#achlioptas-process), fix $a>0$ and $K\geq1$. Conditional on any current [graph](graph.md) with $N_{\geq K}\geq an$, put $W$ equal to the [vertices](graph.md#vertex-graph-theory) in its large [graph components](graph.md#component-graph-theory). There are at most $n/K$ such initial [graph components](graph.md#component-graph-theory). If after $s$ more steps no [graph component](graph.md#component-graph-theory) contains $an/3$ [vertices](graph.md#vertex-graph-theory) of $W$, greedily assign final [graph components](graph.md#component-graph-theory) to two groups so that each meets at least $|W|/3\geq an/3$ [vertices](graph.md#vertex-graph-theory) of $W$. This induces a [set partition](combinatorics.md#set-partition) of the initial large [graph components](graph.md#component-graph-theory), of which there are at most $2^{n/K}$ possibilities.

For any fixed such split $W=A\cup B$, a uniform candidate [edge](#edge-of-a-graph) joins $A$ to $B$ with [probability](probability-theory.md#probability) at least $2a^2/9$. If both candidates do so, the selected [edge](#edge-of-a-graph) cannot avoid the crossing. Thus the [probability](probability-theory.md#probability) that the split survives all $s$ steps is at most $(1-a^4/81)^s$. The deliberately weaker constant also covers distinct candidate sampling for sufficiently large $n$. In the absent-edge version, as long as the split has survived, every $A$--$B$ [edge](#edge-of-a-graph) is absent, so conditioning on absence can only increase this crossing [probability](probability-theory.md#probability). A [union bound](probability-inequality.md#boole-s-inequality) with $s=\lceil A(a)n/K\rceil$ and $A(a)=81(\log2+2)/a^4$ bounds failure by $e^{-2n/K}$. For fixed $K$, a further [union bound](probability-inequality.md#boole-s-inequality) makes the conclusion simultaneous over all starting steps $m\leq3n$. This proof is independent of how the rule chooses between the two candidates.

#### Component-band vertex count

↑ **Parent:** [Achlioptas process](#achlioptas-process)

This is the total number of [vertices](graph.md#vertex-graph-theory) in [graph components](graph.md#component-graph-theory) with orders in the specified half-open interval. It differs from the number of those [graph components](graph.md#component-graph-theory). Write $N_{\geq k}$ for the total above the lower endpoint. Then $N_{[k,\ell)}=N_{\geq k}-N_{\geq\ell}$. Disjoint size bands count disjoint sets of [vertices](graph.md#vertex-graph-theory) at a common time, even though their mass may move between bands as an [Achlioptas process](#achlioptas-process) adds [edges](#edge-of-a-graph).

### Simultaneous giant for fixed random-edge choice

↑ **Parent:** [Random graph](#random-graph)

Offer $k$ independent uniform [edges](#edge-of-a-graph) of the [complete graph](#complete-graph) per row and permit any one to be selected from each row. If a chosen [graph](graph.md) has no [graph component](graph.md#component-graph-theory) of order at least $2n/3$, the [balanced component cut](graph.md#balanced-component-cut) provides an empty cut whose sides both have at least $n/3$ [vertices](graph.md#vertex-graph-theory). Each candidate [edge](#edge-of-a-graph) crosses that cut with [probability](probability-theory.md#probability) at least $4/9$, so a row can avoid crossing with [probability](probability-theory.md#probability) at most $1-(4/9)^k$. The [union bound](probability-inequality.md#boole-s-inequality) over at most $2^n$ cuts gives failure probability at most $2^n[1-(4/9)^k]^{cn}$. Any fixed integer $c$ with $c[-\log(1-(4/9)^k)]>\log2$ suffices. The guarantee is simultaneous even for choices made after seeing every offered [edge](#edge-of-a-graph).

### Giant component

↑ **Parent:** [Random graph](#random-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Giant_component)

A giant component in a sequence of [random graphs](#random-graph) on $n$ [vertices](graph.md#vertex-graph-theory) has order proportional to $n$. Its existence can change at a [threshold function for a monotone graph property](#threshold-function-for-a-monotone-graph-property). A [giant component](#giant-component) need not contain every [vertex](graph.md#vertex-graph-theory), and its uniqueness requires proof for the model in question.

#### Barely-supercritical largest-component expectation

↑ **Parent:** [Giant component](#giant-component)

Suppose $\varepsilon=o(1)$ and $\varepsilon\geq n^{-1/6}$. The [breadth-first exploration of a binomial random graph](#breadth-first-exploration-of-a-binomial-random-graph) has deterministic drift $F(t)=\varepsilon t-t^2/(2n)+O(\varepsilon^3n+\varepsilon)$ up to $3\varepsilon n$ steps. Its weighted [martingale](martingale.md) has [variance](variance.md) $O(\varepsilon n)$. For $h=\sqrt\varepsilon+(n\varepsilon^3)^{-1/8}$, the [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality) makes its maximum smaller than $h\varepsilon^2n/6$ [with high probability](probabilistic-combinatorics.md#with-high-probability). Then $A_t>0$ throughout $[h\varepsilon n,(2-h)\varepsilon n]$, giving a [graph component](graph.md#component-graph-theory) of order $(2-o(1))\varepsilon n$.

For the upper expectation bound, let $K=\lceil\varepsilon^{-3}\rceil$. The dominating [binomial branching process](probability-and-statistics.md#binomial-branching-process) has [branching survival probability](probability-and-statistics.md#survival-probability-of-a-branching-process) $(2+o(1))\varepsilon$ by the [binomial branching survival correction](probability-and-statistics.md#binomial-branching-survival-correction). Its [branching process conditioned on extinction](probability-and-statistics.md#branching-process-conditioned-on-extinction) has mean $1-\varepsilon+O(\varepsilon^2+\varepsilon/n)$ and total-progeny [expected value](probability-theory.md#expected-value) $O(1/\varepsilon)$. Therefore $\mathbb EN_{\geq K}\leq n\rho+O(n/(\varepsilon K))$. Since $L_1\leq K+N_{\geq K}$ and $K=o(\varepsilon n)$, this yields the matching upper bound. Controlling rare large components is necessary to conclude an [expected value](probability-theory.md#expected-value) asymptotic from a typical-size statement.

#### Logarithmic-regime giant component

↑ **Parent:** [Giant component](#giant-component)

Fix $k\geq1$, $\gamma_0>1/(k+1)$, and $\gamma_0\leq\gamma\leq1-\omega(n)/\log n$ with $\omega(n)\to\infty$. A [binomial random graph](#binomial-random-graph) has one [giant component](#giant-component) of the displayed order and all other [graph components](graph.md#component-graph-theory) are [tree components](graph.md#tree-component) of orders at most $k$, [with high probability](probabilistic-combinatorics.md#with-high-probability). The [expected value](probability-theory.md#expected-value) and [variance](variance.md) of the [isolated vertex](#isolated-vertex) count concentrate it around $n^{1-\gamma}\to\infty$. A [Cayley formula](combinatorics.md#cayley-s-formula) upper bound for connected sets excludes component sizes $k+1$ through a small fixed fraction of $n$; the empty-[graph cut](graph.md#graph-cut) bound excludes the remaining sizes up to $n/2$. An extra-[edge](#edge-of-a-graph) count excludes cyclic small [graph components](graph.md#component-graph-theory). The [expected value](probability-theory.md#expected-value) of the number of [vertices](graph.md#vertex-graph-theory) in small nonisolated [tree components](graph.md#tree-component) is $O(n d e^{-2d})=o(n e^{-d})$, where $d=np$. The [Markov inequality](probability-inequality.md#markov-s-inequality) completes the count of [vertices](graph.md#vertex-graph-theory) outside the unique large [graph component](graph.md#component-graph-theory).

### Isolated vertex

↑ **Parent:** [Random graph](#random-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isolated_vertex)

An isolated vertex has degree zero.

<h3 id="erdos-renyi-model">Erdős-Rényi model</h3>

↑ **Parent:** [Random graph](#random-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Erdős–Rényi_model)

In the $G(n,p)$ model, each of the $\binom n2$ possible edges is included independently with probability $p$.

#### Breadth-first exploration of a binomial random graph

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

During [breadth-first search](combinatorics.md#breadth-first-search) of $G(n,p)$ let $U_t$ count unseen [vertices](graph.md#vertex-graph-theory), $A_t$ active [vertices](graph.md#vertex-graph-theory), and $t$ explored [vertices](graph.md#vertex-graph-theory). When $A_{t-1}=0$ start a new unseen root, recorded by $b_t=1$; otherwise $b_t=0$. The newly discovered count is conditionally $\operatorname{Bin}(U_{t-1}-b_t,p)$. Subtract its conditional mean to obtain a [martingale difference](martingale.md#martingale-difference) $D_t$. With $q=1-p$, $U_0=n$ and $A_0=0$, iteration gives

$$
A_t=n-t-nq^t+\sum_{j\leq t}q^{t-j+1}b_j+q^t\sum_{j\leq t}q^{-j}D_j.
$$

The last sum is a [martingale](martingale.md). Positive $A_t$ over an interval means that the [graph component](graph.md#component-graph-theory) under exploration does not finish there. Independently adding phantom children couples each component exploration below a [binomial branching process](probability-and-statistics.md#binomial-branching-process) with offspring law $\operatorname{Bin}(n,p)$.

#### Uniform random graph process

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

Start with the empty [graph](graph.md) and reveal the [edges](#edge-of-a-graph) of the [complete graph](#complete-graph) in a uniformly random order. After $m$ steps its edge set is a uniform $m$-element subset. Independent uniform edge labels couple this process with all [binomial random graphs](#binomial-random-graph): $G(n,p)=G_{n,M(p)}$, where $M(p)$ has a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) with parameters $\binom n2,p$. For a [monotone graph property](#monotone-graph-property), concentration of $M(p)$ transfers a threshold estimate between edge probability and edge count.

##### Connectivity hitting time equals disappearance of isolated vertices

↑ **Parent:** [Uniform random graph process](#uniform-random-graph-process)

Couple the process with independent uniform edge labels, and expose $p_-=(\log n-\frac14\log\log n)/n$. A spanning-tree [union bound](probability-inequality.md#boole-s-inequality) excludes components of orders $2$ through $n/\log n$, and a cut bound excludes orders up to $n/2$. The graph has one large component and at most $\log n$ isolated vertices, with at least one isolated vertex. Before $p_+=(\log n+\frac14\log\log n)/n$, the probability of any new edge between those isolated vertices is $O((\log n)^2\log\log n/n)=o(1)$. All have joined the large component by $p_+$ by the [isolated-vertex threshold in the Erdős-Rényi model](#isolated-vertex-threshold-in-the-erdos-renyi-model). Throughout this window the only obstruction to connectivity is an isolated vertex, establishing the equality of hitting times.

##### Marked-set connectivity threshold

↑ **Parent:** [Uniform random graph process](#uniform-random-graph-process)

For a fixed set $L$ of $\lfloor\sqrt n\rfloor$ [vertices](graph.md#vertex-graph-theory), let $\tau_L$ be the first step at which they all belong to one [graph component](graph.md#component-graph-theory). In the [uniform random graph process](#uniform-random-graph-process), $\tau_L$ lies between $n(\log n-\omega)/4$ and $n(\log n+\omega)/4$ [with high probability](probabilistic-combinatorics.md#with-high-probability) for every $\omega\to\infty$. Below that scale the marked [isolated vertex](#isolated-vertex) count has divergent [expected value](probability-theory.md#expected-value) and small relative [variance](variance.md). Above it the [logarithmic-regime giant component](#logarithmic-regime-giant-component) misses $o(\sqrt n)$ [vertices](graph.md#vertex-graph-theory); [exchangeability](probability-theory.md#exchangeable-random-variables) and a [union bound](probability-inequality.md#boole-s-inequality) show that none are marked. The label coupling then transfers the two assertions to the process.

<h4 id="tree-component-expectation-in-the-erdos-renyi-model">Tree-component expectation in the Erdős-Rényi model</h4>

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

For $X_j$ the number of [tree components](graph.md#tree-component) of order $j$ in a [binomial random graph](#binomial-random-graph), choose their [vertices](graph.md#vertex-graph-theory), choose one of $j^{j-2}$ labelled [trees](combinatorics.md#tree-graph-theory) by the [Cayley formula](combinatorics.md#cayley-s-formula), require its $j-1$ [edges](#edge-of-a-graph), and exclude both the remaining internal [edges](#edge-of-a-graph) and all crossing [edges](#edge-of-a-graph). For $j=1$ interpret $j^{j-2}=1$, recovering the [isolated vertex](#isolated-vertex) count. If $p=\lambda/n$ for fixed positive $\lambda$ and $j=O(\log n)$, the [Stirling formula](real-analysis.md#stirling-formula) gives $\mathbb EX_j\sim n(\lambda e^{1-\lambda})^j/(\lambda\sqrt{2\pi}\,j^{5/2})$. Distinct overlapping vertex sets cannot both be [graph components](graph.md#component-graph-theory); for disjoint sets their joint occurrence gains the factor $(1-p)^{-j^2}$ relative to the product, because their between-set [edges](#edge-of-a-graph) must be absent only once.

##### Fixed-order tree-component window

↑ **Parent:** [Tree-component expectation in the Erdős-Rényi model](#tree-component-expectation-in-the-erdos-renyi-model)

For fixed $k\geq2$ and $\omega\to\infty$, the expected number of [tree components](graph.md#tree-component) of order $k$ is asymptotic to $k^{k-2}n^kp^{k-1}e^{-knp}/k!$ throughout the displayed window. It tends to infinity: split $np$ at $1$ and $(\log n)/(2k)$ to obtain lower bounds of orders $\omega^{k-1}$, $\sqrt n$, and $e^\omega$. Distinct overlapping vertex sets cannot both be components; disjoint sets have joint-to-product probability ratio $(1-p)^{-k^2}=1+o(1)$. Thus the relative variance vanishes, proving a component of order $k$ exists [with high probability](probabilistic-combinatorics.md#with-high-probability).

#### Monotone graph property

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

A graph property is increasing and monotone when adding edges cannot destroy it.

##### Threshold function for a monotone graph property

↑ **Parent:** [Monotone graph property](#monotone-graph-property)

A function $p^*(n)$ is a threshold when the property holds with probability tending to zero for $p/p^*\to0$ and with probability tending to one for $p/p^*\to\infty$.

##### Monotone coupling of binomial random graphs

↑ **Parent:** [Monotone graph property](#monotone-graph-property)

Assign an independent uniform label $U_e$ to every possible edge and include $e$ in $G(n,p)$ exactly when $U_e\leq p$. This couples all edge probabilities so that $p\leq q$ implies $G(n,p)\subseteq G(n,q)$.

#### Sprinkling of a binomial random graph

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

Sprinkling exposes independent rounds $G(n,p_1),\ldots,G(n,p_k)$. Their union has distribution $G(n,p)$ where

$$
1-p=\prod_{i=1}^k(1-p_i).
$$

<h4 id="isolated-vertices-in-the-erdos-renyi-model">Isolated vertices in the Erdős-Rényi model</h4>

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

Let $N$ be the number of isolated vertices in $G(n,p)$. Indicator variables give

$$
\mathbb EN=n(1-p)^{n-1}
$$

and, because a specified pair is simultaneously isolated precisely when the $2n-3$ incident edges are absent,

$$
\mathbb E(N^2)=n(1-p)^{n-1}
+n(n-1)(1-p)^{2n-3}.
$$

<h5 id="isolated-vertex-threshold-in-the-erdos-renyi-model">Isolated-vertex threshold in the Erdős-Rényi model</h5>

↑ **Parent:** [Isolated vertices in the Erdős-Rényi model](#isolated-vertices-in-the-erdos-renyi-model)

For $p=c\log n/n$, the number $N$ of isolated vertices satisfies

$$
\mathbb P(N=0)\longrightarrow
\begin{cases}
1,&c>1,\\
0,&c<1.
\end{cases}
$$

The upper side follows from the first-moment bound. On the lower side, $\mathbb EN\to\infty$ and $\operatorname{var}(N)/(\mathbb EN)^2\to0$, so the second-moment method applies.

<h4 id="connectivity-threshold-in-the-erdos-renyi-model">Connectivity threshold in the Erdős-Rényi model</h4>

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

For every fixed $\varepsilon>0$,

$$
p\geq(1+\varepsilon)\frac{\log n}{n}
\Longrightarrow\mathbb P(G(n,p)\text{ is connected})\to1,
$$

whereas the probability tends to zero when $p\leq(1-\varepsilon)\log n/n$. Above the threshold a union bound excludes every component of size at most $n/2$; below it isolated vertices remain with high probability.

##### Connectivity of a fixed-density binomial random graph

↑ **Parent:** [Connectivity threshold in the Erdős-Rényi model](#connectivity-threshold-in-the-erdos-renyi-model)

A disconnected [binomial random graph](#binomial-random-graph) has a [connected component of a graph](graph.md#component-graph-theory) with at most half its [vertices](graph.md#vertex-graph-theory). The [union bound](probability-inequality.md#boole-s-inequality) over its possible [vertex sets](graph.md#vertex-set) gives

$$
\Pr(G(n,p)\text{ disconnected})
\leq\sum_{s=1}^{\lfloor n/2\rfloor}\binom ns(1-p)^{s(n-s)}
\leq\sum_{s=1}^{\lfloor n/2\rfloor}\bigl(n(1-p)^{n/2}\bigr)^s.
$$

The final [geometric series](real-analysis.md#geometric-series) bound tends to zero for fixed $p>0$.

##### Critical-window connectivity probability of a binomial random graph

↑ **Parent:** [Connectivity threshold in the Erdős-Rényi model](#connectivity-threshold-in-the-erdos-renyi-model)

For fixed real $c$, the number of [isolated vertices](#isolated-vertex) in a [binomial random graph](#binomial-random-graph) with $p=(\log n+c)/n$ converges to a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) of mean $e^{-c}$. Its fixed [factorial moments](markov-process.md#factorial-moment) tend to $(e^{-c})^k$. A [union bound](probability-inequality.md#boole-s-inequality) for small [connected components](geometry-and-topology.md#connected-component), together with exclusion of intermediate components, shows that [isolated vertices](#isolated-vertex) are asymptotically the only obstruction to connectivity. Thus the displayed [limit](calculus.md#limit-of-a-function) is the zero-mass of that [Poisson distribution](discrete-probability-distribution.md#poisson-distribution).

<h4 id="expected-subgraph-count-in-the-erdos-renyi-model">Expected subgraph count in the Erdős-Rényi model</h4>

↑ **Parent:** [Erdős-Rényi model](#erdos-renyi-model)

If a fixed graph $H$ has $v$ vertices, $e$ edges, and $N_H(n)$ unlabelled copies in $K_n$, then the number $X_H$ of its copies in $G(n,p)$ satisfies

$$
\mathbb E X_H=N_H(n)p^e.
$$

This follows by writing $X_H$ as a sum of [indicator random variables](probability-theory.md#indicator-random-variable).

##### Sparse clique-count concentration

↑ **Parent:** [Expected subgraph count in the Erdős-Rényi model](#expected-subgraph-count-in-the-erdos-renyi-model)

For $p=n^{-2/3}\log n$, the number $X$ of copies of $K_4$ satisfies

$$
\mathbb EX=\binom n4p^6\sim\frac{(\log n)^6}{24}
$$

and $\operatorname{var}(X)=o((\mathbb EX)^2)$. Two distinct copies have dependent indicators only when they share at least two vertices; pairs sharing two or three vertices contribute respectively $O(n^6p^{11})$ and $O(n^5p^9)$ to the variance.

###### Pendant extensions of sparse clique copies

↑ **Parent:** [Sparse clique-count concentration](#sparse-clique-count-concentration)

If $H$ is formed by attaching one pendant [edge](#edge-of-a-graph) to a fixed [clique](#clique-graph-theory), each copy has a unique clique core. Its number of extensions is the number of ambient [edges](#edge-of-a-graph) from that core to outside [vertices](graph.md#vertex-graph-theory). At a scale where the core count is tight and its expected extension count diverges sufficiently rapidly, a [Chernoff bound](probability-inequality.md#chernoff-bound) uniformly over all possible cores shows that the total count, divided by the extension [mean](probability-theory.md#expected-value), has the same limiting law as the core count. Non-induced copies are intended; extra ambient [edges](#edge-of-a-graph) are not forbidden.

##### Vertex-disjoint sparse clique copies

↑ **Parent:** [Expected subgraph count in the Erdős-Rényi model](#expected-subgraph-count-in-the-erdos-renyi-model)

For $p=n^{-2/3}\log n$, the expected number of pairs of $K_4$ copies sharing a vertex is

$$
O(n^7p^{12}+n^6p^{11}+n^5p^9)=o(1).
$$

Thus, with probability tending to one, all the $K_4$ copies are vertex-disjoint. Together with [sparse clique-count concentration](#sparse-clique-count-concentration), this gives arbitrarily many vertex-disjoint copies with probability tending to one.

## Probabilistic combinatorics

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](probabilistic-combinatorics.md)

## Complement graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complement_graph)

The complement of a simple graph has exactly the edges absent from the original graph; a vertex of degree $d$ acquires degree $n-1-d$.

### Simultaneously bipartite graph and complement

↑ **Parent:** [Complement graph](#complement-graph)

If a graph and its [complement graph](#complement-graph) are both [bipartite](#bipartite-graph), then the graph has at most four vertices. Indeed, each part of a bipartition of the original graph induces a clique in the complement and therefore has at most two vertices. The bound is attained by the four-vertex path, whose complement is another four-vertex path.

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

On vertices $0,\ldots,7$, join cyclic indices differing by one or two modulo eight. The resulting [planar graph](#planar-graph) has a square face bounded in order by $0,2,4,6$. Deleting at most three vertices cannot disconnect it: each break in the surviving cyclic chain requires two consecutive deleted vertices, and two separate breaks require four deletions. It is therefore four-connected. Disjoint paths joining $0$ to $4$ and $2$ to $6$ would cross in the complementary disk of the square face, contrary to the [Jordan curve theorem](topology.md#jordan-curve-theorem). Thus four-connectivity does not guarantee two-linkage.

#### Rooted dense minor linkage

↑ **Parent:** [Linked graph](#linked-graph)

If a [graph](graph.md) is $2k$-connected and has a [graph minor](#graph-minor) $H$ satisfying $2\delta(H)\ge |H|+4k-1$, it is $k$-linked. Write $d=|H|-1-\delta(H)$, so $|H|\ge2d+4k+1$. The [rooted branch-set reduction](#rooted-branch-set-reduction) replaces the minor model by $|H|-k$ disjoint connected sets, the first $2k$ containing any prescribed terminals separately, each missing at most $d$ of the remaining sets. Every prescribed pair then has at least $k+1$ common adjacent unused sets, allowing the $k$ connections to be selected successively. The reduction uses [rooted separations of a graph](#rooted-separation-of-a-graph), contraction of edges outside distinct branch sets, and a final [Hall marriage theorem](#hall-s-marriage-theorem) matching; the separation condition prevents a contraction from destroying access to the model.

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

**[Figure 35](#image-a-graph-subdivision-of-a-triangle-in-a-graph-with-an-attached-leaf-of-a-graph-colours-track-the-four-branch-paths-of-a-graph-subdivision). A graph subdivision of a triangle in a graph with an attached leaf of a graph: colours track the four branch paths of a graph subdivision**.

Adding $m$ internal [vertices](graph.md#vertex-graph-theory) to a finite [graph](graph.md) increases both its [vertex](graph.md#vertex-graph-theory) count and its [edge](#edge-of-a-graph) count by $m$. Here $m=3$, so four [vertices](graph.md#vertex-graph-theory) and four [edges](#edge-of-a-graph) become seven of each; the [graph excess](#graph-excess) is unchanged. Each replacement [graph path](#path-in-a-graph) remains a route between the same junctions. Thus [graph subdivision](#graph-subdivision) preserves whether a [graph](graph.md) is a [planar graph](#planar-graph): insert intermediate [vertices](graph.md#vertex-graph-theory) along a crossing-free drawing, or trace each replacement [graph path](#path-in-a-graph) as one [edge](#edge-of-a-graph) to recover a drawing of the original [graph](graph.md). Travel times or capacities are separate modelling choices and are not determined by this adjacency construction.

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

A bipartite vertex cover is a [vertex cover](#vertex-cover) restricted to a [bipartite graph](#bipartite-graph); [Kőnig's theorem for bipartite matching](#konig-s-theorem-graph-theory) computes its minimum size.

<h2 id="erdos-gallai-theorem">Erdős-Gallai theorem</h2>

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Erdős–Gallai_theorem)

The [Erdős-Gallai theorem](#erdos-gallai-theorem) characterizes which finite nonincreasing sequences of nonnegative integers form the [degree sequence](#degree-sequence) of a [simple graph](graph.md#simple-graph), using an even total degree and partial-sum inequalities.

## Prism graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prism_graph)

A [prism graph](#prism-graph) joins two copies of a [cycle graph](#cycle-graph) by matching corresponding vertices. The [triangular prism graph](#triangular-prism-graph) is the three-cycle case, with six vertices and nine edges.

## Squaregraph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squaregraph)

A [squaregraph](#squaregraph) has a plane embedding in which every bounded face has four sides and every interior vertex has degree at least four. Its outer face may have more than four sides, so this definition differs from a [planar quadrangulation](#planar-quadrangulation) requiring every face to have degree four.

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

A [pseudoforest](#pseudoforest) is an [undirected graph](#undirected-graph) in which every [connected component of a graph](graph.md#component-graph-theory) contains at most one [cycle in a graph](#cycle-in-a-graph). Thus each component is a [tree](combinatorics.md#tree-graph-theory) or a [unicyclic component](probabilistic-combinatorics.md#unicyclic-component). A finite tree component has one fewer edge than vertices; a finite unicyclic component has equally many edges and vertices.

## ↑ Ancestors (4)

1. [Foundations of mathematics](foundations-of-mathematics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Graph](graph.md)
- [Graph of a function](function.md#graph-of-a-function)
- [Graph theory](graph-theory.md)
- [Ramsey number](ramsey-theory.md#ramsey-number)
