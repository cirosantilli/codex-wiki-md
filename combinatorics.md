# Combinatorics

↑ **Parent:** [Area of mathematics](mathematics.md#area-of-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Combinatorics)

[Combinatorics](combinatorics.md) studies discrete structures through counting, construction, and extremal questions. Its objects include [subsets](set.md#subset), [permutations](#permutation), [graphs](graph.md), and [set partitions](#set-partition). The question is often easy to ask: how many teams can we choose, how many arrangements avoid a collision, or how few connections are enough? The challenge is to organize the possibilities so that every permitted object is counted exactly as intended.

For example, choosing two people from five gives ten teams. Choosing a captain and deputy from those same five gives twenty assignments. The difference is whether order is part of the object: a team is a [subset](set.md#subset), while the two named roles distinguish an [ordered pair](set.md#ordered-pair). The [binomial coefficient](#binomial-coefficient) and the [rule of product](#rule-of-product) encode these two counting problems. Choosing the right objects comes before manipulating a formula.

The beauty is that a change of viewpoint can turn enumeration into an explanation. [Double counting](#double-counting-proof-technique) connects two descriptions of one collection; [Pascal's identity](#pascal-s-rule) splits a selection into cases; the [inclusion-exclusion principle](#inclusion-exclusion-principle) repairs overlapping counts. These methods also supply exact finite models for [probability](probability-theory.md#probability) and help measure the possibilities an [algorithm](computer-science.md#algorithm) must handle. Richard Stanley's textbook introduces the subject through counting questions and then develops these general tools. [Enumerative Combinatorics, Volume 1 (second-edition draft) by Richard Stanley](mathematics-bibliography.md#enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley)

**Table of contents**

- [Pigeonhole principle](#pigeonhole-principle)
  - [Generalized pigeonhole principle](#generalized-pigeonhole-principle)
  - [Infinite pigeonhole principle](#infinite-pigeonhole-principle)
- [Enumerative combinatorics](#enumerative-combinatorics)
  - [q-analogue](#q-analogue)
  - [Board tiling](#board-tiling)
- [Combinatorial structure](#combinatorial-structure)
  - [Labelled combinatorial structure](#labelled-combinatorial-structure)
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
  - [Cycle lemma with increments at most one](#cycle-lemma-with-increments-at-most-one)
- [Cyclic digit run](#cyclic-digit-run)
- [Finite geometry](#finite-geometry)
- [Increasing subsequence](#increasing-subsequence)
  - [Longest increasing subsequence](#longest-increasing-subsequence)
    - [Minimum-tail table for increasing subsequences](#minimum-tail-table-for-increasing-subsequences)
  - [Strictly increasing subsequence](#strictly-increasing-subsequence)
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
    - [Sumset representation function](additive-combinatorics.md#sumset-representation-function)
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
- [Indegree](#indegree)
- [Directed acyclic graph](#directed-acyclic-graph)
  - [Topological sorting](#topological-sorting)
    - [Topological order](#topological-order)
    - [Kahn's algorithm](#kahn-s-algorithm)
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
  - [Labelled tree](#labelled-tree)
  - [Unlabelled tree](#unlabelled-tree)
  - [Regular tree](#regular-tree)
    - [Edge boundary of a finite forest in a regular tree](#edge-boundary-of-a-finite-forest-in-a-regular-tree)
  - [Oriented tree](#oriented-tree)
    - [Three-times-order tournament bound for oriented trees](#three-times-order-tournament-bound-for-oriented-trees)
    - [Arborescence (graph theory)](#arborescence-graph-theory)
  - [Depth-first traversal of a tree](#depth-first-traversal-of-a-tree)
  - [Rooted tree](#rooted-tree)
    - [Root of a tree](#root-of-a-tree)
    - [Parent in a rooted tree](#parent-in-a-rooted-tree)
    - [Child in a rooted tree](#child-in-a-rooted-tree)
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
      - [Prüfer degree formula](#prufer-degree-formula)
        - [Labelled tree count with prescribed degrees](#labelled-tree-count-with-prescribed-degrees)
      - [Uniform labelled tree generation](#uniform-labelled-tree-generation)
  - [Kőnig's lemma](#konig-s-lemma)
  - [Breadth-first search](#breadth-first-search)
- [Double counting (proof technique)](#double-counting-proof-technique)
- [Set partition](#set-partition)
  - [Block of a set partition](#block-of-a-set-partition)
  - [Refinement of a set partition](#refinement-of-a-set-partition)
  - [Integer partition](#integer-partition)
    - [Partition in a rectangle](#partition-in-a-rectangle)
    - [Ferrers diagram](#ferrers-diagram)
  - [Stirling numbers of the second kind](#stirling-numbers-of-the-second-kind)
    - [Bell number](#bell-number)
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
    - [Gaussian binomial coefficient recurrence](#gaussian-binomial-coefficient-recurrence)
    - [Lattice-path interpretation of Gaussian binomial coefficients](#lattice-path-interpretation-of-gaussian-binomial-coefficients)
    - [Partition interpretation of Gaussian binomial coefficients](#partition-interpretation-of-gaussian-binomial-coefficients)
      - [Complement symmetry of Gaussian binomial coefficients](#complement-symmetry-of-gaussian-binomial-coefficients)
    - [Gaussian binomial coefficient counts finite-field subspaces](#gaussian-binomial-coefficient-counts-finite-field-subspaces)
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
  - [Composition of an integer](#composition-of-an-integer)
    - [Weak composition of an integer](#weak-composition-of-an-integer)
  - [Bounded weak compositions](#bounded-weak-compositions)
- [Inclusion-exclusion principle](#inclusion-exclusion-principle)
  - [Inclusion-exclusion principle for probabilities](#inclusion-exclusion-principle-for-probabilities)
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
    - [Fixed point count of a uniform random permutation](#fixed-point-count-of-a-uniform-random-permutation)
  - [Cycle length of a tagged element in a uniform permutation](#cycle-length-of-a-tagged-element-in-a-uniform-permutation)
  - [Derangement of a permutation](#derangement-of-a-permutation)
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
        - [Ramsey number for triangles](ramsey-theory.md#ramsey-number-for-triangles)
          - [Five-cycle Ramsey coloring](ramsey-theory.md#five-cycle-ramsey-coloring)
          - [Six-vertex monochromatic triangle argument](ramsey-theory.md#six-vertex-monochromatic-triangle-argument)
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

## Pigeonhole principle

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pigeonhole_principle)

Place $N$ objects into $m\geq1$ boxes, assigning each object to exactly one box. Here $N$ is a nonnegative [integer](number-theory.md#integer) and $m$ is a [positive integer](number-theory.md#positive-integer). The [pigeonhole principle](#pigeonhole-principle) says that if $N>m$, some box contains at least two objects. Equivalently, a [function](function.md) from an $N$-element [finite set](set.md#finite-set) to an $m$-element [finite set](set.md#finite-set) cannot be an [injective function](algebra.md#injective-function) when $N>m$. The boxes may stand for categories rather than physical containers. [Lehman, Leighton and Meyer, Mathematics for Computer Science, section 14.8, rule 14.8.1](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/mit6_042js15_textbook.pdf#page=581)

For thirteen objects and twelve boxes, a box containing at least two is unavoidable. Thinking of thirteen people and their birth months gives the same conclusion: at least two share a birth month. Twelve people could occupy the twelve months one apiece, so thirteen is the smallest number that forces a shared month. The [generalized pigeonhole principle](#generalized-pigeonhole-principle) quantifies how many objects must share a box when there are still more objects.

The useful surprise is that the [pigeonhole principle](#pigeonhole-principle) proves existence without needing to locate the objects involved. Choosing a good assignment rule is often the creative step: equal labels can mean equal remainders, nearby [points](geometry-and-topology.md#point-geometry), or repeated states of an [algorithm](computer-science.md#algorithm). Once the rule is chosen, a short count can force a relationship among a much larger collection of objects. The [pigeonhole principle](#pigeonhole-principle) itself does not name the crowded box. When the objects and their assignments are explicitly available, a simple [algorithm](computer-science.md#algorithm) finds one: scan the objects, keep the first object seen in each box, and stop when a later object enters an occupied box. At most $m+1$ scanned objects are needed when $N>m$.

**A geometric example.** Any five [points](geometry-and-topology.md#point-geometry) in a [square](geometry-and-topology.md#square) of side one contain two whose [Euclidean distance](topological-analysis.md#euclidean-distance) is at most $1/\sqrt2$. Give each [point](geometry-and-topology.md#point-geometry) [Cartesian coordinates](linear-algebra.md#cartesian-coordinate-system) $(x,y)\in[0,1]^2$. Divide both ranges into the [intervals](real-analysis.md#interval-mathematics) $[0,1/2)$ and $[1/2,1]$, making four cells. Thus $x<1/2$ belongs to the left half and $x\geq1/2$ to the right half; $y<1/2$ belongs to the lower half and $y\geq1/2$ to the upper half. This convention assigns every boundary [point](geometry-and-topology.md#point-geometry) to exactly one cell.

The [pigeonhole principle](#pigeonhole-principle) puts two of the five [points](geometry-and-topology.md#point-geometry) in the same cell. Their differences in [Cartesian coordinates](linear-algebra.md#cartesian-coordinate-system) have magnitude at most $1/2$, so the [Pythagorean theorem](geometry-and-topology.md#pythagorean-theorem) gives their [Euclidean distance](topological-analysis.md#euclidean-distance) $d$ the bound

$$
d^2\leq\left(\frac12\right)^2+\left(\frac12\right)^2=\frac12,
\qquad d\leq\frac1{\sqrt2}\approx0.707107.
$$

For the plotted [points](geometry-and-topology.md#point-geometry) $(0.1,0.1)$, $(0.4,0.4)$, $(0.8,0.2)$, $(0.2,0.8)$ and $(0.8,0.8)$, the first two occupy the lower-left cell and have [Euclidean distance](topological-analysis.md#euclidean-distance) $\sqrt{0.3^2+0.3^2}=\sqrt{0.18}\approx0.424264$. These [Cartesian coordinates](linear-algebra.md#cartesian-coordinate-system) exhibit the forced pair; the argument applies to every placement of five [points](geometry-and-topology.md#point-geometry).

<a id="image-the-pigeonhole-principle-places-two-of-five-points-in-one-of-four-cells-of-a-square-bounding-their-euclidean-distance-by-1-sqrt2"></a>
![](geometric-pigeonhole-square.png)

**[Figure 1](#image-the-pigeonhole-principle-places-two-of-five-points-in-one-of-four-cells-of-a-square-bounding-their-euclidean-distance-by-1-sqrt2). The pigeonhole principle places two of five points in one of four cells of a square, bounding their Euclidean distance by $1/\sqrt2$**.

**An arithmetic example.** Assign eight [integers](number-theory.md#integer) to their seven [residue classes](number-theory.md#residue-class) modulo the [integer modulus](number-theory.md#modulus-in-modular-arithmetic) $7$. The [pigeonhole principle](#pigeonhole-principle) gives two with the same [residue class](number-theory.md#residue-class), so $7$ is an [integer divisor](number-theory.md#divisor) of their difference. In $\{2,5,9,12,16,20,24,27\}$, for example, $2$ and $9$ satisfy the [integer congruence](number-theory.md#integer-congruence) $9\equiv2\pmod7$, and $9-2=7$. Likewise, assigning [fractional parts](calculus.md#fractional-part) to short [intervals](real-analysis.md#interval-mathematics) gives the [Dirichlet approximation theorem](number-theory.md#dirichlet-s-approximation-theorem); its existing article explains the approximation bound.

### Generalized pigeonhole principle

↑ **Parent:** [Pigeonhole principle](#pigeonhole-principle)

For $N$ objects assigned to $m\geq1$ boxes, let $n_i$ be the number in box $i$. The [generalized pigeonhole principle](#generalized-pigeonhole-principle) states

$$
n_1+\cdots+n_m=N
\quad\Longrightarrow\quad
\max_{1\leq i\leq m}n_i\geq\left\lceil\frac Nm\right\rceil.
$$

The [ceiling function](calculus.md#ceiling-function) rounds up because box counts are [integers](number-theory.md#integer). An equivalent threshold formulation says: for a [positive integer](number-theory.md#positive-integer) $k$, if $N>m(k-1)$, some box contains at least $k$ objects. For $N=m(k-1)$, putting $k-1$ objects in each box shows why the strict inequality matters. [Lehman, Leighton and Meyer, Mathematics for Computer Science, section 14.8.1, rule 14.8.2](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/mit6_042js15_textbook.pdf#page=583)

**Computed examples.** For $N=13$ and $m=12$, $\lceil13/12\rceil=2$. Counts $(2,1,1,1,1,1,1,1,1,1,1,1)$ attain this bound. For $N=23$ and $m=7$, $\lceil23/7\rceil=4$, and the balanced counts $(4,4,3,3,3,3,3)$ sum to $23$ and have largest count exactly $4$. The threshold version agrees: $23>7(4-1)=21$. In contrast, seven boxes each containing three hold only $21$ objects.

<a id="image-two-balanced-arrangements-attain-the-generalized-pigeonhole-principle-bounds-thirteen-objects-in-twelve-boxes-force-two-and-twenty-three-in-seven-force-four"></a>
![](pigeonhole-distribution-counts.png)

**[Figure 2](#image-two-balanced-arrangements-attain-the-generalized-pigeonhole-principle-bounds-thirteen-objects-in-twelve-boxes-force-two-and-twenty-three-in-seven-force-four). Two balanced arrangements attain the generalized pigeonhole principle bounds: thirteen objects in twelve boxes force two, and twenty-three in seven force four**.

The bound is sharp for every $N$ and $m$. Use [Euclidean division](number-theory.md#euclidean-division) to write $N=qm+r$ with [integers](number-theory.md#integer) $q\geq0$ and $0\leq r<m$. Place $q+1$ objects in each of $r$ boxes and $q$ objects in each remaining box. The largest count is $q+1$ if $r>0$, and $q$ if $r=0$, exactly $\lceil N/m\rceil$. This balanced arrangement makes the guarantee best possible even though other arrangements can be much more crowded.

**Proof outline.** If every count were at most $k-1$, the total would be at most $m(k-1)$. This contradicts $N>m(k-1)$. Taking $k=\lceil N/m\rceil$ proves the displayed bound for $N>0$; for $N=0$ every count is zero.

### Infinite pigeonhole principle

↑ **Parent:** [Pigeonhole principle](#pigeonhole-principle)

The [infinite pigeonhole principle](#infinite-pigeonhole-principle) says that if an [infinite set](set.md#infinite-set) has a [partition of a set](set.md#partition-of-a-set) into finitely many parts, at least one part is an [infinite set](set.md#infinite-set). Equivalently, assigning infinitely many objects to a finite number of boxes forces some box to contain infinitely many objects. For example, separating the [natural numbers](arithmetic.md#natural-number) into their two [residue classes](number-theory.md#residue-class) modulo $2$ forces at least one class to be an [infinite set](set.md#infinite-set); here both are, as the lists $0,2,4,\ldots$ and $1,3,5,\ldots$ show.

**Proof outline.** A [union](set.md#set-union) of finitely many [finite sets](set.md#finite-set) is a [finite set](set.md#finite-set). If all the parts were [finite sets](set.md#finite-set), their [union](set.md#set-union) could not be the original [infinite set](set.md#infinite-set).

The assumption of finitely many parts is essential. With one box labelled by each [natural number](arithmetic.md#natural-number), assigning $n$ to box $n$ puts exactly one object in every box. Infinitely many objects and infinitely many boxes therefore need not produce even a shared box. The [infinite pigeonhole principle](#infinite-pigeonhole-principle) is useful whenever finitely many labels organize an endless collection: one label must keep occurring infinitely often, providing an [infinite set](set.md#infinite-set) on which that label is constant.

## Enumerative combinatorics

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Enumerative_combinatorics)

### q-analogue

↑ **Parent:** [Enumerative combinatorics](#enumerative-combinatorics)

A parameter-dependent generalization which recovers a familiar object at a specified value or [limit](calculus.md#limit-of-a-function) of the parameter. In [enumerative combinatorics](#enumerative-combinatorics), a [generating function](real-analysis.md#generating-function) can refine an ordinary count by retaining a statistic; [Gaussian binomial coefficients](#gaussian-binomial-coefficient) are one example.

### Board tiling

↑ **Parent:** [Enumerative combinatorics](#enumerative-combinatorics)

Covering a finite board with specified tiles without gaps or overlaps. Counting [board tilings](#board-tiling) connects local placement rules to a [recurrence relation](real-analysis.md#recurrence-relation) and a [generating function](real-analysis.md#generating-function).

## Combinatorial structure

↑ **Parent:** [Combinatorics](combinatorics.md)

### Labelled combinatorial structure

↑ **Parent:** [Combinatorial structure](#combinatorial-structure)

A [combinatorial structure](#combinatorial-structure) whose elements carry distinct labels from a prescribed [finite set](set.md#finite-set). For example, a [rooted tree](#rooted-tree) can have labelled [vertices](graph.md#vertex-graph-theory); assigning labels is part of the structure counted by an [exponential generating function](real-analysis.md#exponential-generating-function).

## Matroid

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matroid)

A [matroid](#matroid) on a finite [set](set.md) $E$ consists of a nonempty family of independent [subsets](set.md#subset) closed under taking [subsets](set.md#subset) and satisfying exchange: if independent [sets](set.md) $I,J$ obey $|I|<|J|$, some $j\in J\setminus I$ has $I\cup\{j\}$ independent. [Linear independence](vector-space.md#linear-independence) of [vectors](vector-space.md#vector) is the motivating example. A [pregeometry](foundations-of-mathematics.md#pregeometry) is a finitary closure-theoretic extension to possibly infinite [sets](set.md).

## Rule of product

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rule_of_product)

For finite [sets](set.md), the number of ordered choices of one element from each is the product of the individual numbers of choices. More generally, if stage $j$ has exactly $n_j$ possible choices after every permitted history of earlier stages, the total number of full choice sequences is $\prod_j n_j$, by [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on the stages. This counts $b^a$ [functions](function.md) between sets of sizes $a,b$, and counts the [injective functions](algebra.md#injective-function) by the [falling factorial](#falling-factorial) $b(b-1)\cdots(b-a+1)$ when $a\le b$.

With five people, choose a captain in five ways and a different deputy in four ways: **$5\cdot4=20$ ordered assignments**. The second choice depends on the first because the captain is excluded, but its number of permitted options is always four. The [rule of product](#rule-of-product) therefore applies without any assumption about [independent events](probability-theory.md#independent-events). To count two-person teams instead, each [subset](set.md#subset) has two possible role assignments, so division by $2!=2$ gives ten teams. This division works because every team was counted equally often.

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

The [cycle lemma](#cycle-lemma) turns a constraint at every prefix into a choice of where to start reading a circular [sequence](real-analysis.md#sequence). Think of a [lattice path](#lattice-path) whose vertical increments record votes for two candidates: $+1$ for one candidate and $-1$ for the other. Its [partial sums](real-analysis.md#partial-sum) are the running lead. Rotating the increments preserves the final lead, but changes whether that lead stays strictly positive throughout. This makes rotation useful for counting [lattice paths](#lattice-path) subject to prefix constraints; the sum-one [cycle lemma](#cycle-lemma) also supplies the cyclic prefix condition in the [cyclic Turán covering construction](hypergraph.md#cyclic-turan-covering-construction).

**The sum-one form.** Let $b=(b_1,\ldots,b_n)$ be any nonempty [sequence](real-analysis.md#sequence) of [integers](number-theory.md#integer) with $\sum_{i=1}^n b_i=1$. A starting position $r\in\{0,\ldots,n-1\}$ means reading the rotated [sequence](real-analysis.md#sequence)

$$
b^{(r)}=(b_{r+1},\ldots,b_n,b_1,\ldots,b_r).
$$

Call $r$ good when every nonempty [partial sum](real-analysis.md#partial-sum) of $b^{(r)}$ is strictly positive, including the full [sum](arithmetic.md#sum):

$$
P_j^{(r)}=\sum_{i=1}^{j}b_i^{(r)}>0\qquad(1\leq j\leq n).
$$

The [cycle lemma](#cycle-lemma) says there is exactly one good starting position. Negative entries, zero entries and positive entries larger than one are all allowed in this sum-one form. The empty [partial sum](real-analysis.md#partial-sum) is zero and is excluded from the positivity requirement. Douglas West's exercise 1.3.46(a) states a stronger result for arbitrary [integer](number-theory.md#integer) entries: take its case with all $n$ [partial sums](real-analysis.md#partial-sum) positive. [West, Combinatorial Mathematics, exercise 1.3.46(a), p. 50](https://api.pageplace.de/preview/DT0400.9781108889520_A49236431/preview-9781108889520_A49236431.pdf#page=72)

**A worked sum-one example.** For $b=(2,-2,0,1)$, the [partial sums](real-analysis.md#partial-sum) starting at zero are $S_0,S_1,S_2,S_3,S_4=0,2,0,0,1$. Starts $0,1,2$ fail: they have, respectively, a zero second [partial sum](real-analysis.md#partial-sum), a negative first [partial sum](real-analysis.md#partial-sum), and a zero first [partial sum](real-analysis.md#partial-sum). Start $3$ reads $(1,2,-2,0)$ and has nonempty [partial sums](real-analysis.md#partial-sum) $1,3,1,1$, all positive. This example both allows an increment larger than one and shows why touching zero fails.

**Why the last minimum works.** Put $S_0=0$ and $S_j=\sum_{i=1}^j b_i$. Choose the last index $r$ attaining the [minimum](set.md#minimum-of-a-subset-of-a-total-order) of the proper [partial sums](real-analysis.md#partial-sum) $S_0,\ldots,S_{n-1}$: include $S_0$ and exclude $S_n$. After that index, later proper [partial sums](real-analysis.md#partial-sum) are strictly larger than $S_r$; also $S_n=1>S_r$, since $S_r\leq0$. Before wrapping, the new [partial sums](real-analysis.md#partial-sum) are therefore positive differences $S_j-S_r$. After wrapping, they are $1+S_j-S_r\geq1$. In the worked example the last [minimum](set.md#minimum-of-a-subset-of-a-total-order) is at $r=3$; choosing the first [minimum](set.md#minimum-of-a-subset-of-a-total-order) at $r=0$ would fail. Uniqueness takes one further observation: two good starts would split the circle into two nonempty arcs, each having a positive [integer](number-theory.md#integer) [sum](arithmetic.md#sum), yet their [sum](arithmetic.md#sum) would be one.

### Cycle lemma with increments at most one

↑ **Parent:** [Cycle lemma](#cycle-lemma)

A standard positive-total form of the [Dvoretzky-Motzkin cycle lemma](#cycle-lemma) uses a nonempty [sequence](real-analysis.md#sequence) $a=(a_1,\ldots,a_n)$ of [integers](number-theory.md#integer) satisfying

$$
a_i\leq1\quad(1\leq i\leq n),\qquad \sum_{i=1}^{n}a_i=k>0.
$$

Exactly $k$ starting positions have every nonempty [partial sum](real-analysis.md#partial-sum) strictly positive, using the same rotation convention as the sum-one [cycle lemma](#cycle-lemma). Negative entries can be arbitrarily large in magnitude, and zero entries are allowed. Addario-Berry's proposition 2.2.1 gives an equivalent form with increments at least $-1$ and negative total; reversing the [sequence](real-analysis.md#sequence) and changing all signs gives the form here. [Addario-Berry, Lecture notes: 2021 CRM-PIMS Probability Summer School, proposition 2.2.1, p. 39](https://problab.ca/louigi/notes/ssprob2021.pdf#page=39)

**Four starts, two successes.** For $a=(1,1,1,-1)$, the [sum](arithmetic.md#sum) is $k=2$. Starts $0$ and $1$ give [partial sums](real-analysis.md#partial-sum) $(1,2,3,2)$ and $(1,2,1,2)$, respectively. Start $2$ gives $(1,0,1,2)$ and touches zero; start $3$ gives $(-1,0,1,2)$ and begins below zero. Thus exactly two starts are good. The rotated [sequence](real-analysis.md#sequence) $(-1,1,1,1)$ has the same positive total, but its first start is bad: a positive final lead alone does not control earlier [partial sums](real-analysis.md#partial-sum).

<a id="image-all-four-starts-of-1-1-1-1-the-cycle-lemma-with-increments-at-most-one-counts-precisely-the-two-paths-whose-nonempty-partial-sums-stay-strictly-above-zero"></a>
![](cycle-lemma-good-rotations.png)

**[Figure 3](#image-all-four-starts-of-1-1-1-1-the-cycle-lemma-with-increments-at-most-one-counts-precisely-the-two-paths-whose-nonempty-partial-sums-stay-strictly-above-zero). All four starts of $(1,1,1,-1)$: the cycle lemma with increments at most one counts precisely the two paths whose nonempty partial sums stay strictly above zero**.

**Positions can give identical words.** The [sequence](real-analysis.md#sequence) $(1,1,-1,1,1,-1)$ repeats a block of length three and has [sum](arithmetic.md#sum) two. Its good starts are $0$ and $3$, both giving the same [word](foundations-of-mathematics.md#string) $(1,1,-1,1,1,-1)$ with [partial sums](real-analysis.md#partial-sum) $(1,2,1,2,3,2)$. Starts $1$ and $4$ touch zero; starts $2$ and $5$ begin negatively. The [cycle lemma with increments at most one](#cycle-lemma-with-increments-at-most-one) counts two starting positions even though there is only one distinct good rotated [word](foundations-of-mathematics.md#string). Counting distinct [words](foundations-of-mathematics.md#string) would lose the multiplicity that makes the statement true.

<a id="image-six-starting-positions-of-the-repeating-sequence-1-1-1-1-1-1-starts-0-and-3-produce-identical-good-words-and-count-twice"></a>
![](cycle-lemma-periodic-start-positions.png)

**[Figure 4](#image-six-starting-positions-of-the-repeating-sequence-1-1-1-1-1-1-starts-0-and-3-produce-identical-good-words-and-count-twice). Six starting positions of the repeating sequence $(1,1,-1,1,1,-1)$: starts $0$ and $3$ produce identical good words and count twice**.

**The upper bound matters.** The one-entry [sequence](real-analysis.md#sequence) $(2)$ has positive [integer](number-theory.md#integer) [sum](arithmetic.md#sum) two, but only one starting position. Thus the sum-$k$ conclusion fails for arbitrary positive increments when $k>1$. The sum-one [cycle lemma](#cycle-lemma) above needs no such upper bound. Strict positivity also matters: counting paths that merely stay at or above zero would include additional starts in both diagrams.

**From rotation to enumeration.** For a fixed admissible [sequence](real-analysis.md#sequence), a start chosen from a [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution) of its $n$ positions is good with [probability](probability-theory.md#probability) $k/n$. More generally, let $\mathcal F$ be any [finite set](set.md#finite-set) of length-$n$ [sequences](real-analysis.md#sequence) satisfying the increment bound and total $k$, closed under rotation. [Double counting](#double-counting-proof-technique) pairs consisting of a [sequence](real-analysis.md#sequence) and a good starting position gives

$$
\#\{a\in\mathcal F:\text{all nonempty partial sums of }a\text{ are positive}\}
=\frac{k}{n}|\mathcal F|.
$$

For each good output [sequence](real-analysis.md#sequence) and each of the $n$ positions, inverse rotation gives one such pair, even when several rotated [words](foundations-of-mathematics.md#string) coincide. For example, the four [sequences](real-analysis.md#sequence) containing three $+1$ votes and one $-1$ vote have exactly $\frac24\binom43=2$ vote orders with a strictly positive running lead: $(1,1,1,-1)$ and $(1,1,-1,1)$. This is how the [cycle lemma with increments at most one](#cycle-lemma-with-increments-at-most-one) converts many prefix inequalities into a simple counting factor.

## Cyclic digit run

↑ **Parent:** [Combinatorics](combinatorics.md)

A cyclic digit run is a consecutive segment of a digit string whose successive digits all increase by one or all decrease by one modulo the base. For example, $8,9,0,1$ is an increasing decimal run. This refers to cyclic digit values, not to joining the final position of the string back to its first position. Overlapping run constraints can be counted with the [inclusion-exclusion principle](#inclusion-exclusion-principle).

## Finite geometry

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_geometry)

Finite geometry studies geometric incidence structures having finitely many points, such as finite projective and affine spaces.

## Increasing subsequence

↑ **Parent:** [Combinatorics](combinatorics.md)

An [increasing subsequence](#increasing-subsequence) of a finite [sequence](real-analysis.md#sequence) $x=(x_1,\ldots,x_n)$ in a [totally ordered set](set.md#totally-ordered-set) selects indices $1\leq i_1<\cdots<i_m\leq n$ such that

$$
x_{i_1}\leq x_{i_2}\leq\cdots\leq x_{i_m}.
$$

Here “increasing” means weakly increasing, also called nondecreasing: equal values are allowed, but indices must increase strictly. This is the convention of [Liben-Nowell, Vee and Zhu, Finding Longest Increasing and Common Subsequences in Streaming Data, section 1](https://cs.carleton.edu/faculty/dlibenno/papers/lis-lcs/lislcs.pdf). A [strictly increasing subsequence](#strictly-increasing-subsequence) instead requires $x_{i_1}<\cdots<x_{i_m}$. Always check which convention an [algorithm](computer-science.md#algorithm) uses, especially when values repeat.

An [increasing subsequence](#increasing-subsequence) may skip positions; it neither rearranges values nor requires consecutive positions. Consider the deliberately constructed example

$$
x=(4,1,3,2,2,5,0).
$$

The indices $(2,4,5,6)$ select $(1,2,2,5)$, an [increasing subsequence](#increasing-subsequence) of length four. The indices $(2,3,6)$ select $(1,3,5)$, a [strictly increasing subsequence](#strictly-increasing-subsequence) of length three. In contrast, $(0,1,2,2,3,4,5)$ rearranges the input and is not a [subsequence](real-analysis.md#subsequence). The longest consecutive nondecreasing block is $(2,2,5)$, of length three; requiring consecutive positions would therefore solve a different problem.

Think of an [increasing subsequence](#increasing-subsequence) as preserving ordered observations while skipping interruptions. For the example, discarding $4,3,0$ leaves four observations with no downward step. The [longest increasing subsequence](#longest-increasing-subsequence) asks how much of the original order can be kept. This is an order comparison, rather than a claim about the size of upward or downward changes: replacing all values by their squares when the values are nonnegative leaves every allowed selection unchanged. More generally, any strictly order-preserving relabeling has this property.

### Longest increasing subsequence

↑ **Parent:** [Increasing subsequence](#increasing-subsequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Longest_increasing_subsequence)

A [longest increasing subsequence](#longest-increasing-subsequence) is an [increasing subsequence](#increasing-subsequence) of [maximum](set.md#maximum-of-a-subset-of-a-total-order) length. Write that length as $L(x)$, with $L(())=0$ for the empty [sequence](real-analysis.md#sequence); a nonempty input has $1\leq L(x)\leq n$. Several selections can attain the same [maximum](set.md#maximum-of-a-subset-of-a-total-order). Here $L$ uses the weak convention $\leq$; write $L_{<}(x)$ for the [maximum](set.md#maximum-of-a-subset-of-a-total-order) length of a [strictly increasing subsequence](#strictly-increasing-subsequence). For $(2,2,2)$, these lengths are three and one respectively; for an input with distinct values they agree.

For $x=(4,1,3,2,2,5,0)$, the answer is $L(x)=4$, attained at indices $(2,4,5,6)$, while $L_{<}(x)=3$. One useful interpretation is the smallest number of deletions needed to make the surviving [sequence](real-analysis.md#sequence) nondecreasing:

$$
\text{minimum deletions}=n-L(x).
$$

Indeed, keeping a [longest increasing subsequence](#longest-increasing-subsequence) attains this bound, and any valid remaining [sequence](real-analysis.md#sequence) is an [increasing subsequence](#increasing-subsequence), so cannot have more than $L(x)$ terms. In this example the answer is $7-4=3$. This makes $L(x)$ a measure of how much order can be recovered without moving any observation.

**A table that ends at each position.** Let $d_i$ be the [maximum](set.md#maximum-of-a-subset-of-a-total-order) length of an [increasing subsequence](#increasing-subsequence) ending specifically at position $i$. The [dynamic programming](mathematical-optimization.md#dynamic-programming) [recurrence relation](real-analysis.md#recurrence-relation) is

$$
d_i=1+\max\bigl(\{0\}\cup\{d_j:1\leq j<i,\ x_j\leq x_i\}\bigr),\qquad L(x)=\max_{1\leq i\leq n}d_i\quad(n>0).
$$

The zero covers a selection consisting only of $x_i$. Otherwise its penultimate index is an eligible $j$; append $x_i$ to an optimal selection ending there. Fill entries in increasing index order. For [strictly increasing subsequences](#strictly-increasing-subsequence), change the comparison to $x_j<x_i$. The strict version and reconstruction are developed in [University of Toronto, CSC373 tutorial 4 solutions (2018), exercise 2](https://www.cs.toronto.edu/~jepson/csc373/tutNotes/tutEx_DynProg_Soln.pdf); the weak version follows by allowing equality at the append step.

In the worked input, the weak table is $(1,1,2,2,3,4,1)$ and the strict table is $(1,1,2,2,2,3,1)$. At the second $2$, equality extends the first $2$ in the weak table. The final entry is only one, although the optimum is four: the best [increasing subsequence](#increasing-subsequence) need not finish at the last input position. Record a maximizing predecessor $p_i=j$ whenever $d_i>1$. Following these stored indices from any position maximizing $d_i$, then reversing them, gives an actual [longest increasing subsequence](#longest-increasing-subsequence). For the weak example the backward chain is $6,5,4,2$.

<a id="image-skipping-positions-and-allowing-equal-values-changes-the-optimum"></a>
![](increasing-subsequence-dp-witness.png)

**[Figure 5](#image-skipping-positions-and-allowing-equal-values-changes-the-optimum). Skipping positions and allowing equal values changes the optimum**. An original toy input, not measured data. The colored selection keeps indices $2,4,5,6$ and values $1,2,2,5$. The two [dynamic programming](mathematical-optimization.md#dynamic-programming) rows give the best lengths ending at every position; the backward arrows reconstruct the weak [longest increasing subsequence](#longest-increasing-subsequence).

Scanning all earlier positions for each $i$ uses [time complexity](computer-science.md#time-complexity) $O(n^2)$ and [space complexity](computer-science.md#space-complexity) $O(n)$ for lengths and predecessors, using [Big O notation](real-analysis.md#big-o-notation) and assuming constant-time comparisons and operations on indices.

**Keep the easiest ending to extend.** The faster [algorithm](computer-science.md#algorithm) maintains a [minimum-tail table for increasing subsequences](#minimum-tail-table-for-increasing-subsequences): $T_\ell$ is the smallest final value of any length-$\ell$ [increasing subsequence](#increasing-subsequence) in the processed prefix. For equal lengths, a smaller ending permits every future extension allowed by a larger ending. Thus only one best ending per length is needed. The table is nondecreasing, since removing the last term of a length-$(\ell+1)$ selection gives $T_\ell\leq T_{\ell+1}$. Start with an empty table. On reading $v=x_i$, use [binary search](computer-science.md#binary-search) to find the first entry strictly greater than $v$: replace it by $v$, or append $v$ if there is no such entry. Its position is one beyond the longest existing length whose ending is at most $v$. See [Liben-Nowell, Vee and Zhu, section 3.1 and Figure 1](https://cs.carleton.edu/faculty/dlibenno/papers/lis-lcs/lislcs.pdf).

Duplicates determine the [binary search](computer-science.md#binary-search) rule: weak increase replaces the first $T_\ell>v$, whereas strict increase replaces the first $T_\ell\geq v$. In Python these positions are returned by `bisect_right(T, v)` and `bisect_left(T, v)` respectively, counting positions from zero. Replace an entry or append; do not insert and shift the remaining entries. The documented equality rules are in [Python documentation, bisect\_left and bisect\_right](https://docs.python.org/3/library/bisect.html). Each search takes $O(\log(n+1))$ comparisons, giving [time complexity](computer-science.md#time-complexity) $O(n\log(n+1))$, conventionally $O(n\log n)$ for $n\geq2$, and [space complexity](computer-science.md#space-complexity) $O(L(x))$ for the weak length alone.

<a id="image-two-binary-search-tie-rules-give-different-minimum-tail-tables"></a>
![](increasing-subsequence-tails-trace.png)

**[Figure 6](#image-two-binary-search-tie-rules-give-different-minimum-tail-tables). Two binary-search tie rules give different minimum-tail tables**. Original exact traces for the same toy input, not measured data. Each cell shows a tail value and the input index supplying it; the outlined cell was updated in that row. At the second $2$, the weak [algorithm](computer-science.md#algorithm) appends and the strict [algorithm](computer-science.md#algorithm) replaces. The final weak table has length four, but its supplier indices $7,4,5,6$ are not in increasing order.

**A length certificate needs separate reconstruction.** The final weak tail values are $(0,2,2,5)$, but they do not form an [increasing subsequence](#increasing-subsequence) of this input: the zero occurs last. Each table entry certifies a selection of its own length; the entries need not come from one compatible selection. To recover a [longest increasing subsequence](#longest-increasing-subsequence) during the fast [algorithm](computer-science.md#algorithm), store a supplier index $q_\ell$ for each tail and a predecessor index for each input position. Before replacing slot $r$, save $p_i=q_{r-1}$, or no predecessor if $r=1$, then set $q_r=i$. Later replacements leave saved $p_i$ unchanged. Follow predecessors from the final $q_{L(x)}$ and reverse. This uses [space complexity](computer-science.md#space-complexity) $O(n)$ and returns indices $(2,4,5,6)$ for the weak trace. The same construction works with the strict comparator; compare the two auxiliary arrays in [CP Algorithms contributors, restoring the subsequence after binary search](https://cp-algorithms.com/dynamic_programming/longest_increasing_subsequence.html#restoring-the-subsequence_1).

**Deleting or changing one term.** If $x^{\setminus k}$ deletes position $k$, then

$$
L(x)-1\leq L(x^{\setminus k})\leq L(x).
$$

Deleting cannot create a longer [increasing subsequence](#increasing-subsequence); removing position $k$ from a previously optimal selection loses at most one term. If $x'$ instead changes just the value at position $k$, both inputs have the same deleted [sequence](real-analysis.md#sequence), so their lengths each lie between its length and its length plus one. Consequently $|L(x')-L(x)|\leq1$. These bounds also hold for [strictly increasing subsequences](#strictly-increasing-subsequence). In the weak example, deleting either $2$ lowers the length to three, while deleting the final zero leaves it four. This is a [Lipschitz bound](real-analysis.md#lipschitz-bound) for single-term edits, regardless of the numerical size of a replacement. Insertion has the same bound by reversing deletion, so $m$ insertions, deletions or replacements can change $L$ by at most $m$.

For historical context, [Fredman, On computing the length of longest increasing subsequences (1975)](https://doi.org/10.1016/0012-365X(75)90103-X) studies the comparison count for distinct elements of a [totally ordered set](set.md#totally-ordered-set). Its distinctness assumption makes the weak and strict conventions coincide. No distinctness assumption is needed for the comparator-specific [algorithms](computer-science.md#algorithm) above.

#### Minimum-tail table for increasing subsequences

↑ **Parent:** [Longest increasing subsequence](#longest-increasing-subsequence)

For a processed prefix $(x_1,\ldots,x_i)$, the [minimum-tail table for increasing subsequences](#minimum-tail-table-for-increasing-subsequences) stores

$$
T_\ell=\min\{x_{j_\ell}:1\leq j_1<\cdots<j_\ell\leq i,\ x_{j_1}\leq\cdots\leq x_{j_\ell}\},\qquad 1\leq\ell\leq L(x_1,\ldots,x_i).
$$

There is no slot for an unattainable length. The table records [minimum](set.md#minimum-of-a-subset-of-a-total-order) endings, rather than the terms of one [longest increasing subsequence](#longest-increasing-subsequence). Replacing the value comparisons by $<$ gives the corresponding table for [strictly increasing subsequences](#strictly-increasing-subsequence), whose entries are strictly increasing.

### Strictly increasing subsequence

↑ **Parent:** [Increasing subsequence](#increasing-subsequence)

A [strictly increasing subsequence](#strictly-increasing-subsequence) selects indices $i_1<\cdots<i_m$ of a [sequence](real-analysis.md#sequence) with $x_{i_1}<\cdots<x_{i_m}$. Equal values cannot both occur in it. Its [maximum](set.md#maximum-of-a-subset-of-a-total-order) possible length is $L_{<}(x)$, with $L_{<}(())=0$; in general $L_{<}(x)\leq L(x)$ for the weak [longest increasing subsequence](#longest-increasing-subsequence). Use strict comparisons in the [dynamic programming](mathematical-optimization.md#dynamic-programming) [recurrence relation](real-analysis.md#recurrence-relation) and replace the first tail at least as large as the next value in the [binary search](computer-science.md#binary-search) [algorithm](computer-science.md#algorithm).

## Additive combinatorics

↑ **Parent:** [Combinatorics](combinatorics.md)

[This section is present in another page, follow this link to view it.](additive-combinatorics.md)

## Indegree

↑ **Parent:** [Combinatorics](combinatorics.md)

The [indegree](#indegree) $d^-(v)$ of a [vertex](graph.md#vertex-graph-theory) $v$ is the number of [directed edges](graph-theory.md#directed-edge) entering it, counting repeated [directed edges](graph-theory.md#directed-edge) separately if permitted. In the toy [Directed acyclic graph](#directed-acyclic-graph), the initial [indegrees](#indegree) of $A,B,C,D,E$ are $0,0,1,2,2$. In [Kahn's algorithm](#kahn-s-algorithm), these counts are updated to describe only the remaining [directed graph](graph-theory.md#directed-graph), so [indegree](#indegree) zero means that no unfinished predecessor remains. [Sedgewick and Wayne, Digraph: definition of indegree](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/Digraph.java)

## Directed acyclic graph

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Directed_acyclic_graph)

A [Directed acyclic graph](#directed-acyclic-graph) is a [directed graph](graph-theory.md#directed-graph) with no [directed cycle](graph-theory.md#directed-cycle): following its [directed edges](graph-theory.md#directed-edge) can never return to the starting [vertex](graph.md#vertex-graph-theory). A [directed edge](graph-theory.md#directed-edge) $u\to v$ can represent the requirement that task $u$ finish before task $v$ starts. A [directed path](graph-theory.md#directed-path) then records a chain of prerequisites. The essential prerequisite for [topological sorting](#topological-sorting) is that these requirements contain no circular dependency. For finite [directed graphs](graph-theory.md#directed-graph), this is equivalent to the existence of a [topological order](#topological-order). [MIT, Introduction to Algorithms, Recitation 10, p. 3: directed acyclic graphs and topological sorts](https://live.ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/d9265b3b33d238ff914b0223ac8e7628_MIT6_006S20_r10.pdf)

Consider an invented publishing workflow with five tasks: $A$ drafts the text, $B$ draws a figure, $C$ reviews the text, $D$ lays out the text and figure, and $E$ publishes the result. Its [directed edges](graph-theory.md#directed-edge) are $A\to C$, $A\to D$, $B\to D$, $C\to E$, and $D\to E$. Reviewing needs the draft; layout needs both the draft and figure; publication needs both review and layout. The drawing below encodes only these prerequisites, with no measured durations or resource constraints.

<a id="image-five-toy-publishing-tasks-and-all-five-valid-topological-orders"></a>
![](topological-task-dependency-orders.png)

**[Figure 7](#image-five-toy-publishing-tasks-and-all-five-valid-topological-orders). Five toy publishing tasks and all five valid topological orders**.

The [Directed acyclic graph](#directed-acyclic-graph) leaves room for choice: $A$ and $B$ can occur in either order, and after both are complete, $C$ and $D$ can occur in either order. Task $C$ may even precede $B$, since the review does not need the figure. A [topological order](#topological-order) turns these local prerequisites into a complete executable list while retaining this freedom. It supplies a feasible sequential plan; task durations, available workers, and earliest finishing times require additional information.

### Topological sorting

↑ **Parent:** [Directed acyclic graph](#directed-acyclic-graph)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_sorting)

A [topological sorting](#topological-sorting) is the task of constructing a [topological order](#topological-order) of a finite [directed graph](graph-theory.md#directed-graph), or reporting that a [directed cycle](graph-theory.md#directed-cycle) makes one impossible. [Kahn's algorithm](#kahn-s-algorithm) repeatedly takes a [vertex](graph.md#vertex-graph-theory) with no unfinished prerequisites. This is useful whenever an operation consumes results produced by earlier operations: once a [vertex](graph.md#vertex-graph-theory) is reached in a [topological order](#topological-order), every prerequisite along a [directed path](graph-theory.md#directed-path) has already been processed. [MIT, Lecture 14: job scheduling and topological sorting](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2008/resources/lec14/)

The reason a choice is always available in a nonempty finite [Directed acyclic graph](#directed-acyclic-graph) is simple. If every [vertex](graph.md#vertex-graph-theory) had an incoming [directed edge](graph-theory.md#directed-edge), repeatedly following predecessors would eventually revisit a [vertex](graph.md#vertex-graph-theory), giving a [directed cycle](graph-theory.md#directed-cycle). Removing a [vertex](graph.md#vertex-graph-theory) and its incident [directed edges](graph-theory.md#directed-edge) cannot create a [directed cycle](graph-theory.md#directed-cycle), so the argument repeats until every [vertex](graph.md#vertex-graph-theory) is listed. This proves existence of a [topological order](#topological-order) and explains why finiteness matters to this procedure.

// Target: combinatorics.bigb

#### Topological order

↑ **Parent:** [Topological sorting](#topological-sorting)

A [topological order](#topological-order) of a finite [directed graph](graph-theory.md#directed-graph) $G=(V,E)$ is a [sequence](real-analysis.md#sequence) $(v_1,\ldots,v_n)$ containing every [vertex](graph.md#vertex-graph-theory) exactly once, with

$$
(v_i,v_j)\in E\quad\Longrightarrow\quad i<j.
$$

Thus every [directed edge](graph-theory.md#directed-edge) points forward in the list. Equivalently, a [bijection](function.md#bijection) $p:V\to\{1,\ldots,n\}$ assigning positions satisfies $p(u)<p(v)$ for every [directed edge](graph-theory.md#directed-edge) $u\to v$. A [topological ordering](#topological-ordering) names the same kind of list. [MIT, Recitation 10, p. 3: the edge-by-edge definition](https://live.ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/d9265b3b33d238ff914b0223ac8e7628_MIT6_006S20_r10.pdf)

The toy [Directed acyclic graph](#directed-acyclic-graph) has exactly five [topological orders](#topological-order): $ABCDE$, $ABDCE$, $ACBDE$, $BACDE$, and $BADCE$. These lists were checked by enumerating all $5!=120$ [permutations](#permutation) and retaining precisely those satisfying all five [directed edge](graph-theory.md#directed-edge) inequalities. Every list ends with $E$, since all other tasks have a [directed path](graph-theory.md#directed-path) to publication. A [topological order](#topological-order) need not put adjacent entries next to one another in the [directed graph](graph-theory.md#directed-graph): $A$ and $B$ are consecutive in $ABCDE$ without a [directed edge](graph-theory.md#directed-edge) between them.

A [directed cycle](graph-theory.md#directed-cycle) would force the impossible chain of position inequalities $p(u_1)<p(u_2)<\cdots<p(u_k)<p(u_1)$. In the toy example, adding $E\to C$ requires review before publication and publication before review, so there are no [topological orders](#topological-order). Together with the construction in [topological sorting](#topological-sorting), this proves that a finite [directed graph](graph-theory.md#directed-graph) admits a [topological order](#topological-order) if and only if it is a [Directed acyclic graph](#directed-acyclic-graph). The empty [directed graph](graph-theory.md#directed-graph) has the empty [sequence](real-analysis.md#sequence) as its [topological order](#topological-order).

There is also a useful connection to [partial orders](set.md#partially-ordered-set): define $u\preceq v$ when $u=v$ or there is a [directed path](graph-theory.md#directed-path) from $u$ to $v$. For a [Directed acyclic graph](#directed-acyclic-graph), this [reachability](graph.md#reachability-in-a-graph) relation is a [partial order](set.md#partially-ordered-set), and its [linear extensions](set.md#linear-extension) are exactly the [topological orders](#topological-order). The [Directed acyclic graph](#directed-acyclic-graph) specifies which pairs must be ordered; a [topological order](#topological-order) chooses positions for all the remaining pairs.

<h4 id="kahn-s-algorithm">Kahn's algorithm</h4>

↑ **Parent:** [Topological sorting](#topological-sorting)

[Kahn's algorithm](#kahn-s-algorithm) maintains each remaining [vertex](graph.md#vertex-graph-theory)'s [indegree](#indegree), the number of its unfinished incoming [directed edges](graph-theory.md#directed-edge), and a [FIFO queue](computer-science.md#fifo-queue) of ready [vertices](graph.md#vertex-graph-theory). Initialize the counts by scanning all [directed edges](graph-theory.md#directed-edge) and enqueue every [vertex](graph.md#vertex-graph-theory) of [indegree](#indegree) zero. Repeatedly dequeue a [vertex](graph.md#vertex-graph-theory) $u$, append it to the output, and decrement the count of each destination $v$ in $u$'s [adjacency list](computer-science.md#adjacency-list). Enqueue $v$ exactly when its count becomes zero. When the [FIFO queue](computer-science.md#fifo-queue) empties, accept the output if it contains all [vertices](graph.md#vertex-graph-theory); otherwise report a [directed cycle](graph-theory.md#directed-cycle). [Sedgewick and Wayne, TopologicalX: queue-based topological sorting](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/TopologicalX.java)

<a id="image-computed-ready-queue-trace-and-the-obstruction-caused-by-a-reverse-dependency"></a>
![](kahn-ready-queue-and-cycle.png)

**[Figure 8](#image-computed-ready-queue-trace-and-the-obstruction-caused-by-a-reverse-dependency). Computed ready-queue trace and the obstruction caused by a reverse dependency**.

In the displayed run, initialize the [FIFO queue](computer-science.md#fifo-queue) as $A,B$ and visit $A$'s destinations in the order $C,D$. Removing $A$ makes $C$ ready but leaves $D$ waiting for $B$. Removing $B$ then makes $D$ ready. Publication becomes ready only after both $C$ and $D$ are removed. The output is $ABCDE$; choosing ready [vertices](graph.md#vertex-graph-theory) differently can produce the other [topological orders](#topological-order). For the modified [directed graph](graph-theory.md#directed-graph) with $E\to C$, the same procedure emits $A,B,D$ and then stops with $C,E$ still waiting on each other.

The invariant is that each stored [indegree](#indegree) counts incoming [directed edges](graph-theory.md#directed-edge) from unprocessed [vertices](graph.md#vertex-graph-theory). A ready [vertex](graph.md#vertex-graph-theory) therefore has every prerequisite already in the output. If the [FIFO queue](computer-science.md#fifo-queue) empties with [vertices](graph.md#vertex-graph-theory) left, every remaining [vertex](graph.md#vertex-graph-theory) has a predecessor in the remaining [directed graph](graph-theory.md#directed-graph); the predecessor argument gives a [directed cycle](graph-theory.md#directed-cycle). The unprocessed [vertices](graph.md#vertex-graph-theory) can also include tasks blocked downstream of a [directed cycle](graph-theory.md#directed-cycle), so the leftover list alone is not a list of exactly the cyclic [vertices](graph.md#vertex-graph-theory).

With [adjacency lists](computer-science.md#adjacency-list), constant-time [array](computer-science.md#array-data-structure) access and counter updates, and constant-time [FIFO queue](computer-science.md#fifo-queue) operations, the [time complexity](computer-science.md#time-complexity) is $O(|V|+|E|)$ in [Big O notation](real-analysis.md#big-o-notation). Initialization scans all [vertices](graph.md#vertex-graph-theory) and [directed edges](graph-theory.md#directed-edge); each [vertex](graph.md#vertex-graph-theory) is then enqueued at most once and each outgoing [directed edge](graph-theory.md#directed-edge) processed at most once. Counts, ready [FIFO queue](computer-science.md#fifo-queue), and output need $O(|V|)$ storage beyond the [adjacency lists](computer-science.md#adjacency-list). Shifting an [array](computer-science.md#array-data-structure) on every dequeue invalidates this bound. [Sedgewick and Wayne, TopologicalX: time and extra-space bounds](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/TopologicalX.java) [Sedgewick and Wayne, Digraph: adjacency lists and outgoing-edge iteration](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/Digraph.java)

The name refers to A. B. Kahn's 1962 paper "Topological sorting of large networks", published in Communications of the ACM, volume 5, issue 11, pages 558–562. Its abstract motivates [topological sorting](#topological-sorting) through network analysis and project planning. [Kahn, Topological sorting of large networks (1962): publisher's record and abstract](https://doi.org/10.1145/368996.369025)

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

A [topological ordering](#topological-ordering) is a [topological order](#topological-order): a list containing every [vertex](graph.md#vertex-graph-theory) once and placing the source of every [directed edge](graph-theory.md#directed-edge) before its destination. In the parent-and-child language of a [Directed acyclic graph](#directed-acyclic-graph), every parent precedes every child, and hence every ancestor precedes every descendant along a [directed path](graph-theory.md#directed-path). This is an ordering of the [vertices](graph.md#vertex-graph-theory), whereas [topological sorting](#topological-sorting) is the task of finding it. See [topological order](#topological-order) for the precise position condition and [Kahn's algorithm](#kahn-s-algorithm) for a construction.

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

A [tree](#tree-graph-theory) is a nonempty [connected graph](graph.md#connected-graph) containing no [graph cycle](graph-theory.md#cycle-in-a-graph). Think of seven locations joined so that everyone can reach everyone else, but no connection supplies an alternative route. For a finite [simple graph](graph.md#simple-graph) with $n\geq1$ [vertices](graph.md#vertex-graph-theory), three descriptions are equivalent: being a [tree](#tree-graph-theory); having exactly one simple [graph path](graph-theory.md#path-in-a-graph) between every pair of distinct [vertices](graph.md#vertex-graph-theory); and being a [connected graph](graph.md#connected-graph) with exactly $n-1$ [edges](graph-theory.md#edge-of-a-graph). Here a simple [graph path](graph-theory.md#path-in-a-graph) repeats no [vertex](graph.md#vertex-graph-theory). Connectedness in the last description is essential. [Trinity College Dublin, graph theory notes, Theorems 4.24–4.26 and Corollary 4.27](https://www.maths.tcd.ie/~dwilkins/Courses/MA2C03/MA2C03Courseware_2014to15/MA2C03_S4_Yr1415.pdf)

For a concrete [tree](#tree-graph-theory), label the [vertices](graph.md#vertex-graph-theory) $1,\ldots,7$ and take the [edges](graph-theory.md#edge-of-a-graph)

$$
E=\{12,13,24,25,36,67\},
$$

where $ij$ abbreviates the unordered pair $\{i,j\}$. There are seven [vertices](graph.md#vertex-graph-theory) and six [edges](graph-theory.md#edge-of-a-graph). The unique [graph path](graph-theory.md#path-in-a-graph) from $4$ to $7$ is $4,2,1,3,6,7$, using five [edges](graph-theory.md#edge-of-a-graph). The [degree sequence](graph-theory.md#degree-sequence) in label order is $(2,3,2,1,1,2,1)$: its sum is $12=2\cdot6$, as the [degree-sum formula](#degree-sum-formula) predicts. Each of $4,5,7$ is a [leaf of a graph](graph-theory.md#leaf-of-a-graph), having [vertex degree](graph-theory.md#degree-graph-theory) one.

<a id="image-a-seven-vertex-tree-one-graph-path-two-connected-components-of-a-graph-after-deletion-and-one-graph-cycle-after-insertion"></a>
![](tree-unique-paths.png)

**[Figure 9](#image-a-seven-vertex-tree-one-graph-path-two-connected-components-of-a-graph-after-deletion-and-one-graph-cycle-after-insertion). A seven-vertex tree: one graph path, two connected components of a graph after deletion, and one graph cycle after insertion**.

Deleting [edge](graph-theory.md#edge-of-a-graph) $13$ leaves precisely two [connected components of a graph](graph.md#component-graph-theory), on $\{1,2,4,5\}$ and $\{3,6,7\}$. Every [edge](graph-theory.md#edge-of-a-graph) of a [tree](#tree-graph-theory) is a [bridge in a graph](graph.md#bridge-graph-theory). Instead add [edge](graph-theory.md#edge-of-a-graph) $57$ to the original [tree](#tree-graph-theory): it closes the unique existing [graph path](graph-theory.md#path-in-a-graph) $5,2,1,3,6,7$ into exactly one [graph cycle](graph-theory.md#cycle-in-a-graph). Thus a [tree](#tree-graph-theory) provides economical connections with no redundancy: a single failed link separates locations. Every finite [tree](#tree-graph-theory) with at least two [vertices](graph.md#vertex-graph-theory) has at least two instances of a [leaf of a graph](graph-theory.md#leaf-of-a-graph); the endpoints of a longest [graph path](graph-theory.md#path-in-a-graph) supply them. [Dalhousie University, Trees: leaves and indispensable edges](https://www.mathstat.dal.ca/~janssen/2113/notes/class14/)

The number $n-1$ alone proves nothing about connectedness: a [cycle graph](graph-theory.md#cycle-graph) on $1,\ldots,6$ together with an isolated [vertex](graph.md#vertex-graph-theory) $7$ has seven [vertices](graph.md#vertex-graph-theory) and six [edges](graph-theory.md#edge-of-a-graph), yet is disconnected. Briefly, two different simple [graph paths](graph-theory.md#path-in-a-graph) between the same [vertices](graph.md#vertex-graph-theory) would contain a [graph cycle](graph-theory.md#cycle-in-a-graph). Repeatedly removing a [leaf of a graph](graph-theory.md#leaf-of-a-graph) and its incident [edge](graph-theory.md#edge-of-a-graph) proves the [tree](#tree-graph-theory) count $n-1$ by [mathematical induction](foundations-of-mathematics.md#mathematical-induction), starting with one [vertex](graph.md#vertex-graph-theory) and no [edges](graph-theory.md#edge-of-a-graph).

### Labelled tree

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)

A [tree](#tree-graph-theory) whose [vertices](graph.md#vertex-graph-theory) carry distinct labels from a fixed [finite set](set.md#finite-set), as a [labelled combinatorial structure](#labelled-combinatorial-structure). Two [labelled trees](#labelled-tree) on the same [vertex set](graph.md#vertex-set) are equal when their sets of [edges](graph-theory.md#edge-of-a-graph) are equal: any comparison must keep every label fixed. [Cayley's formula](#cayley-s-formula) counts these [trees](#tree-graph-theory).

### Unlabelled tree

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)

A [tree](#tree-graph-theory) considered up to [graph isomorphism](graph.md#graph-isomorphism), with [vertex](graph.md#vertex-graph-theory) names ignored. For example, all four [labelled trees](#labelled-tree) that are [star graphs](graph-theory.md#star-graph-theory) on $\{1,2,3,4\}$ represent one [unlabelled tree](#unlabelled-tree). Dividing the total in [Cayley's formula](#cayley-s-formula) by $n!$ does not count [unlabelled trees](#unlabelled-tree): different shapes can have different numbers of distinct labellings.

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

A [rooted tree](#rooted-tree) is a [tree](#tree-graph-theory) with a distinguished [vertex](graph.md#vertex-graph-theory), its [root of a tree](#root-of-a-tree) $r$. Choosing $r$ turns connections into a hierarchy: every other [vertex](graph.md#vertex-graph-theory) has a unique [parent in a rooted tree](#parent-in-a-rooted-tree), the preceding [vertex](graph.md#vertex-graph-theory) on its [graph path](graph-theory.md#path-in-a-graph) from $r$. Conversely, the [vertices](graph.md#vertex-graph-theory) whose [parent in a rooted tree](#parent-in-a-rooted-tree) is $v$ are the [children in a rooted tree](#child-in-a-rooted-tree) of $v$. Choosing the [root of a tree](#root-of-a-tree) changes this description, while the underlying [edges](graph-theory.md#edge-of-a-graph) remain the same. Arrows towards the [root of a tree](#root-of-a-tree) can encode the relationship, as in MIT's counting notes; the undirected [tree](#tree-graph-theory) itself needs no arrows. [MIT, Peter Shor's counting notes, pp. 3–4](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec05-06.pdf)

In the seven-[vertex](graph.md#vertex-graph-theory) [tree](#tree-graph-theory) above, choose $r=1$. The levels, grouped by [graph distance](graph-theory.md#distance-graph-theory) from the [root of a tree](#root-of-a-tree), are $\{1\}$, $\{2,3\}$, $\{4,5,6\}$, $\{7\}$. The [children in a rooted tree](#child-in-a-rooted-tree) of $2$ are $4,5$, and the [parent in a rooted tree](#parent-in-a-rooted-tree) of $7$ is $6$. Choosing $r=7$ instead makes the levels $\{7\}$, $\{6\}$, $\{3\}$, $\{1\}$, $\{2\}$, $\{4,5\}$: now $6$ has [parent in a rooted tree](#parent-in-a-rooted-tree) $7$, reversing their relationship. All six [edges](graph-theory.md#edge-of-a-graph) survive.

This hierarchy supports [structural recursion](computer-science.md#structural-recursion): process the smaller [rooted trees](#rooted-tree) below each [vertex](graph.md#vertex-graph-theory), then combine their results. A [depth-first traversal of a tree](#depth-first-traversal-of-a-tree) explores one branch before returning; [breadth-first search](#breadth-first-search) processes successive levels. The [lowest common ancestor](#lowest-common-ancestor) identifies where two routes from the [root of a tree](#root-of-a-tree) last coincide. For $4,5$ it is $2$ when $r=1$. A [binary tree](computer-science.md#binary-tree) imposes an additional restriction on [children in a rooted tree](#child-in-a-rooted-tree); a general [rooted tree](#rooted-tree) has no such bound.

#### Root of a tree

↑ **Parent:** [Rooted tree](#rooted-tree)

The distinguished [vertex](graph.md#vertex-graph-theory) that specifies a [rooted tree](#rooted-tree). Its choice determines the [parent in a rooted tree](#parent-in-a-rooted-tree) and [children in a rooted tree](#child-in-a-rooted-tree) relationships.

#### Parent in a rooted tree

↑ **Parent:** [Rooted tree](#rooted-tree)

For a nonroot [vertex](graph.md#vertex-graph-theory), its adjacent predecessor on the unique [graph path](graph-theory.md#path-in-a-graph) from the [root of a tree](#root-of-a-tree). The [root of a tree](#root-of-a-tree) has no parent.

#### Child in a rooted tree

↑ **Parent:** [Rooted tree](#rooted-tree)

A [vertex](graph.md#vertex-graph-theory) whose [parent in a rooted tree](#parent-in-a-rooted-tree) is the specified [vertex](graph.md#vertex-graph-theory).

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

A [forest](#forest) is an [undirected graph](graph-theory.md#undirected-graph) with no [graph cycle](graph-theory.md#cycle-in-a-graph); each of its [connected components of a graph](graph.md#component-graph-theory) is a [tree](#tree-graph-theory), including any isolated [vertex](graph.md#vertex-graph-theory). A finite [forest](#forest) with $n$ [vertices](graph.md#vertex-graph-theory) and $c$ [connected components of a graph](graph.md#component-graph-theory) has

$$
|E|=n-c.
$$

Indeed, a [connected component of a graph](graph.md#component-graph-theory) with $n_i$ [vertices](graph.md#vertex-graph-theory) contributes $n_i-1$ [edges](graph-theory.md#edge-of-a-graph); adding these counts gives $n-c$. Equivalently, start with $n$ isolated [vertices](graph.md#vertex-graph-theory): every added [edge](graph-theory.md#edge-of-a-graph) must join different [connected components of a graph](graph.md#component-graph-theory), reducing their number by one. Joining [vertices](graph.md#vertex-graph-theory) already connected would create a [graph cycle](graph-theory.md#cycle-in-a-graph). [MIT, counting notes, p. 4: building forests by merging components](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec05-06.pdf)

Deleting $13$ in our example gives $n=7$, $c=2$, and five [edges](graph-theory.md#edge-of-a-graph): the two [trees](#tree-graph-theory) contribute $3+2=5=7-2$. Deleting $67$ as well leaves $7$ isolated, so $c=3$ and four [edges](graph-theory.md#edge-of-a-graph). A [forest](#forest) therefore describes separate hierarchies or the intermediate stages of building a [spanning tree](#spanning-tree). The [acyclic graph](#forest) condition accounts for missing connections without assuming that all locations are mutually reachable.

#### Two-component spanning forest

↑ **Parent:** [Forest](#forest)

A [two-component spanning forest](#two-component-spanning-forest) of a finite connected [graph](graph.md) is an acyclic spanning subgraph with exactly two [connected components of a graph](graph.md#component-graph-theory). It has $|V|-2$ [edges](graph-theory.md#edge-of-a-graph). For distinct terminals $a,z$, a separating two-component forest places them in different components. Deleting an [edge](graph-theory.md#edge-of-a-graph) of the $a$-to-$z$ [graph path](graph-theory.md#path-in-a-graph) of a [spanning tree](#spanning-tree) produces such a forest; adjoining any original [edge](graph-theory.md#edge-of-a-graph) across its cut reverses this operation. This is the counting correspondence behind the [mean spanning-tree path current](#mean-spanning-tree-path-current).

### Spanning tree

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spanning_tree)

A [spanning tree](#spanning-tree) of a [connected graph](graph.md#connected-graph) $G$ is a [subgraph](graph-theory.md#subgraph) that is a [tree](#tree-graph-theory) and contains every [vertex](graph.md#vertex-graph-theory) of $G$. Its [edges](graph-theory.md#edge-of-a-graph) must come from $G$. For finite $G$ on $n$ [vertices](graph.md#vertex-graph-theory), every [spanning tree](#spanning-tree) has $n-1$ [edges](graph-theory.md#edge-of-a-graph), the minimum possible number preserving [reachability](graph.md#reachability-in-a-graph) between all locations. This makes a [spanning tree](#spanning-tree) a compact certificate that the original [graph](graph.md) is connected. A [minimum spanning tree](#minimum-spanning-tree) additionally minimizes a specified total [edge](graph-theory.md#edge-of-a-graph) weight; merely selecting a [spanning tree](#spanning-tree) supplies no such optimization. [MIT, Mathematics for Computer Science, sections 11.10.3–11.10.4](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/mit6_042js15_textbook.pdf)

Let $G$ be our seven-[vertex](graph.md#vertex-graph-theory) [tree](#tree-graph-theory) with [edge](graph-theory.md#edge-of-a-graph) $57$ added. It has seven [edges](graph-theory.md#edge-of-a-graph) and a [graph cycle](graph-theory.md#cycle-in-a-graph). Removing $57$ gives the original [spanning tree](#spanning-tree) $T$; removing $13$ instead gives another [spanning tree](#spanning-tree) $T'$. Both retain all seven [vertices](graph.md#vertex-graph-theory) and six [edges](graph-theory.md#edge-of-a-graph), but their [graph distances](graph-theory.md#distance-graph-theory) differ: $d_G(5,7)=1$, whereas $d_T(5,7)=5$. In $T'$, $d_{T'}(5,7)=1$ but $d_{T'}(1,3)=5$, along $1,2,5,7,6,3$, compared with $d_G(1,3)=1$. Preserving [reachability](graph.md#reachability-in-a-graph) permits longer journeys; [breadth-first search](#breadth-first-search) can preserve [graph distances](graph-theory.md#distance-graph-theory) from one chosen starting [vertex](graph.md#vertex-graph-theory).

<a id="image-two-spanning-trees-preserve-reachability-but-change-different-graph-distances"></a>
![](spanning-tree-cycle-exchange.png)

**[Figure 10](#image-two-spanning-trees-preserve-reachability-but-change-different-graph-distances). Two spanning trees preserve reachability but change different graph distances**.

To construct a [spanning tree](#spanning-tree), repeatedly delete any [edge](graph-theory.md#edge-of-a-graph) on a [graph cycle](graph-theory.md#cycle-in-a-graph). Its endpoints remain joined through the rest of that [graph cycle](graph-theory.md#cycle-in-a-graph), so the deletion preserves connectedness. Finiteness ensures that this stops at a connected [acyclic graph](#forest). Conversely, adding an omitted [edge](graph-theory.md#edge-of-a-graph) to a [spanning tree](#spanning-tree) creates its unique [fundamental cycle](#fundamental-cycle); deleting any other [edge](graph-theory.md#edge-of-a-graph) on that [graph cycle](graph-theory.md#cycle-in-a-graph) produces another [spanning tree](#spanning-tree). The displayed exchange replaces $13$ by $57$. [Trinity College Dublin, section 4.16: deleting cycle edges preserves connectivity](https://www.maths.tcd.ie/~dwilkins/Courses/MA2C03/MA2C03Courseware_2014to15/MA2C03_S4_Yr1415.pdf)

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

For an integer $n\geq2$, let $\mathcal T_n$ be the set of [labelled trees](#labelled-tree) with fixed [vertex set](graph.md#vertex-set) $\{1,\ldots,n\}$. Each [tree](#tree-graph-theory) is a finite [simple graph](graph.md#simple-graph), with no distinguished [root of a tree](#root-of-a-tree), and two [trees](#tree-graph-theory) are different exactly when their sets of [edges](graph-theory.md#edge-of-a-graph) differ. Then

$$
|\mathcal T_n|=n^{n-2}.
$$

Equivalently, this is the number of [spanning trees](#spanning-tree) of the [complete graph](graph-theory.md#complete-graph) $K_n$. The [labelled combinatorial structure](#labelled-combinatorial-structure) includes the fixed labels: drawings, positions, and the order in which [edges](graph-theory.md#edge-of-a-graph) are listed do not create extra [trees](#tree-graph-theory). For $n=1$, the single [vertex](graph.md#vertex-graph-theory) with no [edges](graph-theory.md#edge-of-a-graph) is the unique [tree](#tree-graph-theory); count it separately, since the [Prüfer sequence](#prufer-sequence) construction requires $n\geq2$. For $n=2$, the unique [tree](#tree-graph-theory) has [edge](graph-theory.md#edge-of-a-graph) $\{1,2\}$ and corresponds to the empty [Prüfer sequence](#prufer-sequence). [Peter Magyar, Michigan State University, Math 481: Cayley's theorem and inverse Prüfer transformations](https://users.math.msu.edu/users/magyarp/math481/)

For four fixed labels, there are $4^2=16$ [labelled trees](#labelled-tree), but only two [unlabelled trees](#unlabelled-tree): the [star graph](graph-theory.md#star-graph-theory) and the [path graph](graph-theory.md#path-graph). There are four [star graphs](graph-theory.md#star-graph-theory), one for each choice of centre. There are $4!/2=12$ [path graphs](graph-theory.md#path-graph): arrange the labels along a [graph path](graph-theory.md#path-in-a-graph), then identify each ordering with its reversal, which describes the same set of [edges](graph-theory.md#edge-of-a-graph). Thus $4+12=16$. For instance, [star graphs](graph-theory.md#star-graph-theory) centred at $1$ and at $2$ have different sets of [edges](graph-theory.md#edge-of-a-graph) even though they have the same shape.

<a id="image-all-sixteen-labelled-trees-on-four-fixed-vertices-four-star-graphs-and-twelve-path-graphs-each-with-its-prufer-sequence"></a>
![](labelled-trees-on-four-vertices.png)

**[Figure 11](#image-all-sixteen-labelled-trees-on-four-fixed-vertices-four-star-graphs-and-twelve-path-graphs-each-with-its-prufer-sequence). All sixteen labelled trees on four fixed vertices: four star graphs and twelve path graphs, each with its Prüfer sequence**.

The striking point is that connectedness and the absence of a [graph cycle](graph-theory.md#cycle-in-a-graph) are global restrictions on [edges](graph-theory.md#edge-of-a-graph), yet the answer is a power with no correction factor. The [Prüfer sequence](#prufer-sequence) supplies a [bijection](function.md#bijection) that turns those restrictions into $n-2$ freely chosen labels. The [rule of product](#rule-of-product) then gives $n^{n-2}$ immediately. The same representation makes [vertex degrees](graph-theory.md#degree-graph-theory) easy to count and supports [uniform labelled tree generation](#uniform-labelled-tree-generation) for simulations and algorithm experiments.

Arthur Cayley's 1889 paper "A theorem on trees", published in the Quarterly Journal of Pure and Applied Mathematics, volume 23, pages 376–378, treats the counting problem and its refinement by [vertex degrees](graph-theory.md#degree-graph-theory). It was reprinted as paper 895 in volume XIII of his Collected Mathematical Papers, pages 26–28. This publication is the historical context for the name [Cayley's formula](#cayley-s-formula); the name alone is not a claim of priority. [Cayley, A theorem on trees (1889), original journal volume, pages 376–378](https://gdz.sub.uni-goettingen.de/id/PPN600494829_0023) [Cayley, A theorem on trees, collected-paper reprint and publisher's first-page preview](https://doi.org/10.1017/CBO9780511703799.010)

#### Labelled forest count with prescribed roots

↑ **Parent:** [Cayley's formula](#cayley-s-formula)

For a fixed set of $k<n$ roots among $n$ labelled [vertices](graph.md#vertex-graph-theory), the number of [forests](#forest) with exactly one root in each [graph component](graph.md#component-graph-theory) is $kn^{n-k-1}$. Orient edges toward their roots. Repeatedly remove the smallest nonroot leaf and record its parent. This gives a code of length $n-k$ whose last entry is a root. Conversely, for any such code choose the smallest remaining nonroot absent from the remaining code, join it to the first entry, and delete it. There is always a choice because the final entry is a root. These inverse operations give $n^{n-k-1}$ choices for the earlier entries and $k$ for the last. For $k=n$, the empty forest is unique.

<h4 id="prufer-sequence">Prüfer sequence</h4>

↑ **Parent:** [Cayley's formula](#cayley-s-formula)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prüfer_sequence)

For $n\geq2$, a [Prüfer sequence](#prufer-sequence) is the encoding of a [labelled tree](#labelled-tree) on $\{1,\ldots,n\}$ by a [sequence](real-analysis.md#sequence)

$$
p=(p_1,\ldots,p_{n-2})\in\{1,\ldots,n\}^{n-2}.
$$

Repeated labels are allowed, and their order matters. To encode the [tree](#tree-graph-theory), repeatedly remove its smallest-labelled [leaf of a graph](graph-theory.md#leaf-of-a-graph) together with its incident [edge](graph-theory.md#edge-of-a-graph), recording the label of its unique neighbour. Stop when two [vertices](graph.md#vertex-graph-theory) remain; do not record their final [edge](graph-theory.md#edge-of-a-graph). Removing a [leaf of a graph](graph-theory.md#leaf-of-a-graph) leaves a [tree](#tree-graph-theory), so the procedure makes exactly $n-2$ deletions. The choice of the smallest label makes the encoding deterministic. [Peter Magyar, Math 481: Prüfer encoding with the smallest leaf](https://users.math.msu.edu/users/magyarp/math481/)

For a concrete example, take six [vertices](graph.md#vertex-graph-theory) and the set of [edges](graph-theory.md#edge-of-a-graph)

$$
E=\bigl\{\{1,2\},\{1,3\},\{3,4\},\{3,5\},\{5,6\}\bigr\}.
$$

Initially $2,4,6$ label the [vertices](graph.md#vertex-graph-theory) of [vertex degree](graph-theory.md#degree-graph-theory) one. Remove $2$ and record its neighbour $1$. Now $1$ has become a [leaf of a graph](graph-theory.md#leaf-of-a-graph), so remove $1$ and record $3$. Next remove $4$ and record $3$ again; then remove $3$ and record $5$. The final [edge](graph-theory.md#edge-of-a-graph) joins $5$ and $6$. Thus the [Prüfer sequence](#prufer-sequence) is

$$
p=(1,3,3,5).
$$

The deletion order is $2,1,4,3$: removing a [leaf of a graph](graph-theory.md#leaf-of-a-graph) can make its neighbour a [leaf of a graph](graph-theory.md#leaf-of-a-graph), so the eligible labels change as the [tree](#tree-graph-theory) shrinks.

<a id="image-encoding-a-six-vertex-tree-as-the-prufer-sequence-1-3-3-5-then-reconstructing-its-five-edges"></a>
![](pruefer-tree-encoding.png)

**[Figure 12](#image-encoding-a-six-vertex-tree-as-the-prufer-sequence-1-3-3-5-then-reconstructing-its-five-edges). Encoding a six-vertex tree as the Prüfer sequence $(1,3,3,5)$, then reconstructing its five edges**.

To decode, keep a set $L$ of remaining labels, initially $\{1,\ldots,n\}$, and the remaining [sequence](real-analysis.md#sequence), initially $p$. While the [sequence](real-analysis.md#sequence) is nonempty, let $v$ be the smallest label in $L$ absent from the entire remaining [sequence](real-analysis.md#sequence). Add an [edge](graph-theory.md#edge-of-a-graph) between $v$ and its first entry, then remove $v$ from $L$ and delete that first entry. Finally join the two labels left in $L$. For the example:

| Remaining [sequence](real-analysis.md#sequence) before the step | Smallest absent remaining label | [Edge](graph-theory.md#edge-of-a-graph) added |
| --- | --- | --- |
| $(1,3,3,5)$ | $2$ | $\{2,1\}$ |
| $(3,3,5)$ | $1$ | $\{1,3\}$ |
| $(3,5)$ | $4$ | $\{4,3\}$ |
| $(5)$ | $3$ | $\{3,5\}$ |
| Empty; $L=\{5,6\}$ | Final pair | $\{5,6\}$ |

The decoder always has a choice: if the remaining [sequence](real-analysis.md#sequence) has length $m$, then $L$ has $m+2$ labels, so at least two of them are absent. Its first entry is still in $L$, and differs from the chosen absent label. Every removed [vertex](graph.md#vertex-graph-theory) attaches to a [vertex](graph.md#vertex-graph-theory) that survives longer; following these attachments eventually reaches the final pair. Consequently the decoded [graph](graph.md) is connected, and its $n-1$ [edges](graph-theory.md#edge-of-a-graph) make it a [tree](#tree-graph-theory). In this construction, each occurrence of $v$ contributes an incident [edge](graph-theory.md#edge-of-a-graph), and $v$ gets one more [edge](graph-theory.md#edge-of-a-graph) at its final attachment. Thus a remaining label is absent from the remaining [sequence](real-analysis.md#sequence) exactly when it labels a [leaf of a graph](graph-theory.md#leaf-of-a-graph). Encoding and decoding choose the same smallest label at each step and undo each other. This [bijection](function.md#bijection) proves [Cayley's formula](#cayley-s-formula) and explains why every freely chosen [sequence](real-analysis.md#sequence) is valid. [Columbia University, Graph Theory Lecture 4: Prüfer degree identity, decoding algorithm, and bijection](https://www.cs.columbia.edu/~cs4203/files/GT-Lec4.pdf)

For $n=2$ there is exactly one empty [sequence](real-analysis.md#sequence), and decoding adds the sole [edge](graph-theory.md#edge-of-a-graph). For $n=1$ there is one [tree](#tree-graph-theory), with [vertex degree](graph-theory.md#degree-graph-theory) zero, but no length-$n-2$ [Prüfer sequence](#prufer-sequence). This is the exception both to the encoding convention and to the [Prüfer degree formula](#prufer-degree-formula).

Heinz Prüfer's 1918 paper "Neuer Beweis eines Satzes über Permutationen" appeared in Archiv der Mathematik und Physik, third series, volume 27, pages 142–144. It gives an encoding proof of the labelled [tree](#tree-graph-theory) count. The historical title means "New proof of a theorem on permutations"; the modern [Prüfer sequence](#prufer-sequence) permits repeated labels, so it is not a [permutation](#permutation). [Prüfer (1918), original opening-page scan, page 142](https://i.sstatic.net/WDvxyMwX.png)

<h5 id="prufer-degree-formula">Prüfer degree formula</h5>

↑ **Parent:** [Prüfer sequence](#prufer-sequence)

For a [labelled tree](#labelled-tree) with $n\geq2$ [vertices](graph.md#vertex-graph-theory), the [vertex degree](graph-theory.md#degree-graph-theory) of label $v$ is one plus the number of occurrences of $v$ in its [Prüfer sequence](#prufer-sequence):

$$
\deg_T(v)=1+\#\{i:p_i=v\}.
$$

Each recording of $v$ corresponds to an incident [edge](graph-theory.md#edge-of-a-graph) removed when a neighbouring [leaf of a graph](graph-theory.md#leaf-of-a-graph) is deleted. Exactly one incident [edge](graph-theory.md#edge-of-a-graph) remains when $v$ itself is deleted, or when it belongs to the final pair. In particular, $v$ is a [leaf of a graph](graph-theory.md#leaf-of-a-graph) exactly when it never occurs in the [Prüfer sequence](#prufer-sequence). The same reasoning applies to each remaining [tree](#tree-graph-theory) and its remaining code. [Columbia University, Graph Theory Lecture 4, Proposition 7.1: degree equals occurrences plus one](https://www.cs.columbia.edu/~cs4203/files/GT-Lec4.pdf)

For $p=(1,3,3,5)$, the occurrence counts in label order are $(1,0,2,0,1,0)$, giving the [degree sequence](graph-theory.md#degree-sequence) $(2,1,3,1,2,1)$. Its sum is $10=2(6-1)$, as required by the [degree-sum formula](#degree-sum-formula). More generally, summing the occurrence counts gives $n-2$, so summing the [vertex degrees](graph-theory.md#degree-graph-theory) gives $n+(n-2)=2(n-1)$.

###### Labelled tree count with prescribed degrees

↑ **Parent:** [Prüfer degree formula](#prufer-degree-formula)

For $n\geq2$ and positive integers $d_1,\ldots,d_n$ with $\sum_v d_v=2(n-1)$, the number of [labelled trees](#labelled-tree) having [vertex degree](graph-theory.md#degree-graph-theory) $d_v$ at label $v$ is

$$
\frac{(n-2)!}{\prod_{v=1}^n(d_v-1)!}.
$$

By the [Prüfer degree formula](#prufer-degree-formula), this is the [multinomial coefficient](#multinomial-coefficient) counting [sequences](real-analysis.md#sequence) with $d_v-1$ occurrences of each label. If a degree is zero or the sum is wrong, there are no such [trees](#tree-graph-theory). For the example [degree sequence](graph-theory.md#degree-sequence) $(2,1,3,1,2,1)$, there are $4!/(1!0!2!0!1!0!)=12$ [labelled trees](#labelled-tree), one for each ordering of the labels $1,3,3,5$. Knowing the [vertex degrees](graph-theory.md#degree-graph-theory) thus constrains, but usually does not determine, the [tree](#tree-graph-theory).

##### Uniform labelled tree generation

↑ **Parent:** [Prüfer sequence](#prufer-sequence)

For $n\geq2$, choose $n-2$ [independent random variables](random-variable.md#independent-random-variables), each with the [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution) $\{1,\ldots,n\}$, and decode their values as a [Prüfer sequence](#prufer-sequence). Every [sequence](real-analysis.md#sequence) has [probability](probability-theory.md#probability) $n^{-(n-2)}$, and the [bijection](function.md#bijection) gives each [labelled tree](#labelled-tree) the same [probability](probability-theory.md#probability). This produces a [uniform spanning tree](#uniform-spanning-tree) of the [complete graph](graph-theory.md#complete-graph) without repeatedly proposing sets of [edges](graph-theory.md#edge-of-a-graph) and rejecting those that fail to be [trees](#tree-graph-theory). It supplies random inputs for testing implementations of [breadth-first search](#breadth-first-search) and a tractable model of random connections. [Doron Zeilberger, Rutgers Math 454 (2020), Lecture 23: generate random labelled trees by sampling and inverting Prüfer codes](https://sites.math.rutgers.edu/~zeilberg/Combo20/hw.html)

This distribution is uniform over fixed-label [trees](#tree-graph-theory), rather than over [unlabelled trees](#unlabelled-tree). With four labels, the [star graph](graph-theory.md#star-graph-theory) shape has [probability](probability-theory.md#probability) $4/16=1/4$ and the [path graph](graph-theory.md#path-graph) shape has [probability](probability-theory.md#probability) $12/16=3/4$. Also, for a fixed label $v$, the [Prüfer degree formula](#prufer-degree-formula) gives

$$
\deg_T(v)-1\sim\operatorname{Binomial}(n-2,1/n),
\qquad
\mathbb E[\deg_T(v)]=1+\frac{n-2}{n}=2-\frac2n.
$$

Here the [binomial distribution](discrete-probability-distribution.md#binomial-distribution) counts the [independent](random-variable.md#independent-random-variables) code positions equal to $v$. The [expected value](probability-theory.md#expected-value) agrees with the average [vertex degree](graph-theory.md#degree-graph-theory) from the [degree-sum formula](#degree-sum-formula). Individual labels have the same distribution by symmetry, though their [vertex degrees](graph-theory.md#degree-graph-theory) are constrained together by their fixed sum. When $n=1$, simply return the single isolated [vertex](graph.md#vertex-graph-theory).

<h3 id="konig-s-lemma">Kőnig's lemma</h3>

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kőnig's_lemma)

Every infinite finitely branching rooted tree has an infinite branch. Starting at the root, repeatedly choose a child above which infinitely many vertices remain.

### Breadth-first search

↑ **Parent:** [Tree (graph theory)](#tree-graph-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Breadth-first_search)

[Breadth-first search](#breadth-first-search) is a [graph search](graph.md#graph-search) that explores successive layers of [graph distance](graph-theory.md#distance-graph-theory) from a starting [vertex](graph.md#vertex-graph-theory) $s$. Here the [graph](graph.md) is an [undirected graph](graph-theory.md#undirected-graph) on a [finite set](set.md#finite-set) of [vertices](graph.md#vertex-graph-theory), and distance counts [edges](graph-theory.md#edge-of-a-graph), with no differing [edge](graph-theory.md#edge-of-a-graph) weights. Mark $s$ as discovered, assign $d(s)=0$, and place it in a [FIFO queue](computer-science.md#fifo-queue). Repeatedly remove the front [vertex](graph.md#vertex-graph-theory) $u$ and scan its [adjacency list](computer-science.md#adjacency-list). Whenever a [graph neighbour](graph-theory.md#neighbour-of-a-vertex) $v$ is still undiscovered, mark it immediately, record $u$ as its [parent in a rooted tree](#parent-in-a-rooted-tree) in the discovery [tree](#tree-graph-theory), assign $d(v)=d(u)+1$, and enqueue $v$ at the rear. Marking on insertion ensures that another [edge](graph-theory.md#edge-of-a-graph) cannot enqueue the same [vertex](graph.md#vertex-graph-theory) again. [Sedgewick and Wayne, Algorithms: BreadthFirstPaths queue and discovery rule](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/BreadthFirstPaths.java)

Use the same [undirected graph](graph-theory.md#undirected-graph) as [depth-first search](computer-science.md#depth-first-search), with [vertex set](graph.md#vertex-set) $V=\{A,B,C,D,E,F,G\}$ and [edges](graph-theory.md#edge-of-a-graph)

$$
E=\{AB,AC,BD,BE,CE,CF,EG,FG\},
$$

where $XY$ denotes the unordered pair $\{X,Y\}$. Start at $A$ and scan [graph neighbours](graph-theory.md#neighbour-of-a-vertex) in [lexicographic order](extremal-set-theory.md#lexicographic-order) of their one-letter labels. The diagram's generator computes the following layers and the [parent in a rooted tree](#parent-in-a-rooted-tree) assigned to each discovered [vertex](graph.md#vertex-graph-theory); the source is the [root of a tree](#root-of-a-tree) and has no [parent in a rooted tree](#parent-in-a-rooted-tree).

| [Graph distance](graph-theory.md#distance-graph-theory) from $A$ | [Vertices](graph.md#vertex-graph-theory) in discovery order | [Parent in a rooted tree](#parent-in-a-rooted-tree) in the same order |
| --- | --- | --- |
| $0$ | $A$ | none |
| $1$ | $B,C$ | $A,A$ |
| $2$ | $D,E,F$ | $B,B,C$ |
| $3$ | $G$ | $E$ |

<a id="image-breadth-first-search-graph-distance-layers-and-two-ordered-fifo-queue-snapshots"></a>
![](breadth-first-search-layers.png)

**[Figure 13](#image-breadth-first-search-graph-distance-layers-and-two-ordered-fifo-queue-snapshots). Breadth-first search: graph distance layers and two ordered FIFO queue snapshots**. Solid [edges](graph-theory.md#edge-of-a-graph) record first discovery; dashed [edges](graph-theory.md#edge-of-a-graph) are still present in the original [graph](graph.md). The [FIFO queue](computer-science.md#fifo-queue) contains $C,D,E$ after processing $B$ and $F,G$ after processing $E$, with its front on the left. Colors encode [graph distance](graph-theory.md#distance-graph-theory) in the [graph](graph.md) without [edge](graph-theory.md#edge-of-a-graph) weights.

The discovery and removal orders both happen to be $A,B,C,D,E,F,G$. After processing $B$, the [FIFO queue](computer-science.md#fifo-queue) is $C,D,E$: $C$ must be processed before the newer $D,E$. Processing $C$ then skips the already discovered $E$ and enqueues $F$, giving $D,E,F$. Processing $D$ adds nothing. Processing $E$ discovers $G$, giving $F,G$; later $F$ sees $G$ already marked and leaves its [parent in a rooted tree](#parent-in-a-rooted-tree) unchanged. The discovery [edges](graph-theory.md#edge-of-a-graph) are $AB,AC,BD,BE,CF,EG$, forming a [rooted tree](#rooted-tree) on all seven [vertices](graph.md#vertex-graph-theory) even though the original [graph](graph.md) contains [graph cycles](graph-theory.md#cycle-in-a-graph). The discovery [tree](#tree-graph-theory) contains six [edges](graph-theory.md#edge-of-a-graph); it need not contain every examined [edge](graph-theory.md#edge-of-a-graph).

First arrival is shortest because the [FIFO queue](computer-science.md#fifo-queue) keeps assigned distances in nondecreasing order, with entries from at most two consecutive layers. While processing distance $k$, newly discovered [vertices](graph.md#vertex-graph-theory) receive distance $k+1$ and join the rear. If an undiscovered [vertex](graph.md#vertex-graph-theory) had a shorter [graph path](graph-theory.md#path-in-a-graph), its preceding [vertex](graph.md#vertex-graph-theory) on that [graph path](graph-theory.md#path-in-a-graph) would lie in an earlier layer and would already have discovered it. Thus $d(v)$ is the minimum number of [edges](graph-theory.md#edge-of-a-graph) from $s$ to $v$. This is a [mathematical induction](foundations-of-mathematics.md#mathematical-induction) over the layers, not an assumption about the drawing. Following the [parent in a rooted tree](#parent-in-a-rooted-tree) backwards at each step gives $G,E,B,A$; reverse that [sequence](real-analysis.md#sequence) to obtain the three-[edge](graph-theory.md#edge-of-a-graph) [graph path](graph-theory.md#path-in-a-graph) $A,B,E,G$. $A,C,F,G$ is another shortest [graph path](graph-theory.md#path-in-a-graph), but the specified [graph neighbour](graph-theory.md#neighbour-of-a-vertex) order makes $E$ discover $G$ first. Changing that order can change the [parent in a rooted tree](#parent-in-a-rooted-tree) without changing [graph distances](graph-theory.md#distance-graph-theory). [MIT 6.006, lecture 13: distance layers and shortest paths, pp. 4–6](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/1208e162775f6f5cedfbb9f2b694ede0_MIT6_006F11_lec13.pdf)

The shortest-route guarantee concerns the [shortest path problem](graph-theory.md#shortest-path-problem) measured by [edge](graph-theory.md#edge-of-a-graph) count. It also minimizes total cost when every [edge](graph-theory.md#edge-of-a-graph) has the same positive cost. With unequal [edge](graph-theory.md#edge-of-a-graph) weights, first discovery need not minimize total cost; nonnegative costs can instead be handled by the [Dijkstra algorithm](graph-theory.md#dijkstra-algorithm). [Breadth-first search](#breadth-first-search) is useful for minimum-hop routes and for finding all [vertices](graph.md#vertex-graph-theory) within a specified [graph distance](graph-theory.md#distance-graph-theory). Its [FIFO queue](computer-science.md#fifo-queue) finishes an older layer before the next one, whereas [depth-first search](computer-science.md#depth-first-search) uses a [call stack](computer-science.md#call-stack) or explicit [LIFO stack](computer-science.md#stack-data-structure) to pursue one branch immediately.

With [adjacency lists](computer-science.md#adjacency-list) and constant-cost discovery checks, together with constant worst-case or [amortized analysis](computer-science.md#amortized-analysis) cost for [FIFO queue](computer-science.md#fifo-queue) insertion and removal, the [time complexity](computer-science.md#time-complexity) is $O(|V|+|E|)$ in [Big O notation](real-analysis.md#big-o-notation). Every reached [vertex](graph.md#vertex-graph-theory) is enqueued and removed once, each incident [edge](graph-theory.md#edge-of-a-graph) is scanned at most twice in an [undirected graph](graph-theory.md#undirected-graph), and initializing all marks and distances takes $O(|V|)$. The [FIFO queue](computer-science.md#fifo-queue) contains at most $|V|$ [vertices](graph.md#vertex-graph-theory); the example's maximum is three. Discovery marks, distances and the recorded [parent in a rooted tree](#parent-in-a-rooted-tree) for each nonroot [vertex](graph.md#vertex-graph-theory) also give $O(|V|)$ auxiliary [space complexity](computer-science.md#space-complexity), excluding the [graph](graph.md). An [array](computer-science.md#array-data-structure) that shifts every entry on front removal can lose the linear [time complexity](computer-science.md#time-complexity); the [FIFO queue](computer-science.md#fifo-queue) abstraction alone does not make removal constant-cost. Ordering the [adjacency lists](computer-science.md#adjacency-list) is a separate preprocessing cost.

A single start reaches only its [connected component of a graph](graph.md#component-graph-theory). Unreached [vertices](graph.md#vertex-graph-theory) retain distance $\infty$ and have no recorded [parent in a rooted tree](#parent-in-a-rooted-tree). Restarting at each still-undiscovered [vertex](graph.md#vertex-graph-theory), while preserving all discovery marks, produces a [forest](#forest) covering the [graph](graph.md); each new [root of a tree](#root-of-a-tree) gets distance zero, so these distances refer to that [root of a tree](#root-of-a-tree), not to the original $s$.

## Double counting (proof technique)

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double_counting_(proof_technique))

Double counting establishes an identity by computing the [cardinality](set-theory.md#cardinality) of the same [finite set](set.md#finite-set) in two ways. The useful step is to identify exactly what the members of that collection are; an algebraic equality then records two legitimate ways to organize them.

Take the [ordered pairs](set.md#ordered-pair) $(S,x)$ where $S$ is a $k$-element [subset](set.md#subset) of an $n$-element [set](set.md) and $x\in S$ is marked. Choosing $S$ first gives $k\binom nk$ pairs. Choosing $x$ first leaves $k-1$ members to choose from the other $n-1$, giving $n\binom{n-1}{k-1}$. Hence

$$
k\binom nk=n\binom{n-1}{k-1}\qquad(1\leq k\leq n).
$$

For five people and two-person teams, both counts give $20$: ten teams with two choices of a marked member, or five choices of that member with four choices of a teammate. The identity is explained by the [bijection](function.md#bijection) between these descriptions, rather than merely verified through [factorials](#factorial).

## Set partition

↑ **Parent:** [Combinatorics](combinatorics.md)

A [set partition](#set-partition) of a [finite set](set.md#finite-set) $X$ is a [set](set.md) $\pi=\{B_1,\ldots,B_k\}$ of nonempty [subsets](set.md#subset), called [blocks of a set partition](#block-of-a-set-partition), with

$$
B_i\ne\varnothing,\qquad B_i\cap B_j=\varnothing\quad(i\ne j),\qquad \bigcup_{i=1}^k B_i=X.
$$

Thus every [set element](set.md#element-of-a-set) of $X$ belongs to exactly one [block of a set partition](#block-of-a-set-partition). This is the finite counting version of a [partition of a set](set.md#partition-of-a-set). The [blocks of a set partition](#block-of-a-set-partition) are **unlabelled**: their subscripts help describe them, but give them no roles or order. Stanley uses this definition in his classification of counting problems.[section 1.9: set partitions and their blocks](mathematics-bibliography.md#enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley)

**All possibilities for three elements.** The [set](set.md) $\{1,2,3\}$ has exactly five [set partitions](#set-partition):

$$
\begin{gathered}
\{\{1,2,3\}\},\\
\{\{1,2\},\{3\}\},\quad \{\{1,3\},\{2\}\},\quad \{\{1\},\{2,3\}\},\\
\{\{1\},\{2\},\{3\}\}.
\end{gathered}
$$

For two [blocks of a set partition](#block-of-a-set-partition), one must have size two and the other size one; the three choices of the lone element give the middle row. One [block of a set partition](#block-of-a-set-partition) forces the whole [set](set.md), and three [blocks of a set partition](#block-of-a-set-partition) force three [singleton sets](set.md#singleton-mathematics). This proves the enumeration complete, with counts $1,3,1$ by number of [blocks of a set partition](#block-of-a-set-partition). Their [sum](arithmetic.md#sum) is the [Bell number](#bell-number) $B_3=5$.

<a id="image-exact-enumeration-of-the-five-set-partitions-of-1-2-3-outlines-show-blocks-of-a-set-partition-whose-positions-and-colours-carry-no-labels"></a>
![](set-partitions-stirling-three-elements.png)

**[Figure 14](#image-exact-enumeration-of-the-five-set-partitions-of-1-2-3-outlines-show-blocks-of-a-set-partition-whose-positions-and-colours-carry-no-labels). Exact enumeration of the five set partitions of $\{1,2,3\}$: outlines show blocks of a set partition, whose positions and colours carry no labels**.

**What information is kept?** Exchanging the two [blocks of a set partition](#block-of-a-set-partition) in $\{\{1,2\},\{3\}\}$ leaves the same [set partition](#set-partition); writing the [tuple](set-theory.md#finite-tuple) $(\{1,2\},\{3\})$ instead makes an ordered list, different from $(\{3\},\{1,2\})$. Exchanging elements within a [block of a set partition](#block-of-a-set-partition) also changes nothing. In contrast, $\{\{1,3\},\{2\}\}$ is a different [set partition](#set-partition), because the actual memberships differ. Both have the same [integer partition](#integer-partition) $2+1$ of sizes. An [integer partition](#integer-partition), or its [Ferrers diagram](#ferrers-diagram), forgets which distinct objects were grouped together.

For four named people, $\{\{1,2\},\{3,4\}\}$ and $\{\{1,3\},\{2,4\}\}$ therefore describe different ways of making two unnamed teams, although both have sizes $2+2$. If every team must have exactly two people, only three [set partitions](#set-partition) qualify; if any nonempty team sizes are permitted, the [Stirling number of the second kind](#stirling-numbers-of-the-second-kind) $S(4,2)=7$ counts them. Naming the teams changes the counting problem again.

A [set partition](#set-partition) is useful whenever membership matters but category names do not. Define $x\sim y$ when $x$ and $y$ belong to the same [block of a set partition](#block-of-a-set-partition). This is an [equivalence relation](set-theory.md#equivalence-relation), and its [equivalence classes](set-theory.md#equivalence-class) recover the [set partition](#set-partition). Conversely, an [equivalence relation](set-theory.md#equivalence-relation) supplies its [set partition](#set-partition) of [equivalence classes](set-theory.md#equivalence-class). The beautiful simplification is that one grouping can be described by whole [subsets](set.md#subset) or by a rule comparing two elements. Additional distinctions are organized by [refinement of a set partition](#refinement-of-a-set-partition).

The [empty set](set.md#empty-set) has one [set partition](#set-partition), the empty collection $\pi=\varnothing$, with zero [blocks of a set partition](#block-of-a-set-partition). This differs from $\{\varnothing\}$, which is forbidden because its proposed [block of a set partition](#block-of-a-set-partition) is empty.

### Block of a set partition

↑ **Parent:** [Set partition](#set-partition)

A [block of a set partition](#block-of-a-set-partition) is one of its nonempty [subsets](set.md#subset). Distinct [blocks of a set partition](#block-of-a-set-partition) have empty [intersection](set.md#set-intersection), and their [union](set.md#set-union) is the original [set](set.md). For $\pi=\{\{1,3\},\{2\}\}$, the [blocks of a set partition](#block-of-a-set-partition) are $\{1,3\}$ and the [singleton set](set.md#singleton-mathematics) $\{2\}$. The indices in a written list of [blocks of a set partition](#block-of-a-set-partition) do not label or order the [set partition](#set-partition).

### Refinement of a set partition

↑ **Parent:** [Set partition](#set-partition)

A [set partition](#set-partition) $\mathcal Q$ refines $\mathcal P$ if every cell of $\mathcal Q$ is contained in a cell of $\mathcal P$. Thus $\mathcal Q$ retains every separation made by $\mathcal P$ and may make additional separations. [Refinement of a set partition](#refinement-of-a-set-partition) is reflexive and transitive. If each partition refines the other, their cells coincide, so [refinement of a set partition](#refinement-of-a-set-partition) is a partial order on partitions. For finite partitions the nonempty intersections of cells form their common [refinement of a set partition](#refinement-of-a-set-partition). In [graph](graph.md) regularity arguments, subdividing cells and treating discarded [vertices](graph.md#vertex-graph-theory) as singletons preserves [refinement of a set partition](#refinement-of-a-set-partition); merging discarded [vertices](graph.md#vertex-graph-theory) into one cell need not. The [refinement variance identity for regularity energy](probabilistic-combinatorics.md#refinement-variance-identity-for-regularity-energy) consequently proves that this singleton treatment cannot decrease the [equitable regularity energy](probabilistic-combinatorics.md#equitable-regularity-energy).

### Integer partition

↑ **Parent:** [Set partition](#set-partition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integer_partition)

An [integer partition](#integer-partition) of a [nonnegative integer](arithmetic.md#natural-number) $n$ is a [multiset](set.md#multiset) of [positive integers](number-theory.md#positive-integer) whose [sum](arithmetic.md#sum) is $n$: repetitions matter, but the order of the summands does not. Equivalently, write its parts in decreasing order, allowing equality:

$$
\lambda=(\lambda_1,\ldots,\lambda_\ell),\qquad
\lambda_1\geq\cdots\geq\lambda_\ell>0,\qquad
\sum_{i=1}^{\ell}\lambda_i=n.
$$

The notation $\lambda\vdash n$ says that $\lambda$ is an [integer partition](#integer-partition) of $n$. The partition count $p(n)$ counts all [integer partitions](#integer-partition) of $n$, with any number of parts. Zero has one empty [integer partition](#integer-partition), so $p(0)=1$. The [partition of an integer](representation-theory-of-the-symmetric-group.md#partition-of-an-integer) article develops the same objects in [representation theory of the symmetric group](representation-theory-of-the-symmetric-group.md).[section 1.7, definitions of partitions and diagrams](mathematics-bibliography.md#enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley)

**Computed example.** The seven [integer partitions](#integer-partition) of five are exactly

$$
5;\quad 4+1;\quad 3+2;\quad 3+1+1;\quad
2+2+1;\quad 2+1+1+1;\quad 1+1+1+1+1.
$$

Thus $p(5)=7$. Sorting each list of positive summands into decreasing order prevents repetitions in this enumeration. Grouping by largest part verifies completeness: largest parts $5,4,3,2,1$ contribute respectively $1,1,2,2,1$ possibilities. For largest part $3$, the remaining $2$ is either $2$ or $1+1$; for largest part $2$, the remaining $3$ uses only $2$ and $1$, giving $2+1$ or $1+1+1$.

<a id="image-all-seven-integer-partitions-of-five-drawn-as-ferrers-diagrams-each-row-has-as-many-dots-as-its-part"></a>
![](integer-partitions-of-five.png)

**[Figure 15](#image-all-seven-integer-partitions-of-five-drawn-as-ferrers-diagrams-each-row-has-as-many-dots-as-its-part). All seven integer partitions of five, drawn as Ferrers diagrams: each row has as many dots as its part**.

An [integer partition](#integer-partition) keeps sizes without named positions. The [compositions of an integer](#composition-of-an-integer) $(3,2)$ and $(2,3)$ are different [tuples](set-theory.md#finite-tuple), but sorting either gives the same [integer partition](#integer-partition) $3+2$. A [weak composition of an integer](#weak-composition-of-an-integer) $(0,3,2)$ also retains its empty first position; dropping its zero and sorting gives that same [integer partition](#integer-partition). Conversely, a [set partition](#set-partition) records which distinct elements belong to each block. For example, the [set partitions](#set-partition) $\{\{1,2,3\},\{4,5\}\}$ and $\{\{1,2,4\},\{3,5\}\}$ differ even though both have the same [integer partition](#integer-partition) $3+2$ of block sizes.

The [Ferrers diagram](#ferrers-diagram) makes an [integer partition](#integer-partition) into a shape. For $3+2$, the column lengths are $2,2,1$: exchanging rows and columns gives its [conjugate partition](representation-theory-of-the-symmetric-group.md#conjugate-partition) $2+2+1$. Exchanging again recovers $3+2$, so this operation is a [bijection](function.md#bijection). In particular, the three [integer partitions](#integer-partition) of five with at most two parts are $5$, $4+1$, and $3+2$; their [conjugate partitions](representation-theory-of-the-symmetric-group.md#conjugate-partition) $1+1+1+1+1$, $2+1+1+1$, and $2+2+1$ are precisely the three with largest part at most two. This visible symmetry explains the equal counts for these two restrictions. The square-cell version is the existing [Young diagram](representation-theory-of-the-symmetric-group.md#young-diagram).

**Counting by a generating function.** An [integer partition](#integer-partition) is determined by its multiplicities $m_j$, the number of parts equal to $j$. Its size condition is $\sum_{j\geq1}j m_j=n$. Consequently its [ordinary generating function](commutative-algebra.md#ordinary-generating-function) is

$$
\sum_{n\geq0}p(n)q^n
=\prod_{j\geq1}\left(1+q^j+q^{2j}+\cdots\right)
=\prod_{j\geq1}\frac{1}{1-q^j}.
$$

**Proof outline.** Choose the term $q^{jm_j}$ from the $j$th [geometric series](real-analysis.md#geometric-series). The product contributes $q^n$ exactly when those multiplicities describe an [integer partition](#integer-partition) of $n$, once for each such [integer partition](#integer-partition). As a [formal power series](commutative-algebra.md#formal-power-series), each [coefficient](vector-space.md#coefficient) is determined by finitely many factors: factors with $j>n$ contribute only their constant term to the [coefficient](vector-space.md#coefficient) of $q^n$. For $n=5$, multiplication through $j=5$ gives $1+q+2q^2+3q^3+5q^4+7q^5$ up to degree five, independently recovering $p(5)=7$. Restricting the factors gives the [generating function for partitions with bounded parts](representation-theory-of-the-symmetric-group.md#generating-function-for-partitions-with-bounded-parts). This is useful because restrictions on summands become choices of factors, while [conjugate partitions](representation-theory-of-the-symmetric-group.md#conjugate-partition) turn restrictions on numbers of rows into restrictions on row lengths.[section 1.8, conjugation and partition generating functions](mathematics-bibliography.md#enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley)

#### Partition in a rectangle

↑ **Parent:** [Integer partition](#integer-partition)

An [integer partition](#integer-partition) whose [Young diagram](representation-theory-of-the-symmetric-group.md#young-diagram) has at most $h$ rows and at most $w$ cells per row. Zeros may pad the list of row lengths. The [partition interpretation of Gaussian binomial coefficients](#partition-interpretation-of-gaussian-binomial-coefficients) counts these diagrams by their number of cells.

#### Ferrers diagram

↑ **Parent:** [Integer partition](#integer-partition)

A [Ferrers diagram](#ferrers-diagram) of an [integer partition](#integer-partition) $\lambda$ is a left-aligned array of dots with $\lambda_i$ dots in row $i$, using the longest row at the top here. Replacing each dot by a square cell gives a [Young diagram](representation-theory-of-the-symmetric-group.md#young-diagram). Reading the column lengths gives the [conjugate partition](representation-theory-of-the-symmetric-group.md#conjugate-partition).[section 1.7, Ferrers and Young diagrams](mathematics-bibliography.md#enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley)

### Stirling numbers of the second kind

↑ **Parent:** [Set partition](#set-partition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stirling_numbers_of_the_second_kind)

For [nonnegative integers](arithmetic.md#natural-number) $n,k$, the [Stirling number of the second kind](#stirling-numbers-of-the-second-kind)

$$
S(n,k)=\left\{\begin{matrix}n\\k\end{matrix}\right\}
$$

counts the [set partitions](#set-partition) of an $n$-element [finite set](set.md#finite-set) into exactly $k$ unlabelled [blocks of a set partition](#block-of-a-set-partition). Set $S(0,0)=1$, $S(n,0)=0$ for $n>0$, and $S(n,k)=0$ for $k>n$. Also $S(n,1)=S(n,n)=1$ for $n\geq1$. Grassl and Levin develop these counts through explicit [set partitions](#set-partition) and a [recurrence relation](real-analysis.md#recurrence-relation). [Grassl and Levin, More Discrete Mathematics via Graph Theory, section 3.1: counting partitions](https://discrete.openmathbooks.org/more/mdm/sec_adv-partitions.html)

**Insert one distinguished element.** For $n\geq1$ and $1\leq k\leq n$, the [Stirling numbers of the second kind](#stirling-numbers-of-the-second-kind) obey

$$
S(n,k)=kS(n-1,k)+S(n-1,k-1).
$$

**Proof outline.** Inspect the [block of a set partition](#block-of-a-set-partition) containing $n$. If it contains another element, removing $n$ leaves a [set partition](#set-partition) into $k$ [blocks of a set partition](#block-of-a-set-partition); conversely, insert $n$ into any of those $k$ [blocks of a set partition](#block-of-a-set-partition). If $n$ is alone, remove its [singleton set](set.md#singleton-mathematics) and obtain a [set partition](#set-partition) into $k-1$ [blocks of a set partition](#block-of-a-set-partition). The cases cannot overlap, and deletion reverses each construction. This explains the factor $k$ even though the [blocks of a set partition](#block-of-a-set-partition) have no names. [Grassl and Levin, More Discrete Mathematics via Graph Theory, section 3.4: Stirling recurrence](https://discrete.openmathbooks.org/more/mdm/sec_adv-stirling.html)

For $n=4,k=2$, start with the three two-block [set partitions](#set-partition) of $\{1,2,3\}$. Inserting $4$ into either [block of a set partition](#block-of-a-set-partition) gives six possibilities. The remaining possibility is $\{\{1,2,3\},\{4\}\}$, obtained by making $4$ a [singleton set](set.md#singleton-mathematics). Hence $S(4,2)=2\cdot3+1=7$. The seven [set partitions](#set-partition) in the diagram comprise four with sizes $3+1$ and three with sizes $2+2$; this grouping by sizes independently gives $4+3=7$.

<a id="image-exact-construction-of-all-seven-two-block-set-partitions-of-1-2-3-4-six-insert-4-into-an-existing-block-of-a-set-partition-and-one-creates-a-singleton-set"></a>
![](set-partitions-stirling-insert-four.png)

**[Figure 16](#image-exact-construction-of-all-seven-two-block-set-partitions-of-1-2-3-4-six-insert-4-into-an-existing-block-of-a-set-partition-and-one-creates-a-singleton-set). Exact construction of all seven two-block set partitions of $\{1,2,3,4\}$: six insert $4$ into an existing block of a set partition, and one creates a singleton set**.

**Three different counting questions.** The [binomial coefficient](#binomial-coefficient) $\binom nk$ selects one $k$-element [subset](set.md#subset). The [Stirling number of the second kind](#stirling-numbers-of-the-second-kind) $S(n,k)$ groups all $n$ distinct elements into $k$ nonempty unnamed [blocks of a set partition](#block-of-a-set-partition). The power $k^n$ counts all [functions](function.md) to a specified $k$-element [finite set](set.md#finite-set), allowing some destination labels to go unused. At $n=4,k=2$, these counts are respectively $6$, $7$, and $16$. Choosing two people, making two unnamed nonempty teams, and assigning each person a red or blue label are different tasks.

**When the destinations have labels.** For fixed [finite sets](set.md#finite-set) $X,Y$ of sizes $n,k$, respectively, the number of [surjective functions](algebra.md#surjective-function) $X\to Y$ is

$$
\#\{f:X\to Y\mid f\text{ is surjective}\}=k!S(n,k).
$$

Here every element of $Y$ must be used. Each [surjective function](algebra.md#surjective-function) gives a [set partition](#set-partition) of $X$ into its nonempty [preimages](set-theory.md#preimage) $f^{-1}(\{y\})$. Conversely, assign the $k$ distinct destination labels to the $k$ [blocks of a set partition](#block-of-a-set-partition) in $k!$ ways, where $k!$ is a [factorial](#factorial). For two labelled teams of four people this gives $2!\cdot7=14$: of the $2^4=16$ assignments, exactly two use only one label. Dividing arbitrary [function](function.md) counts by $k!$ fails in general because unused labels can be permuted without changing a [function](function.md). For example, $3^4/3!=13.5$ cannot count [set partitions](#set-partition). The empty-to-empty [function](function.md) is a [surjection](algebra.md#surjective-function), consistent with $0!S(0,0)=1$. Stanley gives the [bijection](function.md#bijection) underlying this qualification.[section 1.9: Twelvefold Way entry 3](mathematics-bibliography.md#enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley)

For example, the [inclusion-exclusion principle](#inclusion-exclusion-principle) counts the [surjections](algebra.md#surjective-function) from four elements to three labelled destinations as $3^4-3\cdot2^4+3\cdot1^4=36$. Thus $S(4,3)=36/3!=6$. An independent check chooses the only two-element [block of a set partition](#block-of-a-set-partition) in $\binom42=6$ ways; the other two elements form [singleton sets](set.md#singleton-mathematics).

**Why these numbers also occur in algebra.** Classifying all [functions](function.md) to an $m$-element [finite set](set.md#finite-set) by the size $k$ of their [image](set-theory.md#image-of-a-function) gives

$$
m^n=\sum_{k=0}^n S(n,k)(m)_k,\qquad (m)_k=m(m-1)\cdots(m-k+1),\quad (m)_0=1.
$$

For a fixed [set partition](#set-partition), the [falling factorial](#falling-factorial) $(m)_k$ counts assignments of distinct labels to its $k$ [blocks of a set partition](#block-of-a-set-partition), and is zero when $k>m$. At $n=3,m=4$, this reads $64=1\cdot4+3\cdot12+1\cdot24$. Replacing $m$ by $x$ yields a [polynomial](polynomial.md) identity: both sides agree at every [nonnegative integer](arithmetic.md#natural-number). Thus the [Stirling numbers of the second kind](#stirling-numbers-of-the-second-kind) translate powers into [falling factorials](#falling-factorial). Grouping by equal values turns a counting rule into an algebraic change of coordinates. Summing $S(n,k)$ without destination labels instead gives the [Bell number](#bell-number).

#### Bell number

↑ **Parent:** [Stirling numbers of the second kind](#stirling-numbers-of-the-second-kind)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bell_number)

The [Bell number](#bell-number) $B_n$ counts all [set partitions](#set-partition) of an $n$-element [finite set](set.md#finite-set), with no restriction on the number of [blocks of a set partition](#block-of-a-set-partition). Summing the [Stirling numbers of the second kind](#stirling-numbers-of-the-second-kind) gives $B_n=\sum_{k=0}^n S(n,k)$. The first five values, for $n=0,1,2,3,4$, are $1,1,2,5,15$. In particular, $B_4=1+7+6+1=15$. [Grassl and Levin, More Discrete Mathematics via Graph Theory, definition 3.1.2: Bell numbers](https://discrete.openmathbooks.org/more/mdm/sec_adv-partitions.html)

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

For a [nonnegative integer](arithmetic.md#natural-number) $n$, the [factorial](#factorial) $n!$ is the [product](arithmetic.md#product-of-numbers) of the [positive integers](number-theory.md#positive-integer) from $1$ to $n$, with the [empty product](arithmetic.md#empty-product) equal to $1$:

$$
n!=\prod_{j=1}^{n}j,\qquad 0!=1.
$$

Thus $1!=1$, $2!=2$, $3!=6$, $4!=24$ and $5!=120$. The [factorial](#factorial) counts the [permutations](#permutation) of $n$ distinct objects: arranging $A,B,C$ gives exactly $ABC,ACB,BAC,BCA,CAB,CBA$. The choice tree in [permutation](#permutation) shows the three choices for the first position, two for the second, and one for the last.

The value $0!=1$ has a counting explanation: the [empty set](set.md#empty-set) has exactly one ordering, the empty list. Equivalently, it has exactly one [bijection](function.md#bijection) to itself, the empty [function](function.md). There are no choices to make, and one completed outcome. The [factorial](#factorial) therefore obeys the [recurrence relation](real-analysis.md#recurrence-relation)

$$
0!=1,\qquad n!=n(n-1)!\quad(n\geq1).
$$

The useful distinction is how many positions are filled. For [integers](number-theory.md#integer) $0\leq k\leq n$, choosing and ordering $k$ distinct objects by [sampling without replacement](statistical-inference.md#sampling-without-replacement) gives the [falling factorial](#falling-factorial), while choosing an unordered $k$-element [subset](set.md#subset) gives the [binomial coefficient](#binomial-coefficient):

$$
\underbrace{n(n-1)\cdots(n-k+1)}_{k\text{ factors}}=\frac{n!}{(n-k)!},\qquad
\binom nk=\frac{n!}{k!(n-k)!}.
$$

For five people, assigning captain and deputy gives $5!/3!=20$ outcomes; choosing a two-person team gives $\binom52=10$. Every team has exactly $2!$ assignments of the two roles, explaining the division. When $k=0$, both counts are one. The [factorial](#factorial) is useful here because one count of full orderings yields both formulas by cancellation and by forgetting order. [OpenStax, College Algebra 2e, section 9.5: counting ordered selections and combinations](https://openstax.org/books/college-algebra-2e/pages/9-5-counting-principles)

Distinctness matters. If the two copies of $A$ in $AAB$ are indistinguishable, the visible arrangements are just $AAB,ABA,BAA$, numbering $3!/2!=3$. Temporarily labelling them $A_1,A_2$ gives six [permutations](#permutation), but exchanging the two labels leaves each visible word unchanged, so every word was counted $2!$ times.

**Proof outline.** For $n\geq1$, choose the first object in $n$ ways, then order the remaining $n-1$ objects in $(n-1)!$ ways. The [rule of product](#rule-of-product) gives the [recurrence relation](real-analysis.md#recurrence-relation); repeated application gives the displayed [product](arithmetic.md#product-of-numbers), starting from the one empty ordering. This explains why the [factorial](#factorial) grows quickly: every additional distinct object introduces another multiplicative factor.

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

For [nonnegative integers](arithmetic.md#natural-number) $n$ and $0\leq k\leq n$, the binomial coefficient

$$
\binom nk=\frac{n!}{k!(n-k)!}
$$

counts the $k$-element [subsets](set.md#subset) of an $n$-element [set](set.md). To obtain the formula, first choose an ordered list of $k$ different members in $n(n-1)\cdots(n-k+1)$ ways. Each [subset](set.md#subset) appears in exactly $k!$ orders, so divide by that [factorial](#factorial). The cases $k=0$ and $k=n$ each have one selection, the [empty set](set.md#empty-set) and the whole [set](set.md). For integer $k$ outside $0\leq k\leq n$, the combinatorial convention is $\binom nk=0$.

For $n=5$, $k=2$, the calculation is $\binom52=5\cdot4/2=10$. The left-hand panel lists all ten [subsets](set.md#subset) of $\{a,b,c,d,e\}$. Marking an included member with one and an excluded member with zero gives a [bijection](function.md#bijection) with length-five [binary strings](computer-science.md#binary-string) containing exactly two ones. More generally, this makes selection, binary encoding, and coefficients in a [binomial theorem](#binomial-theorem) three descriptions of the same count.

<a id="image-ten-two-element-subsets-of-a-five-element-set-match-the-corresponding-entry-of-pascal-s-triangle"></a>
![](binomial-subsets-and-triangle.png)

**[Figure 17](#image-ten-two-element-subsets-of-a-five-element-set-match-the-corresponding-entry-of-pascal-s-triangle). Ten two-element subsets of a five-element set match the corresponding entry of Pascal's triangle**.

For a uniformly chosen two-person team, a specified person belongs to four of the ten teams, so the [probability](probability-theory.md#probability) of their inclusion is $4/10=2/5$. Uniform selection of a $k$-element [subset](set.md#subset) similarly gives inclusion [probability](probability-theory.md#probability) $k/n$ for each member when $n>0$, as the [double counting](#double-counting-proof-technique) identity shows.

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
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_binomial_coefficient)

A [Gaussian binomial coefficient](#gaussian-binomial-coefficient) refines an ordinary [binomial coefficient](#binomial-coefficient) into a [polynomial](polynomial.md) that remembers a size statistic. For [nonnegative integers](arithmetic.md#natural-number) $n$ and $0\leq k\leq n$, write

$$
G_{n,k}(t)=\binom nk_t=\prod_{j=1}^k\frac{1-t^{n-k+j}}{1-t^j}.
$$

The product represents a [polynomial](polynomial.md); it is not an instruction to divide by zero when $t=1$ or a denominator vanishes. The [Gaussian binomial coefficient recurrence](#gaussian-binomial-coefficient-recurrence) gives a way to compute it with only [addition](arithmetic.md#addition) and [multiplication](arithmetic.md#multiplication). The [empty product](arithmetic.md#empty-product) for $k=0$ is one, and $G_{n,n}(t)=1$ as well. Setting $t=1$ after obtaining the [polynomial](polynomial.md) recovers $\binom nk$.

For example,

$$
\boxed{G_{4,2}(t)=1+t+2t^2+t^3+t^4.}
$$

At $t=1$ this gives six objects, but its [coefficients](vector-space.md#coefficient) reveal how those six objects are distributed across sizes $0,1,2,3,4$: there are two of size two and one of each other size. The [lattice-path interpretation of Gaussian binomial coefficients](#lattice-path-interpretation-of-gaussian-binomial-coefficients) makes that information visible. Take unit steps north or east from $(0,0)$ to $(2,2)$. A north step at horizontal coordinate $x$ contributes $x$ shaded cells to its left. The six step words have total shaded [areas](differential-geometry.md#surface-area) $0,1,2,2,3,4$.

<a id="image-the-six-lattice-paths-counted-by-g-4-2-t-weighted-by-the-number-of-shaded-cells"></a>
![](gaussian-binomial-paths-and-partitions.png)

**[Figure 18](#image-the-six-lattice-paths-counted-by-g-4-2-t-weighted-by-the-number-of-shaded-cells). The six lattice paths counted by $G_{4,2}(t)$, weighted by the number of shaded cells**. Original exact enumeration of paths with two north and two east steps. Reading shaded row lengths from top to bottom gives a [partition in a rectangle](#partition-in-a-rectangle). Equal-sized diagrams contribute to the same [coefficient](vector-space.md#coefficient).

This is useful because an aggregate count can hide the feature one actually wants. A [generating function](real-analysis.md#generating-function) retains the distribution of a statistic, so [coefficient extraction](polynomial.md#coefficient-extraction) answers questions such as “how many allowed diagrams contain exactly two cells?” The [partition interpretation of Gaussian binomial coefficients](#partition-interpretation-of-gaussian-binomial-coefficients) makes every [coefficient](vector-space.md#coefficient) a nonnegative [integer](number-theory.md#integer) without relying on cancellation in the product formula.

An unexpected second use comes from [linear algebra](linear-algebra.md). If $q$ is a [prime power](number-theory.md#prime-power), the value $G_{n,k}(q)$ counts the $k$-dimensional [vector subspaces](vector-space.md#vector-subspace) of $\mathbb F_q^n$. Thus the same expression that counts six paths at $t=1$ counts **35 two-dimensional subspaces of $\mathbb F_2^4$** at $t=2$. The [Gaussian binomial coefficient counts finite-field subspaces](#gaussian-binomial-coefficient-counts-finite-field-subspaces) article explains why selecting a [vector subspace](vector-space.md#vector-subspace) differs from selecting a [subset](set.md#subset) of coordinates. [Enumerative Combinatorics, Volume 1 (second-edition draft) by Richard Stanley](mathematics-bibliography.md#enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley)

This relationship illustrates a [q-analogue](#q-analogue): the parameter can encode a statistic in one interpretation and the size of a [finite field](algebra.md#finite-field) in another. Here $t$ denotes the formal variable, while $q$ denotes a [finite field](algebra.md#finite-field)'s cardinality when we evaluate the [polynomial](polynomial.md). The interpretation using a [finite field](algebra.md#finite-field) requires $q$ to be a [prime power](number-theory.md#prime-power); evaluating the [polynomial](polynomial.md) at an arbitrary number does not construct a field of that size.

#### Gaussian binomial coefficient recurrence

↑ **Parent:** [Gaussian binomial coefficient](#gaussian-binomial-coefficient)

For $n\geq1$ and $1\leq k\leq n$, the displayed [recurrence relation](real-analysis.md#recurrence-relation) uses $G_{n,0}(t)=1$ and $G_{n,k}(t)=0$ when $k<0$ or $k>n$. At $t=1$ it becomes [Pascal's identity](#pascal-s-rule).

An exact weighted-[subset](set.md#subset) formula is

$$
G_{n,k}(t)=\sum_{0\leq j_1<\cdots<j_k<n}t^{\sum_{i=1}^k(j_i-(i-1))}.
$$

The [exponent](arithmetic.md#exponent) measures how far the selected positions lie beyond the earliest possible choices $0,\ldots,k-1$. Split the [subsets](set.md#subset) according to whether they contain $n-1$. Those without it give $G_{n-1,k}(t)$; deleting it from those with it removes exactly $n-k$ from their [exponent](arithmetic.md#exponent). This gives the displayed [recurrence relation](real-analysis.md#recurrence-relation), explaining why it builds [polynomials](polynomial.md) with nonnegative [integer](number-theory.md#integer) [coefficients](vector-space.md#coefficient).

#### Lattice-path interpretation of Gaussian binomial coefficients

↑ **Parent:** [Gaussian binomial coefficient](#gaussian-binomial-coefficient)

Use [lattice paths](#lattice-path) with $k$ north steps and $n-k$ east steps, beginning at $(0,0)$. Let $A(P)$ be the [sum](arithmetic.md#sum) of the horizontal coordinates of its north steps, equivalently the number of unit cells to their left inside the $k$-by-$(n-k)$ [rectangle](geometry-and-topology.md#rectangle). A north step in zero-based word position $j_i$ has $i-1$ earlier north steps, so its horizontal coordinate is $j_i-(i-1)$. The [Gaussian binomial coefficient recurrence](#gaussian-binomial-coefficient-recurrence) therefore counts these [lattice paths](#lattice-path) with weight $t^{A(P)}$.

For $n=4,k=2$, the words `NNEE`, `NENE`, `NEEN`, `ENNE`, `ENEN`, `EENN` have respective [areas](differential-geometry.md#surface-area) $0,1,2,2,3,4$. The word `NEEN` contributes $t^2$ because the two north steps occur at horizontal coordinates zero and two. These paths never move south or west; allowing such extra steps would change the collection being counted.

#### Partition interpretation of Gaussian binomial coefficients

↑ **Parent:** [Gaussian binomial coefficient](#gaussian-binomial-coefficient)

The [Young diagrams](representation-theory-of-the-symmetric-group.md#young-diagram) of [partitions in a rectangle](#partition-in-a-rectangle) with at most $k$ rows and at most $n-k$ cells in each row correspond to the [lattice paths](#lattice-path) in the [lattice-path interpretation of Gaussian binomial coefficients](#lattice-path-interpretation-of-gaussian-binomial-coefficients). Read the shaded row lengths from top to bottom; the result is a nonincreasing list of [nonnegative integers](arithmetic.md#natural-number). This [bijection](function.md#bijection) preserves the number $|\lambda|$ of cells.

In a two-by-two [rectangle](geometry-and-topology.md#rectangle), the possibilities are the empty [integer partition](#integer-partition), $(1)$, $(2)$, $(1,1)$, $(2,1)$, and $(2,2)$. Their sizes are $0,1,2,2,3,4$, giving $G_{4,2}(t)$. In particular, **there are two allowed diagrams of size two**, explaining the middle [coefficient](vector-space.md#coefficient).[§1.7, Proposition 1.7.3, pp. 64–66](mathematics-bibliography.md#enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley)

##### Complement symmetry of Gaussian binomial coefficients

↑ **Parent:** [Partition interpretation of Gaussian binomial coefficients](#partition-interpretation-of-gaussian-binomial-coefficients)

Pad a [partition in a rectangle](#partition-in-a-rectangle) with zero rows until it has $k$ entries, and put $w=n-k$. The complementary rotated diagram has row lengths $\lambda'_i=w-\lambda_{k+1-i}$. This is again a [partition in a rectangle](#partition-in-a-rectangle), and its size is $kw-|\lambda|$. Repeating the operation recovers the original [integer partition](#integer-partition), so it gives a [bijection](function.md#bijection) between diagrams of size $a$ and diagrams of size $kw-a$. Consequently the [coefficients](vector-space.md#coefficient) of the [Gaussian polynomial](#gaussian-binomial-coefficient) read the same in either direction. The displayed identity can be interpreted as an identity of [Laurent polynomials](polynomial.md#laurent-polynomial); it does not require substituting $t^{-1}$ at $t=0$.

For the two-by-two [rectangle](geometry-and-topology.md#rectangle), the empty diagram pairs with $(2,2)$, and $(1)$ pairs with $(2,1)$; $(2)$ and $(1,1)$ each map to themselves. This establishes symmetry, while [unimodality of Gaussian binomial coefficients](#unimodality-of-gaussian-binomial-coefficients) is a stronger statement about the growth and decrease of successive [coefficients](vector-space.md#coefficient).

#### Gaussian binomial coefficient counts finite-field subspaces

↑ **Parent:** [Gaussian binomial coefficient](#gaussian-binomial-coefficient)

For a [prime power](number-theory.md#prime-power) $q$ and $0\leq k\leq n$, count ordered lists of $k$ [linearly independent vectors](vector-space.md#linear-independence) in $\mathbb F_q^n$. The first has $q^n-1$ choices. After $i$ independent choices, their [linear span](vector-space.md#linear-span) contains $q^i$ [vectors](vector-space.md#vector), so the next has $q^n-q^i$ choices. Every $k$-dimensional [vector subspace](vector-space.md#vector-subspace) has exactly $\prod_{i=0}^{k-1}(q^k-q^i)$ [ordered bases](vector-space.md#ordered-basis). Dividing the list count by this common multiplicity gives

$$
\#\operatorname{Gr}(k,\mathbb F_q^n)=\frac{\prod_{i=0}^{k-1}(q^n-q^i)}{\prod_{i=0}^{k-1}(q^k-q^i)}=G_{n,k}(q).
$$

The notation $\operatorname{Gr}$ refers to the [Grassmannian](differential-geometry.md#grassmannian), here considered simply as the finite collection of these [vector subspaces](vector-space.md#vector-subspace).[§1.7, Proposition 1.7.2, pp. 63–64](mathematics-bibliography.md#enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley)

For $n=4,k=2,q=2$, there are $15\cdot14=210$ ordered independent pairs. Each two-dimensional [vector subspace](vector-space.md#vector-subspace) has $3\cdot2=6$ [ordered bases](vector-space.md#ordered-basis), leaving $210/6=35$ [vector subspaces](vector-space.md#vector-subspace). There are only $\binom42=6$ coordinate-selected [vector subspaces](vector-space.md#vector-subspace); most of the 35 also contain [vectors](vector-space.md#vector) combining coordinates.

A unique [reduced row echelon form](numerical-analysis.md#reduced-row-echelon-form) gives another count. Its six possible pivot-column patterns have $4,3,2,2,1,0$ freely chosen entries. Each free entry lies in $\mathbb F_2$, giving $16,8,4,4,2,1$ [vector subspaces](vector-space.md#vector-subspace), respectively. The diagram fixes the zero entries required to make each pivot the first nonzero entry in its row and the only nonzero entry in its column. Different choices describe different [row spaces](vector-space.md#row-space).

<a id="image-the-six-reduced-row-echelon-form-pivot-patterns-give-35-two-dimensional-vector-subspaces-of-mathbb-f-2-4"></a>
![](gaussian-binomial-finite-field-subspaces.png)

**[Figure 19](#image-the-six-reduced-row-echelon-form-pivot-patterns-give-35-two-dimensional-vector-subspaces-of-mathbb-f-2-4). The six reduced row echelon form pivot patterns give 35 two-dimensional vector subspaces of $\mathbb F_2^4$**. Original exact matrix-pattern enumeration. A star is a freely chosen [finite field](algebra.md#finite-field) entry, while every displayed zero or one is fixed. Pivot columns are numbered from one in this image.

#### Unimodality of Gaussian binomial coefficients

↑ **Parent:** [Gaussian binomial coefficient](#gaussian-binomial-coefficient)

For $0\le k\le n$, let $V$ be the $n$-dimensional irreducible [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra) representation. Its weights are $n-1,n-3,\ldots,1-n$. A wedge basis shows $\operatorname{ch}\Lambda^kV=q^{-k(n-k)}G_{n,k}(q^2)$, where $G_{n,k}(t)$ is the [Gaussian binomial coefficient](#gaussian-binomial-coefficient). By the [Weyl complete reducibility theorem](semisimple-lie-algebra.md#weyl-complete-reducibility-theorem), this character is a nonnegative sum of irreducible strings $q^m+q^{m-2}+\cdots+q^{-m}$. All its weights have parity $k(n-k)$, so their coefficients increase toward zero and decrease afterward. Consequently the coefficients of $G_{n,k}(t)$ are symmetric and unimodal. The [symmetric quantum binomial coefficient](#symmetric-quantum-binomial-coefficient) is this character, a [Laurent polynomial](polynomial.md#laurent-polynomial); its coefficients are unimodal on the occupied parity. The full integer-exponent sequence need not be unimodal, as $q+q^{-1}$ demonstrates.

#### Symmetric quantum binomial coefficient

↑ **Parent:** [Gaussian binomial coefficient](#gaussian-binomial-coefficient)

The quotient $[n]_q[n-1]_q\cdots[n-k+1]_q/([k]_q\cdots[1]_q)$ is the displayed shifted [Gaussian binomial coefficient](#gaussian-binomial-coefficient). It is the [formal character](semisimple-lie-algebra.md#formal-character-of-a-weight-module) of $\Lambda^kL_{n-1}$, where $L_{n-1}$ is the $n$-dimensional irreducible [sl2 Lie algebra](semisimple-lie-algebra.md#sl2-lie-algebra) representation. Indeed its exterior-power weights are sums of $k$ distinct terms of $n-1,n-3,\ldots,1-n$. [Parity unimodality of an sl2 character](semisimple-lie-algebra.md#parity-unimodality-of-an-sl2-character) proves unimodality after removing the intervening zero coefficients; equivalently, the ordinary Gaussian polynomial has unimodal coefficients.

<h3 id="pascal-s-triangle">Pascal's triangle</h3>

↑ **Parent:** [Binomial coefficient](#binomial-coefficient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pascal's_triangle)

Row $n$ of Pascal's triangle consists of the [binomial coefficients](#binomial-coefficient) $\binom n0,\ldots,\binom nn$, beginning with row $0$. Boundary entries are one, and [Pascal's identity](#pascal-s-rule) says each interior entry is the sum of the two entries above it. The [hockey-stick identity](#hockey-stick-identity) evaluates sums along its diagonals.

The highlighted entry in the [binomial coefficient](#binomial-coefficient) illustration is $\binom52=10$. Split two-person teams according to whether they contain the fifth person: six choose both members from the other four, and four contain the fifth person together with one of those four. Thus $10=6+4$. All entries can be generated by the same local rule, so a large table of counts needs no repeated enumeration of its [subsets](set.md#subset).

[Blaise Pascal](mathematics.md#blaise-pascal)'s Traité du triangle arithmétique, published in 1665, presents an arithmetic array and connects it to combinations, games of chance, and powers of binomial expressions. This makes the connection between a counting table and several applications visible in the original work. [Pascal, Traité du triangle arithmétique, 1665 edition](https://archive.org/details/bub_gb_UqgUAAAAQAAJ) The University of Cambridge's account of the treatise explains its 1654 composition and the organization of these applications. [Cambridge University Library, account of Pascal's treatise](https://api.repository.cam.ac.uk/server/api/core/bitstreams/9bfbc9c8-fa56-4694-b96d-fc18db0f562f/content)

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

For a [nonnegative integer](arithmetic.md#natural-number) $n$ and [commuting](algebra.md#commuting-elements) quantities $x,y$,

$$
(x+y)^n=\sum_{k=0}^n\binom nkx^ky^{n-k}.
$$

In expanding the $n$ factors, obtain $x^ky^{n-k}$ by selecting the $k$ positions that contribute $x$. There are $\binom nk$ such choices. For example,

$$
(x+y)^5=x^5+5x^4y+10x^3y^2+10x^2y^3+5xy^4+y^5.
$$

The coefficients are row five of [Pascal's triangle](#pascal-s-triangle), in reverse order under the displayed $x^ky^{n-k}$ convention; the row is symmetric. Setting $x=y=1$ gives $1+5+10+10+5+1=32$, the number of [subsets](set.md#subset) of a five-element [set](set.md). Each member has two inclusion choices, agreeing with the [rule of product](#rule-of-product) and the [cardinality](set-theory.md#cardinality) of the [power set](set.md#power-set).

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

[Stars and bars](#stars-and-bars-combinatorics) counts [tuples](set-theory.md#finite-tuple) of [nonnegative integers](arithmetic.md#natural-number) with a prescribed [sum](arithmetic.md#sum). For [integers](number-theory.md#integer) $N\geq0$ and $k\geq1$, its statement is

$$
\#\{(x_1,\ldots,x_k):x_i\geq0,\ x_1+\cdots+x_k=N\}
=\binom{N+k-1}{k-1}.
$$

Such a [tuple](set-theory.md#finite-tuple) is a [weak composition of an integer](#weak-composition-of-an-integer). Think of $k$ labelled bins: $x_1$ counts identical objects in the first bin, $x_2$ in the second, and so on. Bin names distinguish positions even when counts agree. [Stars and bars](#stars-and-bars-combinatorics) counts these count [tuples](set-theory.md#finite-tuple); assigning individually distinct objects requires additional information. [Felix Gotti, MIT 18.211, Lecture 6: Compositions, Proposition 1 and Example 3](https://math.mit.edu/~fgotti/docs/Courses/C.%20Combinatorial%20Analysis/6.%20Compositions/Compositions.pdf)

**Computed example.** With $N=5$ and $k=3$, the number of [weak compositions of an integer](#weak-composition-of-an-integer) is $\binom72=21$. The string `••|•|••` encodes $(2,1,2)$: two dots before the first bar, one between the bars, and two after the second. For a fixed first-bin count $x_1=a$, the second-bin count can be any [integer](number-theory.md#integer) from $0$ to $5-a$ and the third is forced. Thus the direct count is $6+5+4+3+2+1=21$.

<a id="image-stars-and-bars-for-five-identical-objects-and-three-labelled-bins-ordinary-splits-adjacent-bars-and-bars-at-either-end"></a>
![](stars-and-bars-three-bin-allocation.png)

**[Figure 20](#image-stars-and-bars-for-five-identical-objects-and-three-labelled-bins-ordinary-splits-adjacent-bars-and-bars-at-either-end). Stars and bars for five identical objects and three labelled bins: ordinary splits, adjacent bars, and bars at either end**.

Adjacent bars encode an empty middle bin: `••||•••` gives $(2,0,3)$. A bar at the left end encodes an empty first bin, as in `|••|•••` for $(0,2,3)$; a bar at the right end encodes an empty third bin, as in `••|•••|` for $(2,3,0)$. These are valid [weak compositions of an integer](#weak-composition-of-an-integer). For $N=0$ every count is zero, and for $k=1$ the unique [tuple](set-theory.md#finite-tuple) is $(N)$, consistent with $\binom{N}{0}=1$.

**Proof outline.** Replace each count $x_i$ by that many dots and separate successive groups with $k-1$ bars. Reading the group sizes reverses this construction, so it is a [bijection](function.md#bijection) between [weak compositions of an integer](#weak-composition-of-an-integer) and strings of $N$ dots and $k-1$ bars. Choose the bar positions among $N+k-1$ positions; the [binomial coefficient](#binomial-coefficient) counts the choices. The beauty is that empty bins need no separate cases: end bars and adjacent bars encode them automatically.

If every bin must be nonempty, the [tuples](set-theory.md#finite-tuple) are [compositions of an integer](#composition-of-an-integer), and their count is $\binom{N-1}{k-1}$ for $N\geq k\geq1$; for $N<k$ there are none. Subtract one from every count, setting $y_i=x_i-1$. This is a [bijection](function.md#bijection) to [weak compositions of an integer](#weak-composition-of-an-integer) of $N-k$, so [stars and bars](#stars-and-bars-combinatorics) gives $\binom{(N-k)+k-1}{k-1}=\binom{N-1}{k-1}$. For five objects and three bins, this is $\binom42=6$, with the six positive [tuples](set-theory.md#finite-tuple)

$$
(3,1,1),\ (1,3,1),\ (1,1,3),\ (2,2,1),\ (2,1,2),\ (1,2,2).
$$

For instance, $(2,1,2)$ shifts to $(1,0,1)$, whose [sum](arithmetic.md#sum) is $2=5-3$. Sorting the six positive [tuples](set-theory.md#finite-tuple) collapses them to just two [integer partitions](#integer-partition), $3+1+1$ and $2+2+1$. Thus named bins and unordered summands answer different questions.

[Stars and bars](#stars-and-bars-combinatorics) is useful for allocating identical resources or enumerating [integer](number-theory.md#integer) solutions without listing them individually. Prescribed lower bounds can be subtracted just like the nonempty-bin requirement. Upper bounds require removing forbidden [tuples](set-theory.md#finite-tuple); the existing [bounded weak compositions](#bounded-weak-compositions) article applies the [inclusion-exclusion principle](#inclusion-exclusion-principle) to those violations.

### Composition of an integer

↑ **Parent:** [Stars and bars (combinatorics)](#stars-and-bars-combinatorics)

A [composition of an integer](#composition-of-an-integer) $N>0$ is an ordered [tuple](set-theory.md#finite-tuple) of [positive integers](number-theory.md#positive-integer) with [sum](arithmetic.md#sum) $N$. Its length $k$ counts the parts. For example, $(3,2)$ and $(2,3)$ are different [compositions of an integer](#composition-of-an-integer), though they give the same [integer partition](#integer-partition). [Stars and bars](#stars-and-bars-combinatorics) counts [compositions of an integer](#composition-of-an-integer) with fixed length. [Gotti, Lecture 6, definition of a composition](https://math.mit.edu/~fgotti/docs/Courses/C.%20Combinatorial%20Analysis/6.%20Compositions/Compositions.pdf)

#### Weak composition of an integer

↑ **Parent:** [Composition of an integer](#composition-of-an-integer)

A [weak composition of an integer](#weak-composition-of-an-integer) $N\geq0$ into $k\geq1$ parts is an ordered [tuple](set-theory.md#finite-tuple) of [nonnegative integers](arithmetic.md#natural-number) with [sum](arithmetic.md#sum) $N$. Zero parts retain their positions: $(0,2,3)$ and $(2,0,3)$ differ. Fixing the length $k$ is essential when applying [stars and bars](#stars-and-bars-combinatorics), since inserting extra zero parts creates further [tuples](set-theory.md#finite-tuple). [Gotti, Lecture 6, definition and discussion of weak compositions](https://math.mit.edu/~fgotti/docs/Courses/C.%20Combinatorial%20Analysis/6.%20Compositions/Compositions.pdf)

### Bounded weak compositions

↑ **Parent:** [Stars and bars (combinatorics)](#stars-and-bars-combinatorics)

To count nonnegative tuples with $\sum_{i=0}^r n_i=N$ and $n_i<a_i$, mark violations $n_i\geq a_i$. An intersection of violations indexed by $J$ is in [bijection](function.md#bijection) with unrestricted tuples of sum $N-\sum_{i\in J}a_i$, by subtracting the bounds from those coordinates. [Stars and bars](#stars-and-bars-combinatorics) counts this intersection; the [inclusion-exclusion principle](#inclusion-exclusion-principle) then gives the displayed formula. A negative remaining sum contributes zero.

## Inclusion-exclusion principle

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inclusion-exclusion_principle)

For [finite sets](set.md#finite-set) $A_1,\ldots,A_n$, the cardinality of their [union](set.md#set-union) is

$$
\left|\bigcup_{i=1}^n A_i\right|=\sum_{\varnothing\neq J\subseteq\{1,\ldots,n\}}(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.
$$

Add the individual [cardinalities](set-theory.md#cardinality), subtract pairwise [intersection](set.md#set-intersection) counts, add triple [intersection](set.md#set-intersection) counts, and continue alternating. This is useful whenever one object can satisfy several conditions: a search result can match several filters, or a [permutation](#permutation) can have several forbidden [fixed points](function.md#fixed-point).

Among the [integers](number-theory.md#integer) from 1 to 30, let $A$ contain the multiples of 2 and $B$ the multiples of 3. Then $|A|=15$, $|B|=10$, and $|A\cap B|=5$, because their common multiples are the multiples of 6. The naive sum $25$ counts those five twice; the correct [union](set.md#set-union) size is **$15+10-5=20$**. The regions contain ten in $A$ alone, five in both, five in $B$ alone, and ten in neither.

<a id="image-subtracting-overlap-counts-each-selected-integer-once-a-third-divisibility-condition-requires-adding-the-triple-overlap-back"></a>
![](inclusion-exclusion-counting.png)

**[Figure 21](#image-subtracting-overlap-counts-each-selected-integer-once-a-third-divisibility-condition-requires-adding-the-triple-overlap-back). Subtracting overlap counts each selected integer once; a third divisibility condition requires adding the triple overlap back**.

Add a third [set](set.md) $C$ containing the multiples of 5. Its size is 6; the three pairwise [intersections](set.md#set-intersection) have sizes $5,3,2$; and the triple [intersection](set.md#set-intersection) contains only 30. The [inclusion-exclusion principle](#inclusion-exclusion-principle) gives **$15+10+6-5-3-2+1=22$** integers divisible by at least one of 2, 3, and 5.

The alternating corrections have a local explanation. An object belonging to exactly $r\geq1$ of the [sets](set.md) is counted $\binom r1-\binom r2+\cdots+(-1)^{r+1}\binom rr=1$ times, by the [binomial theorem](#binomial-theorem) applied to $(1-1)^r$. An object in none contributes zero. Thus overlapping descriptions are repaired without requiring the [sets](set.md) themselves to be disjoint. For [probability](probability-theory.md#probability), the same calculation applies to event probabilities in place of [cardinalities](set-theory.md#cardinality), giving the [inclusion-exclusion principle for probabilities](#inclusion-exclusion-principle-for-probabilities).

### Inclusion-exclusion principle for probabilities

↑ **Parent:** [Inclusion-exclusion principle](#inclusion-exclusion-principle)

For a finite family of [events](probability-theory.md#event), the [probability](probability-theory.md#probability) of their [union](set.md#set-union) is the alternating sum of their [intersection](set.md#set-intersection) [probabilities](probability-theory.md#probability), with the same pattern as the [inclusion-exclusion principle](#inclusion-exclusion-principle). Expand the [indicator function](measure-theory.md#indicator-function) of the [union](set.md#set-union) and apply [linearity of expectation](probability-theory.md#linearity-of-expectation); this does not require [independent events](probability-theory.md#independent-events).

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

A [permutation](#permutation) of a [set](set.md) $S$ is a [bijection](function.md#bijection) $\sigma:S\to S$: every element has exactly one [image](set-theory.md#image-of-a-function) and every element appears exactly once as an [image](set-theory.md#image-of-a-function). For a [finite set](set.md#finite-set), a [permutation](#permutation) can also be recorded as an ordering of all its elements, once a reference order has been chosen. For three distinct letters $A,B,C$, the six orderings are

$$
ABC,\quad ACB,\quad BAC,\quad BCA,\quad CAB,\quad CBA.
$$

There are three choices for the first letter, two unused letters for the second, and one for the third. Every path in the tree gives one complete ordering, and every ordering has one such path, so the [rule of product](#rule-of-product) gives $3\cdot2\cdot1=3!=6$, a [factorial](#factorial).

<a id="image-the-full-choice-tree-for-the-six-permutations-of-three-distinct-letters-three-first-choices-two-second-choices-and-one-third-choice"></a>
![](factorial-permutation-choice-tree.png)

**[Figure 22](#image-the-full-choice-tree-for-the-six-permutations-of-three-distinct-letters-three-first-choices-two-second-choices-and-one-third-choice). The full choice tree for the six permutations of three distinct letters: three first choices, two second choices, and one third choice**.

**Ordering versus mapping.** Label the reference positions $1,\ldots,n$. An ordering [tuple](set-theory.md#finite-tuple) $(a_1,\ldots,a_n)$ of these labels describes the [function](function.md) $\sigma(i)=a_i$; conversely, reading the [images](set-theory.md#image-of-a-function) $\sigma(1),\ldots,\sigma(n)$ recovers the ordering. For example,

$$
\sigma=\begin{pmatrix}1&2&3&4\\3&1&4&2\end{pmatrix}
$$

means $1\mapsto3$, $2\mapsto1$, $3\mapsto4$, $4\mapsto2$. Its ordered image list is $(3,1,4,2)$, whereas its [cycle decomposition of a permutation](mathematics.md#cycle-decomposition-of-a-permutation) is $(1\,3\,4\,2)$: starting at $1$, follow its successive images back to $1$. Parentheses in the latter expression encode arrows around a [permutation cycle](finite-group-theory.md#permutation-cycle), rather than an image list in reference order. [Felix Gotti, MIT 18.211, lecture 11, pages 1–2: arrangements, bijections and cycles](https://math.mit.edu/~fgotti/docs/Courses/C.%20Combinatorial%20Analysis/11.%20Permutations%20I/Permutations%20I.pdf)

The two viewpoints answer different useful questions about the same object. An ordering tells us which object occupies each position; a [bijection](function.md#bijection) tells us where each label is sent and allows successive rearrangements through [function composition](function.md#function-composition). All [permutations](#permutation) of $n$ labels form the [symmetric group](finite-group-theory.md#symmetric-group), whose [subgroups](group.md#subgroup) are [permutation groups](finite-group-theory.md#permutation-group). The counting viewpoint supplies $n!$ possibilities, a [factorial](#factorial); the mapping viewpoint reveals how rearrangements combine.

**Composition convention.** Apply the rightmost [permutation](#permutation) first:

$$
(\sigma\tau)(i)=\sigma(\tau(i)).
$$

For the displayed $\sigma=(1\,3\,4\,2)$ and the [transposition](#transposition-permutation) $\tau=(1\,2)$, direct evaluation gives

$$
\sigma\tau=\begin{pmatrix}1&2&3&4\\1&3&4&2\end{pmatrix}=(2\,3\,4),\qquad
\tau\sigma=\begin{pmatrix}1&2&3&4\\3&2&4&1\end{pmatrix}=(1\,3\,4).
$$

For instance, $(\sigma\tau)(1)=\sigma(2)=1$, but $(\tau\sigma)(1)=\tau(3)=3$. Thus [function composition](function.md#function-composition) of [permutations](#permutation) need not be [commutative](algebra.md#commutativity); the omitted labels in these [permutation cycles](finite-group-theory.md#permutation-cycle) are [fixed points](function.md#fixed-point).

### Cyclic permutation

↑ **Parent:** [Permutation](#permutation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclic_permutation)

A [cyclic permutation](#cyclic-permutation), also called a [permutation cycle](finite-group-theory.md#permutation-cycle), sends $k\geq1$ distinct elements $a_1\mapsto a_2\mapsto\cdots\mapsto a_k\mapsto a_1$ and fixes every element outside this list. Its notation is $(a_1\,a_2\,\ldots\,a_k)$. For example, $(1\,3\,4\,2)$ is the [permutation](#permutation) with image list $(3,1,4,2)$: all four labels lie on one directed loop. In contrast,

$$
\rho=\begin{pmatrix}1&2&3&4\\3&4&1&2\end{pmatrix}=(1\,3)(2\,4)
$$

has two separate loops, exchanging $1$ with $3$ and $2$ with $4$. It is a [permutation](#permutation) composed of two [transpositions](#transposition-permutation), rather than a single [cyclic permutation](#cyclic-permutation).

<a id="image-two-permutations-on-four-labels-one-cyclic-permutation-1-3-4-2-and-two-disjoint-permutation-cycles-1-3-2-4-with-arrows-showing-every-image"></a>
![](permutation-cycle-structure.png)

**[Figure 23](#image-two-permutations-on-four-labels-one-cyclic-permutation-1-3-4-2-and-two-disjoint-permutation-cycles-1-3-2-4-with-arrows-showing-every-image). Two permutations on four labels: one cyclic permutation $(1\,3\,4\,2)$ and two disjoint permutation cycles $(1\,3)(2\,4)$, with arrows showing every image**.

Starting at a different point of the same loop changes the written list but preserves the [cyclic permutation](#cyclic-permutation): $(1\,3\,4\,2)=(3\,4\,2\,1)$. Reversing the direction generally changes the [permutation](#permutation); it gives the [inverse function](function.md#inverse-function), here $(1\,2\,4\,3)$. A [transposition](#transposition-permutation) is a [cyclic permutation](#cyclic-permutation) of length two; a one-element [permutation cycle](finite-group-theory.md#permutation-cycle) records a [fixed point](function.md#fixed-point). In a [cycle decomposition of a permutation](mathematics.md#cycle-decomposition-of-a-permutation), one-element [permutation cycles](finite-group-theory.md#permutation-cycle) are usually omitted, with the underlying [set](set.md) understood.

The beauty of this representation is that repeated rearrangements become motion around independent loops. Applying $(1\,3\,4\,2)$ four times returns every label to its start, while applying $(1\,3)(2\,4)$ twice already does so. [Disjoint permutation cycles](finite-group-theory.md#disjoint-permutation-cycles) commute under [function composition](function.md#function-composition), since each moves only labels the others fix. On $n\geq1$ labels, there are $(n-1)!$ [cyclic permutations](#cyclic-permutation) whose single loop contains every label: fix $1$ as the first written entry and order the other $n-1$ labels freely, giving a [factorial](#factorial). This is also the count of [cyclic orderings](#cyclic-ordering); choosing a starting position would otherwise count each loop $n$ times. Rotations are identified here, while reversing direction is allowed to give a different [cyclic ordering](#cyclic-ordering).

**Proof outline for decomposition.** Starting at any label in a [finite set](set.md#finite-set), repeatedly apply the [permutation](#permutation). The [pigeonhole principle](#pigeonhole-principle) forces a repeated label. If the first repetition were at a label other than the starting one, its two predecessors would be different labels with the same [image](set-theory.md#image-of-a-function), contradicting the [injective function](algebra.md#injective-function) property. This produces a [permutation cycle](finite-group-theory.md#permutation-cycle) returning to the start. Start again at a label not yet visited; the new [permutation cycle](finite-group-theory.md#permutation-cycle) cannot meet an earlier one, since the [bijection](function.md#bijection) gives every label a unique predecessor. Continue until every label belongs to a loop. The resulting [cycle decomposition of a permutation](mathematics.md#cycle-decomposition-of-a-permutation) is unique up to the order of the [disjoint permutation cycles](finite-group-theory.md#disjoint-permutation-cycles) and the starting point written in each one. [Felix Gotti, MIT 18.211, lecture 11, definitions 1–2 and the preceding argument](https://math.mit.edu/~fgotti/docs/Courses/C.%20Combinatorial%20Analysis/11.%20Permutations%20I/Permutations%20I.pdf)

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

#### Fixed point count of a uniform random permutation

↑ **Parent:** [Uniform random permutation](#uniform-random-permutation)

For a [uniform random permutation](#uniform-random-permutation) $\pi$ of $n\geq1$ objects, let $M_n$ count its [fixed points](function.md#fixed-point). Write $M_n=\sum_{i=1}^n\mathbf1_{\{\pi(i)=i\}}$. Each [indicator random variable](probability-theory.md#indicator-random-variable) has [expected value](probability-theory.md#expected-value) $1/n$, so [linearity of expectation](probability-theory.md#linearity-of-expectation) gives **$\mathbb E[M_n]=1$ for every $n\geq1$**. This average does not require [independence](random-variable.md#independent-random-variables): for $n\geq2$, fixing two specified objects has [probability](probability-theory.md#probability) $1/[n(n-1)]$, greater than the product $1/n^2$ of their individual [probabilities](probability-theory.md#probability).

For four objects, exact enumeration gives counts $9,8,6,0,1$ for $0,1,2,3,4$ [fixed points](function.md#fixed-point) among the $24$ equally likely [permutations](#permutation). Their weighted [arithmetic mean](arithmetic.md#arithmetic-mean) is $(0\cdot9+1\cdot8+2\cdot6+4\cdot1)/24=1$. Exactly three [fixed points](function.md#fixed-point) are impossible: the last object must then also be fixed.

<a id="image-the-fixed-point-count-of-a-uniform-random-permutation-averaged-over-all-24-permutations-of-four-objects"></a>
![](fixed-points-permutation-expectation.png)

**[Figure 24](#image-the-fixed-point-count-of-a-uniform-random-permutation-averaged-over-all-24-permutations-of-four-objects). The fixed point count of a uniform random permutation averaged over all $24$ permutations of four objects**. Each card lists $\pi(1),\pi(2),\pi(3),\pi(4)$. Green entries equal their positions and therefore mark [fixed points](function.md#fixed-point). The [probability mass function](probability-theory.md#probability-mass-function) on the right counts those cards; its [expected value](probability-theory.md#expected-value) is one.

Choose the $m$ fixed objects and derange the remaining $n-m$. Their count is $\binom nmD_{n-m}$ among $n!$ equally likely [permutations](#permutation). The [inclusion-exclusion principle](#inclusion-exclusion-principle) for $D_{n-m}$ proves the displayed law, valid for $0\le m\le n$ and zero otherwise. With $D_0=1$, it includes the all-fixed case and the impossibility of exactly $n-1$ fixed objects. For fixed $m$, the law tends to $e^{-1}/m!$, the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) of mean one.

### Cycle length of a tagged element in a uniform permutation

↑ **Parent:** [Permutation](#permutation)

In a uniformly random [permutation](#permutation) of $N$ objects, the cycle containing one specified object has a uniform length on $\{1,\ldots,N\}$. For length $\ell$, choose the other $\ell-1$ objects, arrange their order around the tagged object, and permute all remaining objects. The count is $\binom{N-1}{\ell-1}(\ell-1)!(N-\ell)!=(N-1)!$, independent of $\ell$. Its mean is $(N+1)/2$, while the mean number of other elements in that cycle is $(N-1)/2$.

### Derangement of a permutation

↑ **Parent:** [Permutation](#permutation)

A [permutation](#permutation) with no fixed points. Applying the [inclusion-exclusion principle](#inclusion-exclusion-principle) to the events that each element is fixed gives $D_n=n!\sum_{k=0}^n(-1)^k/k!$. Therefore $D_n/n!\to e^{-1}$, and the alternating-series remainder is at most $1/(n+1)!$.

// Destination: foundations-of-mathematics.bigb

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

The Lindeberg replacement method, inspired by the [Lindeberg condition](convergence-of-random-variables.md#lindeberg-condition), compares functions of two independent random vectors by replacing their coordinates one at a time. Matching moments cancel the corresponding terms in a [Taylor expansion](calculus.md#taylor-s-theorem).

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

## ← Incoming links (5)

- [Analysis of Boolean functions](#analysis-of-boolean-functions)
- [Borsuk-Ulam theorem](algebraic-topology.md#borsuk-ulam-theorem)
- [Coding theory](coding-theory.md)
- [Combinatorics](combinatorics.md)
- [Ramsey theory](ramsey-theory.md)
