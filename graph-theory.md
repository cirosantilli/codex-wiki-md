# Graph theory

↑ **Parent:** [Foundations of mathematics](foundations-of-mathematics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_theory)

**Table of contents**

- [Graph excess](#graph-excess)
  - [Bicyclic graph](#bicyclic-graph)
    - [Labelled bicyclic graph count](#labelled-bicyclic-graph-count)
    - [Bicyclic kernel classification](#bicyclic-kernel-classification)
- [2-core of a graph](#2-core-of-a-graph)
  - [Graph kernel](#graph-kernel)
- [Chordal graph](#chordal-graph)
  - [Triangulation of an undirected graph](#triangulation-of-an-undirected-graph)
  - [Perfect elimination ordering](#perfect-elimination-ordering)
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
  - [Closed walk](#closed-walk)
- [Undirected graph](#undirected-graph)
- [Graph minor](#graph-minor)
  - [Rooted branch-set reduction](#rooted-branch-set-reduction)
  - [Complete graph minor density threshold](#complete-graph-minor-density-threshold)
    - [Dense minor with bounded order and high minimum degree](#dense-minor-with-bounded-order-and-high-minimum-degree)
  - [Branch set of a graph minor](#branch-set-of-a-graph-minor)
    - [Random branch-set construction of a complete graph minor](#random-branch-set-construction-of-a-complete-graph-minor)
  - [Edge contraction](#edge-contraction)
- [Vertex cover](#vertex-cover)
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
    - [List edge coloring](#list-edge-coloring)
      - [List-chromatic index](#list-chromatic-index)
        - [Galvin theorem for bipartite list edge coloring](#galvin-theorem-for-bipartite-list-edge-coloring)
    - [Chromatic index](#chromatic-index)
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
    - [Girth](#girth)
    - [Odd cycle](#odd-cycle)
    - [Cycle graph](#cycle-graph)
      - [Wheel graph](#wheel-graph)
      - [Hamilton cycle](#hamilton-cycle)
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
  - [Euler circuit](#euler-circuit)
  - [Euler circuit criterion](#euler-circuit-criterion)
- [Line graph](#line-graph)
  - [Line graph of a regular graph is Eulerian](#line-graph-of-a-regular-graph-is-eulerian)
- [Planar graph](#planar-graph)
  - [Plane graph](#plane-graph)
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
  - [Complete graph subdivision](#complete-graph-subdivision)
- [Bipartite vertex cover](#bipartite-vertex-cover)
- [Erdős-Gallai theorem](#erdos-gallai-theorem)
- [Prism graph](#prism-graph)
- [Squaregraph](#squaregraph)
- [Vertex cycle cover](#vertex-cycle-cover)
- [Pósa's theorem](#posa-s-theorem)
- [Pseudoforest](#pseudoforest)

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

A chordal graph is an undirected [graph](graph.md) in which every cycle of length at least four has a chord. Its structure allows exact [junction tree](statistical-model.md#junction-tree) calculations using its [maximal cliques](#maximal-clique).

### Triangulation of an undirected graph

↑ **Parent:** [Chordal graph](#chordal-graph)

Triangulation adds fill edges to an undirected [graph](graph.md) to make it a [chordal graph](#chordal-graph). Given an elimination ordering, join all remaining neighbors of each removed vertex. The completed graph has that [perfect elimination ordering](#perfect-elimination-ordering). Fill edges can enlarge the [cliques](#clique-graph-theory) used for exact [probabilistic graphical model](statistical-model.md#probabilistic-graphical-model) inference, without changing the original probability factors; they do not assert new biological relationships.

### Perfect elimination ordering

↑ **Parent:** [Chordal graph](#chordal-graph)

A perfect elimination ordering successively removes a [graph vertex](graph.md#vertex-graph-theory) whose remaining neighbors form a [clique](#clique-graph-theory). An undirected [graph](graph.md) is a [chordal graph](#chordal-graph) exactly when it has such an ordering. In one direction, the earliest vertex of an induced long cycle would have two nonadjacent later neighbors, contradicting the ordering. The converse follows by the existence of a simplicial vertex in every finite chordal graph.

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

A shortest path minimizes the sum of edge lengths between two vertices. With nonnegative lengths, a shortest walk can be reduced to a simple path by removing cycles, so exponentially many candidate paths can be searched implicitly. The [Dijkstra algorithm](#dijkstra-algorithm) solves this problem in [polynomial time](computer-science.md#polynomial-time).

### Label-setting shortest-path algorithm

↑ **Parent:** [Shortest path problem](#shortest-path-problem)

An algorithm that makes each vertex's distance permanent once it is selected. With nonnegative [directed edge](#directed-edge) lengths, the [Dijkstra algorithm](#dijkstra-algorithm) selects the unfinalized vertex with least tentative distance; a shorter route through another unfinalized vertex is impossible because its remaining route has at least that next tentative distance. For an all-to-one problem, incoming [directed edges](#directed-edge) to the selected vertex are relaxed. Negative lengths can invalidate this finalization argument.

### Bellman inequalities

↑ **Parent:** [Shortest path problem](#shortest-path-problem)

For an all-to-one [shortest path problem](#shortest-path-problem) with root $r$ and $d_r=0$, these inequalities ensure that $d_i$ is no larger than any [directed path](#directed-path) length from $i$ to $r$, by summing along that [directed path](#directed-path). If every finite $d_i$ is also the length of a discovered [directed path](#directed-path), the inequalities certify exact shortest-path labels. Nodes from which the root is unreachable retain infinite distance and are handled separately.

### Label-correcting shortest-path algorithm

↑ **Parent:** [Shortest path problem](#shortest-path-problem)

An algorithm whose tentative distance labels may be revised repeatedly until all relevant [Bellman inequalities](#bellman-inequalities) hold. [Bellman-Ford algorithm](#bellman-ford-algorithm) uses this approach: a label is an upper bound supplied by a discovered [directed path](#directed-path), and relaxing an [directed edge](#directed-edge) can replace it with a shorter discovered [directed path](#directed-path). A finite label is not declared permanent merely because it has been processed.

### Bellman-Ford algorithm

↑ **Parent:** [Shortest path problem](#shortest-path-problem)

For an all-to-one [shortest path problem](#shortest-path-problem) with root $r$, initialize $d_r^{(0)}=0$ and all other labels to infinity. Set $d_i^{(k)}=\min(d_i^{(k-1)},\min_{(i,j)\in A}\{c_{ij}+d_j^{(k-1)}\})$, keeping the root at zero. Induction identifies the labels with the shortest [directed paths](#directed-path) using at most $k$ [directed edges](#directed-edge). Without a reachable negative [directed cycle](#directed-cycle), $|V|-1$ rounds suffice after removing [directed cycles](#directed-cycle) from a shortest walk. In-place or queue variants repeatedly relax incoming [directed edges](#directed-edge) to an improved label. Labels may decrease multiple times, so this is a [label-correcting shortest-path algorithm](#label-correcting-shortest-path-algorithm).

### Dijkstra algorithm

↑ **Parent:** [Shortest path problem](#shortest-path-problem)

Starting with distance zero at the source and infinity elsewhere, repeatedly finalize the unfinalized vertex with least tentative distance and relax its outgoing edges. Nonnegative lengths ensure that no later path can improve a finalized distance: any alternative path first reaches an unfinalized vertex whose tentative distance is at least the finalized one. A binary heap gives $O((|V|+|E|)\log |V|)$ arithmetic operations, and storing predecessors recovers a minimizing path.

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

A vertex whose deletion increases the number of connected components of a [graph](graph.md). A [Hamiltonian](classical-mechanics.md#hamiltonian) graph has no cut vertex: deleting a vertex from a [Hamilton cycle](#hamilton-cycle) leaves a spanning path.

## Hypergraph

↑ **Parent:** [Graph theory](graph-theory.md)

[This section is present in another page, follow this link to view it.](hypergraph.md)

## Walk in a graph

↑ **Parent:** [Graph theory](graph-theory.md)

A sequence of vertices and edges of a [graph](graph.md), with each edge joining its two consecutive vertices. Vertices and edges may repeat; a [path in a graph](#path-in-a-graph) imposes distinctness conditions. A [closed walk](#closed-walk) ends where it starts.

### Closed walk

↑ **Parent:** [Walk in a graph](#walk-in-a-graph)

A [walk in a graph](#walk-in-a-graph) whose first and last vertices agree. An [Euclidean travelling salesman tour](mathematical-optimization.md#euclidean-travelling-salesman-tour) can be estimated by first constructing a closed walk visiting all locations and then using the [triangle inequality](topological-analysis.md#triangle-inequality) to shortcut repeated visits.

## Undirected graph

↑ **Parent:** [Graph theory](graph-theory.md)

An undirected [graph](graph.md) has edges that are unordered pairs of vertices. In a simple undirected graph there are no loops or multiple edges. The [skeleton of a directed graph](#skeleton-of-a-directed-graph) forgets the directions of its edges and is an undirected graph.

## Graph minor

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_minor)

A graph minor is obtained by deleting [vertices](graph.md#vertex-graph-theory), deleting [edges](#edge-of-a-graph), and performing [edge contractions](#edge-contraction). Equivalently, its [vertices](graph.md#vertex-graph-theory) can be represented by disjoint nonempty connected sets of [vertices](graph.md#vertex-graph-theory) in the original [graph](graph.md), with an [edge](#edge-of-a-graph) joining two sets whenever the corresponding [vertices](graph.md#vertex-graph-theory) are adjacent. These are [branch sets of a graph minor](#branch-set-of-a-graph-minor).

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

A branch set is a nonempty set of [vertices](graph.md#vertex-graph-theory) inducing a [connected graph](graph.md#connected-graph) used to represent one [vertex](graph.md#vertex-graph-theory) of a [graph minor](#graph-minor). A $K_t$ [graph minor](#graph-minor) is equivalent to $t$ disjoint branch sets with at least one [edge](#edge-of-a-graph) between every pair. Connectedness allows each set to be reduced to a single [vertex](graph.md#vertex-graph-theory) by [edge contractions](#edge-contraction).

#### Random branch-set construction of a complete graph minor

↑ **Parent:** [Branch set of a graph minor](#branch-set-of-a-graph-minor)

In a dense [graph](graph.md) with many [common neighbours](#common-neighbour) for every pair of [vertices](graph.md#vertex-graph-theory), choose disjoint random small sets. A set is good if few [vertices](graph.md#vertex-graph-theory) have no neighbour in it. The [Markov inequality](probability-inequality.md#markov-inequality) controls the number of bad sets, and random sampling makes almost every pair of good sets adjacent. Add unused [common neighbours](#common-neighbour) to connect each set and to repair the remaining missing adjacencies. If the number of used [vertices](graph.md#vertex-graph-theory) stays below every common-neighbour count, this constructs disjoint [branch sets of a graph minor](#branch-set-of-a-graph-minor) representing a large [complete graph](#complete-graph).

### Edge contraction

↑ **Parent:** [Graph minor](#graph-minor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edge_contraction)

Contracting an [edge](#edge-of-a-graph) $uv$ identifies its endpoints, then removes loops and duplicate [edges](#edge-of-a-graph) to produce a simple [graph](graph.md). It reduces the [edge](#edge-of-a-graph) count by exactly $1+|N(u)\cap N(v)|$: one for $uv$, and one for each [common neighbour](#common-neighbour).

## Vertex cover

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vertex_cover)

A vertex cover is a set of [vertices](graph.md#vertex-graph-theory) meeting every [edge](#edge-of-a-graph) of a [graph](graph.md). The endpoints of any [maximal matching](#maximal-matching) form a vertex cover: an [edge](#edge-of-a-graph) avoiding all endpoints would enlarge that [matching in a graph](#matching-graph-theory). Consequently a [graph](graph.md) with no [matching in a graph](#matching-graph-theory) of size $s$ has a vertex cover of size at most $2(s-1)$.

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

For fixed $0<p<1$, the [missing common-neighbour count in a binomial random graph](#missing-common-neighbour-count-in-a-binomial-random-graph) has [expectation](probability-theory.md#expected-value) tending to zero. The [Markov inequality](probability-inequality.md#markov-inequality) therefore shows that every pair has a [common neighbour](#common-neighbour) with probability tending to one. On that event every [graph distance](#distance-graph-theory) is at most two, so the [graph](graph.md) is [connected](geometry-and-topology.md#connected-space) and its [graph diameter](#graph-diameter) is at most two.

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

If $np\to0$, the [triangle count in a binomial random graph](#triangle-count-in-a-binomial-random-graph) has [expectation](probability-theory.md#expected-value) at most $(np)^3/6\to0$, so the [Markov inequality](probability-inequality.md#markov-inequality) shows there are no [triangles in a graph](graph.md#triangle-in-a-graph) with probability tending to one. If $np\to\infty$, the [triangle variance in a binomial random graph](#triangle-variance-in-a-binomial-random-graph) divided by the squared mean is $O((np)^{-3})+O((n^2p)^{-1})\to0$. The [second moment method](probability-inequality.md#second-moment-method) then gives at least one [triangle in a graph](graph.md#triangle-in-a-graph) with probability tending to one. At the intermediate scale $np\to c\in(0,\infty)$, a nontrivial [Poisson limit for triangles in a binomial random graph](#poisson-limit-for-triangles-in-a-binomial-random-graph) describes the count.

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

A graph colouring assigns labels called colours to graph elements subject to specified constraints. A proper vertex colouring gives adjacent vertices different colours.

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

Order the [vertices](graph.md#vertex-graph-theory) of a [graph](graph.md) and assign each vertex the smallest color not already used by its colored neighbours. This produces a proper [graph coloring](#graph-coloring) with at most $\Delta+1$ colors when the maximum degree is $\Delta$. The result can depend strongly on vertex order and need not achieve the [chromatic number](#chromatic-number).

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

Choose $r=\max\{0,\lceil\log_3(4m/n)\rceil\}$. Then [Markov inequality](probability-inequality.md#markov-inequality) gives $\mathbb P(B>n/2)\leq1/2$. On success, delete one endpoint of every monochromatic [edge](#edge-of-a-graph). This [random alteration method](probabilistic-combinatorics.md#random-alteration-method) leaves at least $n/2$ [vertices](graph.md#vertex-graph-theory) properly colored with

$$
k=2^r=O\left(\max\{1,(m/n)^{\log_3 2}\}\right)=O(n^{\log_3 2}).
$$

The removed [vertices](graph.md#vertex-graph-theory) can retain their original colors, as the [semicoloring](#semicoloring) only requires the retained [induced subgraph](#induced-subgraph) to be proper. A failed draw can be detected and repeated, with at most two trials on average. The case $m=0$ needs just one color. This is the elementary independent-hyperplane construction in [Karger, Motwani and Sudan's paper on approximate graph coloring](https://arxiv.org/abs/cs/9812008).

### Edge coloring

↑ **Parent:** [Graph coloring](#graph-coloring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edge_coloring)

An edge colouring assigns a colour to every [edge of a graph](#edge-of-a-graph). In a red-blue edge colouring of a [complete graph](#complete-graph), a triangle is monochromatic when its three edges have the same colour.

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

The chromatic index is the least number of colors in an [edge coloring](#edge-coloring) for which [edges](#edge-of-a-graph) sharing an endpoint have different colors. It is at least the [maximum degree of a graph](#maximum-degree-of-a-graph). In a [bipartite graph](#bipartite-graph) it equals the maximum degree: for an uncolored edge, choose colors missing at its endpoints and swap the two colors on a suitable alternating component. If the missing colors differ, that component cannot connect the two endpoints, since the necessary even-length path would put them in the same bipartition class.

#### Tait coloring

↑ **Parent:** [Edge coloring](#edge-coloring)

A proper three-color [edge coloring](#edge-coloring) of a [cubic graph](graph.md#cubic-graph). Label its colors by the nonzero elements of $\mathbb F_2^2$: the incident colors at each [vertex](graph.md#vertex-graph-theory) then sum to zero. On a planar map without [bridges in a graph](graph.md#bridge-graph-theory), integrating these labels on the [dual graph](graph.md#dual-graph) gives a four-color face coloring. On a [torus](topology.md#torus), a nonzero period can obstruct this integration.

### Chromatic number

↑ **Parent:** [Graph coloring](#graph-coloring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chromatic_number)

The chromatic number $\chi(G)$ is the least number of colours in a proper vertex colouring of $G$.

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

For each positive integer $t$, the chromatic polynomial $P_G(t)$ counts the proper vertex colourings of a finite graph $G$ using a fixed palette of $t$ colours.

<h4 id="chromatic-polynomial-determines-a-turan-graph">Chromatic polynomial determines a Turán graph</h4>

↑ **Parent:** [Chromatic polynomial](#chromatic-polynomial)

If a simple graph has the same [chromatic polynomial](#chromatic-polynomial) as the [Turán graph](#turan-graph) $T_r(n)$, it has the same number of vertices and edges, and the same [chromatic number](#chromatic-number) $r$. It is therefore $K_{r+1}$-free and attains equality in [Turán's theorem](#turan-s-theorem). The equality case forces it to be isomorphic to $T_r(n)$.

#### Deletion-contraction recurrence for the chromatic polynomial

↑ **Parent:** [Chromatic polynomial](#chromatic-polynomial)

For a non-loop edge $e$,

$$
P_G(t)=P_{G-e}(t)-P_{G/e}(t).
$$

The first term counts colourings after deleting $e$; the second subtracts those giving its endpoints the same colour, which correspond to colourings of the contraction. Together with $P_G(t)=t^{|V(G)|}$ for an edgeless graph, induction proves that $P_G$ is a polynomial.

#### Chromatic polynomial after attaching a leaf

↑ **Parent:** [Chromatic polynomial](#chromatic-polynomial)

Attaching a new [leaf](#leaf-of-a-graph) to a graph multiplies its [chromatic polynomial](#chromatic-polynomial) by $t-1$, because after colouring the old graph the leaf may receive any colour except its neighbour's.

## Independent set (graph theory)

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Independent_set_(graph_theory))

An independent set is a set of vertices no two of which are adjacent. In every proper colouring, each colour class is an independent set.

### Independent transversal

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

For a [graph](graph.md) whose vertices are partitioned into parts, an independent transversal is an [independent set](#independent-set-graph-theory) containing exactly one vertex from each part. If a cycle's parts each have twelve vertices, choose one vertex uniformly and independently per part. A cycle edge joining distinct parts is selected at both ends with [probability](probability-theory.md#probability) $1/144$. Each [event](probability-theory.md#event) depends on at most $47$ others, since each part meets at most $24$ cycle edges. The [Lovász local lemma](probabilistic-combinatorics.md#lovasz-local-lemma) applies because $48e/144<1$, proving existence for an arbitrary such partition.

### Degree-ordered independent-set entropy bound

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)

Order vertices by nonincreasing positive degrees $d_i$, and let $b_i$ count preceding neighbors. The [Madiman-Tetali inequality](information-theory.md#madiman-tetali-entropy-inequality) applied to preceding-neighbor sets and $b_i$ copies of singleton $i$ bounds the entropy of a uniformly chosen [independent set](#independent-set-graph-theory). In each local term, all-zero neighbor assignment permits two choices at $i$, while every other assignment permits at most one. The maximum-entropy bound gives $\log_2(2^{b_i+1}-1)$ for that term. Complete bipartite graphs $K_{d,d}$ attain equality when one part is ordered before the other.

### Independence number

↑ **Parent:** [Independent set (graph theory)](#independent-set-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Independence_number)

The independence number is the largest cardinality of an [independent set](#independent-set-graph-theory) in a graph. Since every colour class is independent,

$$
\chi(G)\geq\frac{|V(G)|}{\alpha(G)}.
$$

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

A Hamilton cycle is a cycle containing every vertex of its graph.

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

For a finite graph with adjacency matrix $A$ and degree matrix $D$, its graph Laplacian is

$$
L=D-A.
$$

Its quadratic form is $x^TLx=\sum_{\{i,j\}\in E}(x_i-x_j)^2$.

### Weighted graph Laplacian

↑ **Parent:** [Laplacian matrix](#laplacian-matrix)

For symmetric edge weights $w_{ij}\geq0$, the weighted graph Laplacian has quadratic form

$$
x^TL_wx=\sum_{\{i,j\}\in E}w_{ij}(x_i-x_j)^2.
$$

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

A flow network is a directed capacitated graph with a source and sink. A feasible flow respects edge capacities and conserves flow at every other vertex.

### Circulation in a flow network

↑ **Parent:** [Flow network](#flow-network)

A [network circulation](#circulation-in-a-flow-network) is a [flow](#flow) with zero net supply at every vertex. A feasible residual [network circulation](#circulation-in-a-flow-network) changes one feasible flow into another with the same prescribed supplies. It decomposes into directed cycles, giving the negative-cycle optimality test for [minimum-cost flow](#minimum-cost-flow-problem).

### Vertex capacity

↑ **Parent:** [Flow network](#flow-network)

An internal vertex capacity bounds the total [flow](#flow) through that vertex, equivalently its total inflow or outflow by [flow conservation](#flow-conservation). Replace the vertex by an input and output vertex, direct incoming edges to the input and outgoing edges from the output, and connect input to output with an edge of the vertex capacity. This converts the constraint into an ordinary [flow network edge capacity](#flow-network-edge-capacity).

### Maximum flow problem

↑ **Parent:** [Flow network](#flow-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_flow_problem)

The maximum flow problem maximises the [strength of a flow](#strength-of-a-flow) from a source to a sink subject to [flow conservation](#flow-conservation) and [flow network edge capacities](#flow-network-edge-capacity). The [max-flow min-cut theorem](#max-flow-min-cut-theorem) identifies the optimum with the least capacity of a [cut of a flow network](#cut-of-a-flow-network). A feasible [flow](#flow) and a [cut of a flow network](#cut-of-a-flow-network) of equal value certify optimality without requiring a particular choice of [augmenting paths](#augmenting-path).

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

This [maximum flow](#maximum-flow-problem) algorithm repeatedly augments along a shortest residual path found by [Breadth-first search](combinatorics.md#breadth-first-search). Residual distances from the source never decrease. If the same arc becomes saturated again after being restored by a reverse augmentation, the distance to its tail has increased by at least two. Thus each arc is critical only $O(|V|)$ times, yielding $O(|V||E|)$ augmentations. Each search costs $O(|E|)$, so the total time is $O(|V||E|^2)$. Termination with no residual source-sink path supplies a [max-flow min-cut theorem](#max-flow-min-cut-theorem) certificate.

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

The greatest value of a feasible source-to-sink flow equals the least capacity of a source-to-sink cut. For a maximum flow, the vertices reachable from the source in the residual graph define a cut whose forward edges are saturated and whose backward edges carry zero flow.

#### Residual reachability certificate for maximum flow

↑ **Parent:** [Max-flow min-cut theorem](#max-flow-min-cut-theorem)

In a finite capacitated directed network, a [maximum flow](#maximum-flow-problem) exists because the feasible flow set is nonempty and compact. A residual source-to-sink path would permit positive augmentation, contradicting maximality. The source-reachable residual vertices therefore define a cut whose outgoing original arcs are saturated and incoming original arcs carry zero flow. Conservation makes the flow value equal to this cut capacity. This proof applies to arbitrary finite real capacities without claiming finite termination of an augmenting-path algorithm.

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

For a feasible flow $f$, the residual network has forward residual capacity $c(u,v)-f(u,v)$ and reverse residual capacity $f(u,v)$. It records every local increase or cancellation that preserves the capacity constraints.

##### Residual maximum flow is the remaining optimality gap

↑ **Parent:** [Residual network](#residual-network)

For an undirected capacitated network, write the net edge flow as $y_{ij}=-y_{ji}$, and the directed residual capacity as $c_{ij}-y_{ij}$. On every source–sink cut, residual capacity is the original cut capacity minus the current net flow value $f$. Taking the minimum over cuts and applying the [max-flow min-cut theorem](#max-flow-min-cut-theorem) to each network gives the displayed remaining-flow identity.

##### Augmenting path

↑ **Parent:** [Residual network](#residual-network)

An augmenting path is a source-to-sink path of positive capacities in the [residual network](#residual-network). Increasing the flow by the smallest residual capacity on the path gives another feasible flow of strictly greater value.

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

An Eulerian graph has a closed trail that traverses every edge exactly once.

### Euler circuit

↑ **Parent:** [Eulerian graph](#eulerian-graph)

An [Euler circuit](#euler-circuit) is a closed edge trail that traverses every edge exactly once. Vertices may repeat, and parallel edges are counted separately. A connected finite undirected multigraph has such a circuit exactly when every vertex has even degree. Necessity follows by pairing arrivals and departures; sufficiency follows by forming closed unused-edge trails and splicing them until every edge is used, as in the [Euler circuit criterion](#euler-circuit-criterion).

### Euler circuit criterion

↑ **Parent:** [Eulerian graph](#eulerian-graph)

A finite graph with at least three vertices is Eulerian exactly when it is connected and every vertex has even degree. A maximal trail closes by parity; closed trails based at vertices with unused incident edges can then be spliced together.

## Line graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Line_graph)

The line graph $L(G)$ has one vertex for each edge of $G$, with adjacency when two original edges share an endpoint.

### Line graph of a regular graph is Eulerian

↑ **Parent:** [Line graph](#line-graph)

If $G$ is connected and $r$-regular, then $L(G)$ is connected and every one of its vertices has degree $2r-2$. The [Euler circuit criterion](#euler-circuit-criterion) therefore applies.

## Planar graph

↑ **Parent:** [Graph theory](graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Planar_graph)

A planar graph admits a drawing in the plane whose edges meet only at common endpoints.

### Plane graph

↑ **Parent:** [Planar graph](#planar-graph)

A [plane graph](#plane-graph) is a [planar graph](#planar-graph) together with a specified crossing-free embedding in the plane. Its faces are the connected complementary regions, including the unbounded region. Face counts and facial boundary walks refer to this embedding. For a finite connected [plane graph](#plane-graph), the [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph) is $v-e+f=2$: deleting a cycle edge lowers both edge and face counts by one until a [tree](combinatorics.md#tree-graph-theory) remains, where $e=v-1$ and $f=1$. The distinction between an abstract [planar graph](#planar-graph) and its chosen embedding matters when discussing which edges bound a face.

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

For a connected planar graph with $n$ vertices, $e$ edges, and $f$ faces,

$$
n-e+f=2.
$$

Deleting a cycle edge preserves connectedness and decreases both $e$ and $f$ by one, reducing the formula to its immediate tree case.

#### Small faces of a spherical polyhedral graph

↑ **Parent:** [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph)

For a connected cellular spherical [planar graph](#planar-graph) with vertex degrees at least three and face sizes at least three, degree/face double counting and the [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph) give $\sum_n(6-n)F_n=12+\sum_m(2m-6)V_m\ge12$. The left side is at most $3(F_3+F_4+F_5)$, proving the displayed bound. In particular a convex polyhedron has at least four faces of size at most five.

#### Planar graph edge bound

↑ **Parent:** [Euler formula for a connected planar graph](#euler-formula-for-a-connected-planar-graph)

A simple planar graph with $n\geq3$ vertices has at most $3n-6$ edges.

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

A graph is bipartite when its vertices split into two classes and every edge joins the two different classes.

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

A perfect matching saturates every vertex of the graph.

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

Fix $k\geq1$, $\gamma_0>1/(k+1)$, and $\gamma_0\leq\gamma\leq1-\omega(n)/\log n$ with $\omega(n)\to\infty$. A [binomial random graph](#binomial-random-graph) has one [giant component](#giant-component) of the displayed order and all other [graph components](graph.md#component-graph-theory) are [tree components](graph.md#tree-component) of orders at most $k$, [with high probability](probabilistic-combinatorics.md#with-high-probability). The [expected value](probability-theory.md#expected-value) and [variance](variance.md) of the [isolated vertex](#isolated-vertex) count concentrate it around $n^{1-\gamma}\to\infty$. A [Cayley formula](combinatorics.md#cayley-s-formula) upper bound for connected sets excludes component sizes $k+1$ through a small fixed fraction of $n$; the empty-[graph cut](graph.md#graph-cut) bound excludes the remaining sizes up to $n/2$. An extra-[edge](#edge-of-a-graph) count excludes cyclic small [graph components](graph.md#component-graph-theory). The [expected value](probability-theory.md#expected-value) of the number of [vertices](graph.md#vertex-graph-theory) in small nonisolated [tree components](graph.md#tree-component) is $O(n d e^{-2d})=o(n e^{-d})$, where $d=np$. The [Markov inequality](probability-inequality.md#markov-inequality) completes the count of [vertices](graph.md#vertex-graph-theory) outside the unique large [graph component](graph.md#component-graph-theory).

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

During [Breadth-first search](combinatorics.md#breadth-first-search) of $G(n,p)$ let $U_t$ count unseen [vertices](graph.md#vertex-graph-theory), $A_t$ active [vertices](graph.md#vertex-graph-theory), and $t$ explored [vertices](graph.md#vertex-graph-theory). When $A_{t-1}=0$ start a new unseen root, recorded by $b_t=1$; otherwise $b_t=0$. The newly discovered count is conditionally $\operatorname{Bin}(U_{t-1}-b_t,p)$. Subtract its conditional mean to obtain a [martingale difference](martingale.md#martingale-difference) $D_t$. With $q=1-p$, $U_0=n$ and $A_0=0$, iteration gives

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

A subdivision of a graph replaces each edge by a path, with all replacement paths internally vertex-disjoint.

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

## ← Incoming links (1)

- [Graph of a function](function.md#graph-of-a-function)
