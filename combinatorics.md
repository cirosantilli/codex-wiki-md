# Combinatorics

↑ **Parent:** [Area of mathematics](mathematics.md#area-of-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Combinatorics)

**Table of contents**

- [Matroid](#matroid)
- [Rule of product](#rule-of-product)
- [Steiner system](#steiner-system)
  - [Block of a Steiner system](#block-of-a-steiner-system)
  - [Difference family for a Steiner 2-design](#difference-family-for-a-steiner-2-design)
    - [Cyclotomic construction of a Steiner 2-design](#cyclotomic-construction-of-a-steiner-2-design)
  - [Small Witt design](#small-witt-design)
    - [Synthematic construction of the small Witt design](#synthematic-construction-of-the-small-witt-design)
- [Six-point matching geometry](#six-point-matching-geometry)
  - [Pentad construction of the exceptional alternating-group automorphism](#pentad-construction-of-the-exceptional-alternating-group-automorphism)
  - [Duad-syntheme duality on six points](#duad-syntheme-duality-on-six-points)
  - [Duad](#duad)
    - [Syntheme](#syntheme)
      - [Total of synthemes](#total-of-synthemes)
        - [Counting synthematic totals](#counting-synthematic-totals)
- [Cycle lemma](#cycle-lemma)
- [Cyclic digit run](#cyclic-digit-run)
- [Finite geometry](#finite-geometry)
- [Increasing subsequence](#increasing-subsequence)
  - [Longest increasing subsequence](#longest-increasing-subsequence)
- [Additive combinatorics](additive-combinatorics.md)
  - [Furstenberg-Katznelson theorem](additive-combinatorics.md#furstenberg-katznelson-theorem)
  - [Bracket-linear frequency function](additive-combinatorics.md#bracket-linear-frequency-function)
  - [Four-term progression hypergraph encoding](additive-combinatorics.md#four-term-progression-hypergraph-encoding)
  - [Roth theorem on three-term arithmetic progressions](additive-combinatorics.md#roth-theorem-on-three-term-arithmetic-progressions)
    - [Roth density increment on an integer progression](additive-combinatorics.md#roth-density-increment-on-an-integer-progression)
    - [Triangle-removal proof of Roth theorem](additive-combinatorics.md#triangle-removal-proof-of-roth-theorem)
    - [Classical Roth bound for three-term progressions](additive-combinatorics.md#classical-roth-bound-for-three-term-progressions)
    - [High-energy Roth theorem](additive-combinatorics.md#high-energy-roth-theorem)
  - [Product set](additive-combinatorics.md#product-set)
    - [Multiplicative energy](additive-combinatorics.md#multiplicative-energy)
      - [Multiplicative energy sumset bound](additive-combinatorics.md#multiplicative-energy-sumset-bound)
  - [Corner in an integer grid](additive-combinatorics.md#corner-in-an-integer-grid)
    - [Corners theorem](additive-combinatorics.md#corners-theorem)
  - [Cut norm](additive-combinatorics.md#cut-norm)
  - [Non-abelian additive combinatorics](additive-combinatorics.md#non-abelian-additive-combinatorics)
    - [Matrix-valued Gowers U2 quantity](additive-combinatorics.md#matrix-valued-gowers-u2-quantity)
      - [Spectral inverse theorem for the matrix-valued U2 quantity](additive-combinatorics.md#spectral-inverse-theorem-for-the-matrix-valued-u2-quantity)
      - [Matrix Fourier block](additive-combinatorics.md#matrix-fourier-block)
    - [Quasirandom group](additive-combinatorics.md#quasirandom-group)
      - [Product mixing in a quasirandom group](additive-combinatorics.md#product-mixing-in-a-quasirandom-group)
    - [Fourier analysis on a finite group](additive-combinatorics.md#fourier-analysis-on-a-finite-group)
      - [Right translation of a group function](additive-combinatorics.md#right-translation-of-a-group-function)
      - [Left translation of a group function](additive-combinatorics.md#left-translation-of-a-group-function)
      - [Fourier transform on a finite group](additive-combinatorics.md#fourier-transform-on-a-finite-group)
        - [Parseval identity on a finite group](additive-combinatorics.md#parseval-identity-on-a-finite-group)
        - [Fourier inversion on a finite group](additive-combinatorics.md#fourier-inversion-on-a-finite-group)
      - [Normalized convolution on a finite group](additive-combinatorics.md#normalized-convolution-on-a-finite-group)
        - [Convolution theorem on a finite group](additive-combinatorics.md#convolution-theorem-on-a-finite-group)
  - [Box norm](additive-combinatorics.md#box-norm)
    - [Random sign rectangle fourth moment](additive-combinatorics.md#random-sign-rectangle-fourth-moment)
    - [Cut norm and rectangle fourth-moment equivalence](additive-combinatorics.md#cut-norm-and-rectangle-fourth-moment-equivalence)
    - [Three-dimensional box norm](additive-combinatorics.md#three-dimensional-box-norm)
      - [Pair-factor correlation bound for the three-dimensional box norm](additive-combinatorics.md#pair-factor-correlation-bound-for-the-three-dimensional-box-norm)
    - [Box norm singular-value identity](additive-combinatorics.md#box-norm-singular-value-identity)
    - [Bilinear correlation bound for the box norm](additive-combinatorics.md#bilinear-correlation-bound-for-the-box-norm)
      - [Triangle counting with one box-uniform pair and constant opposite degree](additive-combinatorics.md#triangle-counting-with-one-box-uniform-pair-and-constant-opposite-degree)
    - [Box Cauchy-Schwarz inequality](additive-combinatorics.md#box-cauchy-schwarz-inequality)
  - [Sum-product phenomenon](additive-combinatorics.md#sum-product-phenomenon)
    - [Closure bounds for small skew-sumset scalars](additive-combinatorics.md#closure-bounds-for-small-skew-sumset-scalars)
      - [Polynomial skew-sumset expansion over a prime field](additive-combinatorics.md#polynomial-skew-sumset-expansion-over-a-prime-field)
    - [Quadratic growth of a sixfold product difference set](additive-combinatorics.md#quadratic-growth-of-a-sixfold-product-difference-set)
    - [Solymosi sum-product theorem over the complex numbers](additive-combinatorics.md#solymosi-sum-product-theorem-over-the-complex-numbers)
  - [Density of a finite subset](additive-combinatorics.md#density-of-a-finite-subset)
    - [Balanced indicator function of a finite subset](additive-combinatorics.md#balanced-indicator-function-of-a-finite-subset)
  - [Sidon set](additive-combinatorics.md#sidon-set)
    - [Sliding-window upper bound for Sidon sets](additive-combinatorics.md#sliding-window-upper-bound-for-sidon-sets)
    - [Bose-Chowla Sidon construction](additive-combinatorics.md#bose-chowla-sidon-construction)
  - [Linear configuration count](additive-combinatorics.md#linear-configuration-count)
    - [Fourier stability of a linear configuration count](additive-combinatorics.md#fourier-stability-of-a-linear-configuration-count)
  - [Transference principle in additive combinatorics](additive-combinatorics.md#transference-principle-in-additive-combinatorics)
    - [Test-function seminorm](additive-combinatorics.md#test-function-seminorm)
      - [Dual test-function norm](additive-combinatorics.md#dual-test-function-norm)
    - [Dense model theorem for a multiplicative test family](additive-combinatorics.md#dense-model-theorem-for-a-multiplicative-test-family)
      - [Polynomial approximation of the positive part](additive-combinatorics.md#polynomial-approximation-of-the-positive-part)
  - [Sumset](additive-combinatorics.md#sumset)
    - [Translated Bohr neighborhood in a triple sumset](additive-combinatorics.md#translated-bohr-neighborhood-in-a-triple-sumset)
      - [Polynomial-length progression in a dense triple sumset](additive-combinatorics.md#polynomial-length-progression-in-a-dense-triple-sumset)
    - [Sum of a subset](additive-combinatorics.md#sum-of-a-subset)
    - [Distinct-positive-integer subset-sum lower bound](additive-combinatorics.md#distinct-positive-integer-subset-sum-lower-bound)
    - [Lexicographic embedding of a sumset](additive-combinatorics.md#lexicographic-embedding-of-a-sumset)
    - [Restricted sumset](additive-combinatorics.md#restricted-sumset)
    - [Plünnecke inequality](additive-combinatorics.md#plunnecke-inequality)
    - [Iterated sumset](additive-combinatorics.md#iterated-sumset)
  - [Difference set](additive-combinatorics.md#difference-set)
  - [Doubling constant](additive-combinatorics.md#doubling-constant)
    - [Polynomial growth of iterated sumsets](additive-combinatorics.md#polynomial-growth-of-iterated-sumsets)
    - [Plünnecke-Ruzsa inequality](additive-combinatorics.md#plunnecke-ruzsa-inequality)
      - [Petridis minimal-growth lemma](additive-combinatorics.md#petridis-minimal-growth-lemma)
      - [Ruzsa triangle inequality](additive-combinatorics.md#ruzsa-triangle-inequality)
        - [Noncommutative Ruzsa triangle inequality](additive-combinatorics.md#noncommutative-ruzsa-triangle-inequality)
          - [Fourfold product bound from small tripling](additive-combinatorics.md#fourfold-product-bound-from-small-tripling)
          - [Small doubling does not control tripling in a noncommutative group](additive-combinatorics.md#small-doubling-does-not-control-tripling-in-a-noncommutative-group)
    - [Freiman-Ruzsa theorem](additive-combinatorics.md#freiman-ruzsa-theorem)
      - [Freiman theorem for integer sets](additive-combinatorics.md#freiman-theorem-for-integer-sets)
      - [Freiman-Ruzsa theorem over a finite field](additive-combinatorics.md#freiman-ruzsa-theorem-over-a-finite-field)
        - [Freiman-Ruzsa bound from Bogolyubov and linear modelling](additive-combinatorics.md#freiman-ruzsa-bound-from-bogolyubov-and-linear-modelling)
        - [Injective linear modelling of a small sumset](additive-combinatorics.md#injective-linear-modelling-of-a-small-sumset)
          - [Lifting a subspace through a Freiman model](additive-combinatorics.md#lifting-a-subspace-through-a-freiman-model)
      - [Szemerédi theorem in a bounded-rank coset progression](additive-combinatorics.md#szemeredi-theorem-in-a-bounded-rank-coset-progression)
      - [Small difference set forces a three-term arithmetic progression](additive-combinatorics.md#small-difference-set-forces-a-three-term-arithmetic-progression)
  - [Approximate group](additive-combinatorics.md#approximate-group)
    - [Breuillard-Green-Tao structure theorem for approximate groups](additive-combinatorics.md#breuillard-green-tao-structure-theorem-for-approximate-groups)
    - [Higher product bound for an approximate group](additive-combinatorics.md#higher-product-bound-for-an-approximate-group)
    - [Intersection of an approximate group power with a subgroup](additive-combinatorics.md#intersection-of-an-approximate-group-power-with-a-subgroup)
    - [Large lower-step product in a torsion-free nilpotent approximate group](additive-combinatorics.md#large-lower-step-product-in-a-torsion-free-nilpotent-approximate-group)
      - [Large lifted product from a coset progression](additive-combinatorics.md#large-lifted-product-from-a-coset-progression)
        - [Fiber-counting lemma for a quotient map](additive-combinatorics.md#fiber-counting-lemma-for-a-quotient-map)
    - [Symmetric subset of a group](additive-combinatorics.md#symmetric-subset-of-a-group)
    - [Ruzsa covering lemma](additive-combinatorics.md#ruzsa-covering-lemma)
  - [Additive energy](additive-combinatorics.md#additive-energy)
    - [Additive energy controls three-term progression mixing](additive-combinatorics.md#additive-energy-controls-three-term-progression-mixing)
    - [Additive energy of a frequency graph](additive-combinatorics.md#additive-energy-of-a-frequency-graph)
      - [Derivative correlations force additive frequency energy](additive-combinatorics.md#derivative-correlations-force-additive-frequency-energy)
        - [Squared derivative correlations force frequency-graph energy](additive-combinatorics.md#squared-derivative-correlations-force-frequency-graph-energy)
    - [Polynomial progression in a high-energy fourfold difference set](additive-combinatorics.md#polynomial-progression-in-a-high-energy-fourfold-difference-set)
    - [Popular sum](additive-combinatorics.md#popular-sum)
    - [Additive quadruple](additive-combinatorics.md#additive-quadruple)
    - [Balog-Szemerédi-Gowers theorem](additive-combinatorics.md#balog-szemeredi-gowers-theorem)
      - [Graph form of the Balog-Szemerédi-Gowers theorem](additive-combinatorics.md#graph-form-of-the-balog-szemeredi-gowers-theorem)
        - [Four-step path lemma for a dense bipartite graph](additive-combinatorics.md#four-step-path-lemma-for-a-dense-bipartite-graph)
      - [Small-difference-set form of the Balog-Szemerédi-Gowers theorem](additive-combinatorics.md#small-difference-set-form-of-the-balog-szemeredi-gowers-theorem)
  - [Bogolyubov lemma](additive-combinatorics.md#bogolyubov-lemma)
    - [Cyclic Bogolyubov lemma with explicit phase radius](additive-combinatorics.md#cyclic-bogolyubov-lemma-with-explicit-phase-radius)
    - [Cyclic Bogolyubov lemma](additive-combinatorics.md#cyclic-bogolyubov-lemma)
    - [Finite-field Bogolyubov lemma](additive-combinatorics.md#finite-field-bogolyubov-lemma)
    - [Additive energy produces a large subspace in a fourfold difference set](additive-combinatorics.md#additive-energy-produces-a-large-subspace-in-a-fourfold-difference-set)
    - [Dense Bogolyubov-Ruzsa lemma](additive-combinatorics.md#dense-bogolyubov-ruzsa-lemma)
  - [Bohr set](additive-combinatorics.md#bohr-set)
    - [Progression in a Bohr set from successive minima](additive-combinatorics.md#progression-in-a-bohr-set-from-successive-minima)
    - [Bohr set in phase-distance convention](additive-combinatorics.md#bohr-set-in-phase-distance-convention)
    - [Dilate of a Bohr set](additive-combinatorics.md#dilate-of-a-bohr-set)
    - [Regular Bohr set](additive-combinatorics.md#regular-bohr-set)
    - [Lower bound for the size of a Bohr set](additive-combinatorics.md#lower-bound-for-the-size-of-a-bohr-set)
    - [Arithmetic progression in a cyclic Bohr set](additive-combinatorics.md#arithmetic-progression-in-a-cyclic-bohr-set)
      - [Nonwrapping progression in a cyclic Bohr set](additive-combinatorics.md#nonwrapping-progression-in-a-cyclic-bohr-set)
  - [Almost period of a function](additive-combinatorics.md#almost-period-of-a-function)
    - [Bohr-set almost periodicity of a convolution](additive-combinatorics.md#bohr-set-almost-periodicity-of-a-convolution)
    - [Lp almost period](additive-combinatorics.md#lp-almost-period)
      - [Finite-field convolution almost-periodicity theorem](additive-combinatorics.md#finite-field-convolution-almost-periodicity-theorem)
    - [Croot-Sisask almost-periodicity theorem](additive-combinatorics.md#croot-sisask-almost-periodicity-theorem)
    - [Finite-field character approximation](additive-combinatorics.md#finite-field-character-approximation)
  - [Normalized Fourier analysis on a finite abelian group](additive-combinatorics.md#normalized-fourier-analysis-on-a-finite-abelian-group)
    - [Large Fourier coefficient from a deficit of three-term progressions](additive-combinatorics.md#large-fourier-coefficient-from-a-deficit-of-three-term-progressions)
    - [Fourth Fourier moment bound for an indicator function](additive-combinatorics.md#fourth-fourier-moment-bound-for-an-indicator-function)
    - [Fourier coefficient on a finite abelian group](additive-combinatorics.md#fourier-coefficient-on-a-finite-abelian-group)
    - [Linear phase](additive-combinatorics.md#linear-phase)
      - [Progression partition with nearly constant linear phase](additive-combinatorics.md#progression-partition-with-nearly-constant-linear-phase)
    - [Sixth Fourier moment as a three-sum collision count](additive-combinatorics.md#sixth-fourier-moment-as-a-three-sum-collision-count)
    - [Large spectrum](additive-combinatorics.md#large-spectrum)
      - [Chang theorem](additive-combinatorics.md#chang-theorem)
      - [Dissociated set](additive-combinatorics.md#dissociated-set)
  - [Density increment](additive-combinatorics.md#density-increment)
    - [Hyperplane density increment for cap sets](additive-combinatorics.md#hyperplane-density-increment-for-cap-sets)
    - [Roth density-increment step](additive-combinatorics.md#roth-density-increment-step)
      - [One-frequency density increment on an integer interval](additive-combinatorics.md#one-frequency-density-increment-on-an-integer-interval)
      - [Fourier detection of a progression-free subset of an interval](additive-combinatorics.md#fourier-detection-of-a-progression-free-subset-of-an-interval)
    - [Bourgain bound for three-term-progression-free sets](additive-combinatorics.md#bourgain-bound-for-three-term-progression-free-sets)
      - [Bohr-set density increment lemma](additive-combinatorics.md#bohr-set-density-increment-lemma)
  - [Meshulam theorem](additive-combinatorics.md#meshulam-theorem)
  - [Finite-field Szemerédi theorem for four-term arithmetic progressions](additive-combinatorics.md#finite-field-szemeredi-theorem-for-four-term-arithmetic-progressions)
  - [Gowers uniformity norm](additive-combinatorics.md#gowers-uniformity-norm)
    - [Multiplicative derivative](additive-combinatorics.md#multiplicative-derivative)
    - [Gowers U2 norm](additive-combinatorics.md#gowers-u2-norm)
      - [Quadratic phase detection by the Gowers U2 norm](additive-combinatorics.md#quadratic-phase-detection-by-the-gowers-u2-norm)
    - [Gowers U3 norm](additive-combinatorics.md#gowers-u3-norm)
      - [Quadratic uniformity of a set](additive-combinatorics.md#quadratic-uniformity-of-a-set)
        - [Four-term progressions in a quadratically uniform interval set](additive-combinatorics.md#four-term-progressions-in-a-quadratically-uniform-interval-set)
        - [Triangular weights count genuine four-term progressions](additive-combinatorics.md#triangular-weights-count-genuine-four-term-progressions)
      - [Generalized von Neumann inequality for four-term progressions](additive-combinatorics.md#generalized-von-neumann-inequality-for-four-term-progressions)
        - [Four-term progression bound with torsion factors](additive-combinatorics.md#four-term-progression-bound-with-torsion-factors)
          - [Unbounded torsion obstructs uniform control of four-term progressions](additive-combinatorics.md#unbounded-torsion-obstructs-uniform-control-of-four-term-progressions)
      - [Gowers U3 norm on an interval](additive-combinatorics.md#gowers-u3-norm-on-an-interval)
      - [Derivative identity for the Gowers U3 norm](additive-combinatorics.md#derivative-identity-for-the-gowers-u3-norm)
    - [Gowers inner product](additive-combinatorics.md#gowers-inner-product)
      - [Gowers-Cauchy-Schwarz inequality](additive-combinatorics.md#gowers-cauchy-schwarz-inequality)
    - [Quadratic phase](additive-combinatorics.md#quadratic-phase)
    - [Inverse theorem for the Gowers U3 norm over a finite field](additive-combinatorics.md#inverse-theorem-for-the-gowers-u3-norm-over-a-finite-field)
      - [Frequency graph extracted from a large Gowers U3 norm](additive-combinatorics.md#frequency-graph-extracted-from-a-large-gowers-u3-norm)
      - [Density-increment proof of the finite-field four-term progression theorem](additive-combinatorics.md#density-increment-proof-of-the-finite-field-four-term-progression-theorem)
  - [Freiman homomorphism](additive-combinatorics.md#freiman-homomorphism)
    - [Freiman s-homomorphism](additive-combinatorics.md#freiman-s-homomorphism)
      - [Freiman s-isomorphism](additive-combinatorics.md#freiman-s-isomorphism)
        - [Freiman lifting of a progression](additive-combinatorics.md#freiman-lifting-of-a-progression)
        - [Freiman 2-isomorphism](additive-combinatorics.md#freiman-2-isomorphism)
          - [Minimal binary Freiman models have full fourfold sumset](additive-combinatorics.md#minimal-binary-freiman-models-have-full-fourfold-sumset)
      - [Ruzsa modelling lemma](additive-combinatorics.md#ruzsa-modelling-lemma)
        - [Cardinality-controlled cyclic Freiman model](additive-combinatorics.md#cardinality-controlled-cyclic-freiman-model)
        - [Cyclic Freiman model of a small-doubling integer set](additive-combinatorics.md#cyclic-freiman-model-of-a-small-doubling-integer-set)
        - [Half-size prime cyclic Freiman model](additive-combinatorics.md#half-size-prime-cyclic-freiman-model)
          - [Half-size cyclic Freiman model with a sharp difference-set bound](additive-combinatorics.md#half-size-cyclic-freiman-model-with-a-sharp-difference-set-bound)
    - [Second-difference obstruction to a Freiman homomorphism](additive-combinatorics.md#second-difference-obstruction-to-a-freiman-homomorphism)
    - [Large Freiman-homomorphic restriction from bounded derivative images](additive-combinatorics.md#large-freiman-homomorphic-restriction-from-bounded-derivative-images)
  - [Generalized arithmetic progression](additive-combinatorics.md#generalized-arithmetic-progression)
    - [Abelian progression](additive-combinatorics.md#abelian-progression)
    - [Coset progression](additive-combinatorics.md#coset-progression)
- [Directed acyclic graph](#directed-acyclic-graph)
  - [Topological sorting](#topological-sorting)
    - [Topological order](#topological-order)
  - [Markov equivalence of directed acyclic graphs](#markov-equivalence-of-directed-acyclic-graphs)
    - [Completed partially directed acyclic graph](#completed-partially-directed-acyclic-graph)
    - [Skeleton and collider characterization of Markov equivalence](#skeleton-and-collider-characterization-of-markov-equivalence)
  - [Moral graph](#moral-graph)
    - [Hammersley-Clifford theorem](#hammersley-clifford-theorem)
  - [Topological ordering](#topological-ordering)
  - [D-separation](#d-separation)
    - [Collider](#collider)
      - [Unshielded collider](#unshielded-collider)
    - [D-separating set](#d-separating-set)
    - [Local Markov property of a directed acyclic graph](#local-markov-property-of-a-directed-acyclic-graph)
    - [Global Markov property of a directed acyclic graph](#global-markov-property-of-a-directed-acyclic-graph)
- [Incidence geometry](#incidence-geometry)
  - [Linear space (geometry)](#linear-space-geometry)
  - [Joint of a line collection](#joint-of-a-line-collection)
    - [Joints theorem](#joints-theorem)
      - [Pruning and minimal-degree polynomial argument](#pruning-and-minimal-degree-polynomial-argument)
  - [Kakeya set](#kakeya-set)
    - [Besicovitch set](#besicovitch-set)
      - [Compact Kakeya construction from small projections](#compact-kakeya-construction-from-small-projections)
      - [Perron tree](#perron-tree)
    - [Kakeya Minkowski dimension conjecture](#kakeya-minkowski-dimension-conjecture)
    - [Kakeya tube](#kakeya-tube)
  - [Ordinary line](#ordinary-line)
    - [Cubic covering from few ordinary lines](#cubic-covering-from-few-ordinary-lines)
  - [Distinct-distance set](#distinct-distance-set)
    - [Székely distinct-distance bound](#szekely-distinct-distance-bound)
      - [Circular-arc graph for distinct distances](#circular-arc-graph-for-distinct-distances)
        - [Rich-bisector deletion bound](#rich-bisector-deletion-bound)
    - [Unit-circle method for a distinct-distance lower bound](#unit-circle-method-for-a-distinct-distance-lower-bound)
  - [Incidences between points and curves](#incidences-between-points-and-curves)
    - [Incidence bound from two-point multiplicity](#incidence-bound-from-two-point-multiplicity)
  - [Szemerédi–Trotter theorem](#szemeredi-trotter-theorem)
    - [Rich line bound](#rich-line-bound)
    - [Szemerédi–Trotter theorem for unit circles](#szemeredi-trotter-theorem-for-unit-circles)
    - [Incidences between points and polynomial graphs](#incidences-between-points-and-polynomial-graphs)
- [Degree-sum formula](#degree-sum-formula)
- [Tree (graph theory)](#tree-graph-theory)
  - [Regular tree](#regular-tree)
    - [Edge boundary of a finite forest in a regular tree](#edge-boundary-of-a-finite-forest-in-a-regular-tree)
  - [Oriented tree](#oriented-tree)
    - [Three-times-order tournament bound for oriented trees](#three-times-order-tournament-bound-for-oriented-trees)
    - [Arborescence (graph theory)](#arborescence-graph-theory)
  - [Depth-first traversal of a tree](#depth-first-traversal-of-a-tree)
  - [Rooted tree](#rooted-tree)
    - [Rooted-tree generating function](#rooted-tree-generating-function)
    - [Homeomorphic embedding of a rooted tree](#homeomorphic-embedding-of-a-rooted-tree)
      - [Natural-sum ordinal rank of a finite rooted tree](#natural-sum-ordinal-rank-of-a-finite-rooted-tree)
      - [Adjacency-preserving rooted-tree embedding](#adjacency-preserving-rooted-tree-embedding)
        - [Branching-depth antichain of rooted trees](#branching-depth-antichain-of-rooted-trees)
      - [Label-monotone tree embedding](#label-monotone-tree-embedding)
    - [Lowest common ancestor](#lowest-common-ancestor)
    - [Recursively repetition-free labelled tree](#recursively-repetition-free-labelled-tree)
      - [Recursively repetition-free labelled trees preserve Dedekind-finiteness](#recursively-repetition-free-labelled-trees-preserve-dedekind-finiteness)
    - [Section of a rooted-tree automorphism](#section-of-a-rooted-tree-automorphism)
  - [Forest](#forest)
    - [Two-component spanning forest](#two-component-spanning-forest)
  - [Spanning tree](#spanning-tree)
    - [Fundamental cycle](#fundamental-cycle)
    - [Minimum spanning tree](#minimum-spanning-tree)
      - [Reverse-delete algorithm](#reverse-delete-algorithm)
      - [Kruskal's algorithm](#kruskal-s-algorithm)
      - [Prim's algorithm](#prim-s-algorithm)
      - [Minimum spanning tree cycle property](#minimum-spanning-tree-cycle-property)
      - [Minimum spanning tree cut property](#minimum-spanning-tree-cut-property)
    - [Uniform spanning tree](#uniform-spanning-tree)
      - [Uniform spanning tree of a recurrent infinite graph](#uniform-spanning-tree-of-a-recurrent-infinite-graph)
      - [Uniform spanning forest](#uniform-spanning-forest)
      - [Free uniform spanning forest](#free-uniform-spanning-forest)
        - [Negative association of uniform spanning-tree edges](#negative-association-of-uniform-spanning-tree-edges)
      - [Transfer-current theorem](#transfer-current-theorem)
        - [Mean spanning-tree path current](#mean-spanning-tree-path-current)
        - [Edge-inclusion formula for a uniform spanning tree](#edge-inclusion-formula-for-a-uniform-spanning-tree)
      - [Translation ergodicity of a uniform spanning forest](#translation-ergodicity-of-a-uniform-spanning-forest)
      - [Aldous-Broder algorithm](#aldous-broder-algorithm)
      - [Wilson's algorithm](#wilson-s-algorithm)
      - [Wired uniform spanning forest](#wired-uniform-spanning-forest)
        - [Wilson algorithm rooted at infinity](#wilson-algorithm-rooted-at-infinity)
        - [Component-number zero-one law for the wired uniform spanning forest](#component-number-zero-one-law-for-the-wired-uniform-spanning-forest)
    - [Directed spanning tree](#directed-spanning-tree)
    - [Kirchhoff's theorem](#kirchhoff-s-theorem)
  - [Cayley's formula](#cayley-s-formula)
    - [Labelled forest count with prescribed roots](#labelled-forest-count-with-prescribed-roots)
    - [Prüfer sequence](#prufer-sequence)
  - [Kőnig's lemma](#konig-s-lemma)
  - [Breadth-first search](#breadth-first-search)
- [Double counting (proof technique)](#double-counting-proof-technique)
- [Set partition](#set-partition)
  - [Refinement of a set partition](#refinement-of-a-set-partition)
  - [Integer partition](#integer-partition)
  - [Stirling numbers of the second kind](#stirling-numbers-of-the-second-kind)
    - [Graphical Stirling number](#graphical-stirling-number)
- [Lattice path](#lattice-path)
  - [Self-avoiding walk](#self-avoiding-walk)
    - [Partially directed self-avoiding walk](#partially-directed-self-avoiding-walk)
      - [North-east-west self-avoiding walk count](#north-east-west-self-avoiding-walk-count)
    - [Self-avoiding walk generating function](#self-avoiding-walk-generating-function)
      - [Even-length walk generating function on a bipartite graph](#even-length-walk-generating-function-on-a-bipartite-graph)
        - [Triangle replacement for self-avoiding walks](#triangle-replacement-for-self-avoiding-walks)
    - [Root-moment bound for open self-avoiding walks](#root-moment-bound-for-open-self-avoiding-walks)
    - [Directed ladder self-avoiding walk count](#directed-ladder-self-avoiding-walk-count)
    - [Connective constant](#connective-constant)
      - [Uniform connective constant of a bounded-degree graph](#uniform-connective-constant-of-a-bounded-degree-graph)
  - [Dyck path](#dyck-path)
    - [Catalan number](#catalan-number)
- [Extremal set theory](extremal-set-theory.md)
  - [Eventown theorem](extremal-set-theory.md#eventown-theorem)
  - [Oddtown theorem](extremal-set-theory.md#oddtown-theorem)
  - [Separating set system](extremal-set-theory.md#separating-set-system)
  - [Large family avoiding a high intersection](extremal-set-theory.md#large-family-avoiding-a-high-intersection)
  - [Forbidden-intersection density increment](extremal-set-theory.md#forbidden-intersection-density-increment)
    - [Quantitative forbidden-intersection bound by widening](extremal-set-theory.md#quantitative-forbidden-intersection-bound-by-widening)
  - [Effective ground-set parameter of a hereditary uniform layer](extremal-set-theory.md#effective-ground-set-parameter-of-a-hereditary-uniform-layer)
    - [Shadow ratio for a hereditary set family](extremal-set-theory.md#shadow-ratio-for-a-hereditary-set-family)
  - [Coordinate shifts of a set family](extremal-set-theory.md#coordinate-shifts-of-a-set-family)
    - [Downward coordinate compression](extremal-set-theory.md#downward-coordinate-compression)
      - [Two cube edges in every direction force many vertices](extremal-set-theory.md#two-cube-edges-in-every-direction-force-many-vertices)
    - [Coordinate-shift shadow containment](extremal-set-theory.md#coordinate-shift-shadow-containment)
  - [Constant-intersection family bound](extremal-set-theory.md#constant-intersection-family-bound)
    - [Constant t-wise intersection dichotomy](extremal-set-theory.md#constant-t-wise-intersection-dichotomy)
      - [Complement-of-singleton extremizers](extremal-set-theory.md#complement-of-singleton-extremizers)
  - [Elementary set shift](extremal-set-theory.md#elementary-set-shift)
    - [Shifted set family](extremal-set-theory.md#shifted-set-family)
      - [Ballot reflection injection](extremal-set-theory.md#ballot-reflection-injection)
  - [Odd cross-intersection bound](extremal-set-theory.md#odd-cross-intersection-bound)
  - [Even cross-intersection bound](extremal-set-theory.md#even-cross-intersection-bound)
  - [Weakly intersecting family in a product alphabet](extremal-set-theory.md#weakly-intersecting-family-in-a-product-alphabet)
  - [Bollobas set-pairs inequality](extremal-set-theory.md#bollobas-set-pairs-inequality)
  - [Separating family of disjoint set pairs](extremal-set-theory.md#separating-family-of-disjoint-set-pairs)
    - [Disjoint subcube packing inequality](extremal-set-theory.md#disjoint-subcube-packing-inequality)
  - [Symmetric chain decomposition of a Boolean lattice](extremal-set-theory.md#symmetric-chain-decomposition-of-a-boolean-lattice)
    - [Symmetric chain in a Boolean lattice](extremal-set-theory.md#symmetric-chain-in-a-boolean-lattice)
    - [Adjacent-level matching in a Boolean lattice](extremal-set-theory.md#adjacent-level-matching-in-a-boolean-lattice)
    - [Minimum chain partition of a Boolean lattice](extremal-set-theory.md#minimum-chain-partition-of-a-boolean-lattice)
  - [Lexicographic order](extremal-set-theory.md#lexicographic-order)
  - [Colexicographic order](extremal-set-theory.md#colexicographic-order)
    - [Colexicographic initial segment](extremal-set-theory.md#colexicographic-initial-segment)
  - [Set family shadow](extremal-set-theory.md#set-family-shadow)
    - [Lower shadow](extremal-set-theory.md#lower-shadow)
      - [Iterated lower shadow](extremal-set-theory.md#iterated-lower-shadow)
        - [Clique counting from iterated shadows](extremal-set-theory.md#clique-counting-from-iterated-shadows)
      - [Kruskal-Katona theorem](extremal-set-theory.md#kruskal-katona-theorem)
        - [Nonisomorphic colex shadow minimizers](extremal-set-theory.md#nonisomorphic-colex-shadow-minimizers)
        - [Lovász shadow bound](extremal-set-theory.md#lovasz-shadow-bound)
        - [Colexicographic section compression](extremal-set-theory.md#colexicographic-section-compression)
        - [Binomial-shadow arithmetic lemma](extremal-set-theory.md#binomial-shadow-arithmetic-lemma)
        - [UV-compression](extremal-set-theory.md#uv-compression)
          - [Intersection-preserving lexicographic UV-compression](extremal-set-theory.md#intersection-preserving-lexicographic-uv-compression)
          - [Left-compressed set family](extremal-set-theory.md#left-compressed-set-family)
          - [Shadow lemma for UV-compressions](extremal-set-theory.md#shadow-lemma-for-uv-compressions)
        - [UV-compression proof of the Kruskal-Katona theorem](extremal-set-theory.md#uv-compression-proof-of-the-kruskal-katona-theorem)
    - [Upper shadow](extremal-set-theory.md#upper-shadow)
  - [Frankl-Wilson theorem](extremal-set-theory.md#frankl-wilson-theorem)
    - [Modular intersection graph](extremal-set-theory.md#modular-intersection-graph)
    - [Modular intersection polynomial](extremal-set-theory.md#modular-intersection-polynomial)
    - [Complement splitting for forbidden midpoint intersections](extremal-set-theory.md#complement-splitting-for-forbidden-midpoint-intersections)
      - [Fixed-core construction avoiding midpoint intersections](extremal-set-theory.md#fixed-core-construction-avoiding-midpoint-intersections)
    - [Prime-power modular intersection bound](extremal-set-theory.md#prime-power-modular-intersection-bound)
    - [Modular-size auxiliary polynomials](extremal-set-theory.md#modular-size-auxiliary-polynomials)
    - [Modular layer vanishing lemma](extremal-set-theory.md#modular-layer-vanishing-lemma)
    - [Nonuniform Frankl-Wilson theorem](extremal-set-theory.md#nonuniform-frankl-wilson-theorem)
    - [Ray-Chaudhuri–Wilson theorem](extremal-set-theory.md#ray-chaudhuri-wilson-theorem)
  - [Set family](extremal-set-theory.md#set-family)
    - [Helly family](extremal-set-theory.md#helly-family)
    - [Incidence matrix of a set system](extremal-set-theory.md#incidence-matrix-of-a-set-system)
    - [Diagonal-intersection set-pair bound](extremal-set-theory.md#diagonal-intersection-set-pair-bound)
    - [Union and intersection of set families](extremal-set-theory.md#union-and-intersection-of-set-families)
    - [Ahlswede–Daykin inequality](extremal-set-theory.md#ahlswede-daykin-inequality)
      - [Two-point four-functions inequality](extremal-set-theory.md#two-point-four-functions-inequality)
    - [Biased measure of a set family](extremal-set-theory.md#biased-measure-of-a-set-family)
    - [Self-dual set family](extremal-set-theory.md#self-dual-set-family)
      - [Complementary-layer bound for biased measure](extremal-set-theory.md#complementary-layer-bound-for-biased-measure)
        - [Weighted Bernoulli majority bound](extremal-set-theory.md#weighted-bernoulli-majority-bound)
    - [Laminar family of sets](extremal-set-theory.md#laminar-family-of-sets)
    - [Union-intersection compression](extremal-set-theory.md#union-intersection-compression)
    - [Cross-Sperner family](extremal-set-theory.md#cross-sperner-family)
    - [Hitting set](extremal-set-theory.md#hitting-set)
      - [Bounded-size transversal kernel](extremal-set-theory.md#bounded-size-transversal-kernel)
    - [Boolean lattice](extremal-set-theory.md#boolean-lattice)
      - [Kleitman diametric theorem](extremal-set-theory.md#kleitman-diametric-theorem)
      - [Injectivity of inclusion between adjacent set layers](extremal-set-theory.md#injectivity-of-inclusion-between-adjacent-set-layers)
      - [Up-set](extremal-set-theory.md#up-set)
      - [Down-set](extremal-set-theory.md#down-set)
        - [Edge boundary of a down-set in a cube](extremal-set-theory.md#edge-boundary-of-a-down-set-in-a-cube)
          - [Largest edge boundary of a down-set](extremal-set-theory.md#largest-edge-boundary-of-a-down-set)
        - [Downward closure of a set family](extremal-set-theory.md#downward-closure-of-a-set-family)
      - [Antichain](extremal-set-theory.md#antichain)
        - [Maximal chain in a Boolean lattice](extremal-set-theory.md#maximal-chain-in-a-boolean-lattice)
          - [Uniformly random maximal chain in a Boolean lattice](extremal-set-theory.md#uniformly-random-maximal-chain-in-a-boolean-lattice)
        - [Lubell-Yamamoto-Meshalkin inequality](extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality)
          - [Equality in the LYM inequality](extremal-set-theory.md#equality-in-the-lym-inequality)
          - [Lubell mass](extremal-set-theory.md#lubell-mass)
          - [Local LYM inequality](extremal-set-theory.md#local-lym-inequality)
            - [Connectedness of adjacent-level incidence in a Boolean lattice](extremal-set-theory.md#connectedness-of-adjacent-level-incidence-in-a-boolean-lattice)
            - [Iterated local LYM inequality](extremal-set-theory.md#iterated-local-lym-inequality)
          - [Sperner's theorem](extremal-set-theory.md#sperner-s-theorem)
            - [Littlewood-Offord inequality](extremal-set-theory.md#littlewood-offord-inequality)
              - [Two-level Littlewood-Offord bound](extremal-set-theory.md#two-level-littlewood-offord-bound)
              - [Separated block decomposition for vector subset sums](extremal-set-theory.md#separated-block-decomposition-for-vector-subset-sums)
            - [Equality in Sperner theorem](extremal-set-theory.md#equality-in-sperner-theorem)
        - [k-Sperner family](extremal-set-theory.md#k-sperner-family)
          - [Weighted theorem for k-Sperner families](extremal-set-theory.md#weighted-theorem-for-k-sperner-families)
            - [Number of maximizing weighted k-Sperner families](extremal-set-theory.md#number-of-maximizing-weighted-k-sperner-families)
          - [Erdős theorem on k-Sperner families](extremal-set-theory.md#erdos-theorem-on-k-sperner-families)
        - [Cross-Sperner inequality](extremal-set-theory.md#cross-sperner-inequality)
          - [Two-block extremisers for the cross-Sperner inequality](extremal-set-theory.md#two-block-extremisers-for-the-cross-sperner-inequality)
    - [Characteristic vector of a set](extremal-set-theory.md#characteristic-vector-of-a-set)
      - [Modular intersection method for set families](extremal-set-theory.md#modular-intersection-method-for-set-families)
    - [Incidence graph](extremal-set-theory.md#incidence-graph)
    - [Trace of a set family](extremal-set-theory.md#trace-of-a-set-family)
      - [Set shattering](extremal-set-theory.md#set-shattering)
        - [Unbounded finite shattering without an infinite universal trace](extremal-set-theory.md#unbounded-finite-shattering-without-an-infinite-universal-trace)
      - [Shearer trace inequality](extremal-set-theory.md#shearer-trace-inequality)
    - [Union-closed family](extremal-set-theory.md#union-closed-family)
      - [Union-closed sets conjecture](extremal-set-theory.md#union-closed-sets-conjecture)
        - [Binary entropy product inequality](extremal-set-theory.md#binary-entropy-product-inequality)
        - [Entropy bound for a union-closed family](extremal-set-theory.md#entropy-bound-for-a-union-closed-family)
    - [Entropy bound for pairwise-union tuples](extremal-set-theory.md#entropy-bound-for-pairwise-union-tuples)
    - [Intersecting family](extremal-set-theory.md#intersecting-family)
      - [Union bound for intersecting families](extremal-set-theory.md#union-bound-for-intersecting-families)
      - [Colexicographic replacement can destroy intersection](extremal-set-theory.md#colexicographic-replacement-can-destroy-intersection)
      - [Lexicographic initial segments preserve ordinary intersection](extremal-set-theory.md#lexicographic-initial-segments-preserve-ordinary-intersection)
      - [Maximal intersecting families choose one member of every complementary pair](extremal-set-theory.md#maximal-intersecting-families-choose-one-member-of-every-complementary-pair)
      - [t-intersecting family](extremal-set-theory.md#t-intersecting-family)
        - [Lexicographic replacement can destroy two-intersection](extremal-set-theory.md#lexicographic-replacement-can-destroy-two-intersection)
        - [Maximal intersection does not imply maximum size](extremal-set-theory.md#maximal-intersection-does-not-imply-maximum-size)
        - [Nonuniform t-intersecting family bound](extremal-set-theory.md#nonuniform-t-intersecting-family-bound)
        - [Ahlswede-Khachatrian theorem](extremal-set-theory.md#ahlswede-khachatrian-theorem)
        - [Complementation of uniform intersecting families](extremal-set-theory.md#complementation-of-uniform-intersecting-families)
        - [Complete-intersection candidate family](extremal-set-theory.md#complete-intersection-candidate-family)
      - [Intersecting two-element set family](extremal-set-theory.md#intersecting-two-element-set-family)
      - [Witness-pair concentration for an intersecting uniform family](extremal-set-theory.md#witness-pair-concentration-for-an-intersecting-uniform-family)
      - [Two-intersecting family](extremal-set-theory.md#two-intersecting-family)
        - [Pair-cover bound for a two-intersecting uniform family](extremal-set-theory.md#pair-cover-bound-for-a-two-intersecting-uniform-family)
        - [Nonuniform two-intersecting family bound](extremal-set-theory.md#nonuniform-two-intersecting-family-bound)
      - [Intersecting shadow lemma](extremal-set-theory.md#intersecting-shadow-lemma)
      - [Weighted intersecting family bound on an odd Boolean lattice](extremal-set-theory.md#weighted-intersecting-family-bound-on-an-odd-boolean-lattice)
      - [Intersecting family in a product alphabet](extremal-set-theory.md#intersecting-family-in-a-product-alphabet)
      - [Exactly one-intersecting family](extremal-set-theory.md#exactly-one-intersecting-family)
        - [Finite linear space](extremal-set-theory.md#finite-linear-space)
          - [De Bruijn--Erdos pair-covering inequality](extremal-set-theory.md#de-bruijn-erdos-pair-covering-inequality)
          - [Near-pencil](extremal-set-theory.md#near-pencil)
          - [Finite projective plane](extremal-set-theory.md#finite-projective-plane)
      - [Cross-intersecting family](extremal-set-theory.md#cross-intersecting-family)
        - [Finite intersection witness for cross-intersecting families](extremal-set-theory.md#finite-intersection-witness-for-cross-intersecting-families)
      - [Upward closure of a set family](extremal-set-theory.md#upward-closure-of-a-set-family)
      - [Dinur-Friedgut junta theorem for intersecting families](extremal-set-theory.md#dinur-friedgut-junta-theorem-for-intersecting-families)
    - [Uniform set family](extremal-set-theory.md#uniform-set-family)
      - [Generating family for a uniform set family](extremal-set-theory.md#generating-family-for-a-uniform-set-family)
        - [Tight pairs of left-compressed generators](extremal-set-theory.md#tight-pairs-of-left-compressed-generators)
        - [Maximum-support generator fibre](extremal-set-theory.md#maximum-support-generator-fibre)
        - [Compatibility bound for complementary generating families](extremal-set-theory.md#compatibility-bound-for-complementary-generating-families)
        - [Small-support generating lemma for extremal intersecting families](extremal-set-theory.md#small-support-generating-lemma-for-extremal-intersecting-families)
          - [Generator replacement proof of the small-support intersection lemma](extremal-set-theory.md#generator-replacement-proof-of-the-small-support-intersection-lemma)
      - [Intersection-free uniform set family](extremal-set-theory.md#intersection-free-uniform-set-family)
        - [Antichain trace bound for intersection-free families](extremal-set-theory.md#antichain-trace-bound-for-intersection-free-families)
      - [Uniform layer of the Boolean cube](extremal-set-theory.md#uniform-layer-of-the-boolean-cube)
        - [Low-degree evaluation rank on a uniform layer](extremal-set-theory.md#low-degree-evaluation-rank-on-a-uniform-layer)
      - [Erdős-Ko-Rado theorem](extremal-set-theory.md#erdos-ko-rado-theorem)
        - [Erdős-Ko-Rado theorem from shadows](extremal-set-theory.md#erdos-ko-rado-theorem-from-shadows)
        - [Katona circle method](extremal-set-theory.md#katona-circle-method)
          - [Cyclic interval antichain bound](extremal-set-theory.md#cyclic-interval-antichain-bound)
          - [Cyclic interval intersection bound](extremal-set-theory.md#cyclic-interval-intersection-bound)
      - [Steiner triple system](extremal-set-theory.md#steiner-triple-system)
- [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)
  - [Rich line covering bound over a finite field](#rich-line-covering-bound-over-a-finite-field)
  - [Schwartz-Zippel lemma](#schwartz-zippel-lemma)
  - [Polynomial vanishing on a finite set of spatial lines](#polynomial-vanishing-on-a-finite-set-of-spatial-lines)
  - [Intersection polynomial](#intersection-polynomial)
  - [Zero-sum sequences as differences of permutations of a prime field](#zero-sum-sequences-as-differences-of-permutations-of-a-prime-field)
  - [Polynomial nonvanishing below the field size](#polynomial-nonvanishing-below-the-field-size)
  - [Cap set](#cap-set)
    - [Meshulam bound for cap sets](#meshulam-bound-for-cap-sets)
    - [Cartesian powers of cap sets](#cartesian-powers-of-cap-sets)
      - [Removal of an exponential prefactor by Cartesian powers](#removal-of-an-exponential-prefactor-by-cartesian-powers)
    - [Ellenberg–Gijswijt cap-set bound](#ellenberg-gijswijt-cap-set-bound)
      - [Low-degree monomial count for the cap-set bound](#low-degree-monomial-count-for-the-cap-set-bound)
  - [Chevalley-Warning theorem](#chevalley-warning-theorem)
    - [Kemnitz theorem](#kemnitz-theorem)
  - [Dyson constant-term identity](#dyson-constant-term-identity)
    - [Good recurrence for the Dyson constant term](#good-recurrence-for-the-dyson-constant-term)
  - [Snevily matching theorem for an elementary abelian group](#snevily-matching-theorem-for-an-elementary-abelian-group)
  - [Alon-Tarsi lemma](#alon-tarsi-lemma)
    - [Combinatorial Nullstellensatz](#combinatorial-nullstellensatz)
      - [Restricted sumset bound for unequal subsets of a prime field](#restricted-sumset-bound-for-unequal-subsets-of-a-prime-field)
      - [Prime-regular subgraph from Boolean polynomial constraints](#prime-regular-subgraph-from-boolean-polynomial-constraints)
      - [Coordinate avoidance from a nonzero permanent](#coordinate-avoidance-from-a-nonzero-permanent)
  - [Modular intersection bound for a set family](#modular-intersection-bound-for-a-set-family)
- [Factorial](#factorial)
  - [Double factorial](#double-factorial)
  - [Falling factorial](#falling-factorial)
  - [Rising factorial](#rising-factorial)
- [Binomial coefficient](#binomial-coefficient)
  - [Vandermonde's identity](#vandermonde-s-identity)
  - [Nested-subset binomial identity](#nested-subset-binomial-identity)
  - [Prime-row binomial coefficient divisibility](#prime-row-binomial-coefficient-divisibility)
    - [Binomial coefficient congruence across a prime row](#binomial-coefficient-congruence-across-a-prime-row)
  - [Gaussian binomial coefficient](#gaussian-binomial-coefficient)
    - [Unimodality of Gaussian binomial coefficients](#unimodality-of-gaussian-binomial-coefficients)
    - [Symmetric quantum binomial coefficient](#symmetric-quantum-binomial-coefficient)
  - [Pascal's triangle](#pascal-s-triangle)
  - [Hockey-stick identity](#hockey-stick-identity)
  - [Lucas's theorem](#lucas-s-theorem)
  - [Prime-power binomial divisibility](#prime-power-binomial-divisibility)
  - [Binomial coefficients with even interior terms](#binomial-coefficients-with-even-interior-terms)
  - [Combinatorial number system](#combinatorial-number-system)
  - [Pascal's rule](#pascal-s-rule)
  - [Central binomial coefficient](#central-binomial-coefficient)
    - [Normalized central binomial coefficients](#normalized-central-binomial-coefficients)
  - [Multinomial coefficient](#multinomial-coefficient)
    - [Multinomial theorem](#multinomial-theorem)
  - [Binomial theorem](#binomial-theorem)
    - [Binomial inversion](#binomial-inversion)
    - [Alternating binomial moment](#alternating-binomial-moment)
    - [Freshman's dream](#freshman-s-dream)
    - [Binomial theorem for commuting matrices](#binomial-theorem-for-commuting-matrices)
    - [Alternating binomial-square sum](#alternating-binomial-square-sum)
- [Alternating-permutation convolution](#alternating-permutation-convolution)
- [Overlap structure of digit spalindromes](#overlap-structure-of-digit-spalindromes)
- [Stars and bars (combinatorics)](#stars-and-bars-combinatorics)
  - [Bounded weak compositions](#bounded-weak-compositions)
- [Inclusion-exclusion principle](#inclusion-exclusion-principle)
  - [Weighted inclusion-exclusion principle](#weighted-inclusion-exclusion-principle)
  - [Inclusion-exclusion for exact block occupancy](#inclusion-exclusion-for-exact-block-occupancy)
  - [Cyclic difference constraints](#cyclic-difference-constraints)
  - [Bonferroni inequalities](#bonferroni-inequalities)
    - [Jordan-Bonferroni exact-occurrence inequalities](#jordan-bonferroni-exact-occurrence-inequalities)
- [Geometric combinatorics](#geometric-combinatorics)
  - [Euclidean body](#euclidean-body)
    - [Axis-parallel box](#axis-parallel-box)
    - [Coordinate projection of a Euclidean body](#coordinate-projection-of-a-euclidean-body)
      - [Uniform cover](#uniform-cover)
        - [Fractional uniform cover](#fractional-uniform-cover)
        - [Uniform covers theorem](#uniform-covers-theorem)
          - [Box theorem](#box-theorem)
            - [Logarithmic linear program for the box theorem](#logarithmic-linear-program-for-the-box-theorem)
          - [Loomis--Whitney inequality](#loomis-whitney-inequality)
            - [Functional Loomis-Whitney inequality](#functional-loomis-whitney-inequality)
            - [Three projection areas of a volume-one body](#three-projection-areas-of-a-volume-one-body)
            - [Equality in the three-dimensional Loomis--Whitney inequality](#equality-in-the-three-dimensional-loomis-whitney-inequality)
        - [Irreducible uniform cover](#irreducible-uniform-cover)
          - [Dickson's lemma](#dickson-s-lemma)
- [Grid graph](#grid-graph)
  - [Small-set edge isoperimetry in a square grid](#small-set-edge-isoperimetry-in-a-square-grid)
  - [Vertex-isoperimetric inequality in a grid](#vertex-isoperimetric-inequality-in-a-grid)
    - [Simplicial order on a grid](#simplicial-order-on-a-grid)
    - [Coordinate compression in a product of paths](#coordinate-compression-in-a-product-of-paths)
      - [Section formula for a grid neighbourhood](#section-formula-for-a-grid-neighbourhood)
    - [Local-to-global lemma for simplicial grid order](#local-to-global-lemma-for-simplicial-grid-order)
  - [Gray-code path embedding of a grid in a hypercube](#gray-code-path-embedding-of-a-grid-in-a-hypercube)
- [Necklace (combinatorics)](#necklace-combinatorics)
  - [Coloring bracelet](#coloring-bracelet)
- [Permutation](#permutation)
  - [Cyclic permutation](#cyclic-permutation)
  - [Finitely supported permutation](#finitely-supported-permutation)
  - [Uniform random permutation](#uniform-random-permutation)
    - [Independent relative ranks of a uniform random permutation](#independent-relative-ranks-of-a-uniform-random-permutation)
      - [Independent record indicators](#independent-record-indicators)
  - [Cycle length of a tagged element in a uniform permutation](#cycle-length-of-a-tagged-element-in-a-uniform-permutation)
  - [Derangement of a permutation](#derangement-of-a-permutation)
    - [Fixed point count of a uniform random permutation](#fixed-point-count-of-a-uniform-random-permutation)
  - [Cyclic ordering](#cyclic-ordering)
    - [Cyclic interval](#cyclic-interval)
  - [Generalised permutation](#generalised-permutation)
  - [Inversion of a permutation](#inversion-of-a-permutation)
  - [Transposition (permutation)](#transposition-permutation)
  - [Product of two transpositions](#product-of-two-transpositions)
  - [Bounded-displacement permutation of the natural numbers](#bounded-displacement-permutation-of-the-natural-numbers)
- [Analysis of Boolean functions](#analysis-of-boolean-functions)
  - [Friedgut-Kalai sharp threshold theorem](#friedgut-kalai-sharp-threshold-theorem)
  - [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem)
    - [Maximum-influence logarithmic lower bound](#maximum-influence-logarithmic-lower-bound)
    - [Squared-influence logarithmic lower bound](#squared-influence-logarithmic-lower-bound)
  - [Boolean hypercube](#boolean-hypercube)
    - [Face of the Boolean hypercube](#face-of-the-boolean-hypercube)
    - [Simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube)
      - [Complementary-size simplicial vertex boundaries can be asymmetric](#complementary-size-simplicial-vertex-boundaries-can-be-asymmetric)
      - [Simplicial vertex boundaries need not increase below half volume](#simplicial-vertex-boundaries-need-not-increase-below-half-volume)
    - [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)
      - [Half-cube vertex-boundary extrema](#half-cube-vertex-boundary-extrema)
      - [Cross-intersection bound from cube separation](#cross-intersection-bound-from-cube-separation)
      - [Nonunique down-set extremizers for Harper theorem](#nonunique-down-set-extremizers-for-harper-theorem)
      - [Simplicial section compression](#simplicial-section-compression)
        - [Terminal families for simplicial section compression](#terminal-families-for-simplicial-section-compression)
      - [Harper theorem implies the Kruskal-Katona theorem](#harper-theorem-implies-the-kruskal-katona-theorem)
    - [Binary order on the discrete cube](#binary-order-on-the-discrete-cube)
      - [Section compression in binary order](#section-compression-in-binary-order)
        - [Families compressed in every binary section](#families-compressed-in-every-binary-section)
      - [Binary initial segment](#binary-initial-segment)
      - [Binary digit-sum inequality](#binary-digit-sum-inequality)
    - [Edge boundary in a graph](#edge-boundary-in-a-graph)
      - [Isoperimetric number of a graph](#isoperimetric-number-of-a-graph)
      - [Edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube)
        - [Entropy proof of cube edge-isoperimetry](#entropy-proof-of-cube-edge-isoperimetry)
          - [Equality cases of entropy cube edge-isoperimetry](#equality-cases-of-entropy-cube-edge-isoperimetry)
        - [Edge-isoperimetric theorem for binary initial segments](#edge-isoperimetric-theorem-for-binary-initial-segments)
          - [Binary initial segments maximize contained square faces](#binary-initial-segments-maximize-contained-square-faces)
        - [Binary entropy function](#binary-entropy-function)
    - [Boolean function](#boolean-function)
      - [Quite fair Boolean function](#quite-fair-boolean-function)
      - [Algebraic normal form](#algebraic-normal-form)
      - [Separated Boolean decomposition](#separated-boolean-decomposition)
      - [Random restriction of a Boolean function](#random-restriction-of-a-boolean-function)
      - [Tribes function](#tribes-function)
        - [Balanced tribes construction with unused coordinates](#balanced-tribes-construction-with-unused-coordinates)
        - [Tribes threshold window](#tribes-threshold-window)
      - [Block sensitivity](#block-sensitivity)
      - [Monotone Boolean function](#monotone-boolean-function)
      - [Fourier-Walsh transform](#fourier-walsh-transform)
        - [Fourier weight](#fourier-weight)
          - [Expected Fourier weight after a random restriction](#expected-fourier-weight-after-a-random-restriction)
        - [Coordinate-flip generator on a hypercube](#coordinate-flip-generator-on-a-hypercube)
          - [Even-function spectral gap on a hypercube](#even-function-spectral-gap-on-a-hypercube)
        - [Walsh character](#walsh-character)
        - [p-biased product measure](#p-biased-product-measure)
          - [p-biased Fourier coefficient](#p-biased-fourier-coefficient)
        - [Discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function)
          - [Influence of a variable](#influence-of-a-variable)
            - [Hypercontractive weighted influence bound](#hypercontractive-weighted-influence-bound)
            - [Total influence](#total-influence)
              - [Margulis–Russo formula](#margulis-russo-formula)
                - [Pivotal for an increasing event](#pivotal-for-an-increasing-event)
        - [Noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube)
          - [Beckner's inequality](#beckner-s-inequality)
            - [Low-degree Fourier mass of a sparse Boolean set](#low-degree-fourier-mass-of-a-sparse-boolean-set)
          - [Noise stability](#noise-stability)
        - [Linear Fourier weight](#linear-fourier-weight)
      - [Junta](#junta)
        - [Friedgut junta inequality](#friedgut-junta-inequality)
          - [Friedgut junta theorem](#friedgut-junta-theorem)
        - [Nisan-Szegedy junta theorem](#nisan-szegedy-junta-theorem)
      - [Quasirandom Boolean function](#quasirandom-boolean-function)
        - [Regularity lemma for Boolean functions](#regularity-lemma-for-boolean-functions)
  - [Bonami lemma](#bonami-lemma)
    - [Hypercontractive inequality on the Boolean hypercube](#hypercontractive-inequality-on-the-boolean-hypercube)
    - [Anticoncentration of a low-degree function](#anticoncentration-of-a-low-degree-function)
  - [Arrow's impossibility theorem](#arrow-s-impossibility-theorem)
    - [Condorcet paradox](#condorcet-paradox)
  - [Invariance principle for a low-degree multilinear polynomial](#invariance-principle-for-a-low-degree-multilinear-polynomial)
    - [Lindeberg replacement method](#lindeberg-replacement-method)
- [Ramsey theory](ramsey-theory.md)
  - [Square-difference recurrence for finite colourings](ramsey-theory.md#square-difference-recurrence-for-finite-colourings)
  - [Multicolour Ramsey bound](ramsey-theory.md#multicolour-ramsey-bound)
  - [Homogeneous set for a colouring](ramsey-theory.md#homogeneous-set-for-a-colouring)
    - [Computable colouring](ramsey-theory.md#computable-colouring)
      - [Finite-injury computable colouring of pairs](ramsey-theory.md#finite-injury-computable-colouring-of-pairs)
      - [Halting-stage colouring of triples](ramsey-theory.md#halting-stage-colouring-of-triples)
  - [Dyadic valuation and scale colouring](ramsey-theory.md#dyadic-valuation-and-scale-colouring)
  - [Space of infinite subsets of the natural numbers](ramsey-theory.md#space-of-infinite-subsets-of-the-natural-numbers)
    - [Finite stem of an infinite subset](ramsey-theory.md#finite-stem-of-an-infinite-subset)
    - [Ramsey family in the homogeneous-cone sense](ramsey-theory.md#ramsey-family-in-the-homogeneous-cone-sense)
    - [Ramsey cone topology](ramsey-theory.md#ramsey-cone-topology)
      - [Meagreness of the Ramsey cone topology](ramsey-theory.md#meagreness-of-the-ramsey-cone-topology)
    - [Ramsey set of infinite subsets](ramsey-theory.md#ramsey-set-of-infinite-subsets)
      - [Open Ramsey theorem](ramsey-theory.md#open-ramsey-theorem)
      - [Finite-symmetric-difference parity colouring](ramsey-theory.md#finite-symmetric-difference-parity-colouring)
      - [Non-Ramsey set from transfinite selection](ramsey-theory.md#non-ramsey-set-from-transfinite-selection)
      - [Completely Ramsey set](ramsey-theory.md#completely-ramsey-set)
        - [Stem-supported Ramsey family need not be completely Ramsey](ramsey-theory.md#stem-supported-ramsey-family-need-not-be-completely-ramsey)
        - [Completely Ramsey-null set](ramsey-theory.md#completely-ramsey-null-set)
          - [Ellentuck meagre-set fusion lemma](ramsey-theory.md#ellentuck-meagre-set-fusion-lemma)
        - [Fusion proof for open Ellentuck sets](ramsey-theory.md#fusion-proof-for-open-ellentuck-sets)
          - [Acceptance and rejection of finite stems](ramsey-theory.md#acceptance-and-rejection-of-finite-stems)
            - [Finitely many accepting extensions of a rejected stem](ramsey-theory.md#finitely-many-accepting-extensions-of-a-rejected-stem)
            - [Deciding all finite stems by fusion](ramsey-theory.md#deciding-all-finite-stems-by-fusion)
    - [Ellentuck topology](ramsey-theory.md#ellentuck-topology)
      - [Ellentuck Borel sets are completely Ramsey](ramsey-theory.md#ellentuck-borel-sets-are-completely-ramsey)
        - [Baire-property reduction for completely Ramsey families](ramsey-theory.md#baire-property-reduction-for-completely-ramsey-families)
      - [Cone on an infinite coinfinite ground set](ramsey-theory.md#cone-on-an-infinite-coinfinite-ground-set)
        - [Ordinarily nowhere-dense sets need not be completely Ramsey](ramsey-theory.md#ordinarily-nowhere-dense-sets-need-not-be-completely-ramsey)
      - [Countable unions of Ellentuck clopen sets need not be closed](ramsey-theory.md#countable-unions-of-ellentuck-clopen-sets-need-not-be-closed)
      - [Baire property in the Ellentuck topology](ramsey-theory.md#baire-property-in-the-ellentuck-topology)
    - [Ordinary topology on infinite subsets](ramsey-theory.md#ordinary-topology-on-infinite-subsets)
      - [Dense countable family of cofinite infinite subsets](ramsey-theory.md#dense-countable-family-of-cofinite-infinite-subsets)
      - [Gap-doubling closed family of infinite subsets](ramsey-theory.md#gap-doubling-closed-family-of-infinite-subsets)
        - [Meagre set meeting every Ramsey cone in both colours](ramsey-theory.md#meagre-set-meeting-every-ramsey-cone-in-both-colours)
      - [Baire property in the ordinary infinite-subset topology](ramsey-theory.md#baire-property-in-the-ordinary-infinite-subset-topology)
  - [Matching Ramsey number](ramsey-theory.md#matching-ramsey-number)
  - [Triangle-packing Ramsey number](ramsey-theory.md#triangle-packing-ramsey-number)
  - [Finite coloring](ramsey-theory.md#finite-coloring)
    - [Colour profile of a finite block](ramsey-theory.md#colour-profile-of-a-finite-block)
    - [Colour class](ramsey-theory.md#colour-class)
    - [Cyclic logarithmic coloring](ramsey-theory.md#cyclic-logarithmic-coloring)
    - [Refinement of a finite coloring](ramsey-theory.md#refinement-of-a-finite-coloring)
    - [Monochromatic set](ramsey-theory.md#monochromatic-set)
  - [Ramsey's theorem](ramsey-theory.md#ramsey-s-theorem)
    - [Simultaneous coefficient patterns from a homogeneous four-set colouring](ramsey-theory.md#simultaneous-coefficient-patterns-from-a-homogeneous-four-set-colouring)
    - [Successive thinning proof of the infinite Ramsey theorem](ramsey-theory.md#successive-thinning-proof-of-the-infinite-ramsey-theorem)
    - [Finite Ramsey theorem](ramsey-theory.md#finite-ramsey-theorem)
      - [Ramsey number](ramsey-theory.md#ramsey-number)
  - [Modular-intersection graph Ramsey lower bound](ramsey-theory.md#modular-intersection-graph-ramsey-lower-bound)
  - [Combinatorial line](ramsey-theory.md#combinatorial-line)
    - [Fixed-active-size obstruction for combinatorial lines](ramsey-theory.md#fixed-active-size-obstruction-for-combinatorial-lines)
    - [Run-count obstruction to interval-active lines](ramsey-theory.md#run-count-obstruction-to-interval-active-lines)
    - [Coordinate duplication for combinatorial lines](ramsey-theory.md#coordinate-duplication-for-combinatorial-lines)
    - [Adequate family of active coordinate sets](ramsey-theory.md#adequate-family-of-active-coordinate-sets)
    - [Hales-Jewett theorem](ramsey-theory.md#hales-jewett-theorem)
      - [Letter-merging proof of the Hales-Jewett theorem](ramsey-theory.md#letter-merging-proof-of-the-hales-jewett-theorem)
      - [Alphabet insensitivity lemma](ramsey-theory.md#alphabet-insensitivity-lemma)
        - [Explicit block bound for alphabet insensitivity](ramsey-theory.md#explicit-block-bound-for-alphabet-insensitivity)
    - [Combinatorial subspace](ramsey-theory.md#combinatorial-subspace)
      - [Extended Hales-Jewett theorem](ramsey-theory.md#extended-hales-jewett-theorem)
  - [Hilbert cube](ramsey-theory.md#hilbert-cube)
    - [Hilbert cube theorem](ramsey-theory.md#hilbert-cube-theorem)
  - [Van der Waerden theorem](ramsey-theory.md#van-der-waerden-theorem)
    - [Colour-focusing proof of Van der Waerden theorem](ramsey-theory.md#colour-focusing-proof-of-van-der-waerden-theorem)
    - [Brauer progression theorem](ramsey-theory.md#brauer-progression-theorem)
    - [Strengthened Van der Waerden theorem](ramsey-theory.md#strengthened-van-der-waerden-theorem)
    - [Color-focused arithmetic progression](ramsey-theory.md#color-focused-arithmetic-progression)
  - [Gallai theorem for an integer lattice](ramsey-theory.md#gallai-theorem-for-an-integer-lattice)
    - [Canonical arithmetic progression dichotomy](ramsey-theory.md#canonical-arithmetic-progression-dichotomy)
    - [Sum map from words to homothetic copies](ramsey-theory.md#sum-map-from-words-to-homothetic-copies)
    - [Arithmetic-progression bipartite Ramsey dichotomy](ramsey-theory.md#arithmetic-progression-bipartite-ramsey-dichotomy)
  - [Partition regular matrix](ramsey-theory.md#partition-regular-matrix)
    - [Scaling invariance of homogeneous partition regularity](ramsey-theory.md#scaling-invariance-of-homogeneous-partition-regularity)
    - [Reciprocal partition regularity](ramsey-theory.md#reciprocal-partition-regularity)
    - [Compactness bound for partition regularity](ramsey-theory.md#compactness-bound-for-partition-regularity)
    - [Partition regularity dichotomy under an extra constraint](ramsey-theory.md#partition-regularity-dichotomy-under-an-extra-constraint)
    - [Columns property](ramsey-theory.md#columns-property)
      - [Rado's theorem](ramsey-theory.md#rado-s-theorem)
        - [Partition-regular system forcing an ordered Schur relation](ramsey-theory.md#partition-regular-system-forcing-an-ordered-schur-relation)
        - [Rado theorem for one equation](ramsey-theory.md#rado-theorem-for-one-equation)
          - [Brauer configuration for a one-row zero-sum equation](ramsey-theory.md#brauer-configuration-for-a-one-row-zero-sum-equation)
          - [Leading-residue obstruction to partition regularity](ramsey-theory.md#leading-residue-obstruction-to-partition-regularity)
          - [One-equation partition regularity over odd integers](ramsey-theory.md#one-equation-partition-regularity-over-odd-integers)
      - [P-adic columns lemma](ramsey-theory.md#p-adic-columns-lemma)
        - [Finite separating-functional proof of the columns condition](ramsey-theory.md#finite-separating-functional-proof-of-the-columns-condition)
        - [Last nonzero digit coloring](ramsey-theory.md#last-nonzero-digit-coloring)
      - [M-p-c set](ramsey-theory.md#m-p-c-set)
        - [Rado solution inside an m-p-c set](ramsey-theory.md#rado-solution-inside-an-m-p-c-set)
        - [Monochromatic m-p-c set theorem](ramsey-theory.md#monochromatic-m-p-c-set-theorem)
          - [Finite sums theorem](ramsey-theory.md#finite-sums-theorem)
            - [Columns partition for finite-sums systems](ramsey-theory.md#columns-partition-for-finite-sums-systems)
  - [Hindman theorem](ramsey-theory.md#hindman-theorem)
    - [Dynamical proof of Hindman's theorem](ramsey-theory.md#dynamical-proof-of-hindman-s-theorem)
    - [Idempotent-ultrafilter proof of Hindman's theorem](ramsey-theory.md#idempotent-ultrafilter-proof-of-hindman-s-theorem)
    - [Finite-sums set](ramsey-theory.md#finite-sums-set)
      - [Divisibility chain inside a finite-sums set](ramsey-theory.md#divisibility-chain-inside-a-finite-sums-set)
      - [IP set](ramsey-theory.md#ip-set)
        - [Alternating dyadic intervals contain disjoint IP sets](ramsey-theory.md#alternating-dyadic-intervals-contain-disjoint-ip-sets)
        - [IP-star set](ramsey-theory.md#ip-star-set)
          - [IP-star filter](ramsey-theory.md#ip-star-filter)
        - [Partition regularity of IP sets](ramsey-theory.md#partition-regularity-of-ip-sets)
    - [Milliken–Taylor theorem](ramsey-theory.md#milliken-taylor-theorem)
  - [Monochromatic sums-and-products obstruction](ramsey-theory.md#monochromatic-sums-and-products-obstruction)
  - [Euclidean Ramsey set](ramsey-theory.md#euclidean-ramsey-set)
    - [Spherical point set](ramsey-theory.md#spherical-point-set)
    - [Product theorem for Euclidean Ramsey sets](ramsey-theory.md#product-theorem-for-euclidean-ramsey-sets)
    - [Three-term unit arithmetic progression is not Euclidean Ramsey](ramsey-theory.md#three-term-unit-arithmetic-progression-is-not-euclidean-ramsey)
    - [Triangle is a Euclidean Ramsey set](ramsey-theory.md#triangle-is-a-euclidean-ramsey-set)
    - [Line segment is a Euclidean Ramsey set](ramsey-theory.md#line-segment-is-a-euclidean-ramsey-set)
    - [Regular polygon is a Euclidean Ramsey set](ramsey-theory.md#regular-polygon-is-a-euclidean-ramsey-set)
    - [Approximately Euclidean Ramsey set](ramsey-theory.md#approximately-euclidean-ramsey-set)
    - [Edge Ramsey set](ramsey-theory.md#edge-ramsey-set)
    - [Cyclic transitive point set](ramsey-theory.md#cyclic-transitive-point-set)
      - [Kriz theorem for cyclic transitive point sets](ramsey-theory.md#kriz-theorem-for-cyclic-transitive-point-sets)
        - [A-invariant coloring of a Cartesian power](ramsey-theory.md#a-invariant-coloring-of-a-cartesian-power)
- [Symmetric function](#symmetric-function)
  - [Cauchy identity for symmetric functions](#cauchy-identity-for-symmetric-functions)
    - [Schur specialization by a generating function](#schur-specialization-by-a-generating-function)
    - [Dual Cauchy identity for symmetric functions](#dual-cauchy-identity-for-symmetric-functions)
  - [Symmetric-function involution](#symmetric-function-involution)
    - [Forgotten symmetric function](#forgotten-symmetric-function)
  - [Monomial symmetric function](#monomial-symmetric-function)
  - [Hall inner product of symmetric functions](#hall-inner-product-of-symmetric-functions)
  - [Complete homogeneous symmetric polynomial](#complete-homogeneous-symmetric-polynomial)
  - [Power-sum symmetric polynomial](#power-sum-symmetric-polynomial)
  - [Schur polynomial](#schur-polynomial)
    - [Bialternant formula](#bialternant-formula)
      - [Schur evaluation at all ones](#schur-evaluation-at-all-ones)
    - [Skew Schur function](#skew-schur-function)
    - [Jacobi–Trudi identity](#jacobi-trudi-identity)
      - [Determinantal form of a symmetric-group character](#determinantal-form-of-a-symmetric-group-character)
  - [Frobenius characteristic map](#frobenius-characteristic-map)
    - [Frobenius alternant character formula](#frobenius-alternant-character-formula)

## Matroid

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matroid)

A [matroid](#matroid) on a finite [set](set.md) $E$ consists of a nonempty family of independent [subsets](set.md#subset) closed under taking [subsets](set.md#subset) and satisfying exchange: if independent [sets](set.md) $I,J$ obey $|I|<|J|$, some $j\in J\setminus I$ has $I\cup\{j\}$ independent. [Linear independence](vector-space.md#linear-independence) of [vectors](vector-space.md#vector) is the motivating example. A [pregeometry](foundations-of-mathematics.md#pregeometry) is a finitary closure-theoretic extension to possibly infinite [sets](set.md).

## Rule of product

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rule_of_product)

For finite [sets](set.md), the number of ordered choices of one element from each is the product of the individual numbers of choices. More generally, if stage $j$ has exactly $n_j$ possible choices after every permitted history of earlier stages, the total number of full choice sequences is $\prod_j n_j$, by [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on the stages. This counts $b^a$ [functions](function.md) between sets of sizes $a,b$, and counts the [injective functions](algebra.md#injective-function) by the [falling factorial](#falling-factorial) $b(b-1)\cdots(b-a+1)$ when $a\le b$.

## Steiner system

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Steiner_system)

A Steiner system $S(t,k,v)$ is a $v$-point set with $k$-point blocks such that every $t$-point subset is contained in exactly one block. Necessarily the number of blocks is $\binom vt/\binom kt$. This count is a necessary consistency check, not a substitute for proving exact containment. The [small Witt design](#small-witt-design) is $S(5,6,12)$.

### Block of a Steiner system

↑ **Parent:** [Steiner system](#steiner-system)

A designated [subset](set.md#subset) in a [Steiner system](#steiner-system) is a [Steiner block](#block-of-a-steiner-system). In a system $S(t,k,v)$, each [Steiner block](#block-of-a-steiner-system) contains $k$ points and each $t$-point [subset](set.md#subset) belongs to exactly one [Steiner block](#block-of-a-steiner-system). For $t=2$, this is the pair-coverage condition used in a [cyclotomic construction of a Steiner 2-design](#cyclotomic-construction-of-a-steiner-2-design).

### Difference family for a Steiner 2-design

↑ **Parent:** [Steiner system](#steiner-system)

In a finite additive [group](group.md), a family of $k$-subsets is a difference family of index one if each nonzero [group](group.md) element occurs exactly once among all their ordered within-block differences. Translating its [Steiner blocks](#block-of-a-steiner-system) by every [group](group.md) element gives a [Steiner system](#steiner-system) with parameters $2$-$(v,k,1)$: the unique representation of a difference determines the unique translated [Steiner block](#block-of-a-steiner-system) through two specified points.

#### Cyclotomic construction of a Steiner 2-design

↑ **Parent:** [Difference family for a Steiner 2-design](#difference-family-for-a-steiner-2-design)

Put $m=\binom{k}{2}$, take odd $q\equiv1\pmod{2m}$, and let $H$ be the index-$m$ multiplicative [subgroup](group.md#subgroup). If a $k$-set $A$ has its unordered pair differences in distinct $H$-cosets, choose $S\subset H$ containing exactly one element from each pair $\{h,-h\}$. Then $\{sA:s\in S\}$ is a [difference family for a Steiner 2-design](#difference-family-for-a-steiner-2-design). Indeed one unordered pair supplies each [coset](group-theory.md#coset), and its two difference orientations multiplied by $S$ cover that [coset](group-theory.md#coset) once. Translations yield a $2$-$(q,k,1)$ [Steiner system](#steiner-system). The [cyclotomic pattern extension by a second-moment bound](algebra.md#cyclotomic-pattern-extension-by-a-second-moment-bound) supplies suitable $A$ for all sufficiently large $q$ in this progression.

### Small Witt design

↑ **Parent:** [Steiner system](#steiner-system)

The small Witt design is a Steiner system $S(5,6,12)$ with 132 blocks. A six-set duad-syntheme duality constructs it on two disjoint six-sets: two whole-half blocks, forty-five blocks of each of the types $(2,4)$ and $(4,2)$, and forty corresponding-partition blocks of type $(3,3)$. The internal-duad/cross-syntheme incidence rule proves that each five-set lies in exactly one of these blocks.

#### Synthematic construction of the small Witt design

↑ **Parent:** [Small Witt design](#small-witt-design)

On a six-point set $X$ and its six [totals of synthemes](#total-of-synthemes) $Y$, each duad determines a partition of $Y$ into three pairs according to their shared synthemes. Include both whole halves, the 45 blocks $D\cup(Y\setminus P)$ for these duad-pair incidences, and their complements. For each partition $X=A\sqcup A^c$ into triples, cross synthemes give two triangular components on $Y$; include the four unions of a part of $X$ with a component. These 132 blocks form the [small Witt design](#small-witt-design).

## Six-point matching geometry

↑ **Parent:** [Combinatorics](combinatorics.md)

The complete graph on six points has fifteen edges and fifteen perfect matchings. Its six one-factorizations organize a dual incidence geometry exchanging points with factorizations and edges with matchings. The classical names are [duads](#duad), [synthemes](#syntheme) and [totals of synthemes](#total-of-synthemes). This geometry supports [duad-syntheme duality on six points](#duad-syntheme-duality-on-six-points) and a construction of the [small Witt design](#small-witt-design).

### Pentad construction of the exceptional alternating-group automorphism

↑ **Parent:** [Six-point matching geometry](#six-point-matching-geometry)

The six [pentads](#total-of-synthemes) are the six one-factorizations of the complete graph on six points. Permuting the ground-set points permutes these factorizations. The action sends a transposition to three disjoint transpositions and a $3$-cycle to two disjoint $3$-cycles. Its restriction to $A_6$ is faithful by simplicity, and the full action of $S_6$ is faithful because an order-two kernel would be central. It is consequently an automorphism of $S_6$. Its restriction preserves $A_6$ and changes $3$-cycle type, so it cannot be induced on $A_6$ by any conjugation from $S_6$.

### Duad-syntheme duality on six points

↑ **Parent:** [Six-point matching geometry](#six-point-matching-geometry)

A bijection from the points of one six-set to the totals of another extends by incidence to bijections from duads to synthemes, synthemes to duads, and totals to points. A duad maps to the intersection of its two point-totals. The same duality exchanges internal duads of a three-versus-three partition with cross synthemes of its corresponding partition. The latter rule follows by splitting the six cross perfect matchings into parity classes of three, yielding two triangles on the six totals.

### Duad

↑ **Parent:** [Six-point matching geometry](#six-point-matching-geometry)

A duad is an unordered pair of distinct points. On a six-point set there are $\binom62=15$ duads. They are the edges of the complete graph and are grouped into [synthemes](#syntheme).

#### Syntheme

↑ **Parent:** [Duad](#duad)

A syntheme partitions six points into three duads, equivalently a perfect matching of the complete graph. There are $6!/(2^3 3!)=15$ synthemes. Every duad belongs to three. Two edge-disjoint synthemes extend to a unique [total of synthemes](#total-of-synthemes): their union is a six-cycle, whose complement has a unique factorization into three matchings.

##### Total of synthemes

↑ **Parent:** [Syntheme](#syntheme)

A total is a set of five edge-disjoint synthemes covering all fifteen duads of a six-point set. There are six totals; each syntheme belongs to two and every two totals share exactly one syntheme. Each total contains exactly one syntheme containing any prescribed duad. Totals are one-factorizations of the complete graph.

###### Counting synthematic totals

↑ **Parent:** [Total of synthemes](#total-of-synthemes)

Two disjoint [synthemes](#syntheme) form a six-cycle, whose complement is a triangular prism. The prism has a unique partition into three perfect matchings, so the pair extends uniquely to a [total of synthemes](#total-of-synthemes). Eight synthemes are disjoint from a fixed syntheme; grouping them four per total yields two totals through it, and double counting gives six totals in all.

// Target: combinatorics.bigb

## Cycle lemma

↑ **Parent:** [Combinatorics](combinatorics.md)

For an integer sequence with total sum one, exactly one cyclic starting position has every nonempty partial sum strictly positive. Starting after the last minimum of the proper partial sums proves existence. Two good starts would divide the sequence into two positive integer arc sums adding to one, proving uniqueness. This form counts cyclic prefix constraints in the [cyclic Turán covering construction](hypergraph.md#cyclic-turan-covering-construction).

## Cyclic digit run

↑ **Parent:** [Combinatorics](combinatorics.md)

A cyclic digit run is a consecutive segment of a digit string whose successive digits all increase by one or all decrease by one modulo the base. For example, $8,9,0,1$ is an increasing decimal run. This refers to cyclic digit values, not to joining the final position of the string back to its first position. Overlapping run constraints can be counted with the [inclusion-exclusion principle](#inclusion-exclusion-principle).

## Finite geometry

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_geometry)

Finite geometry studies geometric incidence structures having finitely many points, such as finite projective and affine spaces.

## Increasing subsequence

↑ **Parent:** [Combinatorics](combinatorics.md)

An increasing subsequence of a sequence $x_1,\ldots,x_n$ is a sequence $x_{i_1}\leq\cdots\leq x_{i_m}$ selected at indices $i_1<\cdots<i_m$.

### Longest increasing subsequence

↑ **Parent:** [Increasing subsequence](#increasing-subsequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Longest_increasing_subsequence)

A longest increasing subsequence is an [increasing subsequence](#increasing-subsequence) of maximum length. Changing or deleting one term changes its length by at most one.

## Additive combinatorics

↑ **Parent:** [Combinatorics](combinatorics.md)

[This section is present in another page, follow this link to view it.](additive-combinatorics.md)

## Directed acyclic graph

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Directed_acyclic_graph)

A directed acyclic graph is a directed graph with no directed cycle.

### Topological sorting

↑ **Parent:** [Directed acyclic graph](#directed-acyclic-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_sorting)

A [topological sorting](#topological-sorting) constructs a [topological order](#topological-order) of a finite [Directed acyclic graph](#directed-acyclic-graph). Repeatedly remove a vertex of indegree zero and place it next in the ordering. Such a vertex exists in every nonempty finite [Directed acyclic graph](#directed-acyclic-graph), since otherwise following predecessor edges eventually creates a directed cycle.

// Target: combinatorics.bigb

#### Topological order

↑ **Parent:** [Topological sorting](#topological-sorting)

A [topological order](#topological-order) is an ordering of a directed graph's vertices in which every arc points from an earlier vertex to a later one. A finite directed graph admits such an ordering exactly when it is a [Directed acyclic graph](#directed-acyclic-graph).

// Target: foundations-of-mathematics.bigb

### Markov equivalence of directed acyclic graphs

↑ **Parent:** [Directed acyclic graph](#directed-acyclic-graph)

Two [Directed acyclic graphs](#directed-acyclic-graph) are Markov equivalent when they encode the same [D-separations](#d-separation) for all disjoint sets of vertices. They consequently impose the same [global Markov property for a directed acyclic graph](causal-inference.md#global-markov-property-for-a-directed-acyclic-graph), although their causal interpretations can differ.

#### Completed partially directed acyclic graph

↑ **Parent:** [Markov equivalence of directed acyclic graphs](#markov-equivalence-of-directed-acyclic-graphs)

The completed partially directed acyclic graph of a [Markov equivalence of directed acyclic graphs](#markov-equivalence-of-directed-acyclic-graphs) class has their common [skeleton of a directed graph](graph-theory.md#skeleton-of-a-directed-graph). An edge is directed exactly when its orientation agrees in every member of the class, and is otherwise undirected. It can be constructed by enumerating all acyclic orientations with the prescribed [unshielded colliders](#unshielded-collider) and retaining only the common directions; practical [PC algorithms](causal-inference.md#pc-algorithm) use orientation propagation instead of enumeration.

#### Skeleton and collider characterization of Markov equivalence

↑ **Parent:** [Markov equivalence of directed acyclic graphs](#markov-equivalence-of-directed-acyclic-graphs)

Two [Directed acyclic graphs](#directed-acyclic-graph) are [Markov equivalent directed acyclic graphs](#markov-equivalence-of-directed-acyclic-graphs) if and only if they have the same [skeleton of a directed graph](graph-theory.md#skeleton-of-a-directed-graph) and the same [unshielded colliders](#unshielded-collider). Thus these two structures determine the observational equivalence class. This structural theorem is what converts the skeleton and collider phases of the [PC algorithm](causal-inference.md#pc-algorithm) into identification of an equivalence class.

### Moral graph

↑ **Parent:** [Directed acyclic graph](#directed-acyclic-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moral_graph)

The moral graph of a [Directed acyclic graph](#directed-acyclic-graph) joins every pair of vertices with a common child and then replaces every directed edge by an undirected edge.

#### Hammersley-Clifford theorem

↑ **Parent:** [Moral graph](#moral-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hammersley-Clifford_theorem)

For a strictly positive probability density, factorization into clique potentials of an undirected graph is equivalent to the global Markov conditional-independence property for that graph.

### Topological ordering

↑ **Parent:** [Directed acyclic graph](#directed-acyclic-graph)

A topological ordering places every parent before each child.

A [topological sorting](#topological-sorting) constructs such a [topological order](#topological-order) of a directed acyclic graph.

### D-separation

↑ **Parent:** [Directed acyclic graph](#directed-acyclic-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/D-separation)

D-separation blocks paths through conditioned noncolliders and through unconditioned colliders without conditioned descendants.

#### Collider

↑ **Parent:** [D-separation](#d-separation)

On a path in a directed graph, an interior vertex is a collider when both adjacent path edges have arrowheads pointing into it. A path through a collider is blocked unless that collider or one of its descendants is conditioned upon.

##### Unshielded collider

↑ **Parent:** [Collider](#collider)

An unshielded [collider](#collider) in a [Directed acyclic graph](#directed-acyclic-graph) is a triple $a\to b\leftarrow c$ with $a$ and $c$ nonadjacent. The absence of an edge between its outer vertices makes this orientation detectable from [conditional independence](random-variable.md#conditional-independence) information under [faithfulness of a directed acyclic graph](causal-inference.md#faithfulness-of-a-directed-acyclic-graph).

#### D-separating set

↑ **Parent:** [D-separation](#d-separation)

A set d-separates two vertex sets when it blocks every path between them.

#### Local Markov property of a directed acyclic graph

↑ **Parent:** [D-separation](#d-separation)

Conditioned on its parents, a vertex is d-separated from all nondescendants other than those parents.

#### Global Markov property of a directed acyclic graph

↑ **Parent:** [D-separation](#d-separation)

The global Markov property of a [Directed acyclic graph](#directed-acyclic-graph) says that d-separation of vertex sets $A$ and $B$ by $S$ implies conditional independence of the corresponding random vectors given the variables at $S$.

## Incidence geometry

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Incidence_geometry)

Incidence geometry studies which points lie on which curves, lines or higher-dimensional objects and how many such incidences a finite configuration can have.

### Linear space (geometry)

↑ **Parent:** [Incidence geometry](#incidence-geometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_space_(geometry))

A linear space is a structure in [incidence geometry](#incidence-geometry) with a [set](set.md) of points and a collection of [subsets](set.md#subset) called lines: any two distinct points lie on exactly one line, and every line contains at least two points. The lines here are incidence-theoretic objects, without a required coordinate realization. A [finite linear space](extremal-set-theory.md#finite-linear-space) imposes finiteness; its nontrivial form excludes a line containing all points. This is distinct from a [vector space](vector-space.md), whose structure involves addition and scalar multiplication.

### Joint of a line collection

↑ **Parent:** [Incidence geometry](#incidence-geometry)

For distinct real affine lines in $\mathbb R^n$, $n\ge2$, a [joint of a line collection](#joint-of-a-line-collection) is a point lying on $n$ lines with [linearly independent](vector-space.md#linear-independence) direction vectors. In three dimensions the directions must not all lie in one plane. Extra incident lines are allowed; existence of one spanning choice is enough. This counts [joint of a line collection](#joint-of-a-line-collection) points, rather than tuples of lines or incidence multiplicities.

#### Joints theorem

↑ **Parent:** [Joint of a line collection](#joint-of-a-line-collection)

The number of [joints of a line collection](#joint-of-a-line-collection) formed by $L$ distinct real affine lines in $\mathbb R^n$ is at most $C_n L^{n/(n-1)}$. The [pruning and minimal-degree polynomial argument](#pruning-and-minimal-degree-polynomial-argument) proves this bound. The exponent is sharp: the coordinate-line grid has $m^n$ [joints of a line collection](#joint-of-a-line-collection) and $n m^{n-1}$ lines. In three dimensions the bound is $C L^{3/2}$.

##### Pruning and minimal-degree polynomial argument

↑ **Parent:** [Joints theorem](#joints-theorem)

Let a line collection have $M$ [joints of a line collection](#joint-of-a-line-collection) and put $D=\lceil nM^{1/n}\rceil$. If $M>LD$, deleting each line with at most $D$ current [joints of a line collection](#joint-of-a-line-collection), together with those [joints of a line collection](#joint-of-a-line-collection), leaves a nonempty configuration in which every line has more than $D$ [joints of a line collection](#joint-of-a-line-collection). A nonzero [polynomial](polynomial.md) of degree at most $D$ vanishes on the retained [joints of a line collection](#joint-of-a-line-collection) by [rank-nullity theorem](linear-algebra.md#rank-nullity-theorem). Choose one of minimum degree. Its restriction vanishes identically on every retained line, so its [gradient](calculus.md#gradient) is orthogonal to a spanning set of directions at every [joint of a line collection](#joint-of-a-line-collection) and hence vanishes there. Each nonzero [partial derivative](calculus.md#partial-derivative) would be a lower-degree [polynomial](polynomial.md) with the same zeros, contradicting minimality. In characteristic zero, all derivatives vanishing forces a constant [polynomial](polynomial.md), another contradiction. Therefore $M\le LD$, giving the [joints theorem](#joints-theorem). The argument's characteristic-zero assumption is essential to its derivative step.

### Kakeya set

↑ **Parent:** [Incidence geometry](#incidence-geometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kakeya_set)

A bounded subset of $\mathbb R^n$ is a [Kakeya set](#kakeya-set) if it contains a unit line segment in every direction. Segment positions may vary with direction. Such a set need not have positive [Lebesgue measure](measure-theory.md#lebesgue-measure); the dimension problem concerns its [Minkowski dimension](geometry-and-topology.md#box-counting-dimension) or other notions of dimension.

#### Besicovitch set

↑ **Parent:** [Kakeya set](#kakeya-set)

A Besicovitch set is a planar Kakeya set of Lebesgue measure zero containing a unit line segment in every direction.

##### Compact Kakeya construction from small projections

↑ **Parent:** [Besicovitch set](#besicovitch-set)

Choose a compact $K\subset[0,1]\times\mathbb R$ with full horizontal projection and zero-length projections $y+tx$ for $t\in[0,1]$. Then the displayed set is compact, has zero area by the [Fubini theorem](measure-theory.md#fubini-s-theorem), and contains a segment of every slope in $[0,1]$. Such parameter sets exist by the [Baire category theorem](topological-analysis.md#baire-category-theorem) in the [Hausdorff metric](topological-analysis.md#hausdorff-distance): fine parallel segments approximate any parameter set while making a fixed band of projections uniformly small. Finite grids and a countable intersection make every required projection null. Four rotated copies supply every planar direction.

##### Perron tree

↑ **Parent:** [Besicovitch set](#besicovitch-set)

A Perron tree is a finite triangular splitting-and-sliding arrangement retaining a prescribed angular range while overlapping its pieces strongly. The compression parameter and the number of generations can make union area an arbitrarily small fraction of total piece area. Suitable longitudinal extensions separate the pieces into disjoint rectangles. This stronger finite geometry is used by the ball-multiplier counterexample; a compact measure-zero [Besicovitch set](#besicovitch-set) alone does not assert that arbitrary segment translates are disjoint.

#### Kakeya Minkowski dimension conjecture

↑ **Parent:** [Kakeya set](#kakeya-set)

The dimension assertion asks that every bounded [Kakeya set](#kakeya-set) in $\mathbb R^n$ have full [Minkowski dimension](geometry-and-topology.md#box-counting-dimension). The [Kakeya maximal conjecture](fourier-analysis.md#kakeya-maximal-conjecture) implies the stronger lower-dimension conclusion: its application to $E_\delta$ gives $|E_\delta|\gtrsim_{n,\varepsilon}\delta^{n\varepsilon}$, hence $N_\delta(E)\gtrsim_{n,\varepsilon}\delta^{-n+n\varepsilon}$ for every $\varepsilon>0$.

#### Kakeya tube

↑ **Parent:** [Kakeya set](#kakeya-set)

A Kakeya tube is a neighborhood of transverse radius $\delta$ of a line segment of fixed unit length. Round cross-sections and comparable rectangular cross-sections are interchangeable up to fixed constants. The tube has [Lebesgue measure](measure-theory.md#lebesgue-measure) comparable to $\delta^{n-1}$ in $\mathbb R^n$.

### Ordinary line

↑ **Parent:** [Incidence geometry](#incidence-geometry)

Relative to a finite point set, an [ordinary line](#ordinary-line) is a line containing exactly two points of that set. It is an exact-richness condition, not a count of unordered pairs alone: a line with three points contains three point pairs but is not ordinary. [Point-line duality](projective-space.md#point-line-duality) turns ordinary lines into intersections incident to exactly two dual lines.

#### Cubic covering from few ordinary lines

↑ **Parent:** [Ordinary line](#ordinary-line)

If a finite planar point set has at most $Kn$ [ordinary lines](#ordinary-line), its points can be covered by $O(K+1)$ possibly reducible cubics. The [Euler defect identity for a projective line arrangement](projective-space.md#euler-defect-identity-for-a-projective-line-arrangement) gives $O(Kn)$ bad edges in the dual. [Bounded-radius propagation of edge defects](projective-space.md#bounded-radius-propagation-of-edge-defects) and averaging select one dual line with $O(K+1)$ unsafe edges. [Cubic propagation along a triangular strip](algebraic-geometry.md#cubic-propagation-along-a-triangular-strip) covers each safe run; each exceptional intersection vertex represents a primal line, covered by a [degenerate cubic containing a line](algebraic-geometry.md#degenerate-cubic-containing-a-line). A dual line with very few intersection vertices instead yields a direct covering by few primal lines.

### Distinct-distance set

↑ **Parent:** [Incidence geometry](#incidence-geometry)

For a finite planar point set $P$, its [distinct-distance set](#distinct-distance-set) is $\Delta(P)=\{|p-q|:p,q\in P\}$. It includes zero for nonempty $P$. Its cardinality measures how many different distances the configuration determines. Ordered point pairs can be grouped according to their distance, which relates the problem to [incidences between points and curves](#incidences-between-points-and-curves).

<h4 id="szekely-distinct-distance-bound">Székely distinct-distance bound</h4>

↑ **Parent:** [Distinct-distance set](#distinct-distance-set)

For a finite set of at least two points in the plane, some point determines the displayed number of different positive [Euclidean distances](topological-analysis.md#euclidean-distance). The [circular-arc graph for distinct distances](#circular-arc-graph-for-distinct-distances) has quadratically many [edges](graph-theory.md#edge-of-a-graph). The [rich-bisector deletion bound](#rich-bisector-deletion-bound) removes high-multiplicity [edges](graph-theory.md#edge-of-a-graph) while retaining that order of growth. The [crossing lemma for multigraphs](graph-theory.md#crossing-lemma-for-multigraphs) then compares its lower crossing bound with the quadratic count of pairs of [circles](topology.md#circle). This strengthens the corresponding bound for the whole [distinct-distance set](#distinct-distance-set). The original result is Theorem11 of [Székely's 1997 paper](https://www.cs.tau.ac.il/~michas/szekely.pdf).

##### Circular-arc graph for distinct distances

↑ **Parent:** [Székely distinct-distance bound](#szekely-distinct-distance-bound)

Around each of $n$ points draw its at most $t$ distinct-distance [circles](topology.md#circle). On every [circle](topology.md#circle) containing at least three points, join cyclically consecutive points by arcs. The resulting loopless [multigraph](graph.md#multigraph) has at least $n(n-1)-2nt$ [edges](graph-theory.md#edge-of-a-graph) and a drawing with $O(n^2t^2)$ crossings. A pair joined by several arcs has every corresponding centre on its [perpendicular bisector](geometry-and-topology.md#perpendicular-bisector), which is the key to bounding multiplicity.

###### Rich-bisector deletion bound

↑ **Parent:** [Circular-arc graph for distinct distances](#circular-arc-graph-for-distinct-distances)

Every supporting centre of an arc between fixed endpoints lies on their [perpendicular bisector](geometry-and-topology.md#perpendicular-bisector). Multiplicity at least $k$ therefore makes that [line](geometry-and-topology.md#straight-line) contain at least $k$ of the original points. For each such [line](geometry-and-topology.md#straight-line) containing $s$ points, its $s$ centres each support at most $t$ [circles](topology.md#circle); on one [circle](topology.md#circle) at most two consecutive-point arcs have that symmetry axis. The [rich line bound](#rich-line-bound) summed over dyadic occupancies gives the displayed bound.

#### Unit-circle method for a distinct-distance lower bound

↑ **Parent:** [Distinct-distance set](#distinct-distance-set)

For every positive distance, draw equal-radius circles centred at the points of $P$. Their [incidences between points and curves](#incidences-between-points-and-curves) count the ordered pairs at that distance. The [Szemerédi–Trotter theorem for unit circles](#szemeredi-trotter-theorem-for-unit-circles) bounds each distance class by $O(|P|^{4/3})$. Summing over all classes accounts for $|P|(|P|-1)$ pairs, proving $|\Delta(P)|\gtrsim |P|^{2/3}$.

### Incidences between points and curves

↑ **Parent:** [Incidence geometry](#incidence-geometry)

For finite sets of points $P$ and geometric curves $\mathcal C$, a point-curve incidence is a pair $(p,\gamma)$ with $p\in\gamma$. The incidence count is $I(P,\mathcal C)=\sum_{\gamma\in\mathcal C}|P\cap\gamma|$. Bounds in [incidence geometry](#incidence-geometry) exploit restrictions on how curves can meet points, rather than treating the incidence relation as an arbitrary bipartite graph.

#### Incidence bound from two-point multiplicity

↑ **Parent:** [Incidences between points and curves](#incidences-between-points-and-curves)

If $n$ points and $m$ curves have the property that each pair of distinct points lies on at most $\lambda$ curves, then [double counting](#double-counting-proof-technique) gives $\sum_\gamma k_\gamma(k_\gamma-1)\le\lambda n(n-1)$, where $k_\gamma=|P\cap\gamma|$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) implies $I^2\le mI+\lambda mn(n-1)$ and hence $I\le m+\sqrt{\lambda mn(n-1)}$. The statement needs only this combinatorial multiplicity condition, not algebraicity.

<h3 id="szemeredi-trotter-theorem">Szemerédi–Trotter theorem</h3>

↑ **Parent:** [Incidence geometry](#incidence-geometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Szemerédi–Trotter_theorem)

For $m$ lines and $n$ points in the real plane, the number of point-line incidences is

$$
O(m+n+m^{2/3}n^{2/3}).
$$

Connecting consecutive incidence points on each line and applying the [Crossing lemma](graph-theory.md#crossing-lemma) proves the bound.

#### Rich line bound

↑ **Parent:** [Szemerédi–Trotter theorem](#szemeredi-trotter-theorem)

For $n$ distinct points in the real plane, $L_{\geq k}$ counts [lines](geometry-and-topology.md#straight-line) containing at least $k\geq2$ points. The [Szemerédi–Trotter theorem](#szemeredi-trotter-theorem) applied to these [lines](geometry-and-topology.md#straight-line) gives the bound by absorbing its additive line-count term; bounded $k$ follows by counting point pairs. Consequently, summing occupancies of [lines](geometry-and-topology.md#straight-line) with at least $k$ points by dyadic ranges gives $O(n^2/k^2+n\log n)$.

<h4 id="szemeredi-trotter-theorem-for-unit-circles">Szemerédi–Trotter theorem for unit circles</h4>

↑ **Parent:** [Szemerédi–Trotter theorem](#szemeredi-trotter-theorem)

For distinct equal-radius circles and a finite point set in the real plane, [incidences between points and curves](#incidences-between-points-and-curves) satisfy $I(P,\mathcal C)=O(|P|^{2/3}|\mathcal C|^{2/3}+|P|+|\mathcal C|)$. Scaling the plane reduces any common positive radius to one. The constant is universal. The fixed-radius condition bounds the number of circles through two prescribed distinct points by two.

#### Incidences between points and polynomial graphs

↑ **Parent:** [Szemerédi–Trotter theorem](#szemeredi-trotter-theorem)

For $m$ distinct real univariate polynomials of degree at most $d$ and $n$ points with distinct first coordinates, the number of incidences between the points and the polynomial graphs is

$$
O\left(m+n+d^{1/3}m^{2/3}n^{2/3}\right).
$$

Two polynomial graphs meet at most $d$ times, so the graph formed from consecutive incidences has $O(dm^2)$ crossings; the [Crossing lemma](graph-theory.md#crossing-lemma) supplies the lower bound.

## Degree-sum formula

↑ **Parent:** [Combinatorics](combinatorics.md)

In every finite undirected graph, the sum of the vertex degrees is twice the number of edges, because each edge contributes one to the degree of each endpoint.

## Tree (graph theory)

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tree_(graph_theory))

A tree is a connected [graph](graph.md) containing no cycle. A finite tree on $n$ vertices has $n-1$ edges.

### Regular tree

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)

An infinite connected [tree](#tree-graph-theory) is regular of degree $k$ if every [vertex](graph.md#vertex-graph-theory) has exactly $k$ neighbours. Necessarily $k\ge2$. For $k=2$ it is a two-sided infinite path. For $k\ge3$, rooting it gives $k$ children at the root and $k-1$ children at each other [vertex](graph.md#vertex-graph-theory); this constructs the unique such tree up to [graph isomorphism](graph.md#graph-isomorphism).

#### Edge boundary of a finite forest in a regular tree

↑ **Parent:** [Regular tree](#regular-tree)

For a nonempty finite [vertex](graph.md#vertex-graph-theory) set $A$ in a degree-$k$ [regular tree](#regular-tree), its induced [forest](#forest) has $|A|-c(A)$ [edges](graph-theory.md#edge-of-a-graph), where $c(A)$ counts its components. Summing degrees and subtracting twice the internal [edge](graph-theory.md#edge-of-a-graph) count gives the displayed number of [edges](graph-theory.md#edge-of-a-graph) with exactly one endpoint in $A$. In particular it is at least $(k-2)|A|+2$.

### Oriented tree

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)

An oriented tree is an orientation of every edge of an undirected [tree](#tree-graph-theory). Its arrows need not all point towards, or away from, any one root. It is acyclic as a [directed graph](graph-theory.md#directed-graph), but different orientations can have different embedding behaviour in [tournaments](graph-theory.md#tournament-graph-theory).

#### Three-times-order tournament bound for oriented trees

↑ **Parent:** [Oriented tree](#oriented-tree)

For a source-rooted [oriented tree](#oriented-tree), let $b$ count edges pointing towards the root and let $c$ count nonempty connected components formed by those edges. A [half-sparse median-order embedding](graph-theory.md#half-sparse-median-order-embedding) exists in $2n+2(b-c)$ vertices. Remove forward leaves, or remove a terminal backward component of order $m$ and replace it temporarily by $2m-2$ outward leaves. Their images contain an in-arborescence copy of the component. Choose the direction and root to minimize $(b-c,b)$ lexicographically; this makes the root a source and gives $b-c\le(n-3)/2$ unless the tree is already an arborescence. The stated bound follows.

#### Arborescence (graph theory)

↑ **Parent:** [Oriented tree](#oriented-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arborescence_(graph_theory))

An arborescence is a rooted [oriented tree](#oriented-tree) whose edges all point away from its root. Reversing every edge gives an in-arborescence. An $n$-vertex arborescence embeds in every [tournament](graph-theory.md#tournament-graph-theory) on $2n-2$ vertices: repeatedly extend an outward leaf in a [half-sparse median-order embedding](graph-theory.md#half-sparse-median-order-embedding). Reversal gives the analogous existence statement for in-arborescences.

### Depth-first traversal of a tree

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)

A depth-first traversal starts at a root, recursively visits each child subtree, and returns along the entering edge. On a finite [tree](#tree-graph-theory), the resulting closed walk traverses each edge exactly once in each direction.

### Rooted tree

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rooted_tree)

A rooted tree is a [tree](#tree-graph-theory) with a distinguished vertex called the root. Its levels consist of the vertices at a fixed [graph distance](graph-theory.md#distance-graph-theory) from the root.

#### Rooted-tree generating function

↑ **Parent:** [Rooted tree](#rooted-tree)

The [exponential generating function](real-analysis.md#exponential-generating-function) for labelled [rooted trees](#rooted-tree) satisfies $T=z e^T$: remove the root and obtain an unordered set of smaller labelled [rooted trees](#rooted-tree). For $0\leq z<1/e$, the convergent series is the solution in $[0,1)$ of $T e^{-T}=z$, rather than the larger real solution. Alternatively, [tree-component expectation in the Erdős-Rényi model](graph-theory.md#tree-component-expectation-in-the-erdos-renyi-model) and subcritical exploration give $T(\theta e^{-\theta})=\theta$ for $0<\theta<1$: their limiting probabilities for the order of the [tree component](graph.md#tree-component) of a uniform [vertex](graph.md#vertex-graph-theory) sum to one. The component tail bound makes this passage through the infinite sum valid.

#### Homeomorphic embedding of a rooted tree

↑ **Parent:** [Rooted tree](#rooted-tree)

For finite [rooted trees](#rooted-tree) in the ancestor [partial order](set.md#partially-ordered-set), a [rooted-tree homeomorphic embedding](#homeomorphic-embedding-of-a-rooted-tree) is an injective vertex map preserving [lowest common ancestors](#lowest-common-ancestor): $h(u\wedge v)=h(u)\wedge h(v)$. The image of the source root need not be the host root. Edge paths and branching are preserved, while paths may be subdivided in the larger tree.

##### Natural-sum ordinal rank of a finite rooted tree

↑ **Parent:** [Homeomorphic embedding of a rooted tree](#homeomorphic-embedding-of-a-rooted-tree)

Give a leaf rank zero, and use [Hessenberg natural sum](set-theory.md#hessenberg-natural-sum) over the immediate rooted subtrees. Every rank is below [epsilon zero](set-theory.md#epsilon-zero); conversely repeated exponentiation and finite summation encode every [Cantor normal form](set-theory.md#cantor-normal-form) below it. A [rooted-tree homeomorphic embedding](#homeomorphic-embedding-of-a-rooted-tree) implies nondecrease of the rank. When roots match, child subtrees embed into distinct branches and exponentiation and natural sum preserve their inequalities. When the source root maps below the host root, its rank is bounded by that of a proper subtree, strictly below the host rank.

##### Adjacency-preserving rooted-tree embedding

↑ **Parent:** [Homeomorphic embedding of a rooted tree](#homeomorphic-embedding-of-a-rooted-tree)

An [adjacency-preserving rooted-tree embedding](#adjacency-preserving-rooted-tree-embedding) is an injective vertex map preserving the root and every adjacency. Because each root-to-vertex path maps to a simple path of the same length, vertex depths are preserved. This is more restrictive than a [homeomorphic embedding of a rooted tree](#homeomorphic-embedding-of-a-rooted-tree), which may stretch edges into paths. The [branching-depth antichain of rooted trees](#branching-depth-antichain-of-rooted-trees) shows that the adjacency relation is not a [well-quasi-ordering](set.md#well-quasi-ordering).

###### Branching-depth antichain of rooted trees

↑ **Parent:** [Adjacency-preserving rooted-tree embedding](#adjacency-preserving-rooted-tree-embedding)

Let $T_m$ consist of a rooted path of $m\geq1$ edges followed by two leaves at its far end. Its only vertex with two children has depth $m$. An [adjacency-preserving rooted-tree embedding](#adjacency-preserving-rooted-tree-embedding) must preserve this depth, so $T_m$ embeds into $T_n$ only when $m=n$. This gives an infinite [bad sequence](set.md#bad-sequence), while [rooted-tree homeomorphic embeddings](#homeomorphic-embedding-of-a-rooted-tree) can stretch the stems.

##### Label-monotone tree embedding

↑ **Parent:** [Homeomorphic embedding of a rooted tree](#homeomorphic-embedding-of-a-rooted-tree)

For [rooted trees](#rooted-tree) labelled in a [preorder](set.md#preorder) $Q$, a label-monotone tree embedding is a [homeomorphic embedding of a rooted tree](#homeomorphic-embedding-of-a-rooted-tree) whose vertex map satisfies $\ell_T(v)\le_Q\ell_S(h(v))$. The root need not map to the host root. For ordered child lists, require in addition that the map preserve the relative order of distinct branches.

#### Lowest common ancestor

↑ **Parent:** [Rooted tree](#rooted-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lowest_common_ancestor)

The [lowest common ancestor](#lowest-common-ancestor) of two vertices is the common ancestor farthest from the root. In the ancestor [partial order](set.md#partially-ordered-set) with the root least, it is their infimum, also called their [greatest common ancestor](#lowest-common-ancestor).

#### Recursively repetition-free labelled tree

↑ **Parent:** [Rooted tree](#rooted-tree)

For a label [set](set.md) $D$, define $\mathcal T(D)$ inductively: choose a root label $d\in D$ and a [finite repetition-free sequence](real-analysis.md#finite-repetition-free-sequence) of [rooted trees](#rooted-tree) in $\mathcal T(D\setminus\{d\})$ as its children. Each object is a finite ordered [rooted tree](#rooted-tree). Labels are distinct along each root-to-leaf path, and child [rooted trees](#rooted-tree) at a vertex are distinct as whole [rooted trees](#rooted-tree). Labels may repeat across different branches; children need not have distinct root labels. For a finite pool of size $m$, the exact number $t_m$ of [rooted trees](#rooted-tree) satisfies

$$
t_0=0,\qquad t_m=m\sum_{k=0}^{t_{m-1}}\frac{t_{m-1}!}{(t_{m-1}-k)!}.
$$

This follows by choosing the root and then an ordered repetition-free list from the finite pool of smaller [rooted trees](#rooted-tree).

##### Recursively repetition-free labelled trees preserve Dedekind-finiteness

↑ **Parent:** [Recursively repetition-free labelled tree](#recursively-repetition-free-labelled-tree)

If $D$ is an [infinite Dedekind-finite set](set.md#infinite-dedekind-finite-set), then $\mathcal T(D)$ is another such [set](set.md). Single-vertex [rooted trees](#rooted-tree) inject $D$ into it. A countable [sequence](real-analysis.md#sequence) of distinct [rooted trees](#rooted-tree) gives finite lists of labels by the [depth-first traversal of a tree](#depth-first-traversal-of-a-tree) in the prescribed child order. By [countable union of explicitly ordered finite lists without choice](set-theory.md#countable-union-of-explicitly-ordered-finite-lists-without-choice), an infinite union of labels contradicts Dedekind-finiteness. A finite union $F$ is equally impossible, since every [rooted tree](#rooted-tree) then lies in the [finite set](set.md#finite-set) $\mathcal T(F)$, by [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on $|F|$ using the recursive child rule. Thus no countably infinite subset of [rooted trees](#rooted-tree) exists.

#### Section of a rooted-tree automorphism

↑ **Parent:** [Rooted tree](#rooted-tree)

For an automorphism $g$ of a regular rooted tree and a first-level vertex $i$, the section $g_i$ is the induced automorphism of the rooted subtree at $i$, defined by

$$
g(iv)=g(i)g_i(v).
$$

An automorphism fixing the first level is determined by the tuple of all its sections.

### Forest

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)

A forest is a graph containing no cycle; each of its connected components is a tree.

#### Two-component spanning forest

↑ **Parent:** [Forest](#forest)

A [two-component spanning forest](#two-component-spanning-forest) of a finite connected [graph](graph.md) is an acyclic spanning subgraph with exactly two [connected components of a graph](graph.md#component-graph-theory). It has $|V|-2$ [edges](graph-theory.md#edge-of-a-graph). For distinct terminals $a,z$, a separating two-component forest places them in different components. Deleting an [edge](graph-theory.md#edge-of-a-graph) of the $a$-to-$z$ [graph path](graph-theory.md#path-in-a-graph) of a [spanning tree](#spanning-tree) produces such a forest; adjoining any original [edge](graph-theory.md#edge-of-a-graph) across its cut reverses this operation. This is the counting correspondence behind the [mean spanning-tree path current](#mean-spanning-tree-path-current).

### Spanning tree

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spanning_tree)

A spanning tree of a connected graph is a tree containing every vertex of the graph.

#### Fundamental cycle

↑ **Parent:** [Spanning tree](#spanning-tree)

Adding a non-tree edge to a [spanning tree](#spanning-tree) creates exactly one [graph cycle](graph-theory.md#cycle-in-a-graph), its [fundamental cycle](#fundamental-cycle). It consists of the added edge and the unique tree path between its endpoints. In the [network simplex algorithm](graph-theory.md#network-simplex-algorithm), modifying flow around this cycle preserves [flow conservation](graph-theory.md#flow-conservation).

// Target: foundations-of-mathematics.bigb

#### Minimum spanning tree

↑ **Parent:** [Spanning tree](#spanning-tree)

A [minimum spanning tree](#minimum-spanning-tree) minimizes total edge weight among [spanning trees](#spanning-tree) of a connected weighted graph. It can be computed in polynomial time by repeatedly adding the least-weight edge joining two current components. The cut-exchange argument preserves the existence of an optimum containing every accepted edge. Removing an edge of a travelling-salesman tour gives a [spanning tree](#spanning-tree), so its optimum is a lower bound on optimal tour cost.

##### Reverse-delete algorithm

↑ **Parent:** [Minimum spanning tree](#minimum-spanning-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reverse-delete_algorithm)

Process [edges](graph-theory.md#edge-of-a-graph) in decreasing weight and delete an [edge](graph-theory.md#edge-of-a-graph) whenever the remaining [graph](graph.md) stays connected. Previously retained heavier [edges](graph-theory.md#edge-of-a-graph) are [bridges in a graph](graph.md#bridge-graph-theory) and remain so under deletion. Thus a deletable [edge](graph-theory.md#edge-of-a-graph) is heaviest on a current [graph cycle](graph-theory.md#cycle-in-a-graph), and the [minimum spanning tree cycle property](#minimum-spanning-tree-cycle-property) excludes it from every [minimum spanning tree](#minimum-spanning-tree). At termination the surviving connected [graph](graph.md) has no [graph cycle](graph-theory.md#cycle-in-a-graph), so it is a [minimum spanning tree](#minimum-spanning-tree).

<h5 id="kruskal-s-algorithm">Kruskal's algorithm</h5>

↑ **Parent:** [Minimum spanning tree](#minimum-spanning-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kruskal's_algorithm)

Process [edges](graph-theory.md#edge-of-a-graph) in increasing weight, accepting an [edge](graph-theory.md#edge-of-a-graph) exactly when its endpoints lie in different current [connected components of a graph](graph.md#component-graph-theory). A rejected [edge](graph-theory.md#edge-of-a-graph) can never cross a later component's boundary, since components only merge. Thus each accepted [edge](graph-theory.md#edge-of-a-graph) is lightest across the [cut of a graph](graph-theory.md#cut-graph-theory) given by one current component. The [minimum spanning tree cut property](#minimum-spanning-tree-cut-property) proves that the final [spanning tree](#spanning-tree) is minimum.

<h5 id="prim-s-algorithm">Prim's algorithm</h5>

↑ **Parent:** [Minimum spanning tree](#minimum-spanning-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prim's_algorithm)

Start from one [graph vertex](graph.md#vertex-graph-theory). Repeatedly add the least-weight [edge](graph-theory.md#edge-of-a-graph) joining the reached [graph vertices](graph.md#vertex-graph-theory) to an unreached [graph vertex](graph.md#vertex-graph-theory). Each step grows a [tree](#tree-graph-theory) and obeys the [minimum spanning tree cut property](#minimum-spanning-tree-cut-property). On a finite connected [graph](graph.md), the result is a [minimum spanning tree](#minimum-spanning-tree).

##### Minimum spanning tree cycle property

↑ **Parent:** [Minimum spanning tree](#minimum-spanning-tree)

The unique heaviest [edge](graph-theory.md#edge-of-a-graph) on a [graph cycle](graph-theory.md#cycle-in-a-graph) belongs to no [minimum spanning tree](#minimum-spanning-tree). If a [spanning tree](#spanning-tree) contains it, deleting it gives two components; the rest of the [graph cycle](graph-theory.md#cycle-in-a-graph) has a lighter [edge](graph-theory.md#edge-of-a-graph) across that [cut of a graph](graph-theory.md#cut-graph-theory). Insert that [edge](graph-theory.md#edge-of-a-graph) to reduce the weight. This is the deletion certificate used by the [reverse-delete algorithm](#reverse-delete-algorithm).

##### Minimum spanning tree cut property

↑ **Parent:** [Minimum spanning tree](#minimum-spanning-tree)

The unique lightest [edge](graph-theory.md#edge-of-a-graph) across a [cut of a graph](graph-theory.md#cut-graph-theory) belongs to every [minimum spanning tree](#minimum-spanning-tree). If a [spanning tree](#spanning-tree) omits it, inserting it creates a [graph cycle](graph-theory.md#cycle-in-a-graph) with another [edge](graph-theory.md#edge-of-a-graph) across that [cut of a graph](graph-theory.md#cut-graph-theory). Removing that heavier [edge](graph-theory.md#edge-of-a-graph) gives a lighter [spanning tree](#spanning-tree), a contradiction. This proves the correctness of [Prim algorithm](#prim-s-algorithm) and [Kruskal algorithm](#kruskal-s-algorithm) for distinct weights.

#### Uniform spanning tree

↑ **Parent:** [Spanning tree](#spanning-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_spanning_tree)

A uniform spanning tree is sampled uniformly from all spanning trees of a finite connected graph.

##### Uniform spanning tree of a recurrent infinite graph

↑ **Parent:** [Uniform spanning tree](#uniform-spanning-tree)

On a connected locally finite [recurrent graph](markov-process.md#recurrent-graph), root [Wilson's algorithm](#wilson-s-algorithm) at a fixed [graph vertex](graph.md#vertex-graph-theory) $r$ and process a countable enumeration of the [graph vertices](graph.md#vertex-graph-theory). Every walk hits the existing [tree](#tree-graph-theory) [almost surely](convergence-of-random-variables.md#almost-sure-convergence), since it contains $r$. Each attached [graph path](graph-theory.md#path-in-a-graph) is finite, and the union is a connected acyclic spanning subgraph. Its law is the infinite [uniform spanning tree](#uniform-spanning-tree).

It is also the common free and wired finite-volume [limit of a sequence](real-analysis.md#limit-of-a-sequence) along every [graph exhaustion](graph-theory.md#graph-exhaustion). For a finite [edge](graph-theory.md#edge-of-a-graph) set, run a finite initial segment of the chosen enumeration containing all its endpoints. Its membership is then permanently decided, because later attachments have new internal [graph vertices](graph.md#vertex-graph-theory). Only finitely many finite random-walk trajectories were used, and their [graph vertices](graph.md#vertex-graph-theory) and [graph neighbours](graph-theory.md#neighbour-of-a-vertex) fit inside all sufficiently large exhaustion sets. Coupling then gives convergence of those finite-dimensional [edge](graph-theory.md#edge-of-a-graph) laws for both boundary conventions. Finite [Wilson's algorithm](#wilson-s-algorithm) is root/order independent, so the limiting law is too. There is no uniform counting measure on all infinite [spanning trees](#spanning-tree); the definition is this limiting [probability](probability-theory.md#probability) law.

##### Uniform spanning forest

↑ **Parent:** [Uniform spanning tree](#uniform-spanning-tree)

A uniform spanning forest is an infinite-volume limit of [uniform spanning trees](#uniform-spanning-tree) on finite graph approximations. Free and wired boundary identifications give the [free uniform spanning forest](#free-uniform-spanning-forest) and [wired uniform spanning forest](#wired-uniform-spanning-forest), respectively.

##### Free uniform spanning forest

↑ **Parent:** [Uniform spanning tree](#uniform-spanning-tree)

The free uniform spanning forest of an infinite locally finite graph is the weak limit of uniform spanning trees on finite induced connected exhaustions with free boundary. Every component is infinite almost surely.

###### Negative association of uniform spanning-tree edges

↑ **Parent:** [Free uniform spanning forest](#free-uniform-spanning-forest)

For a uniform spanning tree, increasing events supported on disjoint sets of edges have nonpositive covariance. This negative association and the spatial Markov property imply monotonicity of free-boundary spanning-tree measures under exhaustion.

##### Transfer-current theorem

↑ **Parent:** [Uniform spanning tree](#uniform-spanning-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transfer-current_theorem)

For oriented edges $e_1,\ldots,e_k$, the probability that their unoriented versions all belong to a uniform spanning tree is the determinant of the matrix of transfer currents between them. In particular, every finite forest that can be extended to a spanning tree has positive inclusion probability.

###### Mean spanning-tree path current

↑ **Parent:** [Transfer-current theorem](#transfer-current-theorem)

In a finite unweighted [connected graph](graph.md#connected-graph), take distinct [graph vertices](graph.md#vertex-graph-theory) $a\ne z$ and orient the unique [graph path](graph-theory.md#path-in-a-graph) from $a$ to $z$ in a [uniform spanning tree](#uniform-spanning-tree) and assign signed unit current to its [edges](graph-theory.md#edge-of-a-graph). Its mean over [trees](#tree-graph-theory) is the electrical [unit flow](graph-theory.md#unit-flow) from $a$ to $z$. The [Kirchhoff node law](markov-process.md#kirchhoff-node-law) follows by averaging [graph path](graph-theory.md#path-in-a-graph) divergences. For the [graph cycle](graph-theory.md#cycle-in-a-graph) law, let $\mathcal F_{az}$ be the [two-component spanning forests](#two-component-spanning-forest) separating the terminals and $A_F$ the component containing $a$. Deleting a tree-path [edge](graph-theory.md#edge-of-a-graph) and conversely adjoining an [edge](graph-theory.md#edge-of-a-graph) across a forest cut are inverse operations. Hence the mean signed current on an [edge](graph-theory.md#edge-of-a-graph) $u\to v$ is

$$
J(u,v)=\frac1{|\mathcal T(G)|}\sum_{F\in\mathcal F_{az}}\bigl(\mathbf1_{A_F}(u)-\mathbf1_{A_F}(v)\bigr).
$$

This is the gradient of $h(u)=|\mathcal T(G)|^{-1}\sum_F\mathbf1_{A_F}(u)$, proving the [graph cycle](graph-theory.md#cycle-in-a-graph) law. In particular $R_{\mathrm{eff}}(a,z)=|\mathcal F_{az}|/|\mathcal T(G)|$. For an oriented existing [edge](graph-theory.md#edge-of-a-graph) $e=(a,z)$, that [edge](graph-theory.md#edge-of-a-graph) is used by the [tree](#tree-graph-theory) [graph path](graph-theory.md#path-in-a-graph) exactly when it belongs to the [tree](#tree-graph-theory), and then has positive orientation. Thus its mean current is $\mathbb P(e\in T)$, giving the [edge-inclusion formula for a uniform spanning tree](#edge-inclusion-formula-for-a-uniform-spanning-tree) by [Ohm's law](electromagnetism.md#ohm-s-law).

###### Edge-inclusion formula for a uniform spanning tree

↑ **Parent:** [Transfer-current theorem](#transfer-current-theorem)

For an edge $e=\{a,b\}$ of conductance $c_e$ in a finite [electrical network](markov-process.md#electrical-network), its inclusion probability in the conductance-weighted [uniform spanning tree](#uniform-spanning-tree) is $c_eR_{\mathrm{eff}}(a,b)$. The same formula holds for the wired limit using the limiting wired [effective resistance](markov-process.md#effective-resistance).

##### Translation ergodicity of a uniform spanning forest

↑ **Parent:** [Uniform spanning tree](#uniform-spanning-tree)

On a transitive graph, the free and wired uniform spanning-forest measures are invariant and ergodic under the transitive automorphism group. Consequently every translation-invariant event has probability zero or one.

##### Aldous-Broder algorithm

↑ **Parent:** [Uniform spanning tree](#uniform-spanning-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Aldous-Broder_algorithm)

The Aldous-Broder algorithm runs a random walk and includes the edge by which each vertex other than the start is first entered. On a finite graph this yields a uniform spanning tree. The same first-entrance construction works on recurrent infinite graphs through the infinite-volume limit.

<h5 id="wilson-s-algorithm">Wilson's algorithm</h5>

↑ **Parent:** [Uniform spanning tree](#uniform-spanning-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wilson's_algorithm)

Wilson's algorithm samples a uniform spanning tree by starting from a root and successively attaching loop-erased random walks from vertices not yet in the tree.

##### Wired uniform spanning forest

↑ **Parent:** [Uniform spanning tree](#uniform-spanning-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wired_uniform_spanning_forest)

The wired uniform spanning forest of an infinite graph is the weak limit of uniform spanning trees on finite exhaustions whose exterior vertices are identified to one wired boundary vertex.

###### Wilson algorithm rooted at infinity

↑ **Parent:** [Wired uniform spanning forest](#wired-uniform-spanning-forest)

Wilson's algorithm rooted at infinity builds the wired uniform spanning forest on a [transient graph](markov-process.md#transient-graph) by successively adding [loop-erased](markov-process.md#loop-erasure) random walks, run forever when they never hit the forest already constructed.

###### Component-number zero-one law for the wired uniform spanning forest

↑ **Parent:** [Wired uniform spanning forest](#wired-uniform-spanning-forest)

The number of trees in a wired uniform spanning forest is almost surely constant. This follows from its tail triviality together with the fact that every component is infinite.

#### Directed spanning tree

↑ **Parent:** [Spanning tree](#spanning-tree)

A directed spanning tree rooted towards a vertex $r$ is a spanning tree whose edges are oriented so that every other vertex has a unique directed path to $r$.

<h4 id="kirchhoff-s-theorem">Kirchhoff's theorem</h4>

↑ **Parent:** [Spanning tree](#spanning-tree)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kirchhoff's_theorem)

The matrix-tree theorem expresses the weighted number of [spanning trees](#spanning-tree) of a finite [graph](graph.md) as a cofactor of its [Graph Laplacian](graph-theory.md#laplacian-matrix). For a directed graph with out-Laplacian $L$, deleting the row and column indexed by a root $r$ gives

$$
\det L^{(r)}=\sum_T\prod_{e\in T}w_e,
$$

where the sum runs over [directed spanning trees](#directed-spanning-tree) rooted towards $r$.

<h3 id="cayley-s-formula">Cayley's formula</h3>

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cayley's_formula)

Cayley's formula says that there are $n^{n-2}$ trees on a fixed set of $n$ labelled vertices.

#### Labelled forest count with prescribed roots

↑ **Parent:** [Cayley's formula](#cayley-s-formula)

For a fixed set of $k<n$ roots among $n$ labelled [vertices](graph.md#vertex-graph-theory), the number of [forests](#forest) with exactly one root in each [graph component](graph.md#component-graph-theory) is $kn^{n-k-1}$. Orient edges toward their roots. Repeatedly remove the smallest nonroot leaf and record its parent. This gives a code of length $n-k$ whose last entry is a root. Conversely, for any such code choose the smallest remaining nonroot absent from the remaining code, join it to the first entry, and delete it. There is always a choice because the final entry is a root. These inverse operations give $n^{n-k-1}$ choices for the earlier entries and $k$ for the last. For $k=n$, the empty forest is unique.

<h4 id="prufer-sequence">Prüfer sequence</h4>

↑ **Parent:** [Cayley's formula](#cayley-s-formula)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prüfer_sequence)

For a labelled [tree](#tree-graph-theory) on $n\geq2$ vertices, repeatedly delete the leaf with smallest label and record its neighbour, until two vertices remain. The recorded sequence has length $n-2$. Conversely, given such a sequence, repeatedly join its first label to the smallest remaining label absent from the remaining sequence, remove that latter vertex, and delete the first sequence entry. Finally join the two remaining vertices. These operations are inverse [bijections](function.md#bijection) between labelled [trees](#tree-graph-theory) and sequences of $n-2$ labels, proving the [Cayley formula](#cayley-s-formula) $n^{n-2}$.

<h3 id="konig-s-lemma">Kőnig's lemma</h3>

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kőnig's_lemma)

Every infinite finitely branching rooted tree has an infinite branch. Starting at the root, repeatedly choose a child above which infinitely many vertices remain.

### Breadth-first search

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Breadth-first_search)

Breadth-first search explores a graph in successive distance layers from a starting vertex. Before two exploration branches meet, the explored edges form a tree.

## Double counting (proof technique)

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double_counting_(proof_technique))

Double counting proves an identity by counting the same finite set in two different ways.

## Set partition

↑ **Parent:** [Combinatorics](combinatorics.md)

A set partition is a collection of nonempty, pairwise disjoint subsets called blocks whose union is the original set.

A set partition is a [partition of a set](set.md#partition-of-a-set) into its disjoint nonempty blocks.

### Refinement of a set partition

↑ **Parent:** [Set partition](#set-partition)

A [set partition](#set-partition) $\mathcal Q$ refines $\mathcal P$ if every cell of $\mathcal Q$ is contained in a cell of $\mathcal P$. Thus $\mathcal Q$ retains every separation made by $\mathcal P$ and may make additional separations. [Refinement of a set partition](#refinement-of-a-set-partition) is reflexive and transitive. If each partition refines the other, their cells coincide, so [refinement of a set partition](#refinement-of-a-set-partition) is a partial order on partitions. For finite partitions the nonempty intersections of cells form their common [refinement of a set partition](#refinement-of-a-set-partition). In [graph](graph.md) regularity arguments, subdividing cells and treating discarded [vertices](graph.md#vertex-graph-theory) as singletons preserves [refinement of a set partition](#refinement-of-a-set-partition); merging discarded [vertices](graph.md#vertex-graph-theory) into one cell need not. The [refinement variance identity for regularity energy](probabilistic-combinatorics.md#refinement-variance-identity-for-regularity-energy) consequently proves that this singleton treatment cannot decrease the [equitable regularity energy](probabilistic-combinatorics.md#equitable-regularity-energy).

### Integer partition

↑ **Parent:** [Set partition](#set-partition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integer_partition)

An integer partition of $n$ is a multiset of positive integers whose sum is $n$. The partition function $p(n)$ counts such multisets.

### Stirling numbers of the second kind

↑ **Parent:** [Set partition](#set-partition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stirling_numbers_of_the_second_kind)

The Stirling number of the second kind $\left\{\begin{smallmatrix}n\\k\end{smallmatrix}\right\}$ counts the [set partitions](#set-partition) of an $n$-element set into $k$ blocks. It satisfies

$$
\left\{\begin{matrix}n\\k\end{matrix}\right\}
=k\left\{\begin{matrix}n-1\\k\end{matrix}\right\}
+\left\{\begin{matrix}n-1\\k-1\end{matrix}\right\}.
$$

#### Graphical Stirling number

↑ **Parent:** [Stirling numbers of the second kind](#stirling-numbers-of-the-second-kind)

The graphical Stirling number $\left\{\begin{smallmatrix}n\\k\end{smallmatrix}\right\}_G$ counts partitions of the vertices of a graph $G$ into $k$ nonempty [independent sets](graph-theory.md#independent-set-graph-theory). Equivalently, it counts proper colourings with $k$ unlabeled nonempty colour classes.

## Lattice path

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lattice_path)

A lattice path is a sequence of points in an integer lattice whose consecutive differences belong to a prescribed finite set of steps.

### Self-avoiding walk

↑ **Parent:** [Lattice path](#lattice-path)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Self-avoiding_walk)

An $n$-step [self-avoiding walk](#self-avoiding-walk) on a [graph](graph.md) is a sequence $v_0,\ldots,v_n$ of distinct [graph vertices](graph.md#vertex-graph-theory) with an [edge](graph-theory.md#edge-of-a-graph) between successive [graph vertices](graph.md#vertex-graph-theory). It is a [graph path](graph-theory.md#path-in-a-graph) with $n$ [edges](graph-theory.md#edge-of-a-graph) and $n+1$ [graph vertices](graph.md#vertex-graph-theory). On a transitive [graph](graph.md), the exponential growth rate of rooted [self-avoiding walk](#self-avoiding-walk) counts is the [connective constant](#connective-constant).

#### Partially directed self-avoiding walk

↑ **Parent:** [Self-avoiding walk](#self-avoiding-walk)

On the [square lattice](graph.md#square-lattice), a [self-avoiding walk](#self-avoiding-walk) using north, east and west steps but no south steps. At each horizontal height, self-avoidance forces one monotone horizontal run. Conversely, such runs separated by north steps always give [self-avoiding walks](#self-avoiding-walk), because every new run is at a previously unvisited height.

##### North-east-west self-avoiding walk count

↑ **Parent:** [Partially directed self-avoiding walk](#partially-directed-self-avoiding-walk)

A horizontal run has [generating function](real-analysis.md#generating-function) $R(z)=(1+z)/(1-z)$. Decomposing each walk into $H(NH)^k$ gives $A(z)=R(z)/(1-zR(z))=(1+z)/(1-2z-z^2)$. Thus $a_0=1,a_1=3$ and $a_n=2a_{n-1}+a_{n-2}$. The exponential growth rate is $1+\sqrt2$, furnishing a strict lower bound greater than two for the [connective constant](#connective-constant) of all square-lattice [self-avoiding walks](#self-avoiding-walk).

#### Self-avoiding walk generating function

↑ **Parent:** [Self-avoiding walk](#self-avoiding-walk)

The [generating function](real-analysis.md#generating-function) weights each [self-avoiding walk](#self-avoiding-walk) by $x$ to the power of its length, including the zero-length walk. Its [radius of convergence](real-analysis.md#radius-of-convergence) is the reciprocal of the upper exponential growth rate of the rooted counts, by the [Cauchy-Hadamard theorem](real-analysis.md#cauchy-hadamard-theorem).

##### Even-length walk generating function on a bipartite graph

↑ **Parent:** [Self-avoiding walk generating function](#self-avoiding-walk-generating-function)

In a [bipartite graph](graph-theory.md#bipartite-graph), a [self-avoiding walk](#self-avoiding-walk) ends in its starting class exactly when it has even length. If degrees are bounded by $\Delta$, deleting the last [edge](graph-theory.md#edge-of-a-graph) gives $\sigma_{2k+1}\leq\Delta\sigma_{2k}$ and hence $Z_G^0(x)\leq Z_G(x)\leq(1+\Delta x)Z_G^0(x)$ for $x\geq0$. Thus these [generating functions](real-analysis.md#generating-function) have the same [radius of convergence](real-analysis.md#radius-of-convergence).

###### Triangle replacement for self-avoiding walks

↑ **Parent:** [Even-length walk generating function on a bipartite graph](#even-length-walk-generating-function-on-a-bipartite-graph)

Replace every degree-three [vertex of a graph](graph.md#vertex-graph-theory) in one class of a [bipartite graph](graph-theory.md#bipartite-graph) by a triangle with one port for each incident [edge](graph-theory.md#edge-of-a-graph). A [self-avoiding walk](#self-avoiding-walk) whose endpoints remain in the other class cannot make two completed passages through the same triangle: each passage needs two unused ports and only three exist. Each old two-edge passage has exactly two replacements, of lengths three and four. Therefore the restricted [generating functions](real-analysis.md#generating-function) satisfy $Z_H^0(x)=Z_G^0(\sqrt{x^3+x^4})$. If the old radius is $1/\mu$, the new radius obeys $\rho^3+\rho^4=\mu^{-2}$.

#### Root-moment bound for open self-avoiding walks

↑ **Parent:** [Self-avoiding walk](#self-avoiding-walk)

In independent [bond percolation](bond-percolation.md) on a [graph](graph.md), let $c_n$ be the number of $n$-step [self-avoiding walks](#self-avoiding-walk) from a fixed [graph vertex](graph.md#vertex-graph-theory) and $\kappa_n$ the number that are open. Then $\mathbb E\kappa_n=c_np^n$. The [Jensen inequality](real-analysis.md#jensen-s-inequality) for the [concave function](real-analysis.md#concave-function) $t^{1/n}$ gives $\mathbb E(\kappa_n^{1/n})\leq p c_n^{1/n}$. No [independence](random-variable.md#independent-random-variables) between different [self-avoiding walk](#self-avoiding-walk) indicators is needed. When $c_n^{1/n}\to\mu$, the [limit superior](real-analysis.md#limit-superior) is at most $p\mu$.

#### Directed ladder self-avoiding walk count

↑ **Parent:** [Self-avoiding walk](#self-avoiding-walk)

On the [doubly infinite ladder graph](graph.md#doubly-infinite-ladder-graph), [self-avoiding walks](#self-avoiding-walk) from a fixed [graph vertex](graph.md#vertex-graph-theory) using only rightward or vertical steps are in [bijection](function.md#bijection) with words in $R,V$ containing no consecutive $V$ symbols. Their count is $\sigma_n=F_{n+2}$, since $\sigma_0=1$, $\sigma_1=2$, and $\sigma_n=\sigma_{n-1}+\sigma_{n-2}$. Its exponential growth rate is the [golden ratio](algebra.md#golden-ratio).

#### Connective constant

↑ **Parent:** [Self-avoiding walk](#self-avoiding-walk)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Connective_constant)

If $b_n$ counts the $n$-step [self-avoiding walks](#self-avoiding-walk) from a fixed vertex of a transitive lattice, the connective constant is the exponential growth rate

$$
\kappa=\lim_{n\to\infty}b_n^{1/n}.
$$

Submultiplicativity of $b_n$ and the [Fekete lemma](real-analysis.md#fekete-s-lemma) applied to $\log b_n$ prove existence of this limit.

##### Uniform connective constant of a bounded-degree graph

↑ **Parent:** [Connective constant](#connective-constant)

For an infinite connected [locally finite graph](graph-theory.md#locally-finite-graph) with a uniform degree bound, let $\sigma_n(v)$ count its length-$n$ [self-avoiding walks](#self-avoiding-walk) from $v$. The suprema satisfy $\sigma_{m+n}\leq\sigma_m\sigma_n$, so the [Fekete lemma](real-analysis.md#fekete-s-lemma) applied to their logarithms gives a finite [connective constant](#connective-constant). Unlike the usual rooted definition on a [vertex-transitive graph](graph.md#vertex-transitive-graph), this definition explicitly takes the supremum over roots.

### Dyck path

↑ **Parent:** [Lattice path](#lattice-path)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dyck_path)

A Dyck path of semilength $n$ starts at $(0,0)$, ends at $(2n,0)$, uses steps $(1,1)$ and $(1,-1)$, and never passes below the horizontal axis.

#### Catalan number

↑ **Parent:** [Dyck path](#dyck-path)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Catalan_number)

The Catalan number

$$
C_n=\frac1{n+1}\binom{2n}{n}
$$

counts [Dyck paths](#dyck-path) of semilength $n$. Its ordinary generating function $C(x)=\sum_{n\geq0}C_nx^n$ satisfies $C(x)=1+xC(x)^2$.

## Extremal set theory

↑ **Parent:** [Combinatorics](combinatorics.md)

[This section is present in another page, follow this link to view it.](extremal-set-theory.md)

## Polynomial method in combinatorics

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_method_in_combinatorics)

The polynomial method in combinatorics encodes a discrete configuration by polynomials and obtains combinatorial bounds from their degree, zeros, coefficients, or linear independence.

### Rich line covering bound over a finite field

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)

Suppose every point of $\mathbb F_q^n$ lies on an [affine line in a vector space](vector-space.md#affine-line-in-a-vector-space) meeting a subset $N$ in at least $m$ points, with $1\le m\le q$. A smaller $N$ would admit a nonzero [multivariate polynomial](polynomial.md#multivariate-polynomial) of [total degree](polynomial.md#total-degree-of-a-polynomial) at most $m-1$ vanishing on it, by the [dimension of a bounded-total-degree polynomial space](polynomial.md#dimension-of-a-bounded-total-degree-polynomial-space). Each selected line then has more [roots of a polynomial](polynomial.md#root-of-a-polynomial) than the degree of its restriction, so the [polynomial](polynomial.md) vanishes at every point. The [Schwartz-Zippel lemma](#schwartz-zippel-lemma) forbids this because $m-1<q$. Thus the displayed bound holds, and is at least $m^n/n!$. This is a point-covering condition; the [finite-field Kakeya set](vector-space.md#finite-field-kakeya-set) condition instead quantifies over directions.

### Schwartz-Zippel lemma

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)

For a nonzero [multivariate polynomial](polynomial.md#multivariate-polynomial) of [total degree](polynomial.md#total-degree-of-a-polynomial) $d$ over a [field](algebra.md#field), and a finite subset $S$ of that field, at most $d|S|^{n-1}$ points of $S^n$ are zeros. For one variable this is the [root bound for a polynomial](polynomial.md#lagrange-root-bound-over-a-field). If $d\ge|S|$, the bound is already trivial. Otherwise, in the inductive proof write the [polynomial](polynomial.md) as degree $k$ in its last variable, with a nonzero leading coefficient of degree at most $d-k$ in the other variables. The leading coefficient vanishes on at most $(d-k)|S|^{n-2}$ fibers; outside those fibers there are at most $k$ [roots of a polynomial](polynomial.md#root-of-a-polynomial) per fiber. Counting the bad fibers with the trivial $|S|$ bound gives the asserted inequality.

### Polynomial vanishing on a finite set of spatial lines

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)

A family of $L\ge1$ lines in $\mathbb R^3$ imposes at most $L(d+1)$ linear conditions on degree-at-most-$d$ polynomials, by [polynomial restriction to a line](polynomial.md#polynomial-restriction-to-a-line). The coefficient space has dimension $\binom{d+3}{3}$. Whenever $(d+2)(d+3)>6L$, a nonzero common vanishing polynomial exists. Taking $d=\lceil\sqrt{6L}\rceil$ gives degree less than $4\sqrt L$.

### Intersection polynomial

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)

For a finite [set](set.md) $A\subseteq[n]$ and a finite list $L$ of allowed intersection sizes, the displayed [polynomial](polynomial.md) satisfies $p_A(\chi_B)=\prod_{\ell\in L}(|A\cap B|-\ell)$ at [characteristic vectors of sets](extremal-set-theory.md#characteristic-vector-of-a-set). For an $r$-[uniform set family](extremal-set-theory.md#uniform-set-family) whose pairwise intersection sizes lie in $L\subseteq\{0,\ldots,r-1\}$, these [polynomials](polynomial.md) vanish at all other family members and have nonzero values at their own members. Their restrictions are therefore [linearly independent](vector-space.md#linear-independence). [Multilinear reduction on the Boolean cube](polynomial.md#multilinear-reduction-on-the-boolean-cube) and [homogenisation on a uniform layer](polynomial.md#homogenisation-on-a-uniform-layer) then prove the [Ray-Chaudhuri–Wilson theorem](extremal-set-theory.md#ray-chaudhuri-wilson-theorem) bound.

### Zero-sum sequences as differences of permutations of a prime field

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)

Every length-$p$ sequence in the [prime field](algebra.md#prime-field) $\mathbb F_p$ with sum zero, including sequences with repetitions, is the coordinatewise difference of two enumerations of that field. Apply the [Combinatorial Nullstellensatz](#combinatorial-nullstellensatz) on $(\mathbb F_p^*)^{p-1}$ to the product of the [Vandermonde determinant](galois-theory.md#vandermonde-determinant) in variables $x_i$ and its translate by the first $p-1$ sequence terms. The [Dyson constant-term identity](#dyson-constant-term-identity) gives a nonzero top coefficient, and the zero-sum condition supplies the final missing field element. The argument includes $p=2$.

### Polynomial nonvanishing below the field size

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)

Let $P\in\mathbb F_p[x_1,\ldots,x_n]$ have [total degree of a polynomial](polynomial.md#total-degree-of-a-polynomial) less than $p$. If the associated [polynomial function](polynomial.md#polynomial-function) vanishes on all of $\mathbb F_p^n$, then $P$ is the zero polynomial. Induct on $n$: write

$$
P=\sum_{j=0}^{p-1}P_j(x_1,\ldots,x_{n-1})x_n^j.
$$

For each fixed $(x_1,\ldots,x_{n-1})$, the resulting univariate polynomial of degree less than $p$ has all $p$ field elements as [roots](polynomial.md#root-of-a-polynomial), so every coefficient $P_j$ vanishes everywhere. The induction hypothesis makes every $P_j$ the zero polynomial.

### Cap set

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cap_set)

A cap set is a subset $A\subseteq\mathbb F_3^n$ containing no three distinct points $x,y,z$ satisfying $x+y+z=0$. Equivalently, it contains no nonconstant three-term [arithmetic progression](arithmetic.md#arithmetic-progression).

#### Meshulam bound for cap sets

↑ **Parent:** [Cap set](#cap-set)

A [cap set](#cap-set) in $\mathbb F_3^n$ has [subset density](additive-combinatorics.md#density-of-a-finite-subset) $O(1/n)$. A [Fourier analysis on a finite abelian group](additive-combinatorics.md#normalized-fourier-analysis-on-a-finite-abelian-group) proof uses a [hyperplane density increment for cap sets](additive-combinatorics.md#hyperplane-density-increment-for-cap-sets) repeatedly: absence of nondiagonal zero-sum triples forces a large [finite abelian Fourier coefficient](additive-combinatorics.md#fourier-coefficient-on-a-finite-abelian-group), and hence a denser slice. This is a weaker bound than the [Ellenberg–Gijswijt cap-set bound](#ellenberg-gijswijt-cap-set-bound), but illustrates the [density increment](additive-combinatorics.md#density-increment) method.

#### Cartesian powers of cap sets

↑ **Parent:** [Cap set](#cap-set)

Every [Cartesian product](set-theory.md#cartesian-product) of [cap sets](#cap-set) is a [cap set](#cap-set). In [characteristic](algebra.md#characteristic-of-a-field) three, $x+y+z=0$ with any two equal forces all three equal. A zero-sum triple in a [Cartesian product](set-theory.md#cartesian-product) of [cap sets](#cap-set) is therefore diagonal in every coordinate block, hence diagonal overall.

##### Removal of an exponential prefactor by Cartesian powers

↑ **Parent:** [Cartesian powers of cap sets](#cartesian-powers-of-cap-sets)

Suppose every [cap set](#cap-set) in $\mathbb F_3^n$ has [cardinality](set-theory.md#cardinality) at most $K\theta^n$, with $K$ independent of $n$. Applying this to the $k$-fold [Cartesian product](set-theory.md#cartesian-product) of a fixed [cap set](#cap-set) $A$ gives $|A|^k\leq K\theta^{nk}$. Taking $k$th roots and letting $k$ tend to infinity proves $|A|\leq\theta^n$. More generally this argument applies to any class of finite objects closed under products with multiplicative size and additive dimension.

<h4 id="ellenberg-gijswijt-cap-set-bound">Ellenberg–Gijswijt cap-set bound</h4>

↑ **Parent:** [Cap set](#cap-set)

There is a constant $C<3$ such that every [cap set](#cap-set) in $\mathbb F_3^n$ has cardinality less than $C^n$.

For the [polynomial method in combinatorics](#polynomial-method-in-combinatorics), use

$$
T(x,y,z)=\prod_{i=1}^n\bigl(1-(x_i+y_i+z_i)^2\bigr).
$$

Over $\mathbb F_3$, this is the [indicator function](measure-theory.md#indicator-function) of $x+y+z=0$. On $A^3$ it is therefore a diagonal tensor with $|A|$ nonzero diagonal entries. Every [monomial](polynomial.md#monomial) in its expansion has individual exponents at most two and total degree at most $2n$, so one of its three variable blocks has degree at most $2n/3$. Grouping terms according to such a block and using the [slice rank of a diagonal tensor](linear-algebra.md#slice-rank-of-a-diagonal-tensor) gives

$$
|A|=\operatorname{slice\ rank}(T|_{A^3})\leq3m_n,
$$

where $m_n$ is the number of $\alpha\in\{0,1,2\}^n$ with $\sum_i\alpha_i\leq2n/3$. If $X_i=1-\alpha_i$ are [independent random variables](random-variable.md#independent-random-variables) uniform on $\{-1,0,1\}$, then

$$
\frac{m_n}{3^n}=\mathbb P\left(\sum_iX_i\geq\frac n3\right).
$$

Any exponential upper bound for this [tail probability](probability-theory.md#tail-probability) gives $m_n\leq(3-\epsilon)^n$ and hence the result after absorbing the factor three and finitely many small dimensions into $C<3$.

##### Low-degree monomial count for the cap-set bound

↑ **Parent:** [Ellenberg–Gijswijt cap-set bound](#ellenberg-gijswijt-cap-set-bound)

The number $m_n$ of [monomials](polynomial.md#monomial) in $n$ variables with each exponent at most two and total [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $\lfloor2n/3\rfloor$ satisfies

$$
m_n\leq\left(\frac74\,2^{2/3}\right)^n.
$$

For each exponent vector $a$ counted on the left, $1\leq2^{2n/3-\sum_i a_i}$. Summing and then allowing all $a\in\{0,1,2\}^n$ gives $m_n\leq2^{2n/3}(1+1/2+1/4)^n$. The base has cube $343/16<27$, so it is strictly less than three. This elementary weighted count gives the exponential saving in the [polynomial method in combinatorics](#polynomial-method-in-combinatorics) without an unstated [probability](probability-theory.md#probability) estimate.

### Chevalley-Warning theorem

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chevalley-Warning_theorem)

If polynomials $f_1,\ldots,f_r$ over a finite field have total degree sum strictly smaller than their number of variables, then the number of their common zeros is divisible by the field characteristic.

#### Kemnitz theorem

↑ **Parent:** [Chevalley-Warning theorem](#chevalley-warning-theorem)

Every sequence of $4p-3$ elements of $\mathbb F_p^2$, where $p$ is prime, contains $p$ terms whose sum is zero. A proof applies the [Chevalley-Warning theorem](#chevalley-warning-theorem) to the cardinality and two coordinate sums and then double-counts zero-sum subsequences.

### Dyson constant-term identity

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dyson_constant-term_identity)

For nonnegative integers $a_1,\ldots,a_n$,

$$
\operatorname{CT}\prod_{i=1}^n\prod_{j\ne i}
\left(1-\frac{X_i}{X_j}\right)^{a_i}
=\frac{(a_1+\cdots+a_n)!}{a_1!\cdots a_n!}.
$$

#### Good recurrence for the Dyson constant term

↑ **Parent:** [Dyson constant-term identity](#dyson-constant-term-identity)

When all exponents are positive, the [Dyson constant-term identity](#dyson-constant-term-identity) satisfies $D(a)=\sum_i D(a-e_i)$. This follows from the rational identity $\sum_i\prod_{j\ne i}(1-X_i/X_j)^{-1}=1$, obtained from [Lagrange interpolation polynomial](numerical-analysis.md#lagrange-polynomial) at zero. When $a_i=0$, taking the constant term in $X_i$ deletes that coordinate, giving the boundary recurrence.

### Snevily matching theorem for an elementary abelian group

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)

Let $A$ and $B$ be $k$-element subsets of the additive group of a field of odd characteristic $p$, with $k<p$. There is a bijection $\pi:A\to B$ for which the sums $a+\pi(a)$ are pairwise distinct. The exterior-algebra proof works because $k!\ne0$ in the field.

### Alon-Tarsi lemma

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)

Let $f\in F[x_1,\ldots,x_n]$ have degree at most $d_1+\cdots+d_n$, and let each $A_i\subset F$ contain $d_i+1$ distinct elements. The Alon-Tarsi coefficient formula is

$$
[x_1^{d_1}\cdots x_n^{d_n}]f
=\sum_{a_i\in A_i}
\frac{f(a_1,\ldots,a_n)}
{\prod_i\prod_{b\in A_i\setminus\{a_i\}}(a_i-b)}.
$$

It follows by applying [Lagrange interpolation](numerical-analysis.md#lagrange-polynomial) successively in each variable.

#### Combinatorial Nullstellensatz

↑ **Parent:** [Alon-Tarsi lemma](#alon-tarsi-lemma)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Combinatorial_Nullstellensatz)

One coefficient form of the Combinatorial Nullstellensatz says that if $\deg f\leq d_1+\cdots+d_n$ and $[x_1^{d_1}\cdots x_n^{d_n}]f\ne0$, then for every choice of sets $A_i$ with $|A_i|=d_i+1$ there is a point $(a_1,\ldots,a_n)\in A_1\times\cdots\times A_n$ at which $f$ does not vanish.

##### Restricted sumset bound for unequal subsets of a prime field

↑ **Parent:** [Combinatorial Nullstellensatz](#combinatorial-nullstellensatz)

Suppose $|A|>|B|>0$ in $\mathbb F_p$. Put $a=|A|$ and $b'=\min(|B|,p+2-a)$, and choose $B'\subseteq B$ of size $b'$. Let $r=a+b'-2$. If the restricted sumset fits in a set $D$ of size $r-1$, then $(x-y)\prod_{d\in D}(x+y-d)$ vanishes on $A\times B'$. Its [coefficient](vector-space.md#coefficient) of $x^{a-1}y^{b'-1}$ is

$$
(a-b')\frac{(r-1)!}{(a-1)!(b'-1)!}\ne0\quad\text{in }\mathbb F_p.
$$

All factorial arguments are below $p$ and $0<a-b'<p$. The [Combinatorial Nullstellensatz](#combinatorial-nullstellensatz) gives a contradiction. Since $r=\min(p,|A|+|B|-2)$, this includes the saturated case as well as the small-set case.

##### Prime-regular subgraph from Boolean polynomial constraints

↑ **Parent:** [Combinatorial Nullstellensatz](#combinatorial-nullstellensatz)

For [prime](number-theory.md#prime-number) $p$, a [graph](graph.md) with $m>(p-1)n$ [edges](graph-theory.md#edge-of-a-graph) and maximum degree at most $2p-1$ contains a nonempty $p$-regular subgraph. Over $\mathbb F_p$, apply the [Combinatorial Nullstellensatz](#combinatorial-nullstellensatz) on the Boolean edge-variable cube to

$$
\prod_v\left(1-\left(\sum_{e\ni v}x_e\right)^{p-1}\right)-\prod_e(1-x_e).
$$

Its full squarefree [coefficient](vector-space.md#coefficient) is nonzero because the first product has degree below $m$. A nonzero value cannot occur at the zero vector; at any other Boolean vector the second product vanishes, and the first forces all selected degrees to be multiples of $p$. The maximum-degree condition makes every positive selected degree exactly $p$.

##### Coordinate avoidance from a nonzero permanent

↑ **Parent:** [Combinatorial Nullstellensatz](#combinatorial-nullstellensatz)

If an $n$ by $n$ matrix $A$ over a field has nonzero [permanent](linear-algebra.md#permanent-mathematics), $b\in F^n$, and every $S_i\subseteq F$ has two elements, then some $x\in\prod_iS_i$ makes every coordinate of $Ax-b$ nonzero. Apply the [Combinatorial Nullstellensatz](#combinatorial-nullstellensatz) to

$$
\prod_{i=1}^n((Ax)_i-b_i),
$$

whose coefficient of $x_1\cdots x_n$ is $\operatorname{perm}A$.

### Modular intersection bound for a set family

↑ **Parent:** [Polynomial method in combinatorics](#polynomial-method-in-combinatorics)

Let $E\subseteq\mathbb F_p$ have size $m$, and let $\mathcal A\subseteq\mathcal P([n])$ satisfy $|A|\notin E$ and $|A\cap B|\in E$ for distinct $A,B\in\mathcal A$. Then

$$
|\mathcal A|\leq\sum_{i=0}^m\binom ni.
$$

The multilinearizations of

$$
P_A(x)=\prod_{e\in E}\left(\sum_{i\in A}x_i-e\right)
$$

are linearly independent functions on the characteristic vectors of the family and lie in the multilinear polynomial space of degree at most $m$.

## Factorial

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Factorial)

For a nonnegative [integer](number-theory.md#integer) $n$, the factorial is

$$
n!=1\cdot2\cdots n,
$$

with $0!=1$.

### Double factorial

↑ **Parent:** [Factorial](#factorial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double_factorial)

The double factorial multiplies the positive integers of the same parity as $n$ up to $n$: $(2m-1)!!=1\cdot3\cdots(2m-1)$ and $(2m)!!=2\cdot4\cdots2m$. Set $(-1)!!=0!!=1$. In particular, $(2m-1)!!=(2m)!/(2^m m!)$, the number of pairings of $2m$ labelled objects.

### Falling factorial

↑ **Parent:** [Factorial](#factorial)

The falling factorial is the product of $j$ successive descending factors, with $(t)_0=1$. Another notation is $t^{\underline j}$; this article uses $(t)_j$ for descending factors, whereas the [rising factorial](#rising-factorial) uses the same notation for ascending factors. For a nonnegative integer $t$, it counts ordered selections of $j$ distinct objects and vanishes when $j>t$. Powers expand as $t^j=\sum_{\ell=0}^j S(j,\ell)(t)_\ell$, where $S(j,\ell)$ is a [Stirling number of the second kind](#stirling-numbers-of-the-second-kind).

### Rising factorial

↑ **Parent:** [Factorial](#factorial)

For a nonnegative integer $n$, the rising factorial is the product of $n$ consecutive increments starting at $a$, with $(a)_0=1$. Another notation is $a^{\overline n}$; the [falling factorial](#falling-factorial) uses descending factors. It compactly expresses the coefficient recurrence of a [confluent hypergeometric function of the first kind](differential-equation.md#confluent-hypergeometric-function-of-the-first-kind).

## Binomial coefficient

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binomial_coefficient)

The [binomial coefficient](#binomial-coefficient)

$$
\binom nk=\frac{n!}{k!(n-k)!}
$$

counts the $k$-element subsets of an $n$-element set. Equivalently, it counts strings containing $k$ copies of one symbol and $n-k$ copies of another.

<h3 id="vandermonde-s-identity">Vandermonde's identity</h3>

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vandermonde's_identity)

Choose a $k$-element [subset](set.md#subset) of a disjoint union of sets of sizes $m$ and $n$. Partition the choices by the number $i$ of selected elements from the first set. The resulting count is the displayed convolution of [binomial coefficients](#binomial-coefficient), where coefficients outside their admissible ranges are zero. This also proves the formula when $k>m+n$.

### Nested-subset binomial identity

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)

For $0\le\ell\le k\le n$, count pairs of [subsets](set.md#subset) $L\subseteq K\subseteq X$ with $|X|=n$, $|L|=\ell$ and $|K|=k$. Choosing $K$ before $L$ gives the left product of [binomial coefficients](#binomial-coefficient). Choosing $L$ and then the $k-\ell$ additional elements of $K$ gives the right product. This [double counting](#double-counting-proof-technique) proof explains the identity without division by factorials.

### Prime-row binomial coefficient divisibility

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)

For a [prime number](number-theory.md#prime-number) $p$, the identity $r!\binom pr=p(p-1)\cdots(p-r+1)$ has right side divisible by $p$, while $r!$ is coprime to $p$. Cancellation in [modular arithmetic](number-theory.md#modular-arithmetic) proves the divisibility.

// Target: combinatorics.bigb

#### Binomial coefficient congruence across a prime row

↑ **Parent:** [Prime-row binomial coefficient divisibility](#prime-row-binomial-coefficient-divisibility)

In polynomial [modular arithmetic](number-theory.md#modular-arithmetic), [prime-row binomial coefficient divisibility](#prime-row-binomial-coefficient-divisibility) gives $(1+X)^p\equiv1+X^p$. Multiply by $(1+X)^k$ and compare coefficients of $X^r$ for $r<p$; the $X^p$ term cannot contribute.

// Target: foundations-of-mathematics.bigb

### Gaussian binomial coefficient

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)

For $0\le k\le n$, this polynomial equals

$$
\sum_{0\le j_1<\cdots<j_k<n}t^{j_1+\cdots+j_k-k(k-1)/2}.
$$

Split the subsets according to whether they contain $n-1$ to obtain $G_{n,k}=G_{n-1,k}+t^{n-k}G_{n-1,k-1}$, with boundary values one. The product satisfies the same recurrence, proving equality and polynomiality. The specialization at $t=1$ is the ordinary [binomial coefficient](#binomial-coefficient).

#### Unimodality of Gaussian binomial coefficients

↑ **Parent:** [Gaussian binomial coefficient](#gaussian-binomial-coefficient)

For $0\le k\le n$, let $V$ be the $n$-dimensional irreducible [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra) representation. Its weights are $n-1,n-3,\ldots,1-n$. A wedge basis shows $\operatorname{ch}\Lambda^kV=q^{-k(n-k)}G_{n,k}(q^2)$, where $G_{n,k}(t)$ is the [Gaussian binomial coefficient](#gaussian-binomial-coefficient). By the [Weyl complete reducibility theorem](semisimple-lie-algebra.md#weyl-complete-reducibility-theorem), this character is a nonnegative sum of irreducible strings $q^m+q^{m-2}+\cdots+q^{-m}$. All its weights have parity $k(n-k)$, so their coefficients increase toward zero and decrease afterward. Consequently the coefficients of $G_{n,k}(t)$ are symmetric and unimodal. The [symmetric quantum binomial coefficient](#symmetric-quantum-binomial-coefficient) is this character, a [Laurent polynomial](polynomial.md#laurent-polynomial); its coefficients are unimodal on the occupied parity. The full integer-exponent sequence need not be unimodal, as $q+q^{-1}$ demonstrates.

#### Symmetric quantum binomial coefficient

↑ **Parent:** [Gaussian binomial coefficient](#gaussian-binomial-coefficient)

The quotient $[n]_q[n-1]_q\cdots[n-k+1]_q/([k]_q\cdots[1]_q)$ is the displayed shifted [Gaussian binomial coefficient](#gaussian-binomial-coefficient). It is the [formal character](semisimple-lie-algebra.md#formal-character-of-a-weight-module) of $\Lambda^kL_{n-1}$, where $L_{n-1}$ is the $n$-dimensional irreducible [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra) representation. Indeed its exterior-power weights are sums of $k$ distinct terms of $n-1,n-3,\ldots,1-n$. [Parity unimodality of an sl2 character](semisimple-lie-algebra.md#parity-unimodality-of-an-sl2-character) proves unimodality after removing the intervening zero coefficients; equivalently, the ordinary Gaussian polynomial has unimodal coefficients.

<h3 id="pascal-s-triangle">Pascal's triangle</h3>

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)

Row $n$ of Pascal's triangle consists of the [binomial coefficients](#binomial-coefficient) $\binom n0,\ldots,\binom nn$, beginning with row $0$. Boundary entries are one, and [Pascal's identity](#pascal-s-rule) says each interior entry is the sum of the two entries above it. The [hockey-stick identity](#hockey-stick-identity) evaluates sums along its diagonals.

### Hockey-stick identity

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)

For nonnegative [integers](number-theory.md#integer) $n,m$, the [binomial coefficients](#binomial-coefficient) satisfy

$$
\sum_{k=0}^m\binom{n+k}k=\binom{n+m+1}m.
$$

The identity follows by [mathematical induction](foundations-of-mathematics.md#mathematical-induction): adding the next term combines two adjacent [binomial coefficients](#binomial-coefficient) through [Pascal's identity](#pascal-s-rule). An equivalent form is $\sum_{r=j}^N\binom rj=\binom{N+1}{j+1}$, a diagonal sum in [Pascal's triangle](#pascal-s-triangle). It provides closed forms for sums of [binomial coefficients](#binomial-coefficient) without expanding individual [factorials](#factorial).

<h3 id="lucas-s-theorem">Lucas's theorem</h3>

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lucas's_theorem)

For a [prime number](number-theory.md#prime-number) $p$, the [binomial coefficient](#binomial-coefficient) modulo $p$ factors into the corresponding digit [binomial coefficients](#binomial-coefficient) in the [base-p expansions](number-theory.md#base-p-expansion) of the nonnegative [integers](number-theory.md#integer) $n,k$. Pad both expansions to the same length and use $\binom ab=0$ when $b>a$. The identity follows by factoring $(1+x)^n$ into digit powers and using the [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism); digit uniqueness identifies each coefficient.

### Prime-power binomial divisibility

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)

For a [prime number](number-theory.md#prime-number) $p$ and integer $r\ge1$, every interior [binomial coefficient](#binomial-coefficient) in row $p^r$ is divisible by $p$. The polynomial identity $(1+x)^p\equiv1+x^p\pmod p$ iterates under the [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism) to $(1+x)^{p^r}\equiv1+x^{p^r}\pmod p$. This concerns divisibility by $p$, not necessarily by $p^r$.

### Binomial coefficients with even interior terms

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)

For a positive integer $N$, all [binomial coefficients](#binomial-coefficient) $\binom Nj$ with $0<j<N$ are even exactly when $N$ is a power of two. Write the binary expansion $N=\sum_{i\in I}2^i$. In the [polynomial ring](commutative-algebra.md#polynomial-ring) $\mathbb F_2[t]$, repeated squaring gives

$$
(1+t)^N=\prod_{i\in I}(1+t^{2^i}).
$$

If $I$ has one element, there are no interior terms. If it has more than one, the coefficient of $t^{2^{\min I}}$ is one and that exponent lies strictly between zero and $N$. This characterization gives a useful parity obstruction directly from the [binary expansion](arithmetic.md#binary-expansion).

### Combinatorial number system

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Combinatorial_number_system)

Every positive integer $m$ has a unique greedy representation

$$
m=\binom{a_r}{r}+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_s}{s},
\qquad a_r>a_{r-1}>\cdots>a_s\geq s.
$$

This is also called the binomial representation of $m$ at level $r$.

<h3 id="pascal-s-rule">Pascal's rule</h3>

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pascal's_rule)

Pascal's identity is

$$
\binom nk=\binom{n-1}k+\binom{n-1}{k-1}.
$$

### Central binomial coefficient

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Central_binomial_coefficient)

The central binomial coefficient is the largest coefficient in the expansion of $(1+1)^{2n}$:

$$
\binom{2n}{n}=\frac{(2n)!}{(n!)^2}.
$$

#### Normalized central binomial coefficients

↑ **Parent:** [Central binomial coefficient](#central-binomial-coefficient)

Set $c_n=4^{-n}\binom{2n}{n}$, with $c_0=1$. Cancellation of factorials gives

$$
c_n=\prod_{j=1}^n\left(1-\frac1{2j}\right),\qquad
\frac{c_{n+1}}{c_n}=1-\frac1{2n+2}.
$$

Consequently $c_n$ decreases to zero: $\log c_n\leq-\frac12\sum_{j=1}^n1/j\leq-\frac12\log(n+1)$. The inequality uses $\log(1-x)\leq-x$ and comparison with $\int_1^{n+1}dt/t$. Conversely $c_n\geq1/(n+1)$ by induction, since its ratio is at least $(n+1)/(n+2)$. Thus $\sum c_n$ diverges while $\sum(-1)^nc_n$ has [conditional convergence](real-analysis.md#conditional-convergence) by the [alternating series test](real-analysis.md#alternating-series-test). These elementary bounds require no asymptotic formula for factorials.

### Multinomial coefficient

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multinomial_coefficient)

For nonnegative integers with $n_1+\cdots+n_r=n$, the [multinomial coefficient](#multinomial-coefficient)

$$
\binom{n}{n_1,\ldots,n_r}
=\frac{n!}{n_1!\cdots n_r!}
$$

counts arrangements of a multiset containing $n_j$ copies of symbol $j$.

#### Multinomial theorem

↑ **Parent:** [Multinomial coefficient](#multinomial-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multinomial_theorem)

For a nonnegative integer $n$,

$$
(x_1+\cdots+x_r)^n
=\sum_{\alpha_1+\cdots+\alpha_r=n}
\frac{n!}{\alpha_1!\cdots\alpha_r!}
x_1^{\alpha_1}\cdots x_r^{\alpha_r}.
$$

### Binomial theorem

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binomial_theorem)

For a nonnegative integer $n$,

$$
(x+y)^n=\sum_{k=0}^n\binom nkx^ky^{n-k}.
$$

Combinatorics studies finite and discrete structures through counting, construction, and extremal arguments.

#### Binomial inversion

↑ **Parent:** [Binomial theorem](#binomial-theorem)

These two finite-sum transformations are inverses over any [commutative ring](commutative-algebra.md#commutative-ring). Substitute one sum into the other and use $\binom nk\binom kj=\binom nj\binom{n-j}{k-j}$. The inner alternating sum is $(1-1)^{n-j}$ by the [binomial theorem](#binomial-theorem), so only $j=n$ survives. In a [Mahler expansion](arithmetic.md#mahler-s-theorem), $b_n$ is the nth [finite difference](finite-difference.md) of the sampled values $a_k$.

#### Alternating binomial moment

↑ **Parent:** [Binomial theorem](#binomial-theorem)

For nonnegative integers $r,n$, the alternating binomial moment satisfies $S_r(n)=0$ when $r<n$ and $S_n(n)=(-1)^nn!$. Expand the [polynomial](polynomial.md) $X^r$ in [falling factorials](#falling-factorial) and differentiate the [binomial theorem](#binomial-theorem) to prove these identities. Equivalently, alternating [binomial coefficients](#binomial-coefficient) implement a finite difference that annihilates polynomials of degree less than $n$.

<h4 id="freshman-s-dream">Freshman's dream</h4>

↑ **Parent:** [Binomial theorem](#binomial-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Freshman's_dream)

In a commutative ring of characteristic $p$,

$$
(x+y)^p=x^p+y^p.
$$

Iteration gives $(x+y)^{p^n}=x^{p^n}+y^{p^n}$.

#### Binomial theorem for commuting matrices

↑ **Parent:** [Binomial theorem](#binomial-theorem)

If square matrices $A$ and $B$ commute, then

$$
(A+B)^n=\sum_{k=0}^n\binom nkA^{n-k}B^k.
$$

The usual proof works because commutativity allows words with the same numbers of $A$ and $B$ factors to be collected.

#### Alternating binomial-square sum

↑ **Parent:** [Binomial theorem](#binomial-theorem)

Coefficient extraction from $(1-x)^n(1+x)^n=(1-x^2)^n$ gives

$$
\sum_{r=0}^n(-1)^r\binom nr^2
=\begin{cases}0,&n\text{ odd},\\(-1)^{n/2}\binom n{n/2},&n\text{ even}.
\end{cases}
$$

## Alternating-permutation convolution

↑ **Parent:** [Combinatorics](combinatorics.md)

Splitting an alternating permutation at its maximum gives

$$
2A_{n+1}=\sum_{k=0}^n\binom nkA_kA_{n-k},
$$

where $A_n$ counts up-down permutations and complementation identifies up-down with down-up permutations.

## Overlap structure of digit spalindromes

↑ **Parent:** [Combinatorics](combinatorics.md)

Two length-$2k$ palindromes with distinct first-half digits cannot begin fewer than $k$ positions apart: the later first half would include the repeated middle pair of the earlier palindrome. At separation $k$, their union has form $A A^{\rm rev}A$.

## Stars and bars (combinatorics)

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stars_and_bars_(combinatorics))

The number of nonnegative integer solutions of $x_1+\cdots+x_k=N$ is $\binom{N+k-1}{k-1}$.

### Bounded weak compositions

↑ **Parent:** [Stars and bars (combinatorics)](#stars-and-bars-combinatorics)

To count nonnegative tuples with $\sum_{i=0}^r n_i=N$ and $n_i<a_i$, mark violations $n_i\geq a_i$. An intersection of violations indexed by $J$ is in [bijection](function.md#bijection) with unrestricted tuples of sum $N-\sum_{i\in J}a_i$, by subtracting the bounds from those coordinates. [Stars and bars](#stars-and-bars-combinatorics) counts this intersection; the [inclusion-exclusion principle](#inclusion-exclusion-principle) then gives the displayed formula. A negative remaining sum contributes zero.

## Inclusion-exclusion principle

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inclusion-exclusion_principle)

For finite sets $A_1,\ldots,A_n$, the cardinality of their union is the alternating sum of the cardinalities of their nonempty intersections.

### Weighted inclusion-exclusion principle

↑ **Parent:** [Inclusion-exclusion principle](#inclusion-exclusion-principle)

For finite [subsets](set.md#subset) $A_i$ of a finite ambient [set](set.md) $X$, the [indicator function](measure-theory.md#indicator-function) of their complement is $\prod_i(1-\mathbf1_{A_i})$. Expanding this finite product and summing it against any weight $f:X\to\mathbb R$ proves the weighted formula. The empty intersection is $X$. Negative weights are allowed; finiteness removes every convergence issue.

### Inclusion-exclusion for exact block occupancy

↑ **Parent:** [Inclusion-exclusion principle](#inclusion-exclusion-principle)

Suppose $N$ disjoint blocks each have $m$ elements. The number of $K$-element subsets having exactly $q>0$ elements in at least one block is the displayed sum, with $1\leq r\leq\min(N,\lfloor K/q\rfloor)$ and invalid [binomial coefficients](#binomial-coefficient) interpreted as zero. For a specified set of $r$ blocks, choose $q$ elements in each and all remaining elements outside those blocks; [inclusion-exclusion](#inclusion-exclusion-principle) then counts the union of the exact-occupancy events. Excluding the rest of each specified block is essential.

// Target: algebra.bigb

### Cyclic difference constraints

↑ **Parent:** [Inclusion-exclusion principle](#inclusion-exclusion-principle)

Let $f$ take values in the additive [cyclic group](group.md#cyclic-group) $\mathbb Z/n\mathbb Z$ on a cycle with $n$ vertices. A constraint on edge $j$ prescribes $f(j)-f(j-1)=c_j$. Any proper selection of $k<n$ edges leaves disjoint paths, hence $n-k$ free initial values and $n^{n-k}$ solutions. The full cycle has $n$ solutions if $\sum_jc_j=0$ and none otherwise. Combining these intersection counts with the [inclusion-exclusion principle](#inclusion-exclusion-principle) gives

$$
\#\{f:\ f(j)-f(j-1)\ne c_j\text{ for every }j\}=(n-1)^n+(-1)^n(F-1),
$$

where $F$ is $n$ or zero according to the full-cycle consistency condition. This is a useful example in which every proper collection of local constraints is independent, but the full collection has one global obstruction.

### Bonferroni inequalities

↑ **Parent:** [Inclusion-exclusion principle](#inclusion-exclusion-principle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bonferroni_inequalities)

Truncating the [inclusion-exclusion principle](#inclusion-exclusion-principle) after an odd number of terms gives an upper bound, and truncating after an even number gives a lower bound. In particular,

$$
\mathbb P\left(\bigcup_iA_i\right)
\geq\sum_i\mathbb P(A_i)-\sum_{i<j}\mathbb P(A_i\cap A_j).
$$

#### Jordan-Bonferroni exact-occurrence inequalities

↑ **Parent:** [Bonferroni inequalities](#bonferroni-inequalities)

For the number $N$ of occurring events, write $S_j=\mathbb E\binom Nj$ and $T_m=\sum_{r=0}^m(-1)^r\binom{k+r}kS_{k+r}$. Then odd truncations bound $\Pr(N=k)$ below and even truncations above. For each integer $N>k$, the truncated binomial sum equals $(-1)^m\binom Nk\binom{N-k-1}m$ when $m<N-k$, and is zero otherwise. Its sign proves the bounds on taking [expectations](probability-theory.md#expected-value). This is the exact-count version of the [Bonferroni inequalities](#bonferroni-inequalities).

## Geometric combinatorics

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_combinatorics)

Geometric combinatorics studies discrete aspects of geometric objects and uses combinatorial methods to prove geometric inequalities.

### Euclidean body

↑ **Parent:** [Geometric combinatorics](#geometric-combinatorics)

A Euclidean body is a nonempty bounded [Lebesgue measurable set](measure-theory.md#lebesgue-measurable-set) in $\mathbb R^n$ of positive [Lebesgue measure](measure-theory.md#lebesgue-measure). Projection inequalities require measurable coordinate projections, as for a [compact set](topology.md#compact-space) or a bounded [Borel set](measure-theory.md#borel-set). Modifying a body on a set of volume zero can change its coordinate-projection measures, so the actual projection sets matter. Geometric equality statements commonly impose additional regularity.

#### Axis-parallel box

↑ **Parent:** [Euclidean body](#euclidean-body)

An axis-parallel box in $\mathbb R^n$ is a [Cartesian product](set-theory.md#cartesian-product) $I_1\times\cdots\times I_n$ of bounded intervals. Its volume is the product of its side lengths, and each coordinate projection is the product of the corresponding intervals.

#### Coordinate projection of a Euclidean body

↑ **Parent:** [Euclidean body](#euclidean-body)

For $A\subseteq[n]$, the coordinate projection $S_A$ of $S\subseteq\mathbb R^n$ consists of the coordinate tuples $(x_i)_{i\in A}$ obtained from points $x\in S$. Its measure is denoted $|S_A|$.

##### Uniform cover

↑ **Parent:** [Coordinate projection of a Euclidean body](#coordinate-projection-of-a-euclidean-body)

A multiset $\mathcal C$ of subsets of $[n]$ is a $k$-uniform cover when every index belongs to exactly $k$ members of $\mathcal C$, counted with multiplicity.

###### Fractional uniform cover

↑ **Parent:** [Uniform cover](#uniform-cover)

Nonnegative weights $\lambda_A$ on coordinate subsets form a fractional uniform cover when the displayed equality holds for each coordinate. Rational weights can be multiplied by a common denominator to become an integer [uniform cover](#uniform-cover). The [uniform covers theorem](#uniform-covers-theorem) then gives $\log|S|\leq\sum_A\lambda_A\log|S_A|$. Exact equality of coordinate coverage matters when projection measures may be less than one.

###### Uniform covers theorem

↑ **Parent:** [Uniform cover](#uniform-cover)

If $\mathcal C$ is a $k$-uniform cover of $[n]$ and $S\subseteq\mathbb R^n$ is a [Euclidean body](#euclidean-body), then

$$
|S|^k\leq\prod_{A\in\mathcal C}|S_A|.
$$

Slicing in one coordinate, applying the theorem inductively to each slice, and then applying [Hölder's inequality](real-analysis.md#holder-s-inequality) to the $k$ projected slice functions proves the inequality.

Exact covering is essential for unrestricted real volumes. Finite subsets of a Cartesian product satisfy the analogous cardinality inequality, and in that discrete version covering at least $k$ times suffices.

###### Box theorem

↑ **Parent:** [Uniform covers theorem](#uniform-covers-theorem)

A [Euclidean body](#euclidean-body) has an [axis-parallel box](#axis-parallel-box) of the same volume with every coordinate-projection volume no larger than its own. In logarithmic coordinates the box side lengths solve a [linear program](mathematical-optimization.md#linear-programming) with constraints $\sum_{i\in A}x_i\leq\log|K_A|$. Its dual uses nonnegative exact fractional covers; the [uniform cover inequality](#uniform-covers-theorem) bounds every dual objective below by $\log|K|$, proving existence by [strong duality](mathematical-optimization.md#strong-duality).

An alternative proof minimizes an array of candidate projection volumes subject to the finitely many inequalities from [irreducible uniform covers](#irreducible-uniform-cover). Tight constraints force the array to factor into its singleton coordinates, which become the side lengths of the box.

###### Logarithmic linear program for the box theorem

↑ **Parent:** [Box theorem](#box-theorem)

Set $x_i=\log b_i$ for candidate [axis-parallel box](#axis-parallel-box) side lengths. Its coordinate-projection constraints are the displayed [linear program](mathematical-optimization.md#linear-programming). The dual feasible weights are [fractional uniform covers](#fractional-uniform-cover). Its optimal extreme point is rational, so the [uniform covers theorem](#uniform-covers-theorem) forces its objective to be at least $\log|S|$. Weight one on the full coordinate set attains that value. [Strong duality](mathematical-optimization.md#strong-duality) therefore supplies box side lengths with volume $|S|$ and no larger coordinate projections.

<h6 id="loomis-whitney-inequality">Loomis--Whitney inequality</h6>

↑ **Parent:** [Uniform covers theorem](#uniform-covers-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loomis–Whitney_inequality)

The sets $[n]\setminus\{i\}$ form an $(n-1)$-uniform cover, so the [uniform covers theorem](#uniform-covers-theorem) gives

$$
|S|^{n-1}\leq\prod_{i=1}^n|S_{[n]\setminus\{i\}}|.
$$

###### Functional Loomis-Whitney inequality

↑ **Parent:** [Loomis--Whitney inequality](#loomis-whitney-inequality)

Each nonnegative integrable $f_j$ depends on all coordinates except the $j$th. In dimension three, [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) first in the third coordinate and then in the remaining pair proves the displayed estimate. Induction integrates the last coordinate by [Hölder's inequality](real-analysis.md#holder-s-inequality) on the first $d-1$ factors, then applies [Hölder's inequality](real-analysis.md#holder-s-inequality) to the remaining factor and the dimension-$(d-1)$ product. Taking indicators of [coordinate projections of a Euclidean body](#coordinate-projection-of-a-euclidean-body) gives the volume version of the [Loomis--Whitney inequality](#loomis-whitney-inequality).

###### Three projection areas of a volume-one body

↑ **Parent:** [Loomis--Whitney inequality](#loomis-whitney-inequality)

Positive numbers $a,b,c$ are the areas of the three coordinate projections of a volume-one [Euclidean body](#euclidean-body) exactly when $abc\geq1$. Necessity is the three-dimensional [Loomis--Whitney inequality](#loomis-whitney-inequality). For sufficiency take box lengths $x=\sqrt{ac/b}$, $y=\sqrt{ab/c}$ and $z=\sqrt{bc/a}$, and retain the union of the three slabs with first, second or third normalized coordinate at most $t$. All three projections are full rectangles, while volume is $\sqrt{abc}[1-(1-t)^3]$. Choosing $t=1-(1-1/\sqrt{abc})^{1/3}$ gives volume one. The slabs have positive thickness, so the construction uses a body with interior rather than zero-volume additions.

<h6 id="equality-in-the-three-dimensional-loomis-whitney-inequality">Equality in the three-dimensional Loomis--Whitney inequality</h6>

↑ **Parent:** [Loomis--Whitney inequality](#loomis-whitney-inequality)

Equality in the three-dimensional [Loomis--Whitney inequality](#loomis-whitney-inequality) forces a measurable body to agree up to a null set with a Cartesian product $E_1\times E_2\times E_3$. This follows from the equality conditions in the two [Cauchy-Schwarz inequalities](probability-and-statistics.md#cauchy-schwarz-inequality) used in its proof. If the body is connected and is a finite union of positive-volume [axis-parallel boxes](#axis-parallel-box), each $E_i$ is an interval and equality up to a null set upgrades to exact equality with one box.

###### Irreducible uniform cover

↑ **Parent:** [Uniform cover](#uniform-cover)

A uniform cover is irreducible when it is not the disjoint union, as a multiset, of two nonempty uniform covers. There are only finitely many irreducible uniform covers of a fixed finite set: their multiplicity vectors form an [antichain](extremal-set-theory.md#antichain) in $\mathbb N^{2^n}$, and [Dickson lemma](#dickson-s-lemma) forbids an infinite antichain there.

<h6 id="dickson-s-lemma">Dickson's lemma</h6>

↑ **Parent:** [Irreducible uniform cover](#irreducible-uniform-cover)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dickson's_lemma)

Every subset of $\mathbb N^d$ has finitely many coordinatewise minimal elements. Equivalently, $\mathbb N^d$ has no infinite antichain in its coordinatewise partial order.

## Grid graph

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Grid_graph)

The grid graph $[k]^d$ has vertices in the Cartesian power $\{1,\ldots,k\}^d$ and joins two vertices when they differ by one in exactly one coordinate.

### Small-set edge isoperimetry in a square grid

↑ **Parent:** [Grid graph](#grid-graph)

For the $n\times n$ [grid graph](#grid-graph), if $b$ is an integer, $b<n/2$, and $(b-1)^2<a\leq b(b-1)$, the minimum [edge boundary](#edge-boundary-in-a-graph) of an $a$-vertex set is $2b-1$. A corner $(b-1)\times(b-1)$ square with a nonempty partial adjacent column attains it. The lower bound counts occupied rows and columns; full rows or columns are treated separately because they contribute no boundary in their own direction.

### Vertex-isoperimetric inequality in a grid

↑ **Parent:** [Grid graph](#grid-graph)

Among vertex subsets of $[k]^d$ with a fixed cardinality, initial segments of the [simplicial order on a grid](#simplicial-order-on-a-grid) minimize the external vertex boundary.

#### Simplicial order on a grid

↑ **Parent:** [Vertex-isoperimetric inequality in a grid](#vertex-isoperimetric-inequality-in-a-grid)

The simplicial order on $[k]^d$ orders points first by increasing coordinate sum and breaks ties by reverse lexicographic order.

#### Coordinate compression in a product of paths

↑ **Parent:** [Vertex-isoperimetric inequality in a grid](#vertex-isoperimetric-inequality-in-a-grid)

Coordinate compression in direction $i$ replaces every $i$-section of a subset of $[k]^d$ by the initial segment of the [simplicial order on a grid](#simplicial-order-on-a-grid) having the same size. Assuming the vertex-isoperimetric theorem one dimension lower, this operation preserves cardinality and does not increase the [external vertex boundary](graph-theory.md#external-vertex-boundary).

##### Section formula for a grid neighbourhood

↑ **Parent:** [Coordinate compression in a product of paths](#coordinate-compression-in-a-product-of-paths)

Let $A_j\subseteq[k]^{d-1}$ be the section of $A\subseteq[k]^d$ with one coordinate fixed at $j$, and put $A_0=A_{k+1}=\varnothing$. The corresponding section of its [closed graph neighbourhood](graph-theory.md#closed-graph-neighbourhood) is

$$
N[A]_j=N[A_j]\cup A_{j-1}\cup A_{j+1}.
$$

After coordinate compression, the three sets on the right are nested initial simplicial segments. Their union therefore has the largest of their three cardinalities, which is no larger than the original union.

#### Local-to-global lemma for simplicial grid order

↑ **Parent:** [Vertex-isoperimetric inequality in a grid](#vertex-isoperimetric-inequality-in-a-grid)

If initial segments of the simplicial order minimize vertex boundary in $[k]^2$, then they do so in every $[k]^d$. Inductively compress all coordinate sections. The [section formula for a grid neighbourhood](#section-formula-for-a-grid-neighbourhood) shows that no compression enlarges the boundary. Among boundary-minimizing compressed sets choose one with minimum coordinate-sum weight. Any departure from an initial simplicial segment produces an inversion in a two-coordinate face; the two-dimensional theorem replaces that face by its initial segment without enlarging the boundary and strictly lowers the weight. Hence no inversion remains and the set is an initial simplicial segment.

### Gray-code path embedding of a grid in a hypercube

↑ **Parent:** [Grid graph](#grid-graph)

The order $00,01,11,10$ is a [Gray code](graph.md#gray-code) through the four vertices of $Q_2$. Applying this identification independently in $n$ coordinate pairs makes $[4]^n=P_4^n$ a [spanning subgraph](graph-theory.md#spanning-subgraph) of the [hypercube graph](graph.md#hypercube-graph) $Q_{2n}$. Therefore every vertex boundary in $Q_{2n}$ contains the corresponding boundary in $[4]^n$.

## Necklace (combinatorics)

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Necklace_(combinatorics))

A coloring necklace is an equivalence class of colorings of cyclically arranged positions under rotation. [Burnside lemma](representation-theory.md#burnside-s-lemma) counts necklaces by averaging the numbers of colorings fixed by each rotation.

### Coloring bracelet

↑ **Parent:** [Necklace (combinatorics)](#necklace-combinatorics)

A coloring bracelet also identifies colorings related by reflection, so it is an orbit under a [dihedral group](finite-group-theory.md#dihedral-group) rather than only a [cyclic group](group.md#cyclic-group).

## Permutation

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Permutation)

A permutation of a set is a [bijection](function.md#bijection) from that set to itself.

### Cyclic permutation

↑ **Parent:** [Permutation](#permutation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclic_permutation)

A cyclic permutation sends $a_1$ to $a_2$, then through $a_k$ back to $a_1$, fixing elements outside the cycle. A [transposition](#transposition-permutation) is a two-cycle. Every finite [permutation](#permutation) decomposes into disjoint cycles.

### Finitely supported permutation

↑ **Parent:** [Permutation](#permutation)

A finitely supported [permutation](#permutation) fixes every element outside some finite [subset](set.md#subset). The finitely supported [permutations](#permutation) of $\mathbb N$ are the union of the finite [symmetric groups](finite-group-theory.md#symmetric-group) acting on $\{1,\ldots,k\}$, and hence form a [countable set](set-theory.md#countable-set). All [permutations](#permutation) of $\mathbb N$ form an [uncountable set](set-theory.md#uncountable-set): independently swapping or fixing each pair $(2j-1,2j)$ injects the [power set](set.md#power-set) of $\mathbb N$ into this larger [set](set.md).

### Uniform random permutation

↑ **Parent:** [Permutation](#permutation)

A uniform random permutation of $n$ distinct objects gives each of the $n!$ [permutations](#permutation) the same [probability](probability-theory.md#probability). Restricting the order to any fixed subset gives a uniform ordering on that subset. Relative ranks encode such a permutation bijectively by independent choices of an insertion position.

#### Independent relative ranks of a uniform random permutation

↑ **Parent:** [Uniform random permutation](#uniform-random-permutation)

For a [uniform random permutation](#uniform-random-permutation) $a_1,\ldots,a_n$, define $R_i$ as the rank of $a_i$ among $a_1,\ldots,a_i$, with rank one assigned to the smallest value. Each sequence $r_i\in\{1,\ldots,i\}$ corresponds to exactly one [permutation](#permutation): insert index $i$ in position $r_i$ of the current increasing-value list, then assign the final list the values $1,\ldots,n$. The $n!$ equally likely permutations therefore correspond to the $\prod_{i=1}^n i=n!$ equally likely rank sequences. Consequently the $R_i$ are [independent random variables](random-variable.md#independent-random-variables), each with the displayed [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution).

##### Independent record indicators

↑ **Parent:** [Independent relative ranks of a uniform random permutation](#independent-relative-ranks-of-a-uniform-random-permutation)

The indicators $Y_i=\mathbf1_{\{R_i=1\}}$ of successively smaller records are [independent](random-variable.md#independent-random-variables) and have [Bernoulli distributions](discrete-probability-distribution.md#bernoulli-distribution) of parameters $1/i$. Successively larger records use $R_i=i$ and have the same laws. For $K_n=\sum_{i=1}^nY_i$, [expectation](probability-theory.md#expected-value) and [variance additivity for independent random variables](variance.md#variance-additivity-for-independent-random-variables) give $E K_n=\sum_{i=1}^n1/i$ and $\operatorname{Var}K_n=\sum_{i=1}^n(1/i-1/i^2)$.

### Cycle length of a tagged element in a uniform permutation

↑ **Parent:** [Permutation](#permutation)

In a uniformly random [permutation](#permutation) of $N$ objects, the cycle containing one specified object has a uniform length on $\{1,\ldots,N\}$. For length $\ell$, choose the other $\ell-1$ objects, arrange their order around the tagged object, and permute all remaining objects. The count is $\binom{N-1}{\ell-1}(\ell-1)!(N-\ell)!=(N-1)!$, independent of $\ell$. Its mean is $(N+1)/2$, while the mean number of other elements in that cycle is $(N-1)/2$.

### Derangement of a permutation

↑ **Parent:** [Permutation](#permutation)

A [permutation](#permutation) with no fixed points. Applying the [inclusion-exclusion principle](#inclusion-exclusion-principle) to the events that each element is fixed gives $D_n=n!\sum_{k=0}^n(-1)^k/k!$. Therefore $D_n/n!\to e^{-1}$, and the alternating-series remainder is at most $1/(n+1)!$.

// Destination: foundations-of-mathematics.bigb

#### Fixed point count of a uniform random permutation

↑ **Parent:** [Derangement of a permutation](#derangement-of-a-permutation)

Choose the $m$ fixed objects and derange the remaining $n-m$. Their count is $\binom nmD_{n-m}$ among $n!$ equally likely [permutations](#permutation). The [inclusion-exclusion principle](#inclusion-exclusion-principle) for $D_{n-m}$ proves the displayed law, valid for $0\le m\le n$ and zero otherwise. With $D_0=1$, it includes the all-fixed case and the impossibility of exactly $n-1$ fixed objects. For fixed $m$, the law tends to $e^{-1}/m!$, the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) of mean one.

### Cyclic ordering

↑ **Parent:** [Permutation](#permutation)

A [cyclic ordering](#cyclic-ordering) of a finite ground set records its elements around an oriented circle, identifying [permutations](#permutation) that differ by rotation. There are $(n-1)!$ such orderings for $n\geq1$. A uniformly random [permutation](#permutation) induces a uniformly random [cyclic ordering](#cyclic-ordering).

#### Cyclic interval

↑ **Parent:** [Cyclic ordering](#cyclic-ordering)

A [cyclic interval](#cyclic-interval) of length $r$ is the set of $r$ consecutive positions in a [cyclic ordering](#cyclic-ordering). For $1\leq r<n$, there are $n$ distinct intervals, one ending at each position. Under a uniformly random [permutation](#permutation), a fixed $r$-set appears as an interval with probability $n/\binom nr$. This is the counting mechanism of the [Katona circle method](extremal-set-theory.md#katona-circle-method).

### Generalised permutation

↑ **Parent:** [Permutation](#permutation)

A generalised permutation is a finite multiset of ordered pairs, displayed as a two-row array or encoded by a finite-support matrix of nonnegative integer multiplicities $m_{a,b}$. The no-repeated-column condition means every multiplicity is zero or one; entries within either individual row may still repeat.

### Inversion of a permutation

↑ **Parent:** [Permutation](#permutation)

For a [permutation](#permutation) $\pi$ of $\{1,\ldots,n\}$, an inversion is a pair $i<j$ with $\pi(i)>\pi(j)$. Its number equals the [Coxeter length](semisimple-lie-algebra.md#coxeter-length) for adjacent [transpositions](#transposition-permutation): each adjacent swap changes the count by one, and swapping adjacent descents sorts the permutation in exactly that many steps.

### Transposition (permutation)

↑ **Parent:** [Permutation](#permutation)

A transposition is a [permutation](#permutation) that exchanges two elements and fixes every other element. Every transposition has order two.

A transposition is a [cyclic permutation](#cyclic-permutation) of length two.

### Product of two transpositions

↑ **Parent:** [Permutation](#permutation)

A product of two transpositions is the identity when they coincide, a [three-cycle](finite-group-theory.md#three-cycle) when their supports meet in one letter, and a product of two [disjoint permutation cycles](finite-group-theory.md#disjoint-permutation-cycles) when their supports are disjoint.

### Bounded-displacement permutation of the natural numbers

↑ **Parent:** [Permutation](#permutation)

A permutation $\sigma$ of $\mathbb N$ has displacement at most one when $|\sigma(j)-j|\leq1$. Such a permutation is a disjoint collection of fixed points and adjacent transpositions, so independently swapping the pairs $(2n-1,2n)$ already gives uncountably many examples.

## Analysis of Boolean functions

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Analysis_of_Boolean_functions)

Analysis of Boolean functions studies real-valued [functions](function.md) on a [Boolean hypercube](#boolean-hypercube) using [Fourier analysis](#fourier-walsh-transform), [probability theory](probability-theory.md), and [combinatorics](combinatorics.md).

### Friedgut-Kalai sharp threshold theorem

↑ **Parent:** [Analysis of Boolean functions](#analysis-of-boolean-functions)

There is an absolute $C>0$ such that any nontrivial [transitive increasing event](probability-inequality.md#transitive-increasing-event) on $n\geq2$ independent bits satisfies $\mu_q(A)>1-\varepsilon$ if $\mu_p(A)>\varepsilon$, $0<\varepsilon<1/2$, and the displayed bound holds with $p<q<1$. A uniform weighted [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem) gives one pivotal probability at least $c\mu_r(A)(1-\mu_r(A))\log(n)/n$. Transitivity makes the [total influence](#total-influence) at least $c\mu_r(A)(1-\mu_r(A))\log n$. The [Margulis–Russo formula](#margulis-russo-formula) identifies this with the derivative of $\mu_r(A)$. Integration of the derivative of its log odds proves the threshold bound.

### Kahn-Kalai-Linial theorem

↑ **Parent:** [Analysis of Boolean functions](#analysis-of-boolean-functions)

For a [Boolean function](#boolean-function) $f:\{0,1\}^n\to\{0,1\}$ under the uniform [probability measure](probability-theory.md#probability-measure), some coordinate has [influence of a variable](#influence-of-a-variable) at least $c\operatorname{Var}(f)\log(n)/n$, where $c>0$ is an absolute constant and $I_i(f)$ is the probability that flipping coordinate $i$ changes $f$. For [variance](variance.md) bounded below, this is order $\log(n)/n$. The [tribes function](#tribes-function) shows that this order cannot be improved for general balanced [Boolean functions](#boolean-function).

#### Maximum-influence logarithmic lower bound

↑ **Parent:** [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem)

For a zero-one [Boolean function](#boolean-function) on the unbiased [Boolean hypercube](#boolean-hypercube) with flip-probability [influences](#influence-of-a-variable) $\beta_i\leq\beta$, the displayed bound holds for sufficiently small $\beta>0$. If it fails, write $b=\log(1/\beta)/3$. The [total influence](#total-influence) identity puts at least half the nonconstant [Fourier weight](#fourier-weight) on levels $1\leq|S|\leq b$. The [hypercontractive weighted influence bound](#hypercontractive-weighted-influence-bound) at $\delta=e^{-1}$ then gives $\sum_i\beta_i^{2/(1+\delta)}\geq2b\delta^b\operatorname{Var}(f)$. Its upper bound $\beta^{(1-\delta)/(1+\delta)}\sum_i\beta_i$ contradicts $(1-\delta)/(1+\delta)>1/3$.

#### Squared-influence logarithmic lower bound

↑ **Parent:** [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem)

For a zero-one [Boolean function](#boolean-function) of mean $t$, the displayed bound holds for sufficiently large $n$, uniformly in $t$. If it failed, put $v=t(1-t)$, $\lambda=v\log n$ and split its nonconstant [Fourier weight](#fourier-weight) at level $b=(\log n)/3$. The [total influence](#total-influence) bound puts at most $3v/4$ above that level. The [hypercontractive weighted influence bound](#hypercontractive-weighted-influence-bound) with $\delta=1-3\log\log n/\log n$ puts only $o(v)$ below it: the conversion factor $\max_{1\leq s\leq b}[s\delta^{s-1}]^{-1}$ stays bounded, while $\lambda^{2/(1+\delta)}n^{1-2/(1+\delta)}=vO((\log n)^{-1/2+o(1)})$. This contradicts total nonconstant weight $v$.

### Boolean hypercube

↑ **Parent:** [Analysis of Boolean functions](#analysis-of-boolean-functions)

The Boolean hypercube is the set $\{-1,1\}^n$, or equivalently $\{0,1\}^n$. Its [hypercube graph](graph.md#hypercube-graph) joins two vertices exactly when they differ in one coordinate.

#### Face of the Boolean hypercube

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

A face is obtained by fixing some coordinates of the [Boolean hypercube](#boolean-hypercube) and letting the remaining $d$ coordinates vary freely. It is isomorphic to $Q_d$. A two-dimensional face is a square with four vertices, and a face is contained in a [set family](extremal-set-theory.md#set-family) when all its vertices belong to that family.

#### Simplicial order on the discrete cube

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

Order subsets first by increasing [cardinality](set-theory.md#cardinality) and, within each level, by [lexicographic order](extremal-set-theory.md#lexicographic-order), with the smallest differing coordinate belonging to the earlier set. This convention makes simplicial [initial segments](set.md#initial-segment) the extremizers in [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube).

##### Complementary-size simplicial vertex boundaries can be asymmetric

↑ **Parent:** [Simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube)

In the seven-dimensional [Boolean hypercube](#boolean-hypercube), $C(63)$ contains every set of size at most three except $\{5,6,7\}$. Its external [vertex boundary](graph-theory.md#external-vertex-boundary) consists of that missing triple and all 35 four-sets. The complementary-size [initial segment](set.md#initial-segment) $C(65)$ contains every set of size at most three and $\{1,2,3,4\}$. Its external [vertex boundary](graph-theory.md#external-vertex-boundary) has the other 34 four-sets and three five-sets. Thus complementary family sizes do not impose a symmetric boundary profile.

##### Simplicial vertex boundaries need not increase below half volume

↑ **Parent:** [Simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube)

In dimension three, the first three vertices are $\varnothing,\{1\},\{2\}$. Their closed [vertex neighbourhood](graph.md#vertex-neighbourhood) has seven vertices. Adding $\{3\}$ does not change that [vertex neighbourhood](graph.md#vertex-neighbourhood), so the external [vertex boundary](graph-theory.md#external-vertex-boundary) decreases from four to three even though both family sizes are at most half the cube.

#### Vertex-isoperimetric inequality in the discrete cube

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

For the [Boolean hypercube](#boolean-hypercube), the [initial segment](set.md#initial-segment) of the [simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube) minimizes the size of the closed [vertex neighbourhood](graph.md#vertex-neighbourhood) among families of a given size. Equivalently, it minimizes the [external vertex boundary](graph-theory.md#external-vertex-boundary). This is a vertex assertion, distinct from the [edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube).

##### Half-cube vertex-boundary extrema

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

For $n\geq1$, a family of $2^{n-1}$ vertices in the [Boolean hypercube](#boolean-hypercube) has these minimum and maximum external [vertex boundary](graph-theory.md#external-vertex-boundary) sizes. The [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube) gives the minimum: in odd dimension take the lower half of the levels, and in even dimension add the middle-level sets containing coordinate one to all lower levels. The family of even [Hamming weight](coding-theory.md#hamming-weight) attains the maximum, since every remaining vertex has an adjacent even-weight vertex.

##### Cross-intersection bound from cube separation

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

If two nonempty [set families](extremal-set-theory.md#set-family) on $m\geq1$ coordinates have every cross-intersection greater than an integer $w\geq0$, their density product obeys the displayed bound. Complementing the second [set family](extremal-set-theory.md#set-family) separates it from the first by [Hamming distance](coding-theory.md#hamming-distance) greater than $w$. [Harper inequality](#vertex-isoperimetric-inequality-in-the-discrete-cube) bounds the first [set family](extremal-set-theory.md#set-family)'s radius-$w$ neighbourhood from below. If $S_m(a-1)<|\mathcal F|\leq S_m(a)$, disjointness yields $|\mathcal F||\mathcal G|\leq S_m(a)S_m(m-a-w)$. The [binary entropy function](#binary-entropy-function) tail estimate bounds these two factors by Gaussian tails; their deficits from the middle rank sum to at least $w$, proving the claim.

##### Nonunique down-set extremizers for Harper theorem

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

Equality in [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube) need not make a [down-set](extremal-set-theory.md#down-set) a cube-automorphic image of a simplicial [initial segment](set.md#initial-segment). In $Q_4$, take all sets of size at most one and the four two-element sets forming a four-cycle. This family has size nine and [closed graph neighbourhood](graph-theory.md#closed-graph-neighbourhood) size fifteen, just like the size-nine [simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube) [initial segment](set.md#initial-segment). The induced [degree of a vertex](graph-theory.md#degree-graph-theory) distributions differ, so they cannot be related by a [graph automorphism](graph.md#graph-automorphism).

##### Simplicial section compression

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

Split a [set family](extremal-set-theory.md#set-family) in the [hypercube graph](graph.md#hypercube-graph) according to whether coordinate $i$ is present, and delete that coordinate from the present section. Replace both sections by [initial segments](set.md#initial-segment) of the [simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube) with the same respective sizes. Induction and nesting of initial-segment [closed graph neighbourhoods](graph-theory.md#closed-graph-neighbourhood) show that this operation cannot enlarge the original [closed graph neighbourhood](graph-theory.md#closed-graph-neighbourhood). Repeated nontrivial compressions terminate because the sum of simplicial positions strictly decreases.

###### Terminal families for simplicial section compression

↑ **Parent:** [Simplicial section compression](#simplicial-section-compression)

A family fixed by every [simplicial section compression](#simplicial-section-compression) is either an [initial segment](set.md#initial-segment) of the [simplicial order on the discrete cube](#simplicial-order-on-the-discrete-cube) or that segment with its last vertex exchanged for the next vertex, where the exchanged vertices are complementary. Indeed, an earlier absent vertex and a later present vertex must differ in every coordinate, and cannot have another vertex between them. Complementary consecutive vertices occur only across the two central ranks in odd dimension, or at the transition from middle-rank sets containing coordinate one to those avoiding it in even dimension. Direct [closed graph neighbourhood](graph-theory.md#closed-graph-neighbourhood) comparison resolves these exceptions in the proof of [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube).

##### Harper theorem implies the Kruskal-Katona theorem

↑ **Parent:** [Vertex-isoperimetric inequality in the discrete cube](#vertex-isoperimetric-inequality-in-the-discrete-cube)

Adjoin all lower levels to a [uniform set family](extremal-set-theory.md#uniform-set-family) before applying [Harper theorem](#vertex-isoperimetric-inequality-in-the-discrete-cube). Its remaining neighbourhood contribution is the [upper shadow](extremal-set-theory.md#upper-shadow), so lexicographic [initial segments](set.md#initial-segment) minimize upper shadows. Complementation and reversal of coordinates turn this into [colexicographic order](extremal-set-theory.md#colexicographic-order) minimizing the [lower shadow](extremal-set-theory.md#lower-shadow), giving the [Kruskal-Katona theorem](extremal-set-theory.md#kruskal-katona-theorem).

#### Binary order on the discrete cube

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

Identify a vertex $(x_1,\ldots,x_n)$ with the integer $\sum_{i=1}^n2^{i-1}x_i$. Binary order is increasing order of these integers. Its initial segment of size $a$ has $F(a)=\sum_{j=0}^{a-1}s_2(j)$ induced edges, where $s_2(j)$ is the [Hamming weight](coding-theory.md#hamming-weight) of the binary expansion of $j$.

##### Section compression in binary order

↑ **Parent:** [Binary order on the discrete cube](#binary-order-on-the-discrete-cube)

Fix a coordinate of the [Boolean hypercube](#boolean-hypercube), delete it in each of the two sections, and replace each section by a [binary initial segment](#binary-initial-segment) of the same size. This preserves the total size. [Mathematical induction](foundations-of-mathematics.md#mathematical-induction) on dimension proves that it does not decrease contained edge counts; the crossing contribution is the size of the section intersection, maximized by nested initial segments.

###### Families compressed in every binary section

↑ **Parent:** [Section compression in binary order](#section-compression-in-binary-order)

If both sections for every coordinate are [binary initial segments](#binary-initial-segment), then the family itself is a binary initial segment, apart from the possible family $(\mathcal P([n-1])\setminus\{[n-1]\})\cup\{\{n\}\}$. Any missing vertex earlier than a present vertex must disagree with it in every coordinate; the two are therefore complementary and consecutive in [binary order on the discrete cube](#binary-order-on-the-discrete-cube), forcing this sole exceptional shape.

##### Binary initial segment

↑ **Parent:** [Binary order on the discrete cube](#binary-order-on-the-discrete-cube)

An [initial segment](set.md#initial-segment) of the [binary order on the discrete cube](#binary-order-on-the-discrete-cube) contains the vertices whose integer encodings are $0,\ldots,m-1$. It is a [down-set](extremal-set-theory.md#down-set), so its internal edges and two-dimensional [cube faces](#face-of-the-boolean-hypercube) can be counted at their unique upper vertices by $\sum_{j<m}\operatorname{wt}(j)$ and $\sum_{j<m}\binom{\operatorname{wt}(j)}2$.

##### Binary digit-sum inequality

↑ **Parent:** [Binary order on the discrete cube](#binary-order-on-the-discrete-cube)

For $F(a)=\sum_{j=0}^{a-1}s_2(j)$ and nonnegative integers $a,b$, the displayed inequality follows by induction from $F(2r)=2F(r)+r$ and $F(2r+1)=F(r)+F(r+1)+r$. Splitting a vertex set of a [hypercube graph](graph.md#hypercube-graph) into its two coordinate sections then proves the [edge-isoperimetric theorem for binary initial segments](#edge-isoperimetric-theorem-for-binary-initial-segments).

#### Edge boundary in a graph

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)

The edge boundary of a vertex set $A$ consists of graph edges with exactly one endpoint in $A$. In a $d$-regular graph,

$$
|\partial_eA|=d|A|-2e(A),
$$

where $e(A)$ counts edges with both endpoints in $A$.

##### Isoperimetric number of a graph

↑ **Parent:** [Edge boundary in a graph](#edge-boundary-in-a-graph)

For a finite [graph](graph.md) with at least two [vertices](graph.md#vertex-graph-theory), the displayed minimum measures the fewest outgoing [edges](graph-theory.md#edge-of-a-graph) per vertex in a nonempty set occupying at most half the [graph](graph.md). It uses the [edge boundary](#edge-boundary-in-a-graph), rather than the [external vertex boundary](graph-theory.md#external-vertex-boundary). For the [hypercube graph](graph.md#hypercube-graph) $Q_n$, $n\ge1$, it equals one: edge-isoperimetry gives the lower bound and a coordinate half-cube attains it.

##### Edge-isoperimetric inequality in the discrete cube

↑ **Parent:** [Edge boundary in a graph](#edge-boundary-in-a-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edge-isoperimetric_inequality_in_the_discrete_cube)

For $A\subseteq\{0,1\}^n$,

$$
|\partial_eA|\geq|A|\log_2\frac{2^n}{|A|}.
$$

Equivalently, $A$ spans at most $\frac12|A|\log_2|A|$ cube edges. Induction on the dimension and concavity of [binary entropy](#binary-entropy-function) prove the inequality.

###### Entropy proof of cube edge-isoperimetry

↑ **Parent:** [Edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube)

For a vertex set of size $m$ in a [hypercube graph](graph.md#hypercube-graph), split one coordinate into sections of sizes $a,b$. Induction bounds the internal edges within the sections by $(a\log_2a+b\log_2b)/2$; at most $\min(a,b)$ edges cross between them. Put $t=\min(a,b)/(a+b)$. The chord bound for the [binary entropy function](#binary-entropy-function) gives $H_2(t)\ge2t$, hence $a\log_2a+b\log_2b+2\min(a,b)\le m\log_2m$. Thus at most $m\log_2m/2$ internal edges are present, and the [edge boundary](#edge-boundary-in-a-graph) is at least $m(n-\log_2m)$. Coordinate subcubes attain equality when $m$ is a power of two.

###### Equality cases of entropy cube edge-isoperimetry

↑ **Parent:** [Entropy proof of cube edge-isoperimetry](#entropy-proof-of-cube-edge-isoperimetry)

For a nonempty subset of a [hypercube graph](graph.md#hypercube-graph), split it into sections of sizes $a,b$. The proof of the entropy edge bound uses $H_2(t)\ge2t$, $t=\min(a,b)/(a+b)$. Strict concavity makes equality possible only at $t=0$ or $t=1/2$. In the first case one section is empty; in the second the sections coincide, since all possible crossing [edges](graph-theory.md#edge-of-a-graph) must be present. Induction forces a [coordinate subcube](#face-of-the-boolean-hypercube). Conversely every [coordinate subcube](#face-of-the-boolean-hypercube) has the displayed edge count. At size $2^{n-1}$ these are exactly the two halves determined by fixing one coordinate.

###### Edge-isoperimetric theorem for binary initial segments

↑ **Parent:** [Edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube)

Among subsets of the $n$-dimensional [hypercube graph](graph.md#hypercube-graph) with $a$ vertices, initial segments of the [binary order on the discrete cube](#binary-order-on-the-discrete-cube) minimize the [edge boundary](#edge-boundary-in-a-graph). Its exact minimum is $na-2\sum_{j=0}^{a-1}s_2(j)$. This strengthens the entropy lower bound on the same boundary.

###### Binary initial segments maximize contained square faces

↑ **Parent:** [Edge-isoperimetric theorem for binary initial segments](#edge-isoperimetric-theorem-for-binary-initial-segments)

Among families of a given size in the [Boolean hypercube](#boolean-hypercube), a [binary initial segment](#binary-initial-segment) maximizes the number of contained two-dimensional [cube faces](#face-of-the-boolean-hypercube). Under [section compression in binary order](#section-compression-in-binary-order), faces crossing the selected coordinate correspond to internal edges in the intersection of its two sections. The edge extremal theorem and [mathematical induction](foundations-of-mathematics.md#mathematical-induction) control that contribution and the faces within the sections.

###### Binary entropy function

↑ **Parent:** [Edge-isoperimetric inequality in the discrete cube](#edge-isoperimetric-inequality-in-the-discrete-cube)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_entropy_function)

The binary entropy function is

$$
H_2(x)=-x\log_2x-(1-x)\log_2(1-x).
$$

It is concave on $[0,1]$ and satisfies $H_2(x)\geq2x$ for $0\leq x\leq1/2$ by comparison with the chord from $(0,0)$ to $(1/2,1)$.

#### Boolean function

↑ **Parent:** [Boolean hypercube](#boolean-hypercube)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boolean_function)

A Boolean function is a function on a [Boolean hypercube](#boolean-hypercube), often with codomain $\{-1,1\}$ or $\{0,1\}$.

##### Quite fair Boolean function

↑ **Parent:** [Boolean function](#boolean-function)

Under uniform independent input bits, a zero-one [Boolean function](#boolean-function) is quite fair when its mean lies between one quarter and three quarters. This convention excludes functions whose output is nearly constant; it does not require exact balance or equal coordinate influences.

##### Algebraic normal form

↑ **Parent:** [Boolean function](#boolean-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_normal_form)

The algebraic normal form is the unique multilinear polynomial representation of a [Boolean function](#boolean-function) over the field with two elements, using [exclusive or](computer-science.md#exclusive-or) for addition and ordinary bit multiplication for products. The empty product is one. Existence and uniqueness follow by induction from $f(z',z_d)=f(z',0)\oplus z_d(f(z',0)\oplus f(z',1))$: the first polynomial supplies all coefficients not containing $z_d$, and the difference supplies exactly those that do. For split inputs $(x,y)$, each monomial factors into one locally computed product of Alice's bits and one of Bob's bits, yielding a [separated Boolean decomposition](#separated-boolean-decomposition).

##### Separated Boolean decomposition

↑ **Parent:** [Boolean function](#boolean-function)

Every [Boolean function](#boolean-function) of distributed inputs is an [exclusive or](computer-science.md#exclusive-or) of products of locally computable bits. The displayed identity follows because exactly one indicator is one. It uses at most $2^m$ terms, each a function of $x$ times a function of $y$; exchanging the two input roles gives at most $2^n$ terms. This elementary truth-table factorization is useful for distributed computation with [PR boxes](quantum-theory.md#popescu-rohrlich-box) and does not depend on a probabilistic approximation.

##### Random restriction of a Boolean function

↑ **Parent:** [Boolean function](#boolean-function)

A $p$-random restriction independently leaves each coordinate live with probability $p$, otherwise fixing it to zero or one with probability $(1-p)/2$ each. Composing independent restrictions with live probabilities $p_1,\ldots,p_d$ produces the same distribution with live probability $\prod_jp_j$. Fixed values stay unbiased.

##### Tribes function

↑ **Parent:** [Boolean function](#boolean-function)

A tribes function is an OR of AND blocks: partition $mw$ coordinates into $m$ blocks of size $w$, and let $f=1$ when at least one block consists entirely of ones. For [independent random variables](random-variable.md#independent-random-variables) with each bit uniform, $\mathbb P(f=0)=(1-2^{-w})^m$. The [influence of a variable](#influence-of-a-variable) is $2^{-(w-1)}(1-2^{-w})^{m-1}$, because every other bit in its block must be one and every other block must fail. Taking $m$ approximately $(\log2)2^w$ keeps both output probabilities bounded away from zero and gives influences of order $\log(mw)/(mw)$. This shows the order in the [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem) is sharp.

###### Balanced tribes construction with unused coordinates

↑ **Parent:** [Tribes function](#tribes-function)

Choose $w\geq1$ maximal such that $wm\leq n$ for the displayed $m$, and take the OR of $m$ AND blocks of size $w$, ignoring unused coordinates. Its failure probability is $(1-2^{-w})^m$, between one quarter and three quarters. Active coordinates have [influence](#influence-of-a-variable) $2^{1-w}(1-2^{-w})^{m-1}$ and unused ones have zero influence. Maximality gives $2^{1-w}<4(\log2)(w+1)/n$; for $n\geq2$, $w\leq\log_2n$, so every influence is below $8\log n/n$. The construction is therefore a [quite fair Boolean function](#quite-fair-boolean-function) with small influences for every $n\geq2$. The logarithmic bound cannot hold at $n=1$, where every quite fair function has influence one.

###### Tribes threshold window

↑ **Parent:** [Tribes function](#tribes-function)

For $m$ tribes of size $w$ with $m\sim(\log2)2^w$ and $n=mw$, the success probability under the [p-biased product measure](#p-biased-product-measure) is $1-(1-p^w)^m$. Its $x$-quantile is $p_x=[1-(1-x)^{1/m}]^{1/w}$. For fixed $0<x<1$,

$$
p_x=\frac12+\frac1{2w}\log\frac{-\log(1-x)}{\log2}+O_x(w^{-2}).
$$

Thus the fixed-error window has order $1/\log n$. For small fixed error the leading coefficient grows with $\log(1/\varepsilon)$, so the general [Friedgut-Kalai sharp threshold theorem](#friedgut-kalai-sharp-threshold-theorem) also has the correct error dependence up to absolute constants.

##### Block sensitivity

↑ **Parent:** [Boolean function](#boolean-function)

For an input $x$, count the largest family of pairwise disjoint nonempty sets of coordinates such that flipping each set individually changes the [Boolean function](#boolean-function) value. Maximizing over inputs gives block sensitivity. Sensitive sets need not be contiguous and need not consist of single bits. The standard bounded-error [quantum query complexity](computer-science.md#quantum-query-complexity) lower bound is $\Omega(\sqrt{\operatorname{bs}(f)})$. A certificate for $f(x)$ meets every sensitive set, so its size bounds their disjoint count.

##### Monotone Boolean function

↑ **Parent:** [Boolean function](#boolean-function)

A Boolean function $f:\{0,1\}^n\to\{0,1\}$ is a [monotone function](calculus.md#monotonic-function) when $x_i\leq y_i$ for every $i$ implies $f(x)\leq f(y)$.

##### Fourier-Walsh transform

↑ **Parent:** [Boolean function](#boolean-function)

For $f:\{-1,1\}^n\to\mathbb R$, the characters $\chi_S(x)=\prod_{i\in S}x_i$ form an [orthonormal basis](linear-algebra.md#orthonormal-basis), and the Fourier-Walsh expansion is

$$
f=\sum_{S\subseteq[n]}\widehat f(S)\chi_S,
\qquad
\widehat f(S)=\mathbb E[f\chi_S].
$$

On the finite Boolean hypercube, these coefficients are the [Hadamard transform](quantum-theory.md#hadamard-transform) of the vector of function values, with expectation normalization.

###### Fourier weight

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

Fourier weight is the squared [Fourier-Walsh transform](#fourier-walsh-transform) coefficient mass on specified levels or a specified family of subsets. [Parseval's identity](fourier-analysis.md#parseval-identity) identifies the total weight with $\mathbb E|f|^2$, and the nonconstant weight with [variance](variance.md). A decision tree of depth at most $s$ has no weight above level $s$.

###### Expected Fourier weight after a random restriction

↑ **Parent:** [Fourier weight](#fourier-weight)

For a [random restriction](#random-restriction-of-a-boolean-function), first fix the live set $J$ and average over the unbiased assignment $a$ outside it. The coefficient at $U\subset J$ is $\sum_{B\subset J^c}\widehat f(U\cup B)\chi_B(a)$. Orthogonality eliminates cross terms in its squared expectation. Averaging over $J$ gives the displayed identity. The original [Fourier weight](#fourier-weight) is weighted by a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) survival probability, not simply preserved.

###### Coordinate-flip generator on a hypercube

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

For independent coordinate flips at rate $1/2$, a [Walsh character](#walsh-character) $w_A$ is an eigenfunction with [eigenvalue](linear-operator-theory.md#eigenvalue) $-|A|$. The generator is self-adjoint and negative semidefinite. Its [Dirichlet form of a Markov chain](markov-process.md#dirichlet-form-of-a-markov-chain) is $-\mathbb E[fLf]=\frac14\sum_i\mathbb E(f(\omega^{(i)})-f(\omega))^2$.

###### Even-function spectral gap on a hypercube

↑ **Parent:** [Coordinate-flip generator on a hypercube](#coordinate-flip-generator-on-a-hypercube)

Global sign-even functions have zero coefficients on odd-size [Walsh characters](#walsh-character). Every nonconstant remaining character has generator [eigenvalue](linear-operator-theory.md#eigenvalue) at most $-2$, yielding the displayed improvement from gap one to gap two. Combining this with the convexity of a [norm](functional-analysis.md#norm) proves the [sharp Rademacher second-moment inequality](fourier-analysis.md#sharp-rademacher-second-moment-inequality).

###### Walsh character

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

For $S\subseteq[n]$, the Walsh character on the [Boolean hypercube](#boolean-hypercube) is $\chi_S(x)=\prod_{i\in S}x_i$, equivalently $(-1)^{\sum_{i\in S}x_i}$ in the zero-one convention.

###### p-biased product measure

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

Under the $p$-biased product measure $\mu_p$ on $\{-1,1\}^n$, the coordinates are [independent random variables](random-variable.md#independent-random-variables) with $\mathbb P(x_i=-1)=p$ and $\mathbb P(x_i=1)=1-p$. Writing $\mu=1-2p$, $\sigma=2\sqrt{p(1-p)}$, and $\phi_i=(x_i-\mu)/\sigma$, the products $\phi_S=\prod_{i\in S}\phi_i$ form the $p$-biased [Fourier basis](#fourier-walsh-transform).

###### p-biased Fourier coefficient

↑ **Parent:** [P-biased product measure](#p-biased-product-measure)

The $p$-biased Fourier coefficient of $f$ at $S$ is $\widehat f_p(S)=\mathbb E_{\mu_p}[f\phi_S]$.

###### Discrete derivative of a Boolean function

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

On the unbiased cube, the discrete derivative is

$$
D_i f(x)=\frac{f(x^{i\to1})-f(x^{i\to-1})}{2}
=\sum_{S\ni i}\widehat f(S)\chi_{S\setminus\{i\}}(x).
$$

For the [p-biased product measure](#p-biased-product-measure), the normalization factor is $\sigma/2$.

###### Influence of a variable

↑ **Parent:** [Discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function)

For the $\{-1,1\}$-valued convention on the unbiased [Boolean hypercube](#boolean-hypercube), the influence of coordinate $i$ is $\operatorname{Inf}_i(f)=\lVert D_i f\rVert_2^2$, where $D_i f$ is the [discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function). It equals the [probability](probability-theory.md#probability) that flipping coordinate $i$ changes $f$. For the $\{0,1\}$-valued convention, the same flip probability is instead $4\lVert D_i f\rVert_2^2$, since a nonzero discrete derivative has magnitude $1/2$.

###### Hypercontractive weighted influence bound

↑ **Parent:** [Influence of a variable](#influence-of-a-variable)

For a zero-one [Boolean function](#boolean-function), the flip-probability [influence](#influence-of-a-variable) is $\beta_i=4\sum_{S\ni i}\widehat f(S)^2$. Apply [Beckner's inequality](#beckner-s-inequality) with noise parameter $\sqrt\delta$ to the [discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function), whose nonzero magnitude is $1/2$. Its $L^{1+\delta}$ norm squared is $\beta_i^{2/(1+\delta)}/4$. Summing over coordinates gives the displayed weighted [Fourier weight](#fourier-weight) bound, a useful intermediate step in influence lower bounds.

###### Total influence

↑ **Parent:** [Influence of a variable](#influence-of-a-variable)

The total influence is

$$
\mathbf I(f)=\sum_i\operatorname{Inf}_i(f)
=\sum_{S\subseteq[n]}|S|\widehat f(S)^2.
$$

This [Fourier-Walsh transform](#fourier-walsh-transform) identity uses $\{-1,1\}$-valued $f$ and the flip-probability convention for [influence of a variable](#influence-of-a-variable). For $\{0,1\}$-valued $f$, the right-hand side is multiplied by four. Indeed [Parseval's identity](fourier-analysis.md#parseval-identity) applied to the [discrete derivative of a Boolean function](#discrete-derivative-of-a-boolean-function) gives $\|D_i f\|_2^2=\sum_{S\ni i}\widehat f(S)^2$; sum over coordinates and apply the chosen normalization.

<h6 id="margulis-russo-formula">Margulis–Russo formula</h6>

↑ **Parent:** [Total influence](#total-influence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Margulis–Russo_formula)

For the indicator $f$ of a monotone family under a [p-biased product measure](#p-biased-product-measure), the Margulis–Russo formula identifies the derivative of $\mathbb E_{\mu_p}f$ with the suitably normalized [total influence](#total-influence) of $f$.

###### Pivotal for an increasing event

↑ **Parent:** [Margulis–Russo formula](#margulis-russo-formula)

A coordinate is pivotal for an increasing event in a configuration when changing only that coordinate changes whether the event occurs. Its pivotal probability is the coordinate's influence.

###### Noise operator on the Boolean hypercube

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

The noise operator averages $f(y)$ over a random $y$ correlated with $x$ by $\rho$. It acts diagonally on the [Fourier-Walsh transform](#fourier-walsh-transform):

$$
T_\rho f=\sum_S\rho^{|S|}\widehat f(S)\chi_S.
$$

<h6 id="beckner-s-inequality">Beckner's inequality</h6>

↑ **Parent:** [Noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube)

For $1<p\leq q<\infty$ and $0\leq\rho\leq\sqrt{(p-1)/(q-1)}$, the [noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube) satisfies $\|T_\rho f\|_q\leq\|f\|_p$ for the uniform [probability measure](probability-theory.md#probability-measure). In particular,

$$
\sum_S\rho^{2|S|}|\widehat f(S)|^2\leq\|f\|_{1+\rho^2}^2
\qquad(0\leq\rho\leq1).
$$

Here $\widehat f(S)$ are [Fourier-Walsh transform](#fourier-walsh-transform) coefficients. The endpoint $\rho=0$ follows by averaging. This [hypercontractive inequality on the Boolean hypercube](#hypercontractive-inequality-on-the-boolean-hypercube) controls [Fourier-Walsh transform](#fourier-walsh-transform) coefficients of [discrete derivatives of a Boolean function](#discrete-derivative-of-a-boolean-function) and is a principal ingredient in the [Kahn-Kalai-Linial theorem](#kahn-kalai-linial-theorem).

###### Low-degree Fourier mass of a sparse Boolean set

↑ **Parent:** [Beckner's inequality](#beckner-s-inequality)

For a subset of the unbiased [Boolean hypercube](#boolean-hypercube) of density $\alpha$, use normalized [Fourier-Walsh transform](#fourier-walsh-transform) coefficients. Applying [Beckner's inequality](#beckner-s-inequality) with $\rho=1/\sqrt3$ gives $\|T_\rho1_A\|_2^2\leq\|1_A\|_{4/3}^2=\alpha^{3/2}$. On levels at most two the weights $\rho^{2|S|}$ are at least $1/9$, giving the displayed bound. [Parseval's identity](fourier-analysis.md#parseval-identity) gives total Fourier mass $\alpha$, so when $9\sqrt\alpha<1/2$ the higher levels contain strictly more than the lower levels.

###### Noise stability

↑ **Parent:** [Noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noise_stability)

The noise stability is

$$
\operatorname{Stab}_\rho(f)=\langle f,T_\rho f\rangle
=\sum_S\rho^{|S|}\widehat f(S)^2.
$$

###### Linear Fourier weight

↑ **Parent:** [Fourier-Walsh transform](#fourier-walsh-transform)

The linear Fourier weight is $W_1(f)=\sum_{|S|=1}\widehat f(S)^2$.

##### Junta

↑ **Parent:** [Boolean function](#boolean-function)

A $J$-junta is a function whose value depends only on coordinates indexed by $J$. A $k$-junta depends on at most $k$ coordinates.

###### Friedgut junta inequality

↑ **Parent:** [Junta](#junta)

If $f:\{-1,1\}^n\to\{-1,1\}$ satisfies $\lVert f^{\leq k}\rVert_2^2\geq1-\varepsilon$, then it has a real-valued $J$-junta approximation $g$ with $\lVert f-g\rVert_2^2\leq2\varepsilon$ and

$$
|J|\leq\frac{3^{2k}\mathbf I(f)^3}{\varepsilon^2}.
$$

###### Friedgut junta theorem

↑ **Parent:** [Friedgut junta inequality](#friedgut-junta-inequality)

For every $\varepsilon>0$, a Boolean function $f$ has an $\exp(O(\mathbf I(f)/\varepsilon))$-junta approximation with squared $L^2$ error at most $2\varepsilon$.

###### Nisan-Szegedy junta theorem

↑ **Parent:** [Junta](#junta)

Every Boolean function of degree at most $k$ is a $k2^{k-1}$-junta.

##### Quasirandom Boolean function

↑ **Parent:** [Boolean function](#boolean-function)

A Boolean function $f:\{0,1\}^n\to\{0,1\}$ is $(\varepsilon,p,r)$-quasirandom when conditioning any set of at most $r$ coordinates to any values changes its $\mu_p$-expectation by at most $\varepsilon$.

###### Regularity lemma for Boolean functions

↑ **Parent:** [Quasirandom Boolean function](#quasirandom-boolean-function)

For every $\varepsilon,p,r,\delta$, there is $T$ such that every Boolean function has a set $J$ with $|J|\leq T$ for which a $\mu_p$-random restriction on $J$ leaves an $(\varepsilon,p,r)$-quasirandom function with probability at least $1-\delta$.

### Bonami lemma

↑ **Parent:** [Analysis of Boolean functions](#analysis-of-boolean-functions)

The Bonami lemma states that a function of [Fourier degree](#fourier-walsh-transform) at most $k$ satisfies $\lVert f\rVert_4\leq3^{k/2}\lVert f\rVert_2$.

#### Hypercontractive inequality on the Boolean hypercube

↑ **Parent:** [Bonami lemma](#bonami-lemma)

One form of the hypercontractive inequality is $\lVert T_{1/\sqrt3}f\rVert_4\leq\lVert f\rVert_2$, where $T_\rho$ is the [noise operator on the Boolean hypercube](#noise-operator-on-the-boolean-hypercube).

#### Anticoncentration of a low-degree function

↑ **Parent:** [Bonami lemma](#bonami-lemma)

If a nonzero function on the [Boolean hypercube](#boolean-hypercube) has degree at most $k$, then its support has measure at least $2^{-k}$. This sharp bound follows by induction on the dimension.

<h3 id="arrow-s-impossibility-theorem">Arrow's impossibility theorem</h3>

↑ **Parent:** [Analysis of Boolean functions](#analysis-of-boolean-functions)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arrow's_impossibility_theorem)

Arrow's theorem says that a rank-order voting system with at least three alternatives cannot simultaneously satisfy unrestricted preferences, unanimity, independence of irrelevant alternatives, and absence of a dictator.

#### Condorcet paradox

↑ **Parent:** [Arrow's impossibility theorem](#arrow-s-impossibility-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Condorcet_paradox)

The Condorcet paradox is a cycle in collective pairwise preferences even though each individual voter's preference is transitive.

### Invariance principle for a low-degree multilinear polynomial

↑ **Parent:** [Analysis of Boolean functions](#analysis-of-boolean-functions)

Let $X_i$ and $Y_i$ be independent, centered, variance-one random variables with vanishing third moments and fourth moments at most $9$. If $f$ is multilinear of degree at most $k$ and $\lVert\psi^{(4)}\rVert_\infty\leq M$, then

$$
|\mathbb E\psi(f(X))-\mathbb E\psi(f(Y))|
\leq\frac{M}{12}9^k\sum_i\operatorname{Inf}_i(f)^2.
$$

#### Lindeberg replacement method

↑ **Parent:** [Invariance principle for a low-degree multilinear polynomial](#invariance-principle-for-a-low-degree-multilinear-polynomial)

The Lindeberg replacement method, inspired by the [Lindeberg condition](convergence-of-random-variables.md#lindeberg-condition), compares functions of two independent random vectors by replacing their coordinates one at a time. Matching moments cancel the corresponding terms in a [Taylor expansion](calculus.md#taylor-theorem).

## Ramsey theory

↑ **Parent:** [Combinatorics](combinatorics.md)

[This section is present in another page, follow this link to view it.](ramsey-theory.md)

## Symmetric function

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_function)

A symmetric function is a formal power series of bounded total degree that is invariant under every finite permutation of its variables. Symmetric functions form a graded ring with several useful bases.

### Cauchy identity for symmetric functions

↑ **Parent:** [Symmetric function](#symmetric-function)

Expand each factor as a [geometric series](real-analysis.md#geometric-series) indexed by a nonnegative [matrix](vector-space.md#matrix). The [RSK correspondence](representation-theory-of-the-symmetric-group.md#robinson-schensted-knuth-correspondence) preserves its row and column contents, changing the sum to pairs of [Semistandard Young tableaux](representation-theory-of-the-symmetric-group.md#semistandard-young-tableau) of the same shape and proving the displayed formal identity. Its kernel is also $\sum_\lambda h_\lambda(x)m_\lambda(y)=\sum_\lambda p_\lambda(x)p_\lambda(y)/z_\lambda$. These are dual-basis kernels for the [Hall inner product of symmetric functions](#hall-inner-product-of-symmetric-functions), so the Schur expansion proves orthonormality. Applying the [symmetric-function involution](#symmetric-function-involution) in one alphabet gives the dual identity $\prod_{i,j}(1+x_iy_j)=\sum_\lambda s_\lambda(x)s_{\lambda'}(y)$.

#### Schur specialization by a generating function

↑ **Parent:** [Cauchy identity for symmetric functions](#cauchy-identity-for-symmetric-functions)

Given $F(t)=\sum_{r\ge0}f_rt^r$ with $f_0=1$, put $f_r=0$ for $r<0$. The [Cauchy identity for symmetric functions](#cauchy-identity-for-symmetric-functions) and [Jacobi–Trudi identity](#jacobi-trudi-identity) give $\prod_iF(t_i)=\sum_\lambda s_\lambda^Fs_\lambda(t)$, degree by degree in the completion. For $F(t)=\prod_j(1-x_jt)^{-1}$ the coefficients are $s_\lambda(x)$; for $F(t)=\prod_j(1+x_jt)$ they are $s_{\lambda'}(x)$.

#### Dual Cauchy identity for symmetric functions

↑ **Parent:** [Cauchy identity for symmetric functions](#cauchy-identity-for-symmetric-functions)

Apply the [symmetric-function involution](#symmetric-function-involution) in one alphabet to the ordinary [Cauchy identity](#cauchy-identity-for-symmetric-functions). It changes complete generators to elementary ones and, by the dual [Jacobi–Trudi identity](#jacobi-trudi-identity), sends $s_\lambda$ to $s_{\lambda'}$. This proves the identity as a formal series and relates pairings with transposed Young shapes to squarefree [matrix](vector-space.md#matrix) weights.

### Symmetric-function involution

↑ **Parent:** [Symmetric function](#symmetric-function)

The [Fundamental theorem of symmetric polynomials](polynomial.md#fundamental-theorem-of-symmetric-polynomials) gives freely generated elementary functions, so sending each $e_r$ to $h_r$ defines an [algebra homomorphism](algebra.md#algebra-homomorphism-over-a-field). For $E(t)=\sum e_rt^r$ and $H(t)=\sum h_rt^r$, $E(-t)H(t)=1$. Applying the homomorphism shows $\omega(H(t))=E(t)$, hence $\omega^2=1$. Taking logarithms of $H$ gives the displayed action on power sums. It preserves the [Hall inner product of symmetric functions](#hall-inner-product-of-symmetric-functions) because each power-sum [basis](vector-space.md#basis) vector acquires only a sign.

#### Forgotten symmetric function

↑ **Parent:** [Symmetric-function involution](#symmetric-function-involution)

The coefficient of $m_\mu$ in $f_\lambda$ counts distinct rearrangements of the parts of $\lambda$ whose prefix-sum set contains the prefix sums of $\mu$. Indeed, [Hall inner product of symmetric functions](#hall-inner-product-of-symmetric-functions) duality between $m_\lambda,h_\lambda$ turns this coefficient into $(-1)^{|\lambda|-\ell(\lambda)}$ times the coefficient of $h_\lambda$ in $e_\mu$. Expanding $E(t)=H(-t)^{-1}$ expresses each $e_{\mu_j}$ as a signed sum of compositions of $\mu_j$. Concatenating these compositions gives precisely the counted rearrangements, and every sign is $(-1)^{|\lambda|-\ell(\lambda)}$.

### Monomial symmetric function

↑ **Parent:** [Symmetric function](#symmetric-function)

For an [integer partition](#integer-partition) $\lambda$, $m_\lambda$ sums the distinct [monomials](polynomial.md#monomial) whose positive exponent multiset is $\lambda$. No multiplicity is attached to repeated parts. The functions of fixed total degree form a [basis](vector-space.md#basis) of the [symmetric functions](#symmetric-function) of that degree, since finite variable [permutations](#permutation) identify precisely these [monomial](polynomial.md#monomial) orbits.

### Hall inner product of symmetric functions

↑ **Parent:** [Symmetric function](#symmetric-function)

Here $p_\alpha$ is a product of power-sum [symmetric functions](#symmetric-function) and $z_\alpha=\prod_r r^{m_r}m_r!$ for part multiplicities $m_r$. The [Frobenius characteristic map](#frobenius-characteristic-map) identifies this product with the [ordinary character](representation-theory.md#ordinary-character) [inner product](linear-algebra.md#inner-product). [Schur functions](#schur-polynomial) are orthonormal, and the adjoint of multiplication by $p_k$ is $k\partial/\partial p_k$. These properties turn a power-sum multiplication formula into the [Murnaghan–Nakayama rule](representation-theory-of-the-symmetric-group.md#murnaghan-nakayama-rule).

### Complete homogeneous symmetric polynomial

↑ **Parent:** [Symmetric function](#symmetric-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_homogeneous_symmetric_polynomial)

The complete homogeneous symmetric polynomial $h_n$ is the sum of all monomials of total degree $n$. Its generating function is

$$
H(t)=\sum_{n\geq0}h_nt^n
=\exp\left(\sum_{k\geq1}\frac{p_kt^k}{k}\right).
$$

### Power-sum symmetric polynomial

↑ **Parent:** [Symmetric function](#symmetric-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Power-sum_symmetric_polynomial)

The power-sum symmetric polynomial is $p_n=\sum_i x_i^n$. For an [integer partition](#integer-partition) $\mu$, write $p_\mu=\prod_i p_{\mu_i}$.

### Schur polynomial

↑ **Parent:** [Symmetric function](#symmetric-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_polynomial)

The Schur polynomials form a basis of the ring of symmetric functions indexed by [integer partitions](#integer-partition).

#### Bialternant formula

↑ **Parent:** [Schur polynomial](#schur-polynomial)

Let $a_\gamma=\det[x_j^{\gamma_i}]$ and $\delta=(N-1,\ldots,0)$. Multiply the [Jacobi–Trudi identity](#jacobi-trudi-identity) [matrix](vector-space.md#matrix) by $B_{jk}=(-1)^{N-j}e_{N-j}(X\setminus x_k)$. The generating-function identity $H(t)\prod_{i\ne k}(1-x_it)=(1-x_kt)^{-1}$ makes the product [matrix](vector-space.md#matrix) $[x_k^{\lambda_i+N-i}]$. Setting $\lambda=0$ shows $\det B=a_\delta$, proving the formula as a [polynomial](polynomial.md) identity.

##### Schur evaluation at all ones

↑ **Parent:** [Bialternant formula](#bialternant-formula)

Put $b_i=\lambda_i+N-i$. In the [bialternant formula](#bialternant-formula), substitute $x_j=e^{ty_j}$ with distinct $y_j$ and compare the first nonzero [determinant](linear-algebra.md#determinant) coefficients as $t\to0$. They arise from the distinct degrees $0,\ldots,N-1$ in the exponential expansions. The common factor in the $y_j$ and the factorials cancel, leaving the product of differences of the $b_i$ divided by the differences of $N-i$. This proves the displayed integral specialization without dividing by a vanishing Vandermonde value.

#### Skew Schur function

↑ **Parent:** [Schur polynomial](#schur-polynomial)

Sum the weight [monomials](polynomial.md#monomial) of all [Semistandard Young tableaux](representation-theory-of-the-symmetric-group.md#semistandard-young-tableau) on the [skew Young diagram](representation-theory-of-the-symmetric-group.md#skew-young-diagram) $\lambda/\mu$, with weak rows and strict columns. A [Bender-Knuth involution](representation-theory-of-the-symmetric-group.md#bender-knuth-involution) interchanges the counts of adjacent letters without changing the shape, so the sum is a [symmetric function](#symmetric-function). Taking $\mu$ empty gives the [Schur function](#schur-polynomial).

<h4 id="jacobi-trudi-identity">Jacobi–Trudi identity</h4>

↑ **Parent:** [Schur polynomial](#schur-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi–Trudi_identity)

The Jacobi–Trudi identity expresses a Schur polynomial as

$$
s_\lambda=\det(h_{\lambda_i-i+j}).
$$

In particular, $s_{(a,b)}=h_ah_b-h_{a+1}h_{b-1}$.

##### Determinantal form of a symmetric-group character

↑ **Parent:** [Jacobi–Trudi identity](#jacobi-trudi-identity)

Here $[a]$ is the trivial [character](representation-theory.md#character-of-a-representation) of $S_a$, $[0]$ is the induction-product unit, $[a]=0$ for $a<0$, and multiplication is induction of external [tensor products](linear-algebra.md#tensor-product). The [Frobenius characteristic map](#frobenius-characteristic-map) turns the expression into the [Jacobi–Trudi identity](#jacobi-trudi-identity). A sign-reversing involution on intersecting lattice-path systems leaves precisely the nonintersecting systems corresponding to [Semistandard Young tableaux](representation-theory-of-the-symmetric-group.md#semistandard-young-tableau), proving the [determinant](linear-algebra.md#determinant) identity.

### Frobenius characteristic map

↑ **Parent:** [Symmetric function](#symmetric-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frobenius_characteristic_map)

The Frobenius characteristic map sends class functions on $S_n$ to homogeneous symmetric functions of degree $n$. It satisfies

$$
\operatorname{ch}(\chi^\lambda)=s_\lambda,
\qquad
\operatorname{ch}(\chi)=\sum_{\mu\vdash n}\frac{\chi(\mu)}{z_\mu}p_\mu.
$$

#### Frobenius alternant character formula

↑ **Parent:** [Frobenius characteristic map](#frobenius-characteristic-map)

For a [partition of an integer](representation-theory-of-the-symmetric-group.md#partition-of-an-integer) $\lambda\vdash n$, padded to $m$ rows, let $\delta=(m-1,\ldots,0)$. If a permutation has $\alpha_q$ cycles of length $q$, put $p_\alpha=\prod_q(\sum_i x_i^q)^{\alpha_q}$. The [character](representation-theory.md#character-of-a-representation) of the [Specht module](representation-theory-of-the-symmetric-group.md#specht-module) $S^\lambda$ is the displayed coefficient. Equivalently $p_\alpha A_\delta=\sum_\lambda\chi^\lambda(\alpha)A_{\lambda+\delta}$, the alternant form of the [Frobenius characteristic map](#frobenius-characteristic-map). It gives finite coefficient computations without constructing representation matrices.

## ↑ Ancestors (3)

1. [Area of mathematics](mathematics.md#area-of-mathematics)
2. [Mathematics](mathematics.md)
3. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Analysis of Boolean functions](#analysis-of-boolean-functions)
