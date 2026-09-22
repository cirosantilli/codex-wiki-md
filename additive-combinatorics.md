# Additive combinatorics

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Additive_combinatorics)

Additive combinatorics studies how the sizes and representation functions of [sumsets](#sumset) reveal algebraic structure in subsets of [abelian groups](group.md#abelian-group).

**Table of contents**

- [Furstenberg-Katznelson theorem](#furstenberg-katznelson-theorem)
- [Bracket-linear frequency function](#bracket-linear-frequency-function)
- [Four-term progression hypergraph encoding](#four-term-progression-hypergraph-encoding)
- [Roth theorem on three-term arithmetic progressions](#roth-theorem-on-three-term-arithmetic-progressions)
  - [Roth density increment on an integer progression](#roth-density-increment-on-an-integer-progression)
  - [Triangle-removal proof of Roth theorem](#triangle-removal-proof-of-roth-theorem)
  - [Classical Roth bound for three-term progressions](#classical-roth-bound-for-three-term-progressions)
  - [High-energy Roth theorem](#high-energy-roth-theorem)
- [Product set](#product-set)
  - [Multiplicative energy](#multiplicative-energy)
    - [Multiplicative energy sumset bound](#multiplicative-energy-sumset-bound)
- [Corner in an integer grid](#corner-in-an-integer-grid)
  - [Corners theorem](#corners-theorem)
- [Cut norm](#cut-norm)
- [Non-abelian additive combinatorics](#non-abelian-additive-combinatorics)
  - [Matrix-valued Gowers U2 quantity](#matrix-valued-gowers-u2-quantity)
    - [Spectral inverse theorem for the matrix-valued U2 quantity](#spectral-inverse-theorem-for-the-matrix-valued-u2-quantity)
    - [Matrix Fourier block](#matrix-fourier-block)
  - [Quasirandom group](#quasirandom-group)
    - [Product mixing in a quasirandom group](#product-mixing-in-a-quasirandom-group)
  - [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group)
    - [Right translation of a group function](#right-translation-of-a-group-function)
    - [Left translation of a group function](#left-translation-of-a-group-function)
    - [Fourier transform on a finite group](#fourier-transform-on-a-finite-group)
      - [Parseval identity on a finite group](#parseval-identity-on-a-finite-group)
      - [Fourier inversion on a finite group](#fourier-inversion-on-a-finite-group)
    - [Normalized convolution on a finite group](#normalized-convolution-on-a-finite-group)
      - [Convolution theorem on a finite group](#convolution-theorem-on-a-finite-group)
- [Box norm](#box-norm)
  - [Random sign rectangle fourth moment](#random-sign-rectangle-fourth-moment)
  - [Cut norm and rectangle fourth-moment equivalence](#cut-norm-and-rectangle-fourth-moment-equivalence)
  - [Three-dimensional box norm](#three-dimensional-box-norm)
    - [Pair-factor correlation bound for the three-dimensional box norm](#pair-factor-correlation-bound-for-the-three-dimensional-box-norm)
  - [Box norm singular-value identity](#box-norm-singular-value-identity)
  - [Bilinear correlation bound for the box norm](#bilinear-correlation-bound-for-the-box-norm)
    - [Triangle counting with one box-uniform pair and constant opposite degree](#triangle-counting-with-one-box-uniform-pair-and-constant-opposite-degree)
  - [Box Cauchy-Schwarz inequality](#box-cauchy-schwarz-inequality)
- [Sum-product phenomenon](#sum-product-phenomenon)
  - [Closure bounds for small skew-sumset scalars](#closure-bounds-for-small-skew-sumset-scalars)
    - [Polynomial skew-sumset expansion over a prime field](#polynomial-skew-sumset-expansion-over-a-prime-field)
  - [Quadratic growth of a sixfold product difference set](#quadratic-growth-of-a-sixfold-product-difference-set)
  - [Solymosi sum-product theorem over the complex numbers](#solymosi-sum-product-theorem-over-the-complex-numbers)
- [Density of a finite subset](#density-of-a-finite-subset)
  - [Balanced indicator function of a finite subset](#balanced-indicator-function-of-a-finite-subset)
- [Sidon set](#sidon-set)
  - [Sliding-window upper bound for Sidon sets](#sliding-window-upper-bound-for-sidon-sets)
  - [Bose-Chowla Sidon construction](#bose-chowla-sidon-construction)
- [Linear configuration count](#linear-configuration-count)
  - [Fourier stability of a linear configuration count](#fourier-stability-of-a-linear-configuration-count)
- [Transference principle in additive combinatorics](#transference-principle-in-additive-combinatorics)
  - [Test-function seminorm](#test-function-seminorm)
    - [Dual test-function norm](#dual-test-function-norm)
  - [Dense model theorem for a multiplicative test family](#dense-model-theorem-for-a-multiplicative-test-family)
    - [Polynomial approximation of the positive part](#polynomial-approximation-of-the-positive-part)
- [Sumset](#sumset)
  - [Translated Bohr neighborhood in a triple sumset](#translated-bohr-neighborhood-in-a-triple-sumset)
    - [Polynomial-length progression in a dense triple sumset](#polynomial-length-progression-in-a-dense-triple-sumset)
  - [Sum of a subset](#sum-of-a-subset)
  - [Distinct-positive-integer subset-sum lower bound](#distinct-positive-integer-subset-sum-lower-bound)
  - [Lexicographic embedding of a sumset](#lexicographic-embedding-of-a-sumset)
  - [Restricted sumset](#restricted-sumset)
  - [Plünnecke inequality](#plunnecke-inequality)
  - [Iterated sumset](#iterated-sumset)
- [Difference set](#difference-set)
- [Doubling constant](#doubling-constant)
  - [Polynomial growth of iterated sumsets](#polynomial-growth-of-iterated-sumsets)
  - [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality)
    - [Petridis minimal-growth lemma](#petridis-minimal-growth-lemma)
    - [Ruzsa triangle inequality](#ruzsa-triangle-inequality)
      - [Noncommutative Ruzsa triangle inequality](#noncommutative-ruzsa-triangle-inequality)
        - [Fourfold product bound from small tripling](#fourfold-product-bound-from-small-tripling)
        - [Small doubling does not control tripling in a noncommutative group](#small-doubling-does-not-control-tripling-in-a-noncommutative-group)
  - [Freiman-Ruzsa theorem](#freiman-ruzsa-theorem)
    - [Freiman theorem for integer sets](#freiman-theorem-for-integer-sets)
    - [Freiman-Ruzsa theorem over a finite field](#freiman-ruzsa-theorem-over-a-finite-field)
      - [Freiman-Ruzsa bound from Bogolyubov and linear modelling](#freiman-ruzsa-bound-from-bogolyubov-and-linear-modelling)
      - [Injective linear modelling of a small sumset](#injective-linear-modelling-of-a-small-sumset)
        - [Lifting a subspace through a Freiman model](#lifting-a-subspace-through-a-freiman-model)
    - [Szemerédi theorem in a bounded-rank coset progression](#szemeredi-theorem-in-a-bounded-rank-coset-progression)
    - [Small difference set forces a three-term arithmetic progression](#small-difference-set-forces-a-three-term-arithmetic-progression)
- [Approximate group](#approximate-group)
  - [Breuillard-Green-Tao structure theorem for approximate groups](#breuillard-green-tao-structure-theorem-for-approximate-groups)
  - [Higher product bound for an approximate group](#higher-product-bound-for-an-approximate-group)
  - [Intersection of an approximate group power with a subgroup](#intersection-of-an-approximate-group-power-with-a-subgroup)
  - [Large lower-step product in a torsion-free nilpotent approximate group](#large-lower-step-product-in-a-torsion-free-nilpotent-approximate-group)
    - [Large lifted product from a coset progression](#large-lifted-product-from-a-coset-progression)
      - [Fiber-counting lemma for a quotient map](#fiber-counting-lemma-for-a-quotient-map)
  - [Symmetric subset of a group](#symmetric-subset-of-a-group)
  - [Ruzsa covering lemma](#ruzsa-covering-lemma)
- [Additive energy](#additive-energy)
  - [Additive energy controls three-term progression mixing](#additive-energy-controls-three-term-progression-mixing)
  - [Additive energy of a frequency graph](#additive-energy-of-a-frequency-graph)
    - [Derivative correlations force additive frequency energy](#derivative-correlations-force-additive-frequency-energy)
      - [Squared derivative correlations force frequency-graph energy](#squared-derivative-correlations-force-frequency-graph-energy)
  - [Polynomial progression in a high-energy fourfold difference set](#polynomial-progression-in-a-high-energy-fourfold-difference-set)
  - [Popular sum](#popular-sum)
  - [Additive quadruple](#additive-quadruple)
  - [Balog-Szemerédi-Gowers theorem](#balog-szemeredi-gowers-theorem)
    - [Graph form of the Balog-Szemerédi-Gowers theorem](#graph-form-of-the-balog-szemeredi-gowers-theorem)
      - [Four-step path lemma for a dense bipartite graph](#four-step-path-lemma-for-a-dense-bipartite-graph)
    - [Small-difference-set form of the Balog-Szemerédi-Gowers theorem](#small-difference-set-form-of-the-balog-szemeredi-gowers-theorem)
- [Bogolyubov lemma](#bogolyubov-lemma)
  - [Cyclic Bogolyubov lemma with explicit phase radius](#cyclic-bogolyubov-lemma-with-explicit-phase-radius)
  - [Cyclic Bogolyubov lemma](#cyclic-bogolyubov-lemma)
  - [Finite-field Bogolyubov lemma](#finite-field-bogolyubov-lemma)
  - [Additive energy produces a large subspace in a fourfold difference set](#additive-energy-produces-a-large-subspace-in-a-fourfold-difference-set)
  - [Dense Bogolyubov-Ruzsa lemma](#dense-bogolyubov-ruzsa-lemma)
- [Bohr set](#bohr-set)
  - [Progression in a Bohr set from successive minima](#progression-in-a-bohr-set-from-successive-minima)
  - [Bohr set in phase-distance convention](#bohr-set-in-phase-distance-convention)
  - [Dilate of a Bohr set](#dilate-of-a-bohr-set)
  - [Regular Bohr set](#regular-bohr-set)
  - [Lower bound for the size of a Bohr set](#lower-bound-for-the-size-of-a-bohr-set)
  - [Arithmetic progression in a cyclic Bohr set](#arithmetic-progression-in-a-cyclic-bohr-set)
    - [Nonwrapping progression in a cyclic Bohr set](#nonwrapping-progression-in-a-cyclic-bohr-set)
- [Almost period of a function](#almost-period-of-a-function)
  - [Bohr-set almost periodicity of a convolution](#bohr-set-almost-periodicity-of-a-convolution)
  - [Lp almost period](#lp-almost-period)
    - [Finite-field convolution almost-periodicity theorem](#finite-field-convolution-almost-periodicity-theorem)
  - [Croot-Sisask almost-periodicity theorem](#croot-sisask-almost-periodicity-theorem)
  - [Finite-field character approximation](#finite-field-character-approximation)
- [Normalized Fourier analysis on a finite abelian group](#normalized-fourier-analysis-on-a-finite-abelian-group)
  - [Large Fourier coefficient from a deficit of three-term progressions](#large-fourier-coefficient-from-a-deficit-of-three-term-progressions)
  - [Fourth Fourier moment bound for an indicator function](#fourth-fourier-moment-bound-for-an-indicator-function)
  - [Fourier coefficient on a finite abelian group](#fourier-coefficient-on-a-finite-abelian-group)
  - [Linear phase](#linear-phase)
    - [Progression partition with nearly constant linear phase](#progression-partition-with-nearly-constant-linear-phase)
  - [Sixth Fourier moment as a three-sum collision count](#sixth-fourier-moment-as-a-three-sum-collision-count)
  - [Large spectrum](#large-spectrum)
    - [Chang theorem](#chang-theorem)
    - [Dissociated set](#dissociated-set)
- [Density increment](#density-increment)
  - [Hyperplane density increment for cap sets](#hyperplane-density-increment-for-cap-sets)
  - [Roth density-increment step](#roth-density-increment-step)
    - [One-frequency density increment on an integer interval](#one-frequency-density-increment-on-an-integer-interval)
    - [Fourier detection of a progression-free subset of an interval](#fourier-detection-of-a-progression-free-subset-of-an-interval)
  - [Bourgain bound for three-term-progression-free sets](#bourgain-bound-for-three-term-progression-free-sets)
    - [Bohr-set density increment lemma](#bohr-set-density-increment-lemma)
- [Meshulam theorem](#meshulam-theorem)
- [Finite-field Szemerédi theorem for four-term arithmetic progressions](#finite-field-szemeredi-theorem-for-four-term-arithmetic-progressions)
- [Gowers uniformity norm](#gowers-uniformity-norm)
  - [Multiplicative derivative](#multiplicative-derivative)
  - [Gowers U2 norm](#gowers-u2-norm)
    - [Quadratic phase detection by the Gowers U2 norm](#quadratic-phase-detection-by-the-gowers-u2-norm)
  - [Gowers U3 norm](#gowers-u3-norm)
    - [Quadratic uniformity of a set](#quadratic-uniformity-of-a-set)
      - [Four-term progressions in a quadratically uniform interval set](#four-term-progressions-in-a-quadratically-uniform-interval-set)
      - [Triangular weights count genuine four-term progressions](#triangular-weights-count-genuine-four-term-progressions)
    - [Generalized von Neumann inequality for four-term progressions](#generalized-von-neumann-inequality-for-four-term-progressions)
      - [Four-term progression bound with torsion factors](#four-term-progression-bound-with-torsion-factors)
        - [Unbounded torsion obstructs uniform control of four-term progressions](#unbounded-torsion-obstructs-uniform-control-of-four-term-progressions)
    - [Gowers U3 norm on an interval](#gowers-u3-norm-on-an-interval)
    - [Derivative identity for the Gowers U3 norm](#derivative-identity-for-the-gowers-u3-norm)
  - [Gowers inner product](#gowers-inner-product)
    - [Gowers-Cauchy-Schwarz inequality](#gowers-cauchy-schwarz-inequality)
  - [Quadratic phase](#quadratic-phase)
  - [Inverse theorem for the Gowers U3 norm over a finite field](#inverse-theorem-for-the-gowers-u3-norm-over-a-finite-field)
    - [Frequency graph extracted from a large Gowers U3 norm](#frequency-graph-extracted-from-a-large-gowers-u3-norm)
    - [Density-increment proof of the finite-field four-term progression theorem](#density-increment-proof-of-the-finite-field-four-term-progression-theorem)
- [Freiman homomorphism](#freiman-homomorphism)
  - [Freiman s-homomorphism](#freiman-s-homomorphism)
    - [Freiman s-isomorphism](#freiman-s-isomorphism)
      - [Freiman lifting of a progression](#freiman-lifting-of-a-progression)
      - [Freiman 2-isomorphism](#freiman-2-isomorphism)
        - [Minimal binary Freiman models have full fourfold sumset](#minimal-binary-freiman-models-have-full-fourfold-sumset)
    - [Ruzsa modelling lemma](#ruzsa-modelling-lemma)
      - [Cardinality-controlled cyclic Freiman model](#cardinality-controlled-cyclic-freiman-model)
      - [Cyclic Freiman model of a small-doubling integer set](#cyclic-freiman-model-of-a-small-doubling-integer-set)
      - [Half-size prime cyclic Freiman model](#half-size-prime-cyclic-freiman-model)
        - [Half-size cyclic Freiman model with a sharp difference-set bound](#half-size-cyclic-freiman-model-with-a-sharp-difference-set-bound)
  - [Second-difference obstruction to a Freiman homomorphism](#second-difference-obstruction-to-a-freiman-homomorphism)
  - [Large Freiman-homomorphic restriction from bounded derivative images](#large-freiman-homomorphic-restriction-from-bounded-derivative-images)
- [Generalized arithmetic progression](#generalized-arithmetic-progression)
  - [Abelian progression](#abelian-progression)
  - [Coset progression](#coset-progression)

## Furstenberg-Katznelson theorem

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

The multidimensional [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem) says that a subset $A\subseteq\mathbb Z^d$ with positive upper density contains a translated positive integer dilate $a+tF$ of every finite set $F\subseteq\mathbb Z^d$. In the finite formulation, for every $\alpha>0$ and finite $F$, all sufficiently large integer boxes have this property for every subset occupying at least an $\alpha$ fraction of the box. The one-dimensional case for $F=\{0,1,\ldots,r-1\}$ is the [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem). The general result follows from multiple recurrence for commuting measure-preserving transformations.

## Bracket-linear frequency function

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

A frequency function built from an affine variable and its [fractional part](calculus.md#fractional-part). Irrational $\gamma$ and $\beta$ can give many exact additive relations because each pair sum has only two possible floor carries. For example $\beta=\sqrt3$, $\gamma=\sqrt2$ gives $\gg N^3$ additive quadruples on $[-N,N]$, but agreement with every ordinary affine function occurs on only $o(N)$ shifts. Integer floor points underlying affine agreement must be collinear.

## Four-term progression hypergraph encoding

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

Use four parts indexed by $0,1,2,3$ in a [cyclic group](group.md#cyclic-group) $G$, and include the triple missing part $i$ when $L_i\in A$. A transversal [three-uniform tetrahedron](hypergraph.md#three-uniform-tetrahedron) then has the four values $S_1-iS_0$, where $S_0=\sum_jx_j$ and $S_1=\sum_jjx_j$, so it encodes a four-term [arithmetic progression](arithmetic.md#arithmetic-progression). Constant progressions give $|A||G|^2$ edge-disjoint tetrahedra. This is the bridge from the [tetrahedron removal lemma](hypergraph.md#tetrahedron-removal-lemma) to the [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem).

## Roth theorem on three-term arithmetic progressions

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

For every $\delta>0$, every sufficiently long integer interval has a nonconstant three-term [arithmetic progression](arithmetic.md#arithmetic-progression) in each subset of [subset density](#density-of-a-finite-subset) at least $\delta$. This is a theorem about [additive combinatorics](additive-combinatorics.md), distinct from the [Roth theorem](number-theory.md#roth-s-theorem) on approximation of algebraic irrational numbers. The [Roth density-increment step](#roth-density-increment-step) proves it by repeatedly increasing [subset density](#density-of-a-finite-subset) on a shorter [arithmetic progression](arithmetic.md#arithmetic-progression).

### Roth density increment on an integer progression

↑ **Parent:** [Roth theorem on three-term arithmetic progressions](#roth-theorem-on-three-term-arithmetic-progressions)

If a density-$\delta$ subset of a sufficiently long integer interval has no nonconstant three-term arithmetic progression, Fourier expansion of the progression count gives a large coefficient of its balanced indicator. Dirichlet approximation supplies a step at most $\sqrt N$ on which that character varies slowly. Partitioning the interval into equal-length progressions of that step, and controlling the short tails, produces the displayed density increment. Iteration must terminate since density cannot exceed one. The same argument treats the three-point pattern with coefficients $2,-3,1$.

### Triangle-removal proof of Roth theorem

↑ **Parent:** [Roth theorem on three-term arithmetic progressions](#roth-theorem-on-three-term-arithmetic-progressions)

Embed $A\subseteq[N]$ in the odd [cyclic group](group.md#cyclic-group) $G=\mathbb Z/(2N+1)\mathbb Z$, so additive three-term relations in $A$ cannot wrap around. Form three copies of $G$, putting [edges](graph-theory.md#edge-of-a-graph) $x\!\sim\!y$ when $y-x\in A$, $y\!\sim\!z$ when $z-y\in A$, and $x\!\sim\!z$ when $(z-x)/2\in A$. A [triangle in a graph](graph.md#triangle-in-a-graph) encodes $a+b=2c$ in $A$. If $A$ has no nonconstant [arithmetic progression](arithmetic.md#arithmetic-progression), every [triangle in a graph](graph.md#triangle-in-a-graph) has $a=b=c$; there are exactly $|G||A|$ [triangles in a graph](graph.md#triangle-in-a-graph), and they are edge-disjoint. Thus at least $|G||A|$ [edges](graph-theory.md#edge-of-a-graph) must be removed to eliminate them. For fixed positive [subset density](#density-of-a-finite-subset) of $A$, this is a positive fraction of the squared [vertex](graph.md#vertex-graph-theory) count, whereas the [triangle in a graph](graph.md#triangle-in-a-graph) count is only quadratic. The [triangle removal lemma](probabilistic-combinatorics.md#triangle-removal-lemma) permits deletion of an arbitrarily small quadratic fraction when the cubic [triangle in a graph](graph.md#triangle-in-a-graph) [subset density](#density-of-a-finite-subset) is sufficiently small. This contradiction establishes [Roth theorem on three-term arithmetic progressions](#roth-theorem-on-three-term-arithmetic-progressions).

### Classical Roth bound for three-term progressions

↑ **Parent:** [Roth theorem on three-term arithmetic progressions](#roth-theorem-on-three-term-arithmetic-progressions)

Write $r_3(N)$ for the maximum [cardinality](set-theory.md#cardinality) of a [subset](set.md#subset) of $[N]$ containing no nonconstant three-term [arithmetic progression](arithmetic.md#arithmetic-progression). There is an absolute constant $C$ such that every three-term-progression-free [subset](set.md#subset) $A\subseteq[N]$ satisfies $|A|\leq CN/\log\log N$ for $N\geq3$. A quantitative [Roth density-increment step](#roth-density-increment-step) gives, for [subset density](#density-of-a-finite-subset) $\delta$ and $N\geq4\cdot10^6\delta^{-4}$, a [arithmetic progression](arithmetic.md#arithmetic-progression) of length at least $\delta^2\sqrt N/2000$ and increased [subset density](#density-of-a-finite-subset) at least $\delta+\delta^2/64$. The increment decreases reciprocal [subset density](#density-of-a-finite-subset) by at least $1/65$, so fewer than $\lceil65/\delta\rceil$ iterations are possible. If $N_j$ is the successive length, then $\log N_{j+1}\geq\frac12\log N_j-\log(2000/\delta^2)$, using the initial [subset density](#density-of-a-finite-subset) to bound all later ones. Hence $\log N_j\geq2^{-j}\log N-2\log(2000/\delta^2)$. If $\delta\log\log N$ exceeds a sufficiently large absolute constant, all these intervals remain above the [density increment](#density-increment) threshold, a contradiction. This proves the displayed bound. The result is a classical quantitative version of [Roth theorem on three-term arithmetic progressions](#roth-theorem-on-three-term-arithmetic-progressions), without asserting an optimal bound.

### High-energy Roth theorem

↑ **Parent:** [Roth theorem on three-term arithmetic progressions](#roth-theorem-on-three-term-arithmetic-progressions)

For fixed $\theta>0$, a sufficiently large finite set of [integers](number-theory.md#integer) with [additive energy](#additive-energy) at least $\theta|A|^3$ has a nonconstant three-term [arithmetic progression](arithmetic.md#arithmetic-progression). The [Balog-Szemerédi-Gowers theorem](#balog-szemeredi-gowers-theorem) and [Ruzsa modelling lemma](#ruzsa-modelling-lemma) reduce the problem to the [Roth theorem on three-term arithmetic progressions](#roth-theorem-on-three-term-arithmetic-progressions) in a dense cyclic model.

## Product set

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

The product set of two sets of real numbers is $A\cdot B=\{ab:a\in A,b\in B\}$. It is a multiplicative counterpart of a [sumset](#sumset), not the [Cartesian product](set-theory.md#cartesian-product) $A\times B$.

### Multiplicative energy

↑ **Parent:** [Product set](#product-set)

For finite sets of nonzero real numbers, the multiplicative energy is the number of quadruples $(a,b,c,d)\in A\times B\times A\times B$ satisfying $a/b=c/d$. Swapping $b,d$ shows that it also counts quadruples with $ab=cd$. Thus $E(A,B)=\sum_x r_{A\cdot B}(x)^2$, where $r_{A\cdot B}(x)$ counts product representations. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) yields $E(A,B)\geq |A|^2|B|^2/|A\cdot B|$.

#### Multiplicative energy sumset bound

↑ **Parent:** [Multiplicative energy](#multiplicative-energy)

For finite sets of positive real numbers $A,B$ with $|B|\geq2$, $E(A,B)\leq4\lceil\log|B|\rceil|A+A||B+B|$, with natural or binary [logarithm](calculus.md#logarithm). Partition ray occupancies of $A\times B$ into $\lceil\log|B|\rceil$ classes of multiplicative width $e$, or width $2$ for the binary convention. [Injectivity of sums on two distinct rays](geometry-and-topology.md#injectivity-of-sums-on-two-distinct-rays) and disjoint [open planar sectors](geometry-and-topology.md#open-planar-sector) bound each class's sum of squared occupancies by $4|A+A||B+B|$. A singleton class contributes at most $|A||B|$. Combining this with the energy lower bound gives a sum-product inequality.

## Corner in an integer grid

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

A corner consists of these three points in the [integer](number-theory.md#integer) grid, all contained in the set being studied. The displacement may be positive or negative, but must be nonzero, so the points are distinct. The [corners theorem](#corners-theorem) guarantees a corner in every subset of positive fixed [density of a finite subset](#density-of-a-finite-subset) of a sufficiently large square grid.

### Corners theorem

↑ **Parent:** [Corner in an integer grid](#corner-in-an-integer-grid)

For every $\delta>0$, all sufficiently large integers $n$ have the property that every $A\subseteq[n]^2$ with $|A|\geq\delta n^2$ contains a [corner in an integer grid](#corner-in-an-integer-grid). The [tripartite graph encoding of a grid](graph.md#tripartite-graph-encoding-of-a-grid) turns the absence of a corner into a family of many [edge-disjoint triangles](graph.md#edge-disjoint-triangles) but only quadratically many total [triangles in a graph](graph.md#triangle-in-a-graph), contradicting the [triangle removal lemma](probabilistic-combinatorics.md#triangle-removal-lemma).

## Cut norm

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

For a [real-valued function](function.md#real-valued-function) $H$ on a nonempty finite [Cartesian product](set-theory.md#cartesian-product) $X\times Y$, its normalized cut norm is the maximum of $|\mathbb E_{x,y}H(x,y)1_A(x)1_B(y)|$ over $A\subseteq X,B\subseteq Y$. It measures all rectangular subset discrepancies. The convention using arbitrary test functions bounded by one is equivalent within a factor of four, by decomposing their positive and negative parts into [indicator functions](measure-theory.md#indicator-function).

## Non-abelian additive combinatorics

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

Non-abelian additive combinatorics studies product sets and configuration counts in noncommutative [groups](group.md). [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group) and [quasirandom groups](#quasirandom-group) connect small-dimensional [group representations](representation-theory.md#group-representation) with multiplicative mixing.

### Matrix-valued Gowers U2 quantity

↑ **Parent:** [Non-abelian additive combinatorics](#non-abelian-additive-combinatorics)

For $f:G\to M_n(\mathbb C)$ on a [finite group](group.md#finite-group), use uniform [expectation](probability-theory.md#expected-value) over the solutions of $xy^{-1}zw^{-1}=e$ and the ordinary, unnormalized [trace](linear-algebra.md#matrix-trace) to define the displayed fourth-order quantity. If $T_\rho$ is its [matrix Fourier block](#matrix-fourier-block), this quantity equals $\sum_\rho d_\rho\operatorname{Tr}((T_\rho T_\rho^*)^2)$, so it is real and nonnegative. For a scalar function on an [abelian group](group.md#abelian-group), it reduces to the usual fourth power of the [Gowers uniformity norm](#gowers-uniformity-norm) of order two. The unnormalized [trace](linear-algebra.md#matrix-trace) means a unitary matrix-valued function can have fourth-order quantity as large as $n$.

#### Spectral inverse theorem for the matrix-valued U2 quantity

↑ **Parent:** [Matrix-valued Gowers U2 quantity](#matrix-valued-gowers-u2-quantity)

If $\|f(x)\|_{\mathrm{op}}\leq1$ and $\|f\|_{U^2}^4\geq cn>0$, select the [singular values](linear-algebra.md#singular-value) $\lambda_p\geq\sqrt{c/2}$ of the [matrix Fourier blocks](#matrix-fourier-block). Their weighted count $m=\sum_pd_{\rho_p}$ lies between $cn/2$ and $2n/c$. Scaling unit [right singular vectors](linear-algebra.md#right-singular-vector) and their corresponding unit [left singular vectors](linear-algebra.md#left-singular-vector) by $\sqrt{d_{\rho_p}}$ gives matrices $U(p),V(p)$ satisfying $\mathbb E_xf(x)U(p)\rho_p(x)^*=\lambda_pV(p)$ and [Hilbert-Schmidt inner product](compact-operator.md#hilbert-schmidt-inner-product) orthogonality within each chosen [irreducible representation](representation-theory.md#irreducible-representation). The [Schur averaging of rectangular matrices](representation-theory.md#schur-averaging-of-rectangular-matrices) then gives $\mathbb E_x\|UP(x)^*b\|_2^2=\|b\|_2^2$ for the concatenated $U$ and the corresponding [block diagonal matrix](vector-space.md#block-diagonal-matrix) $P(x)$.

#### Matrix Fourier block

↑ **Parent:** [Matrix-valued Gowers U2 quantity](#matrix-valued-gowers-u2-quantity)

For $f:G\to M_n(\mathbb C)$ and a degree-$d_\rho$ [unitary irreducible representation](representation-theory.md#unitary-irreducible-representation), the matrix Fourier block is the operator $T_\rho$ on $M_{n\times d_\rho}(\mathbb C)$ defined in the title. Its [singular values](linear-algebra.md#singular-value) $\lambda_{\rho,j}$ satisfy

$$
\sum_{\rho,j}d_\rho\lambda_{\rho,j}^2=\mathbb E_x\|f(x)\|_{\mathrm{HS}}^2,
\qquad
\sum_{\rho,j}d_\rho\lambda_{\rho,j}^4=\|f\|_{U^2}^4.
$$

Pointwise [operator norm](continuous-dual-space.md#operator-norm) at most one implies $\|T_\rho\|_{\mathrm{op}}\leq1$. These blocks are operators on a matrix space, rather than simply the entrywise scalar [Fourier transform on a finite group](#fourier-transform-on-a-finite-group) without any reshaping.

### Quasirandom group

↑ **Parent:** [Non-abelian additive combinatorics](#non-abelian-additive-combinatorics)

A [finite group](group.md#finite-group) is $m$-quasirandom if every nontrivial [irreducible representation](representation-theory.md#irreducible-representation) over the [complex numbers](complex-analysis.md#complex-number) has degree at least $m$. The [trivial representation](representation-theory.md#trivial-representation) is excluded. Large $m$ suppresses correlations of products of arbitrary subsets, through [product mixing in a quasirandom group](#product-mixing-in-a-quasirandom-group).

#### Product mixing in a quasirandom group

↑ **Parent:** [Quasirandom group](#quasirandom-group)

For an $m$-[quasirandom group](#quasirandom-group), uniform [expectations](probability-theory.md#expected-value), and the [normalized convolution on a finite group](#normalized-convolution-on-a-finite-group), a scalar [mean-zero function](probability-theory.md#mean-zero-function) $f$ satisfies

$$
\|f*g\|_2\leq m^{-1/2}\|f\|_2\|g\|_2.
$$

The [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group) proof bounds each nontrivial matrix component of $f$ in [operator norm](continuous-dual-space.md#operator-norm) using its weighted [Hilbert-Schmidt norm](compact-operator.md#hilbert-schmidt-norm). For subsets of [subset density](#density-of-a-finite-subset) values $a,b,c$, the error in their normalized product count is at most $\sqrt{a(1-a)b(1-b)c(1-c)/m}$. In particular $abc>1/m$ guarantees a solution of $xy=z$ in the three subsets.

### Fourier analysis on a finite group

↑ **Parent:** [Non-abelian additive combinatorics](#non-abelian-additive-combinatorics)

For a [finite group](group.md#finite-group), choose one [unitary irreducible representation](representation-theory.md#unitary-irreducible-representation) $\rho$ of degree $d_\rho$ from each equivalence class. One consistent normalized [Fourier transform on a finite group](#fourier-transform-on-a-finite-group) convention is $\widehat f(\rho)=\mathbb E_xf(x)\rho(x)$. The [Schur orthogonality relations](representation-theory.md#schur-orthogonality-relations) give

$$
f(x)=\sum_\rho d_\rho\operatorname{tr}(\widehat f(\rho)\rho(x)^*),
\qquad
\mathbb E_x|f(x)|^2=\sum_\rho d_\rho\|\widehat f(\rho)\|_{\mathrm{HS}}^2.
$$

The [normalized convolution on a finite group](#normalized-convolution-on-a-finite-group) satisfies $\widehat{f*g}(\rho)=\widehat f(\rho)\widehat g(\rho)$ in this convention. Using $\rho(x)^*$ in the transform instead reverses that product order for scalar functions with the same [normalized convolution on a finite group](#normalized-convolution-on-a-finite-group) convention. The [Fourier transform on a finite group](#fourier-transform-on-a-finite-group) has matrix-valued components even when the original function is scalar-valued.

#### Right translation of a group function

↑ **Parent:** [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group)

For a scalar function on a [group](group.md), use $(R_af)(x)=f(xa)$ as the right-translation convention. For [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group) this gives $\widehat{R_af}(\rho)=\widehat f(\rho)\rho(a)^*$. Specifying whether $a$ or $a^{-1}$ appears in the definition avoids sign and multiplication-order ambiguity.

#### Left translation of a group function

↑ **Parent:** [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group)

For a scalar function on a [group](group.md), left translation by $a$ is $(L_af)(x)=f(a^{-1}x)$. With the positive-representation convention for [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group), $\widehat{L_af}(\rho)=\rho(a)\widehat f(\rho)$.

#### Fourier transform on a finite group

↑ **Parent:** [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group)

For a scalar function on a [finite group](group.md#finite-group), one normalized transform convention assigns the matrix $\mathbb E_xf(x)\rho(x)$ to each chosen [unitary irreducible representation](representation-theory.md#unitary-irreducible-representation). This map is a weighted [Hilbert space](hilbert-space.md) isomorphism by the [Parseval identity on a finite group](#parseval-identity-on-a-finite-group). Another common convention uses $\rho(x)^*$; the corresponding [convolution theorem on a finite group](#convolution-theorem-on-a-finite-group) then reverses the matrix product order for $(f*g)(x)=\mathbb E_yf(y)g(y^{-1}x)$.

##### Parseval identity on a finite group

↑ **Parent:** [Fourier transform on a finite group](#fourier-transform-on-a-finite-group)

For the [Fourier transform on a finite group](#fourier-transform-on-a-finite-group), the displayed identity uses uniform [expectation](probability-theory.md#expected-value) in the original function space and a weighted [Hilbert-Schmidt inner product](compact-operator.md#hilbert-schmidt-inner-product) in the matrix components. In particular $\|f\|_2^2=\sum_\rho d_\rho\|\widehat f(\rho)\|_{\mathrm{HS}}^2$. For an [abelian group](group.md#abelian-group), all $d_\rho=1$, and the identity becomes a sum of squared scalar coefficients.

##### Fourier inversion on a finite group

↑ **Parent:** [Fourier transform on a finite group](#fourier-transform-on-a-finite-group)

The [Fourier transform on a finite group](#fourier-transform-on-a-finite-group) convention $\widehat f(\rho)=\mathbb E_xf(x)\rho(x)$ has the displayed inversion formula. The sum is over one representative from each equivalence class of [unitary irreducible representations](representation-theory.md#unitary-irreducible-representation). It follows from the [Schur orthogonality relations](representation-theory.md#schur-orthogonality-relations) and the [regular representation](representation-theory.md#regular-representation) decomposition, and holds at every group element without a limiting argument.

#### Normalized convolution on a finite group

↑ **Parent:** [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group)

For scalar functions on a [finite group](group.md#finite-group), [normalized convolution on a finite group](#normalized-convolution-on-a-finite-group) is $(f*g)(x)=|G|^{-1}\sum_y f(y)g(y^{-1}x)$. It is associative and need not commute. Its identity is $|G|1_{\{e\}}$, rather than the unscaled [indicator function](measure-theory.md#indicator-function) of the identity element. The [Fourier analysis on a finite group](#fourier-analysis-on-a-finite-group) convention $\widehat f(\rho)=\mathbb E f(x)\rho(x)$ turns it into matrix multiplication in the same order.

##### Convolution theorem on a finite group

↑ **Parent:** [Normalized convolution on a finite group](#normalized-convolution-on-a-finite-group)

The [normalized convolution on a finite group](#normalized-convolution-on-a-finite-group) and the [Fourier transform on a finite group](#fourier-transform-on-a-finite-group) convention with $\rho(x)$ satisfy the displayed identity. Substitute $x=yz$ in the defining [expectation](probability-theory.md#expected-value) and use $\rho(yz)=\rho(y)\rho(z)$. With the convention using $\rho(x)^*$ instead, the scalar convolution has transform $\widehat g(\rho)\widehat f(\rho)$; multiplication order matters for noncommutative [groups](group.md).

## Box norm

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

For nonempty [finite sets](set.md#finite-set) $X,Y$ and a [function](function.md) $f:X\times Y\to\mathbb C$ on their [Cartesian product](set-theory.md#cartesian-product), using uniform [expectations](probability-theory.md#expected-value), define

$$
\|f\|_{\square}^4=\mathbb E_{x,x',y,y'}f(x,y)\overline{f(x',y)}\overline{f(x,y')}f(x',y').
$$

This equals $\mathbb E_{y,y'}|\mathbb E_xf(x,y)\overline{f(x,y')}|^2$. Hence it is nonnegative, and vanishing forces $f=0$ by taking $y=y'$. Absolute homogeneity and the [box Cauchy-Schwarz inequality](#box-cauchy-schwarz-inequality) establish that it is a [norm](functional-analysis.md#norm). For a [real-valued function](function.md#real-valued-function) the complex conjugates can be omitted. The [bilinear correlation bound for the box norm](#bilinear-correlation-bound-for-the-box-norm) also holds for complex functions.

### Random sign rectangle fourth moment

↑ **Parent:** [Box norm](#box-norm)

Give every entry of an $m$ by $n$ matrix an independent uniformly random sign. A four-entry rectangle product has expectation zero unless its two row indices coincide or its two column indices coincide; in those cases it is one. Counting the union of these diagonal cases gives $mn^2+m^2n-mn$ before normalization. Thus some sign matrix has [box norm](#box-norm) fourth power at most the displayed expectation, and its [cut norm](#cut-norm) tends to zero when both dimensions tend to infinity.

### Cut norm and rectangle fourth-moment equivalence

↑ **Parent:** [Box norm](#box-norm)

For a real function $f$ bounded by one on a finite Cartesian product, the fourth power of its [box norm](#box-norm) is the mean of $f(x,y)f(x,y')f(x',y)f(x',y')$. Two applications of the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bound every rectangular discrepancy by the [box norm](#box-norm). Conversely, decompose each bounded real test function into positive and negative parts and use the [layer cake representation](functional-analysis.md#layer-cake-representation). Its bilinear pairing with $f$ is at most four times the [cut norm](#cut-norm). Applying this to the row and column tests furnished by fixed $x',y'$ bounds the fourth moment by four times the [cut norm](#cut-norm). These dimension-independent estimates make the two notions of small discrepancy equivalent.

### Three-dimensional box norm

↑ **Parent:** [Box norm](#box-norm)

For a complex function on $X_1\times X_2\times X_3$, its eighth power is the average of the conjugated product over the eight vertices of a coordinate cube. Three successive applications of the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) show that it bounds correlation with a product of three bounded functions, each omitting one coordinate. This is the analytic estimate behind the [tetrahedron counting lemma](hypergraph.md#tetrahedron-counting-lemma).

#### Pair-factor correlation bound for the three-dimensional box norm

↑ **Parent:** [Three-dimensional box norm](#three-dimensional-box-norm)

For a real [function](function.md) $g$ on $X\times Y\times Z$ and [functions](function.md) $a(y,z),b(x,z),c(x,y)$ bounded in absolute value by one,

$$
|\mathbb E_{x,y,z}g(x,y,z)a(y,z)b(x,z)c(x,y)|\leq\|g\|_{\square^3}.
$$

First apply [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) in $(y,z)$ to remove $a$, duplicating $x$. Apply it in $(x_0,x_1,z)$ to remove $b(x_0,z)b(x_1,z)$, duplicating $y$. Finally apply it in $(x_0,x_1,y_0,y_1)$ to remove the four $c$ factors, duplicating $z$. The resulting eighth-power bound is exactly the eight-factor average defining the [three-dimensional box norm](#three-dimensional-box-norm). [Functions](function.md) depending on just one coordinate, or constants, can be incorporated in any of the three pair factors.

### Box norm singular-value identity

↑ **Parent:** [Box norm](#box-norm)

For a [real-valued function](function.md#real-valued-function) $H$ on a nonempty finite [Cartesian product](set-theory.md#cartesian-product), let $T_Hv(x)=\mathbb E_yH(x,y)v(y)$ with uniform [inner products](linear-algebra.md#inner-product). The [box norm](#box-norm) obeys $\|H\|_\square^4=\operatorname{Tr}((T_HT_H^*)^2)=\sum_j\sigma_j^4$, where $\sigma_j$ are its [singular values](linear-algebra.md#singular-value). For a [biregular graph](graph-theory.md#biregular-graph) this separates the constant component $\gamma^4$ from the other fourth powers.

### Bilinear correlation bound for the box norm

↑ **Parent:** [Box norm](#box-norm)

With uniform [expectations](probability-theory.md#expected-value) and real or complex [functions](function.md),

$$
|\mathbb E_{x,y}f(x,y)u(x)v(y)|\leq\|f\|_{\square}\|u\|_2\|v\|_2.
$$

Apply the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) first in $y$. Expand the remaining square, and apply the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) in $(x,x')$ to $u(x)u(x')$ and $\mathbb E_y f(x,y)f(x',y)$. Their squared averages are $\|u\|_2^4$ and $\|f\|_{\square}^4$, respectively.

#### Triangle counting with one box-uniform pair and constant opposite degree

↑ **Parent:** [Bilinear correlation bound for the box norm](#bilinear-correlation-bound-for-the-box-norm)

Let a [tripartite graph](graph.md#tripartite-graph) have nonempty parts $X,Y,Z$, pair [edge density of a bipartite graph](probabilistic-combinatorics.md#edge-density-of-a-bipartite-graph) values $\alpha,\beta,\gamma$ on $XY,YZ,XZ$, and $\|G(X,Y)-\alpha\|_{\square}\leq c$. If every $z\in Z$ has exactly $\beta|Y|$ neighbors in $Y$, its normalized [triangle count](graph.md#triangle-count) $\tau$ obeys

$$
|\tau-\alpha\beta\gamma|\leq c\sqrt{\beta\gamma}.
$$

The constant-degree assumption makes the contribution of the constant $\alpha$ exactly $\alpha\beta\gamma$. For each fixed $z$, apply the [bilinear correlation bound for the box norm](#bilinear-correlation-bound-for-the-box-norm) to the [indicator functions](measure-theory.md#indicator-function) of its two [vertex neighbourhoods](graph.md#vertex-neighbourhood). Their squared $L^2$ [norms](functional-analysis.md#norm) are $\beta$ and the relative $X$-degree of $z$. Average over $z$ and use the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to bound the mean square root of that degree by $\sqrt\gamma$.

### Box Cauchy-Schwarz inequality

↑ **Parent:** [Box norm](#box-norm)

For four [real-valued functions](function.md#real-valued-function) on a finite [Cartesian product](set-theory.md#cartesian-product), let $\Lambda(f_{00},f_{01},f_{10},f_{11})=\mathbb E_{x_0,x_1,y_0,y_1}\prod_{i,j=0}^1 f_{ij}(x_i,y_j)$. Repeated [Cauchy-Schwarz inequalities](probability-and-statistics.md#cauchy-schwarz-inequality) give

$$
|\Lambda(f_{00},f_{01},f_{10},f_{11})|\leq\prod_{i,j=0}^1\|f_{ij}\|_{\square}.
$$

First separate the two $y$ averages and apply [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) in $(x_0,x_1)$. Each resulting squared factor is $\mathbb E_{y,y'}(\mathbb E_x f(x,y)f(x,y'))(\mathbb E_x g(x,y)g(x,y'))$, bounded by $\|f\|_{\square}^2\|g\|_{\square}^2$ by another [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Expanding the four factors of $f+g$ and applying this inequality to each of the sixteen terms gives the [triangle inequality](topological-analysis.md#triangle-inequality) for the [box norm](#box-norm).

## Sum-product phenomenon

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sum-product_phenomenon)

The sum-product phenomenon says that a finite subset of a [field](algebra.md#field) cannot usually have both a small [sumset](#sumset) and a small product set unless it has additional subfield-like structure.

### Closure bounds for small skew-sumset scalars

↑ **Parent:** [Sum-product phenomenon](#sum-product-phenomenon)

Write $D(t)=|A+tA|/|A|$ and suppose some nonzero $b$ has $D(b)\leq K$. The mixed-set [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality) gives $|3A-2A|\leq K^5|A|$ and $|A+A|\leq K^2|A|$. The [Ruzsa covering lemma](#ruzsa-covering-lemma) covers $tA$ by at most $D(t)$ translates of $A-A$. Covering two dilates proves the addition bound. First covering $sA$, then both copies of $rA$ in $r(A-A)$, proves the multiplication bound. The [Ruzsa triangle inequality](#ruzsa-triangle-inequality) also gives $D(-r)\leq K^2D(r)$. These bounds transfer controlled additive expansion through a bounded-complexity expression in [scalars](vector-space.md#scalar).

#### Polynomial skew-sumset expansion over a prime field

↑ **Parent:** [Closure bounds for small skew-sumset scalars](#closure-bounds-for-small-skew-sumset-scalars)

For positive $\alpha,\beta$, suppose $p^\alpha\leq|A|\leq p^{1-\alpha}$ and $|B|\geq p^\beta$. Repeatedly replace a [scalar](vector-space.md#scalar) set $S$ by $3SS-3SS$. [Quadratic growth of a sixfold product difference set](#quadratic-growth-of-a-sixfold-product-difference-set) reaches size at least $p/2$ in a number of steps depending only on $\beta$. The [closure bounds for small skew-sumset scalars](#closure-bounds-for-small-skew-sumset-scalars) transfer a putative bound $|A+bA|\leq K|A|$ to all these [scalars](vector-space.md#scalar) with exponent depending only on the number of steps. Averaging collisions over the resulting large [scalar](vector-space.md#scalar) set then forces $K^L\geq\frac14\min(|A|,p/|A|)\geq p^\alpha/4$. This supplies a positive exponent depending only on $\alpha,\beta$. The finitely many smaller primes are covered by the strict inequality $|A+bA|>|A|$ for every nonzero $b$ when $1<|A|<p$.

### Quadratic growth of a sixfold product difference set

↑ **Parent:** [Sum-product phenomenon](#sum-product-phenomenon)

For $S\subseteq\mathbb F_p$ with $|S|\geq2$, put $R=(S-S)/(S-S)$ using nonzero denominators. If $R$ is proper, some $r\in R+1$ lies outside $R$, since invariance under addition of one would give all of the [prime field](algebra.md#prime-field). The map $(x,y)\mapsto x+ry$ on $S^2$ is injective. Clearing the denominator in a representation of $r-1$ puts a dilate of its image inside $3SS-3SS$. If $R$ is the full field, averaging the collision count of $S+rS$ gives some $r$ with $|S+rS|\geq\frac12\min(p,|S|^2)$. Clearing its denominator puts a dilate inside $2SS-2SS\subseteq3SS-3SS$. Here $SS$ is a [product set](#product-set), and the prefactors denote repeated [sumsets](#sumset), not [scalar](vector-space.md#scalar) multiplication.

### Solymosi sum-product theorem over the complex numbers

↑ **Parent:** [Sum-product phenomenon](#sum-product-phenomenon)

For finite $U,V,W\subseteq\mathbb C$ with $U\ne\{0\}$ and $W\ne\{0\}$,

$$
|U+V|\,|UW|
\geq\frac1{56}|U|^{3/2}|V|^{1/2}|W|^{1/2}.
$$

In particular, addition and multiplication cannot both expand a nontrivial finite set of [complex numbers](complex-analysis.md#complex-number) only slightly.

## Density of a finite subset

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

The density of $A$ in a nonempty finite ambient set $X$ is the proportion $|A|/|X|$.

### Balanced indicator function of a finite subset

↑ **Parent:** [Density of a finite subset](#density-of-a-finite-subset)

For nonempty [finite set](set.md#finite-set) $I$ and $A\subseteq I$, let $\alpha=|A|/|I|$ be the [density of a finite subset](#density-of-a-finite-subset). The balanced [indicator function](measure-theory.md#indicator-function) $f=1_A-\alpha1_I$, extended by zero to an ambient finite [group](group.md), has sum zero and vanishing zero [Fourier coefficient](fourier-series.md#fourier-coefficient). The sum of $f$ on a subset $P\subseteq I$ is $|A\cap P|-\alpha|P|$, measuring the excess [density of a finite subset](#density-of-a-finite-subset) there.

## Sidon set

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sidon_set)

A Sidon set in an [abelian group](group.md#abelian-group) is a subset $A$ for which an equality $a+b=c+d$ with $a,b,c,d\in A$ forces the unordered pairs $\{a,b\}$ and $\{c,d\}$ to be equal. Equivalently, the ordered nonzero differences $a-b$ with $a\ne b$ are all distinct.

### Sliding-window upper bound for Sidon sets

↑ **Parent:** [Sidon set](#sidon-set)

For a [Sidon set](#sidon-set) $A\subseteq[1,N]$, put $m=|A|$ and let $A_i$ count points in a window of $u$ consecutive integers. Each point occurs in $u$ windows, so $\sum A_i=um$. [Cauchy-Schwarz](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\sum\binom{A_i}2\geq[u^2m^2/(N+u)-um]/2$. Each positive difference occurs at most once and contributes $u-d$ windows, giving the upper bound $u(u-1)/2$. Thus $m^2\leq(N+u)(1+(m-1)/u)$. Taking $u=\lfloor N^{3/4}\rfloor$ gives the displayed estimate, which combines with the [Bose-Chowla Sidon construction](#bose-chowla-sidon-construction) to determine the asymptotic maximum.

### Bose-Chowla Sidon construction

↑ **Parent:** [Sidon set](#sidon-set)

Choose a generator $\theta$ of the multiplicative group of the quadratic [finite field extension](algebra.md#finite-field-extension). Its $p$ shifts $\theta+t$ define $p$ distinct exponents modulo $p^2-1$. Equality of two sums of exponents gives $(\theta+s)(\theta+t)=(\theta+u)(\theta+v)$. Since $1,\theta$ are independent over the prime field, $s+t=u+v$ and $st=uv$, so the unordered pairs coincide. Thus the exponents form a [Sidon set](#sidon-set) in the cyclic group. Taking integer representatives preserves the Sidon property. Primes within $o(\sqrt N)$ below $\sqrt N$ give $\sqrt N-o(\sqrt N)$ representatives in an interval of length $N$.

## Linear configuration count

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

A linear configuration count is a weighted sum over tuples satisfying prescribed [linear equations](linear-algebra.md#linear-equation). [Orthogonality of complex exponentials](fourier-analysis.md#orthogonality-of-complex-exponentials) often rewrites such a count as an integral of [Fourier transforms](analysis.md#fourier-transform).

### Fourier stability of a linear configuration count

↑ **Parent:** [Linear configuration count](#linear-configuration-count)

Suppose a linear configuration count has a Fourier-integral representation with $k$ factors. If one has a uniform Fourier bound for the difference between two weights and compatible $L^{k-1}$ bounds for each weight, expanding the difference one factor at a time and applying [Hölder's inequality](real-analysis.md#holder-s-inequality) bounds the change in the count.

## Transference principle in additive combinatorics

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

A transference principle replaces a function bounded by a sparse pseudorandom majorant with a bounded dense model that is indistinguishable by a chosen family of tests. Results for bounded functions can then be transferred to the sparse setting.

### Test-function seminorm

↑ **Parent:** [Transference principle in additive combinatorics](#transference-principle-in-additive-combinatorics)

For a family $\mathcal F$ of real-valued functions on a finite set and normalized [inner product](linear-algebra.md#inner-product) $\langle\cdot,\cdot\rangle$, the test-function seminorm is

$$
\|g\|_{\mathcal F}=\sup_{f\in\mathcal F}|\langle g,f\rangle|.
$$

It measures the largest correlation of $g$ with an allowed test. It is a [seminorm](topological-vector-space.md#seminorm), and becomes a [norm](functional-analysis.md#norm) when the tests separate points.

#### Dual test-function norm

↑ **Parent:** [Test-function seminorm](#test-function-seminorm)

The dual test-function norm is

$$
\|g\|_{\mathcal F}^{*}=\sup_{\|h\|_{\mathcal F}\leq1}|\langle g,h\rangle|.
$$

If $\mathcal F$ is closed, convex, and symmetric, the [Bipolar theorem for a dual pair](topological-vector-space.md#bipolar-theorem-for-a-dual-pair) identifies its dual unit ball with $\mathcal F$. Submultiplicativity under pointwise products allows a polynomial in one test function to remain controlled in this norm.

### Dense model theorem for a multiplicative test family

↑ **Parent:** [Transference principle in additive combinatorics](#transference-principle-in-additive-combinatorics)

Let $\mathcal F$ be a closed, convex, symmetric family of functions into $[-1,1]$ that contains the constant function $1$, and suppose its [dual test-function norm](#dual-test-function-norm) is submultiplicative under pointwise products. If a nonnegative majorant $\nu$ has average at most one and $\|\nu-1\|_{\mathcal F}$ is exponentially small in $1/\varepsilon$, then every $0\leq g\leq\nu$ has a dense model $0\leq\widetilde g\leq1$ satisfying

$$
\|g-\widetilde g\|_{\mathcal F}\leq\varepsilon.
$$

The proof separates $g$ from the convex set of dense models, then approximates the positive part of the separating test by a polynomial. Submultiplicativity controls every power in that polynomial.

#### Polynomial approximation of the positive part

↑ **Parent:** [Dense model theorem for a multiplicative test family](#dense-model-theorem-for-a-multiplicative-test-family)

On any fixed compact interval, the [positive part of a real-valued function](function.md#positive-part-of-a-real-valued-function) $t_+=\max(0,t)$ can be approximated uniformly by a real polynomial. Quantitative dense-model arguments use a version whose degree and coefficient growth are explicitly controlled in terms of the approximation error.

## Sumset

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sumset)

For subsets $A,B$ of an additive group, their sumset is $A+B=\{a+b:a\in A,b\in B\}$.

### Translated Bohr neighborhood in a triple sumset

↑ **Parent:** [Sumset](#sumset)

For a subset $A$ of density $\alpha$ in a finite cyclic group, put $F=1_A*1_A*1_A$ using [normalized convolution on a finite group](#normalized-convolution-on-a-finite-group). Its average is $\alpha^3$, so choose $t_0$ with $F(t_0)\geq\alpha^3$. Retain the [large spectrum](#large-spectrum) where $|\widehat{1_A}|\geq\alpha^2/8$. The [Parseval identity on a finite group](#parseval-identity-on-a-finite-group) gives at most $64\alpha^{-3}$ frequencies. Their phases change by at most $\alpha/4$ on the associated [Bohr set](#bohr-set), contributing at most $\alpha^3/4$ to the change of $F$. The discarded frequencies contribute at most another $\alpha^3/4$, since $\sum |\widehat{1_A}|^2=\alpha$. Therefore $F(t_0+b)\geq\alpha^3/2>0$ on the [Bohr set](#bohr-set), proving the containment.

#### Polynomial-length progression in a dense triple sumset

↑ **Parent:** [Translated Bohr neighborhood in a triple sumset](#translated-bohr-neighborhood-in-a-triple-sumset)

For fixed positive density $\delta$, every sufficiently large $A\subseteq[1,N]$ of size at least $\delta N$ has a long [arithmetic progression](arithmetic.md#arithmetic-progression) in its triple [sumset](#sumset). Embed it in $\mathbb Z/(8N)\mathbb Z$, where its density is at least $\delta/8$. A [translated Bohr neighborhood in a triple sumset](#translated-bohr-neighborhood-in-a-triple-sumset) has bounded rank and fixed positive radius depending only on $\delta$. A torus [pigeonhole principle](algebra.md#pigeonhole-principle) argument supplies a nonzero step whose small multiples stay in the [Bohr set](#bohr-set), with polynomially many multiples. All resulting residues have representatives in $[3,3N]$, an interval shorter than half the modulus, so their successive ordinary integer differences agree and give an actual integer [arithmetic progression](arithmetic.md#arithmetic-progression). The positive constant prefactor is absorbed by reducing the exponent for sufficiently large $N$.

### Sum of a subset

↑ **Parent:** [Sumset](#sumset)

Given numbers $s_1,\ldots,s_n$, the sum associated with a subset $A$ of indices is $\sum_{i\in A}s_i$. The empty subset gives zero. The set of all these values is the [sumset](#sumset) $\{0,s_1\}+\cdots+\{0,s_n\}$.

### Distinct-positive-integer subset-sum lower bound

↑ **Parent:** [Sumset](#sumset)

For $0<s_1<\cdots<s_n$, adding the largest integer creates at least $n$ new [sums of subsets](#sum-of-a-subset). If $P=\sum_{i<n}s_i$ is the previous maximum, the values $P+s_n$ and $P+s_n-s_i$ for $i<n$ are distinct new sums above $P$. Induction gives the displayed bound. Equality holds for $s_i=i$, whose subset sums fill the interval of integers from zero to $n(n+1)/2$.

### Lexicographic embedding of a sumset

↑ **Parent:** [Sumset](#sumset)

Represent each element of $S_1+\cdots+S_n$ by the lexicographically least tuple with that sum. Every coordinate projection of the resulting tuple set is itself lexicographically least for its partial sum: replacing it by a smaller representative would improve the original tuple without changing its sum. Consequently projected cardinalities are at most the corresponding partial [sumset](#sumset) cardinalities. Projection inequalities, including the [box theorem](combinatorics.md#box-theorem), therefore give [sumset](#sumset) inequalities.

### Restricted sumset

↑ **Parent:** [Sumset](#sumset)

For finite sets in an [abelian group](group.md#abelian-group) and a [bipartite graph](graph-theory.md#bipartite-graph) $\Gamma\subseteq A\times B$, the restricted [sumset](#sumset) is $\{a+b:(a,b)\in\Gamma\}$. It retains only sums corresponding to graph edges.

<h3 id="plunnecke-inequality">Plünnecke inequality</h3>

↑ **Parent:** [Sumset](#sumset)

For nonempty finite subsets $A,B$ of an [abelian group](group.md#abelian-group), $|A+B|\leq K|A|$ implies that some nonempty $X\subseteq A$ satisfies this bound simultaneously for every integer $m\geq0$, with $0B=\{0\}$. The [Petridis minimal-growth lemma](#petridis-minimal-growth-lemma) proves this by choosing $X$ to minimize $|X+B|/|X|$. The [Ruzsa triangle inequality](#ruzsa-triangle-inequality) then gives the [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality) $|kB-\ell B|\leq K^{k+\ell}|A|$.

### Iterated sumset

↑ **Parent:** [Sumset](#sumset)

For a [nonnegative integer](arithmetic.md#natural-number) $m$, the iterated sumset $mA$ is the sum of $m$ copies of $A$, with $0A=\{0\}$. Repetitions are allowed, so its elements are sums $a_1+\cdots+a_m$ with each $a_i\in A$.

## Difference set

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Difference_set)

For subsets $A,B$ of an additive group, their difference set is $A-B=\{a-b:a\in A,b\in B\}$.

## Doubling constant

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doubling_constant)

The doubling constant of a nonempty finite set $A$ is $|A+A|/|A|$. A small doubling constant indicates that $A$ behaves approximately like a [coset](group-theory.md#coset) of a [subgroup](group.md#subgroup).

### Polynomial growth of iterated sumsets

↑ **Parent:** [Doubling constant](#doubling-constant)

For a finite nonempty subset of an [abelian group](group.md#abelian-group) with [doubling constant](#doubling-constant) at most $K$, the [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality) gives $|3A-2A|\leq K^5|A|$. Applying the [Ruzsa covering lemma](#ruzsa-covering-lemma) to $2(A-A)$ using $A$ gives $2T\subseteq D+T$ for $T=A-A$ and $|D|=q\leq K^5$. Thus $\ell T\subseteq(\ell-1)D+T$, and counting multiplicities in the finite set $D$ proves the displayed polynomial bound. For fixed $K>1$, it is eventually at most $K^{\epsilon\ell}|A|$ for every $\epsilon>0$.

<h3 id="plunnecke-ruzsa-inequality">Plünnecke-Ruzsa inequality</h3>

↑ **Parent:** [Doubling constant](#doubling-constant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Plünnecke-Ruzsa_inequality)

If finite sets satisfy $|A+B|\leq K|A|$, then the Plünnecke-Ruzsa inequality bounds iterated sumsets and difference sets by

$$
|\ell B-mB|\leq K^{\ell+m}|A|.
$$

#### Petridis minimal-growth lemma

↑ **Parent:** [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality)

If a nonempty finite set $X$ minimizes $|X+B|/|X|$ among the nonempty subsets of $A$, with minimum $K'$, then

$$
|X+B+C|\leq K'|X+C|
$$

for every finite set $C$. Iteration is a short proof of the [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality).

#### Ruzsa triangle inequality

↑ **Parent:** [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ruzsa_triangle_inequality)

For finite subsets $A,B,C$ of an abelian group with $A$ nonempty,

$$
|B-C|\leq\frac{|A+B|\,|A+C|}{|A|}.
$$

An injective encoding chooses one representation of each element of $B-C$ and translates it by every element of $A$.

##### Noncommutative Ruzsa triangle inequality

↑ **Parent:** [Ruzsa triangle inequality](#ruzsa-triangle-inequality)

For nonempty finite subsets $A,B,C$ of an arbitrary group,

$$
|A|\,|BC^{-1}|\leq|AB^{-1}|\,|AC^{-1}|.
$$

Choose one representation $x=b_xc_x^{-1}$ for each $x\in BC^{-1}$. The map $(a,x)\mapsto(ab_x^{-1},ac_x^{-1})$ is injective.

###### Fourfold product bound from small tripling

↑ **Parent:** [Noncommutative Ruzsa triangle inequality](#noncommutative-ruzsa-triangle-inequality)

If a finite subset $A$ of a group satisfies $|A^3|\leq K|A|$, then repeated use of the [Noncommutative Ruzsa triangle inequality](#noncommutative-ruzsa-triangle-inequality) gives

$$
|A^4|\leq K^3|A|\leq K^4|A|.
$$

###### Small doubling does not control tripling in a noncommutative group

↑ **Parent:** [Noncommutative Ruzsa triangle inequality](#noncommutative-ruzsa-triangle-inequality)

Let $H$ be a finite subgroup and choose $x$ with $H\cap xHx^{-1}=\{1\}$. For $A=H\cup\{x\}$, the set $A^2$ has size at most $3|H|+1$, while $A^3$ contains the double coset $HxH$ of size $|H|^2$. Thus bounded doubling alone gives no tripling bound in arbitrary groups.

### Freiman-Ruzsa theorem

↑ **Parent:** [Doubling constant](#doubling-constant)

For every $K$, a finite set $A$ in an abelian group with $|A+A|\leq K|A|$ is contained in a coset progression of rank and relative size bounded in terms of $K$ alone.

#### Freiman theorem for integer sets

↑ **Parent:** [Freiman-Ruzsa theorem](#freiman-ruzsa-theorem)

A finite nonempty set of integers with bounded doubling lies in a generalized arithmetic progression with rank and relative size bounded only by the doubling constant. A proof models a large subset in a dense cyclic set, finds a Bohr set in its fourfold difference set by Fourier analysis, and uses the [progression in a Bohr set from successive minima](#progression-in-a-bohr-set-from-successive-minima). The progression lifts through a sufficiently high-order Freiman isomorphism. A greedy covering of the original set by translates of its doubled progression then gives the claimed containing progression. Geometry-of-numbers properification may make the final progression proper.

#### Freiman-Ruzsa theorem over a finite field

↑ **Parent:** [Freiman-Ruzsa theorem](#freiman-ruzsa-theorem)

If $A\subseteq\mathbb F_p^n$ and $|A+A|\leq K|A|$, then $A$ is contained in a [vector subspace](vector-space.md#vector-subspace) $H$ satisfying

$$
|H|\leq K^2p^{K^4}|A|.
$$

##### Freiman-Ruzsa bound from Bogolyubov and linear modelling

↑ **Parent:** [Freiman-Ruzsa theorem over a finite field](#freiman-ruzsa-theorem-over-a-finite-field)

Let $A$ be a nonempty subset of $\mathbb F_2^N$ with [doubling constant](#doubling-constant) at most $C\ge1$. Translate to $B=A+a$ containing zero. The [Petridis minimal-growth lemma](#petridis-minimal-growth-lemma) and [Ruzsa triangle inequality](#ruzsa-triangle-inequality) bound $|kB|\le C^k|B|$. In [injective linear modelling of a small sumset](#injective-linear-modelling-of-a-small-sumset), the image has density at least $1/(4C^{12})$. The [Finite-field Bogolyubov lemma](#finite-field-bogolyubov-lemma) finds a subspace of codimension at most $\lceil32C^{24}\rceil$ in its fourfold sumset.

After [lifting a subspace through a Freiman model](#lifting-a-subspace-through-a-freiman-model), obtain $\widetilde W\subseteq4B$ with $|\widetilde W|\ge2^{-\lceil32C^{24}\rceil}|B|$. The set $B+\widetilde W\subseteq5B$ uses at most $C^5 2^{\lceil32C^{24}\rceil}$ cosets. Their representatives generate a quotient group of size at most two to this number. Since $|\widetilde W|\le C^4|B|$, adjoining those representatives and $a$ proves the displayed bound. Its constants are deliberately coarse, but depend only on $C$. The nonempty assumption is necessary: no vector subspace has cardinality at most a constant times the size of the empty set.

##### Injective linear modelling of a small sumset

↑ **Parent:** [Freiman-Ruzsa theorem over a finite field](#freiman-ruzsa-theorem-over-a-finite-field)

For a finite subset $B\subseteq\mathbb F_2^N$ containing zero, choose $m=\lceil\log_2(2|12B|)\rceil$ and a uniformly random [linear map](vector-space.md#linear-map) $L:\mathbb F_2^N\to\mathbb F_2^m$. Each fixed nonzero vector has zero image with [probability](probability-theory.md#probability) $2^{-m}$. The [union bound](probability-inequality.md#boole-s-inequality) gives a map whose [kernel](linear-algebra.md#kernel-of-a-linear-map) meets $12B$ only at zero. It is injective on $6B$, and $2^m<4|12B|$. The [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality) makes the image of $B$ have density at least $1/(4C^{12})$ if $|B+B|\le C|B|$.

###### Lifting a subspace through a Freiman model

↑ **Parent:** [Injective linear modelling of a small sumset](#injective-linear-modelling-of-a-small-sumset)

Under [injective linear modelling of a small sumset](#injective-linear-modelling-of-a-small-sumset), every $w\in W$ has a unique lift $\sigma(w)\in4B$, because differences of two lifts lie in $8B\subseteq12B$. For $w_1,w_2\in W$, the discrepancy $\sigma(w_1)+\sigma(w_2)+\sigma(w_1+w_2)$ lies in $12B\cap\ker L$, so it is zero. Thus $\sigma$ is a [linear map](vector-space.md#linear-map) and its image is a [vector subspace](vector-space.md#vector-subspace) of the same size as $W$. This verifies the additive lifting step rather than assuming that a preimage chosen from a sumset is automatically a subspace.

<h4 id="szemeredi-theorem-in-a-bounded-rank-coset-progression">Szemerédi theorem in a bounded-rank coset progression</h4>

↑ **Parent:** [Freiman-Ruzsa theorem](#freiman-ruzsa-theorem)

For fixed density $\delta>0$, rank $r$, and progression length, every sufficiently large proper coset progression of rank at most $r$ has the property that each subset of relative density at least $\delta$ contains a nontrivial arithmetic progression of that length. This follows from the multidimensional [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem).

#### Small difference set forces a three-term arithmetic progression

↑ **Parent:** [Freiman-Ruzsa theorem](#freiman-ruzsa-theorem)

For every $C$ there is $N(C)$ such that a set $A\subseteq\mathbb Z$ with $|A|\geq N(C)$ and $|A-A|\leq C|A|$ contains a nontrivial three-term [arithmetic progression](arithmetic.md#arithmetic-progression). The [Freiman-Ruzsa theorem](#freiman-ruzsa-theorem) places $A$ densely in a bounded-rank coset progression, where the [Szemerédi theorem in a bounded-rank coset progression](#szemeredi-theorem-in-a-bounded-rank-coset-progression) applies.

## Approximate group

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Approximate_group)

A $K$-approximate group is a finite [symmetric subset of a group](#symmetric-subset-of-a-group) $A$ for which some set $X$ with $|X|\leq K$ satisfies $A^2\subseteq XA$. In additive notation the covering condition is $A+A\subseteq X+A$.

### Breuillard-Green-Tao structure theorem for approximate groups

↑ **Parent:** [Approximate group](#approximate-group)

For every finite $K$-[approximate group](#approximate-group) $A$ in a group $G$, there are subgroups $H\trianglelefteq C<G$ such that

$$
H\subseteq A^4,
$$

$C/H$ is a [nilpotent group](group-theory.md#nilpotent-group) of class $O_K(1)$, and $A$ is contained in the union of $O_K(1)$ left [cosets](group-theory.md#coset) of $C$.

### Higher product bound for an approximate group

↑ **Parent:** [Approximate group](#approximate-group)

If $A$ is a finite $K$-[approximate group](#approximate-group), then

$$
A^m\subseteq X^{m-1}A,\qquad |A^m|\leq K^{m-1}|A|
$$

for every [positive integer](number-theory.md#positive-integer) $m$, where $A^2\subseteq XA$ and $|X|\leq K$. This follows immediately by [mathematical induction](foundations-of-mathematics.md#mathematical-induction).

### Intersection of an approximate group power with a subgroup

↑ **Parent:** [Approximate group](#approximate-group)

If $A$ is a $K$-[approximate group](#approximate-group) in $G$ and $H\leq G$, then $A^m\cap H$ is a $K^{O(m)}$-approximate group. Indeed, the at most $K^{m-1}$ translates of $A$ covering $A^m$ induce at most that many translates of $A^2\cap H$ covering $A^m\cap H$, and the same argument covers its square inside $A^{2m}\cap H$.

### Large lower-step product in a torsion-free nilpotent approximate group

↑ **Parent:** [Approximate group](#approximate-group)

If $A$ is a finite $K$-[approximate group](#approximate-group) in a torsion-free $s$-step [nilpotent group](group-theory.md#nilpotent-group), then there are $r\leq K^{O(1)}$ approximate groups $A_0,\ldots,A_r\subseteq A^{O(1)}$, each with approximation parameter $K^{O(1)}$ and each generating a group of class less than $s$, such that

$$
|A_0\cdots A_r|\geq\exp(-K^{O(1)})|A|.
$$

The proof applies the large-progression form of the [Freiman-Green-Ruzsa theorem](#freiman-ruzsa-theorem) in the [abelianization](group-theory.md#abelianization), lifts its subgroup and cyclic directions, and uses the [intersection of an approximate group power with a subgroup](#intersection-of-an-approximate-group-power-with-a-subgroup).

#### Large lifted product from a coset progression

↑ **Parent:** [Large lower-step product in a torsion-free nilpotent approximate group](#large-lower-step-product-in-a-torsion-free-nilpotent-approximate-group)

Let $\pi:G\to G/[G,G]$ be the [abelianization](group-theory.md#abelianization) map and let $A$ be a finite $K$-[approximate group](#approximate-group). Suppose a coset progression $HP(x_1,\ldots,x_r;L_1,\ldots,L_r)$ lies in $\pi(A^4)$ and has size at least $\delta|\pi(A)|$. Then

$$
\left|
\bigl(A^{16}\cap\pi^{-1}(H)\bigr)
\prod_{i=1}^r\bigl(A^{22}\cap\pi^{-1}(\langle x_i\rangle)\bigr)
\right|\geq\delta|A|.
$$

A section of $\pi$ is multiplicative up to a bounded power of $A$ inside the [commutator subgroup](group-theory.md#commutator-subgroup); successively separating the subgroup and progression coordinates proves the inclusion needed for this estimate.

##### Fiber-counting lemma for a quotient map

↑ **Parent:** [Large lifted product from a coset progression](#large-lifted-product-from-a-coset-progression)

Let $\pi:G\to G/N$ be a [quotient group](group-theory.md#quotient-group) map, let $A$ be finite and symmetric, and suppose $P\subseteq\pi(A^m)$ has $|P|\geq\delta|\pi(A)|$. Then

$$
|\pi^{-1}(P)\cap A^{m+2}|\geq\delta|A|.
$$

Choose one lift in $A^m$ of each member of $P$ and multiply those lifts by $A^2\cap N$. Distinct fibers are disjoint, while $|\pi(A)|\,|A^2\cap N|\geq|A|$.

### Symmetric subset of a group

↑ **Parent:** [Approximate group](#approximate-group)

A subset $A$ of a multiplicatively written [group](group.md) is symmetric when it contains the [identity element](group.md#identity-element) and $A^{-1}=A$. Consequently $\langle A\rangle=\bigcup_{m\geq1}A^m$.

### Ruzsa covering lemma

↑ **Parent:** [Approximate group](#approximate-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ruzsa_covering_lemma)

If finite sets satisfy $|S+T|\leq K|T|$, then a maximal family of disjoint translates $x+T$, with $x\in S$, has at most $K$ members and gives

$$
S\subseteq X+T-T,
\qquad |X|\leq K.
$$

## Additive energy

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Additive_energy)

The additive energy of a finite set $A$ is the number of [additive quadruples](#additive-quadruple) in $A^4$, often normalized by $|A|^3$.

### Additive energy controls three-term progression mixing

↑ **Parent:** [Additive energy](#additive-energy)

If a subset $A$ of a cyclic group has normalized [additive energy](#additive-energy) at most $\alpha^4+\epsilon$, every nonconstant [Fourier coefficient on a finite abelian group](#fourier-coefficient-on-a-finite-abelian-group) of its indicator has modulus at most $\epsilon^{1/4}$. Expanding the count of $a+c=2b$ gives the frequency product $\widehat{1_A}(r)\widehat{1_C}(r)\widehat{1_B}(-2r)$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and [Parseval identity on a finite group](#parseval-identity-on-a-finite-group) bound its nonconstant part by the displayed quantity. Character doubling has multiplicity $\gcd(2,N)$, so no assumption that the modulus is odd is needed. The error is a normalized density error multiplied by $N^2$.

### Additive energy of a frequency graph

↑ **Parent:** [Additive energy](#additive-energy)

For a set of shifts $H$ and a map $\theta$ into a [circle group](lie-theory.md#circle-group), this [additive energy](#additive-energy) counts quadruples whose shift sums and frequency sums both agree. It is the [additive energy](#additive-energy) of the graph of $\theta$ in the product [abelian group](group.md#abelian-group).

#### Derivative correlations force additive frequency energy

↑ **Parent:** [Additive energy of a frequency graph](#additive-energy-of-a-frequency-graph)

Suppose $|f|\leq1$ on a finite cyclic group, $H$ has density $\beta$, and for each $h\in H$ the [multiplicative derivative](#multiplicative-derivative) has a [Fourier coefficient on a finite abelian group](#fourier-coefficient-on-a-finite-abelian-group) of magnitude at least $\eta$ at $\theta(h)$. Align the correlation phases, apply [Cauchy-Schwarz](probability-and-statistics.md#cauchy-schwarz-inequality), group pairs by their shift and frequency differences, and apply [Parseval identity](fourier-analysis.md#parseval-identity). This proves the displayed lower bound on [additive energy of a frequency graph](#additive-energy-of-a-frequency-graph) without replacing exact frequency equalities by approximate ones.

##### Squared derivative correlations force frequency-graph energy

↑ **Parent:** [Derivative correlations force additive frequency energy](#derivative-correlations-force-additive-frequency-energy)

Use the unnormalized [Fourier transform](analysis.md#fourier-transform) and $|f|\le1$. Normalize each derivative correlation by $N$ and align its phase. Their absolute sum is at least $\alpha N$. One [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), expansion by shift/frequency differences, and a second [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bound its fourth power by $N$ times the [additive energy of a frequency graph](#additive-energy-of-a-frequency-graph). [Parseval identity on a finite group](#parseval-identity-on-a-finite-group) supplies the factor $N$; exact equality of both shift sums and frequency sums is retained.

### Polynomial progression in a high-energy fourfold difference set

↑ **Parent:** [Additive energy](#additive-energy)

For every $\theta>0$, some $\gamma(\theta)>0$ has this property: any nonempty finite $A\subseteq\mathbb Z$ with $E(A)\geq\theta|A|^3$ has an [arithmetic progression](arithmetic.md#arithmetic-progression) of length at least $|A|^{\gamma(\theta)}$ in $2A-2A$. The [small-difference-set form of the Balog-Szemerédi-Gowers theorem](#small-difference-set-form-of-the-balog-szemeredi-gowers-theorem), [Ruzsa modelling lemma](#ruzsa-modelling-lemma), [cyclic Bogolyubov lemma](#cyclic-bogolyubov-lemma) and [nonwrapping progression in a cyclic Bohr set](#nonwrapping-progression-in-a-cyclic-bohr-set) prove it. An order-eight [Freiman s-isomorphism](#freiman-s-isomorphism) suffices to lift the progression because its consecutive second-difference equations expand into equalities of eight-term sums.

### Popular sum

↑ **Parent:** [Additive energy](#additive-energy)

A popular sum of a finite set $A$ is an element having at least a specified number $u$ of ordered representations as $a+b$, with $a,b\in A$. Popular sums define a dense [bipartite graph](graph-theory.md#bipartite-graph) when [additive energy](#additive-energy) is large. Since the total representation count is $|A|^2$, there are at most $|A|^2/u$ popular sums.

### Additive quadruple

↑ **Parent:** [Additive energy](#additive-energy)

An additive quadruple is a tuple $(a,b,c,d)$ satisfying $a+b=c+d$.

<h3 id="balog-szemeredi-gowers-theorem">Balog-Szemerédi-Gowers theorem</h3>

↑ **Parent:** [Additive energy](#additive-energy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Balog-Szemerédi-Gowers_theorem)

If a finite set $A$ has at least $\eta|A|^3$ [additive quadruples](#additive-quadruple), then it contains $A'$ with $|A'|\geq\eta^C|A|$ and $|A'+A'|\leq\eta^{-C}|A'|$ for an absolute constant $C$.

<h4 id="graph-form-of-the-balog-szemeredi-gowers-theorem">Graph form of the Balog-Szemerédi-Gowers theorem</h4>

↑ **Parent:** [Balog-Szemerédi-Gowers theorem](#balog-szemeredi-gowers-theorem)

There are absolute $c,C>0$ such that finite sets $A,B$ of size $n$, a [bipartite graph](graph-theory.md#bipartite-graph) of density at least $\delta$, and a [restricted sumset](#restricted-sumset) of size at most $Kn$ yield subsets $A',B'$ with $|A'|,|B'|\geq c\delta^Cn$ and $|A'+B'|\leq C\delta^{-C}K^Cn$. A graph formed by popular representations of sums turns this into the usual large-[additive energy](#additive-energy) form of the [Balog-Szemerédi-Gowers theorem](#balog-szemeredi-gowers-theorem).

##### Four-step path lemma for a dense bipartite graph

↑ **Parent:** [Graph form of the Balog-Szemerédi-Gowers theorem](#graph-form-of-the-balog-szemeredi-gowers-theorem)

Let a [bipartite graph](graph-theory.md#bipartite-graph) have $n$ vertices in each class and at least $\rho n^2$ edges. There is a subset $B$ of one class with $|B|\geq\rho n/4$ such that every pair of its vertices has at least $\rho^5n^3/4096$ four-edge walks between them. Declare a pair of left vertices bad if it has fewer than $\tau n$ common neighbours, with $\tau=\rho^2/32$. For a random right vertex $y$, put $U=N(y)$ and let $b(U)$ count ordered bad pairs inside $U$. Then $\mathbb E|U|\geq\rho n$ and $\mathbb Eb(U)\leq\tau n^2$. Some $y$ has $|U|-16b(U)/(\rho n)\geq\rho n/2$, so $|U|\geq\rho n/2$ and $b(U)\leq|U|^2/8$. Remove vertices with more than $|U|/4$ bad partners. At least half remain. For any two remaining vertices, at least $|U|/2$ middle vertices are good partners of both. Each supplies at least $(\tau n)^2$ walks, giving the bound.

<h4 id="small-difference-set-form-of-the-balog-szemeredi-gowers-theorem">Small-difference-set form of the Balog-Szemerédi-Gowers theorem</h4>

↑ **Parent:** [Balog-Szemerédi-Gowers theorem](#balog-szemeredi-gowers-theorem)

If $E(A)\geq\theta|A|^3$, a subset $B\subseteq A$ satisfies $|B|\geq c_\theta|A|$ and $|B-B|\leq K_\theta|B|$. A [dependent random choice](probabilistic-combinatorics.md#dependent-random-choice) argument in the [popular sum](#popular-sum) graph finds many four-edge paths representing each member of the [difference set](#difference-set). The [Petridis minimal-growth lemma](#petridis-minimal-growth-lemma) then bounds all higher [iterated sumsets](#iterated-sumset) and [difference sets](#difference-set).

## Bogolyubov lemma

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bogolyubov_lemma)

If $A$ has positive density in a finite abelian group, then $A+A-A-A$ contains a structured neighbourhood of zero. In a finite-dimensional vector space this neighbourhood can be taken to be a large [vector subspace](vector-space.md#vector-subspace); in a cyclic group it can be taken to be a [Bohr set](#bohr-set).

### Cyclic Bogolyubov lemma with explicit phase radius

↑ **Parent:** [Bogolyubov lemma](#bogolyubov-lemma)

For a set of density $\alpha$ in a finite cyclic group, select frequencies whose normalized [Fourier coefficients on a finite abelian group](#fourier-coefficient-on-a-finite-abelian-group) have magnitude at least $\alpha^{3/2}/2$. [Parseval identity](fourier-analysis.md#parseval-identity) bounds their number by $4\alpha^{-2}$. [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) of the fourfold [convolution](fourier-analysis.md#convolution) shows it is positive on the [Bohr set in phase-distance convention](#bohr-set-in-phase-distance-convention) of radius $1/6$. This is an explicit form of the [Bogolyubov lemma](#bogolyubov-lemma).

### Cyclic Bogolyubov lemma

↑ **Parent:** [Bogolyubov lemma](#bogolyubov-lemma)

For $D\subseteq\mathbb Z/q\mathbb Z$ of [subset density](#density-of-a-finite-subset) $\alpha$, $2D-2D$ contains a [Bohr set](#bohr-set) of rank at most $8\alpha^{-2}$ and a fixed positive width, including for composite $q$. With normalized [Fourier coefficients on a finite abelian group](#fourier-coefficient-on-a-finite-abelian-group), retain the frequencies where $|\widehat{1_D}|\geq\alpha^{3/2}/\sqrt8$. [Parseval identity on a finite group](#parseval-identity-on-a-finite-group) bounds their number and the discarded fourth moment. Their nearly constant phases make $1_D*1_D*1_{-D}*1_{-D}$ positive on the [Bohr set](#bohr-set).

### Finite-field Bogolyubov lemma

↑ **Parent:** [Bogolyubov lemma](#bogolyubov-lemma)

If $A\subseteq\mathbb F_p^n$ has density $\alpha$, then $2A-2A$ contains a vector subspace of codimension at most $2\alpha^{-2}$. It is the annihilator of the Fourier spectrum on which $|\widehat{1_A}|$ is at least $\alpha^{3/2}/\sqrt2$.

### Additive energy produces a large subspace in a fourfold difference set

↑ **Parent:** [Bogolyubov lemma](#bogolyubov-lemma)

For fixed $c>0$ and prime $p$, if $A\subseteq\mathbb F_p^N$ has at least $c|A|^3$ [additive quadruples](#additive-quadruple), then $2A-2A$ contains a vector subspace of size at least $c'(c,p)|A|$. Combine the [Balog-Szemerédi-Gowers theorem](#balog-szemeredi-gowers-theorem), the [Freiman-Ruzsa theorem over a finite field](#freiman-ruzsa-theorem-over-a-finite-field), and the [Finite-field Bogolyubov lemma](#finite-field-bogolyubov-lemma).

### Dense Bogolyubov-Ruzsa lemma

↑ **Parent:** [Bogolyubov lemma](#bogolyubov-lemma)

For every $\alpha>0$, if $A$ has density at least $\alpha$ in a cyclic group of prime order, then $2A-2A$ contains a proper [generalized arithmetic progression](#generalized-arithmetic-progression) of rank $O_\alpha(1)$ and size $\Omega_\alpha(|G|)$.

## Bohr set

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bohr_set)

For a finite abelian group $G$, frequencies $\Gamma\subseteq\widehat G$, and $\rho>0$, the Bohr set is

$$
B(\Gamma,\rho)=\{x\in G:|\gamma(x)-1|\leq\rho\text{ for every }\gamma\in\Gamma\}.
$$

Its rank is $|\Gamma|$ and its width is $\rho$.

### Progression in a Bohr set from successive minima

↑ **Parent:** [Bohr set](#bohr-set)

For a cyclic group $G$, a rank-$d$ phase-radius-$\rho$ [Bohr set](#bohr-set) contains a symmetric proper generalized arithmetic progression of rank at most $d+1$ and cardinality at least $c(d,\rho)|G|$. The constant can be taken to depend only on $d$ and $\rho$. This geometry-of-numbers consequence follows by applying successive minima to the lattice recording the simultaneous character congruences; any cyclic subgroup factor can be represented by one additional progression coordinate. It is stronger than finding just one long ordinary progression.

### Bohr set in phase-distance convention

↑ **Parent:** [Bohr set](#bohr-set)

A [Bohr set](#bohr-set) defined by distance of each character phase to the nearest integer. For $0\leq\epsilon\leq1/2$, it corresponds to the chord-distance radius $2\sin(\pi\epsilon)$. Numerical radius constants depend on the convention. In a group of prime order and with $d=|R|\geq1$, simultaneous torus approximation yields a nonzero element when $\epsilon>N^{-1/d}$ and an [arithmetic progression](arithmetic.md#arithmetic-progression) of length at least $\min(N,\lceil\epsilon N^{1/d}\rceil)$.

### Dilate of a Bohr set

↑ **Parent:** [Bohr set](#bohr-set)

If $B=B(\Gamma,\rho)$ is a [Bohr set](#bohr-set), its $\delta$-dilate is $B_\delta=B(\Gamma,\delta\rho)$. The triangle inequality on the unit circle gives $B_\delta+B_\eta\subseteq B_{\delta+\eta}$.

### Regular Bohr set

↑ **Parent:** [Bohr set](#bohr-set)

A rank-$d$ [Bohr set](#bohr-set) $B$ is regular when small changes of its width produce proportionally small changes of its size: for $|\kappa|\leq c/d$,

$$
|B_{1+\kappa}|=(1+O(d|\kappa|))|B|.
$$

Every Bohr set has a regular dilate $B_\lambda$ with $1/2\leq\lambda\leq1$.

### Lower bound for the size of a Bohr set

↑ **Parent:** [Bohr set](#bohr-set)

A [Bohr set](#bohr-set) of rank $d$ and width $\rho$ satisfies

$$
|B(\Gamma,\rho)|\geq\left(\frac{\rho}{8}\right)^d|G|.
$$

The proof partitions each circle coordinate into arcs and applies translation averaging and the pigeonhole principle.

### Arithmetic progression in a cyclic Bohr set

↑ **Parent:** [Bohr set](#bohr-set)

When $N$ is prime, simultaneous approximation of the frequencies shows that $B(\Gamma,\rho)\subseteq\mathbb Z/N\mathbb Z$ contains a centered [arithmetic progression](arithmetic.md#arithmetic-progression) of length at least

$$
\frac18\rho N^{1/|\Gamma|}.
$$

#### Nonwrapping progression in a cyclic Bohr set

↑ **Parent:** [Arithmetic progression in a cyclic Bohr set](#arithmetic-progression-in-a-cyclic-bohr-set)

In a [cyclic group](group.md#cyclic-group) of arbitrary order $q$, a [Bohr set](#bohr-set) with $d$ frequencies, defined by $\|rx/q\|\leq1/16$, contains an [arithmetic progression](arithmetic.md#arithmetic-progression) of distinct residues of length at least $q^{1/(d+1)}/32$. Partition the $d$-dimensional cube into $Q^d$ boxes, with $Q=\lfloor q^{1/(d+1)}\rfloor$. The [pigeonhole principle](algebra.md#pigeonhole-principle) supplies $1\leq t\leq Q^d$ with $\|rt/q\|\leq1/Q$ simultaneously. The residues $jt$, $0\leq j\leq\lfloor Q/16\rfloor$, remain in the [Bohr set](#bohr-set) and do not wrap around the cyclic group. The weaker exponent permits composite moduli without assuming that every nonzero step has large order.

## Almost period of a function

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

An almost period of a function $F$ in a normed space is a shift $t$ for which $\|\tau_tF-F\|$ is small.

### Bohr-set almost periodicity of a convolution

↑ **Parent:** [Almost period of a function](#almost-period-of-a-function)

Let $A\subseteq\mathbb Z_n$ have [density of a finite subset](#density-of-a-finite-subset) $\alpha$ and let $f=\mathbf1_A*\mathbf1_A$ use [normalized convolution on a finite group](#normalized-convolution-on-a-finite-group). If $K=\{r:|\widehat{\mathbf1_A}(r)|\geq\theta\}$ and $u\in B(K;\varepsilon)$, then the displayed estimate holds for normalized physical-space [L2 norm](real-analysis.md#l2-norm) and $T_uf(x)=f(x-u)$. The [Bohr set](#bohr-set) controls the translation factors on the [large spectrum](#large-spectrum); the [fourth Fourier moment bound for an indicator function](#fourth-fourier-moment-bound-for-an-indicator-function) controls their total weight. Outside $K$, use $|1-e^{2\pi iru/n}|\leq2$ and [Parseval identity on a finite group](#parseval-identity-on-a-finite-group).

### Lp almost period

↑ **Parent:** [Almost period of a function](#almost-period-of-a-function)

For $f:G\to\mathbb C$ and $X\geq0$, an $L^p$ almost period of $f$ with error $X$ is an element $t\in G$ such that

$$
\|\tau_tf-f\|_p\leq X,
\qquad (\tau_tf)(x)=f(x+t).
$$

#### Finite-field convolution almost-periodicity theorem

↑ **Parent:** [Lp almost period](#lp-almost-period)

If $A\subseteq\mathbb F_p^n$, $m\geq1$, and $\varepsilon>0$, then the $L^{2m}$ almost periods of $1_A*1_A$ with error $\varepsilon|A|p^{n/(2m)}$ contain a [vector subspace](vector-space.md#vector-subspace) of codimension $O(m\varepsilon^{-2})$. One proof samples the Fourier expansion of the convolution using the [Marcinkiewicz–Zygmund inequality](real-analysis.md#marcinkiewicz-zygmund-inequality); the sampled characters have a common kernel of the required codimension.

### Croot-Sisask almost-periodicity theorem

↑ **Parent:** [Almost period of a function](#almost-period-of-a-function)

If finite sets $A,S$ in a group satisfy $|A+S|\leq K|A|$, then for $q\geq2$ and $0<\epsilon<1$ there is $T\subseteq S$ with $|T|\geq(2K)^{-O(q/\epsilon^2)}|S|$ such that every $t\in T-T$ is an $L^q$ almost period of $1_A*f$:

$$
\|\tau_t(1_A*f)-1_A*f\|_q\leq\epsilon\|1_A\|_1\|f\|_q.
$$

### Finite-field character approximation

↑ **Parent:** [Almost period of a function](#almost-period-of-a-function)

Sampling the normalized Fourier expansion of $f:\mathbb F_p^n\to\mathbb C$ gives an average of $O(q/\epsilon^2)$ phase-adjusted characters whose $L^q$ error is at most $\epsilon\|\widehat f\|_1$. The common kernel of those characters is therefore a low-codimension subspace of almost periods of $f$.

## Normalized Fourier analysis on a finite abelian group

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

For a finite abelian group $G$, use the normalized average $\mathbb E_x=|G|^{-1}\sum_x$, normalized convolution

$$
(f*g)(x)=\mathbb E_y f(x-y)g(y),
$$

and Fourier transform $\widehat f(\gamma)=\mathbb E_xf(x)\overline{\gamma(x)}$. Then Parseval's identity and the convolution identity take the forms

$$
\langle f,g\rangle=\sum_{\gamma\in\widehat G}\widehat f(\gamma)\overline{\widehat g(\gamma)},
\qquad
\widehat{f*g}(\gamma)=\widehat f(\gamma)\widehat g(\gamma).
$$

### Large Fourier coefficient from a deficit of three-term progressions

↑ **Parent:** [Normalized Fourier analysis on a finite abelian group](#normalized-fourier-analysis-on-a-finite-abelian-group)

In a [cyclic group](group.md#cyclic-group) of odd prime order, the normalized ordered three-term [arithmetic progression](arithmetic.md#arithmetic-progression) count is $\sum_r\widehat{1_A}(r)^2\widehat{1_A}(-2r)$. The zero frequency contributes $\alpha^3$. If the count is less than $\alpha^3/2$, its nonzero-frequency contribution has magnitude greater than $\alpha^3/2$. The [Parseval identity on a finite group](#parseval-identity-on-a-finite-group) bounds that magnitude by $\alpha\max_{r\ne0}|\widehat{1_A-\alpha}(r)|$, proving the displayed estimate. The count includes progressions of zero common difference.

### Fourth Fourier moment bound for an indicator function

↑ **Parent:** [Normalized Fourier analysis on a finite abelian group](#normalized-fourier-analysis-on-a-finite-abelian-group)

For a subset $A$ of a [finite abelian group](group.md#finite-abelian-group) of [density of a finite subset](#density-of-a-finite-subset) $\alpha$, take normalized [Fourier coefficients on a finite abelian group](#fourier-coefficient-on-a-finite-abelian-group) and an unnormalized sum over frequencies. The bound follows from $|\widehat{\mathbf1_A}(\chi)|\leq\alpha$ and the [Parseval identity on a finite group](#parseval-identity-on-a-finite-group) $\sum_\chi|\widehat{\mathbf1_A}(\chi)|^2=\alpha$. It bounds the energy of the [normalized convolution on a finite group](#normalized-convolution-on-a-finite-group) $\mathbf1_A*\mathbf1_A$.

### Fourier coefficient on a finite abelian group

↑ **Parent:** [Normalized Fourier analysis on a finite abelian group](#normalized-fourier-analysis-on-a-finite-abelian-group)

For a scalar function on a [finite abelian group](group.md#finite-abelian-group), its coefficient at an [additive character](analysis.md#additive-character) $\chi$ is the displayed uniform [expectation](probability-theory.md#expected-value). On $\mathbb F_3^d$, write $\chi_\xi(x)=e^{2\pi i\xi\cdot x/3}$. The coefficient at the constant character is the mean of $f$, and the [Parseval identity on a finite group](#parseval-identity-on-a-finite-group) becomes $\sum_\chi|\widehat f(\chi)|^2=\mathbb E|f|^2$ after relabelling characters to match the transform convention.

### Linear phase

↑ **Parent:** [Normalized Fourier analysis on a finite abelian group](#normalized-fourier-analysis-on-a-finite-abelian-group)

A linear phase on an [abelian group](group.md#abelian-group) is an [additive character](analysis.md#additive-character), such as $x\mapsto e(\theta x)$ on the [integers](number-theory.md#integer) or $x\mapsto\omega^{rx}$ on $\mathbb Z_N$.

#### Progression partition with nearly constant linear phase

↑ **Parent:** [Linear phase](#linear-phase)

For a [linear phase](#linear-phase) $e^{2\pi i\theta x}$ on $[n]$, set $Q=\lfloor\sqrt n\rfloor$. The [Dirichlet approximation theorem](number-theory.md#dirichlet-s-approximation-theorem) gives $1\leq q\leq Q$ with $\|q\theta\|_{\mathbb R/\mathbb Z}\leq Q^{-1}$. If $1\leq L$ and $2L\leq Q$, split each residue chain modulo $q$ into [arithmetic progressions](arithmetic.md#arithmetic-progression) of lengths between $L$ and $2L-1$, merging the final remainder into the preceding block. Each chain has at least $Q$ points, so this is possible. On each resulting [arithmetic progression](arithmetic.md#arithmetic-progression), the [linear phase](#linear-phase) varies from its first value by at most $4\pi L/Q$. This converts a large [Fourier coefficient](fourier-series.md#fourier-coefficient) of a zero-sum real [function](function.md) into positive mean on one block: freezing the [linear phase](#linear-phase) controls the weighted block sums, and their positive and negative total masses agree.

### Sixth Fourier moment as a three-sum collision count

↑ **Parent:** [Normalized Fourier analysis on a finite abelian group](#normalized-fourier-analysis-on-a-finite-abelian-group)

For $A$ in a finite [abelian group](group.md#abelian-group) and normalized [Fourier transform](analysis.md#fourier-transform) $\widehat{1_A}$, the normalized number of sextuples satisfying

$$
x_1+x_2+x_3=x_4+x_5+x_6
$$

is

$$
\sum_{\gamma\in\widehat G}|\widehat{1_A}(\gamma)|^6.
$$

This follows by inserting [orthogonality of complex exponentials](fourier-analysis.md#orthogonality-of-complex-exponentials) for the displayed equation: the three variables on one side contribute $\widehat{1_A}(\gamma)^3$ and those on the other side contribute its [complex conjugate](complex-analysis.md#complex-conjugate).

### Large spectrum

↑ **Parent:** [Normalized Fourier analysis on a finite abelian group](#normalized-fourier-analysis-on-a-finite-abelian-group)

For a set $A$ of density $\alpha$ in a finite abelian group,

$$
\operatorname{Spec}_\rho(1_A)=\{\gamma:|\widehat{1_A}(\gamma)|\geq\rho\alpha\}.
$$

#### Chang theorem

↑ **Parent:** [Large spectrum](#large-spectrum)

Chang's theorem says that $\operatorname{Spec}_\rho(1_A)$ is contained in the span of a [dissociated set](#dissociated-set) of size $O(\rho^{-2}\log(\alpha^{-1}))$.

#### Dissociated set

↑ **Parent:** [Large spectrum](#large-spectrum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dissociated_set)

A subset $\Lambda$ of an abelian group is dissociated when a relation

$$
\sum_{\lambda\in\Lambda}\varepsilon_\lambda\lambda=0,
\qquad \varepsilon_\lambda\in\{-1,0,1\},
$$

forces every coefficient to vanish.

## Density increment

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

A density increment replaces a set by its intersection with a structured subset, translated back to a smaller ambient group, on which its relative density is larger. Iterating increments must stop before the density exceeds one.

### Hyperplane density increment for cap sets

↑ **Parent:** [Density increment](#density-increment)

If a [cap set](combinatorics.md#cap-set) $A\subseteq\mathbb F_3^d$ has [subset density](#density-of-a-finite-subset) $\alpha>0$ and $3^d\alpha^2\geq2$, some [affine subspace](vector-space.md#affine-subspace) of codimension one has relative [subset density](#density-of-a-finite-subset) at least $\alpha+\alpha^2/2$. The zero-sum count and the [Parseval identity on a finite group](#parseval-identity-on-a-finite-group) give a nonzero [finite abelian Fourier coefficient](#fourier-coefficient-on-a-finite-abelian-group) of magnitude at least $\alpha^2/2$. The three slice densities are $\alpha+2\operatorname{Re}(z\omega^j)$, where $z$ is this [finite abelian Fourier coefficient](#fourier-coefficient-on-a-finite-abelian-group) and $\omega$ a primitive cube [root of unity](algebra.md#root-of-unity); one slice has increment at least $|z|$. Translation preserves the zero-sum condition because the [characteristic](algebra.md#characteristic-of-a-field) is three.

### Roth density-increment step

↑ **Parent:** [Density increment](#density-increment)

There is an absolute constant $c>0$ such that, for every $\delta>0$ and all sufficiently large $N$, a subset $A\subseteq[N]$ whose [density of a finite subset](#density-of-a-finite-subset) is $\delta$ and which has no nonconstant three-term [arithmetic progression](arithmetic.md#arithmetic-progression) has an [arithmetic progression](arithmetic.md#arithmetic-progression) $P\subseteq[N]$ satisfying

$$
|P|\geq\eta(\delta)\sqrt N,
\qquad
\frac{|A\cap P|}{|P|}\geq\delta+c\delta^2.
$$

The [Fourier transform](analysis.md#fourier-transform) of the balanced function $f=1_A-\delta1_{[N]}$ has a coefficient of magnitude at least $c_0\delta^2N$. Indeed, the trilinear count

$$
\Lambda(g_1,g_2,g_3)=\sum_{x+z=2y}g_1(x)g_2(y)g_3(z)
$$

satisfies $\Lambda(1_A,1_A,1_A)=|A|$, whereas $\Lambda(1_{[N]},1_{[N]},1_{[N]})\gg N^2$. Expanding $1_A=\delta1_{[N]}+f$ and using the [Parseval identity](fourier-analysis.md#parseval-identity) and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to bound every error term forces $\|\widehat f\|_\infty\gg\delta^2N$ once $N$ is sufficiently large in terms of $\delta$.

Choose $\theta$ at which this large coefficient occurs. The [Dirichlet approximation theorem](number-theory.md#dirichlet-s-approximation-theorem) gives $1\leq d\leq\sqrt N$ with $\|d\theta\|_{\mathbb R/\mathbb Z}\leq N^{-1/2}$. Partition $[N]$ into progressions of common difference $d$ and lengths between $\eta\sqrt N$ and $2\eta\sqrt N$, where $\eta>0$ is a sufficiently small multiple of $\delta^2$. The [linear phase](#linear-phase) $e(\theta x)$ varies by $O(\eta)$ on each cell. The large Fourier coefficient then gives

$$
\sum_P\left|\sum_{x\in P}f(x)\right|\gg\delta^2N.
$$

Since $\sum_{x\in[N]}f(x)=0$, the total positive discrepancy is half the total absolute discrepancy, so at least one cell has average of $f$ at least $c\delta^2$. This is the required density increment.

#### One-frequency density increment on an integer interval

↑ **Parent:** [Roth density-increment step](#roth-density-increment-step)

For an [indicator function](measure-theory.md#indicator-function) of a subset of $[N]$ with [subset density](#density-of-a-finite-subset) $\alpha$, a large [Fourier coefficient](fourier-series.md#fourier-coefficient) of $1_A-\alpha1_{[N]}$ gives a [density increment](#density-increment) on an [arithmetic progression](arithmetic.md#arithmetic-progression). The [Dirichlet approximation theorem](number-theory.md#dirichlet-s-approximation-theorem) supplies a step $d\le\sqrt N$ on which the detected [linear phase](#linear-phase) changes slowly. Split its residue classes into progressions of lengths comparable to $\alpha^2\sqrt N$. Replacing the phase by one constant on each cell preserves a fixed fraction of the Fourier correlation. Since the balanced function has total sum zero, positive discrepancies sum to half the total absolute discrepancy; one cell has the displayed increased density. One may take $c=1/(2304\pi)$ when $N$ is sufficiently large in terms of $\alpha$.

#### Fourier detection of a progression-free subset of an interval

↑ **Parent:** [Roth density-increment step](#roth-density-increment-step)

Let $I=[n]$ for odd $n\geq3$, embed it in the [cyclic group](group.md#cyclic-group) $G=\mathbb Z/(2n+1)\mathbb Z$, and let $A\subseteq I$ have [density of a finite subset](#density-of-a-finite-subset) $\alpha$. If $A$ has no nonconstant three-term [arithmetic progression](arithmetic.md#arithmetic-progression) and $n\geq4\alpha^{-2}$, its balanced [indicator function](measure-theory.md#indicator-function) $f=1_A-\alpha1_I$ satisfies

$$
\max_{r\ne0}|\widehat f(r)|\geq\alpha^2/36,
\qquad \widehat f(r)=\mathbb E_{x\in G}f(x)e^{-2\pi irx/|G|}.
$$

Indeed, the normalized trilinear [arithmetic progression](arithmetic.md#arithmetic-progression) count has the [Fourier analysis on a finite abelian group](#normalized-fourier-analysis-on-a-finite-abelian-group) formula $\Lambda(h_1,h_2,h_3)=\sum_r\widehat h_1(r)\widehat h_2(-2r)\widehat h_3(r)$. Its values on $1_A$ and $\alpha1_I$ are $\alpha n/|G|^2$ and $\alpha^3(n^2+1)/(2|G|^2)$. Telescoping their difference into three terms containing $f$, the [Parseval identity](fourier-analysis.md#parseval-identity) and [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bound its magnitude by $3\max|\widehat f|\alpha n/|G|$. The difference is at least $\alpha^3n^2/(4|G|^2)$, giving the claim. The zero [Fourier coefficient](fourier-series.md#fourier-coefficient) vanishes by the definition of $\alpha$.

### Bourgain bound for three-term-progression-free sets

↑ **Parent:** [Density increment](#density-increment)

If $G$ is a finite [abelian group](group.md#abelian-group) of odd order $N$ and $A\subseteq G$ contains no nonconstant three-term [arithmetic progression](arithmetic.md#arithmetic-progression), then Bourgain's bound is

$$
|A|\ll N\left(\frac{\log\log N}{\log N}\right)^{1/2}.
$$

#### Bohr-set density increment lemma

↑ **Parent:** [Bourgain bound for three-term-progression-free sets](#bourgain-bound-for-three-term-progression-free-sets)

Let $A$ have relative density $\alpha$ in a rank-$d$ [Regular Bohr set](#regular-bohr-set) $B$, and suppose $A$ has no nonconstant three-term [arithmetic progression](arithmetic.md#arithmetic-progression). Then either

$$
|A|\leq(d/\alpha)^{O(d)}|B|^{1/2},
$$

or some translate of $A$ has relative density at least $(1+c\alpha)\alpha$ in a regular [Bohr set](#bohr-set) $B'\subseteq B$ of rank at most $d+1$ and width at least $\rho(B)(\alpha/d)^{O(1)}$.

## Meshulam theorem

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

For each fixed odd prime $p$ and density $\alpha>0$, every sufficiently large subset of $\mathbb F_p^n$ of density at least $\alpha$ contains a nontrivial three-term [arithmetic progression](arithmetic.md#arithmetic-progression).

<h2 id="finite-field-szemeredi-theorem-for-four-term-arithmetic-progressions">Finite-field Szemerédi theorem for four-term arithmetic progressions</h2>

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)

For $p\geq5$ and every $\alpha>0$, a sufficiently large subset of $\mathbb F_p^n$ of density at least $\alpha$ contains a nontrivial four-term [arithmetic progression](arithmetic.md#arithmetic-progression).

## Gowers uniformity norm

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gowers_uniformity_norm)

The Gowers uniformity norm measures the average multiplicative derivative of a function around affine cubes. The $U^k$ norm detects polynomial phases of degree below $k$.

### Multiplicative derivative

↑ **Parent:** [Gowers uniformity norm](#gowers-uniformity-norm)

A product that cancels constant phases and lowers the degree of a polynomial phase. For $f(x)=e(\alpha x^2)$, it is $e(2\alpha hx+\alpha h^2)$. Some conventions conjugate the entire expression and reverse the frequency signs. The [Gowers uniformity norm](#gowers-uniformity-norm) derivative identity relates a higher norm to the average of lower norms of these derivatives.

### Gowers U2 norm

↑ **Parent:** [Gowers uniformity norm](#gowers-uniformity-norm)

For a function on a finite abelian group,

$$
\|f\|_{U^2}^4=\mathbb E_{x,a,b}f(x)\overline{f(x+a)}\,\overline{f(x+b)}f(x+a+b)
=\sum_{\gamma\in\widehat G}|\widehat f(\gamma)|^4.
$$

#### Quadratic phase detection by the Gowers U2 norm

↑ **Parent:** [Gowers U2 norm](#gowers-u2-norm)

Let $|f|\leq1$ on $\mathbb Z_N$ and put $g(x)=f(x)\omega^{-x^2}$. If $\|g\|_{U^2}^4\geq c$, then the [Parseval identity](fourier-analysis.md#parseval-identity) gives

$$
c\leq\sum_r|\widehat g(r)|^4
\leq\left(\max_r|\widehat g(r)|^2\right)\sum_r|\widehat g(r)|^2
\leq\max_r|\widehat g(r)|^2.
$$

Consequently $f$ correlates with a [quadratic phase](#quadratic-phase): for some $r\in\mathbb Z_N$,

$$
\left|\mathbb E_xf(x)\omega^{-rx-x^2}\right|\geq c^{1/2}.
$$

### Gowers U3 norm

↑ **Parent:** [Gowers uniformity norm](#gowers-uniformity-norm)

The third Gowers norm is the eighth root of the conjugated product around a three-dimensional affine cube:

$$
\|f\|_{U^3}^8=\mathbb E_{x,a,b,c}
\prod_{\epsilon\in\{0,1\}^3}\mathcal C^{|\epsilon|}f(x+\epsilon_1a+\epsilon_2b+\epsilon_3c).
$$

#### Quadratic uniformity of a set

↑ **Parent:** [Gowers U3 norm](#gowers-u3-norm)

A [subset](set.md#subset) $A$ of a [finite abelian group](group.md#finite-abelian-group) $G$ with [subset density](#density-of-a-finite-subset) $\eta=|A|/|G|$ is quadratically $\alpha$-uniform, in the [norm](functional-analysis.md#norm) convention, if its [balanced subset indicator](#balanced-indicator-function-of-a-finite-subset) $g=1_A-\eta$ has [Gowers U3 norm](#gowers-u3-norm) at most $\alpha$. This controls correlations on additive three-dimensional cubes after the [subset density](#density-of-a-finite-subset) contribution is removed. If a convention instead bounds the eighth power of the [norm](functional-analysis.md#norm) by $\alpha$, its parameter corresponds to the [norm](functional-analysis.md#norm) parameter $\alpha^{1/8}$. The convention must therefore be stated when giving quantitative thresholds.

##### Four-term progressions in a quadratically uniform interval set

↑ **Parent:** [Quadratic uniformity of a set](#quadratic-uniformity-of-a-set)

Balance the indicator by its density on the interval, and extend it by zero to a cyclic group of order greater than twelve times the interval length and coprime to six. An eighth-power interval cube bound $\alpha$ bounds every four-term counting error by $\alpha^{1/8}$ through three Cauchy–Schwarz steps. The density contribution is bounded below by a constant times $\delta^4$, and the diagonal contribution tends to zero with interval length. A sufficiently small constant times $\delta^{32}$ therefore guarantees a nonconstant four-term progression. Stating the cube normalization distinguishes this parameter from the norm convention.

##### Triangular weights count genuine four-term progressions

↑ **Parent:** [Quadratic uniformity of a set](#quadratic-uniformity-of-a-set)

For $A\subseteq\mathbb Z_N$, $N\geq16$, put $\eta=|A|/N$, $M=\lfloor N/16\rfloor$, $J=\{0,\ldots,M-1\}$, and $w=1_J*1_J$ using [normalized convolution on a finite group](#normalized-convolution-on-a-finite-group). The weights $w(x)w(d-M)$ are supported where $0\leq x\leq2M-2$ and $M\leq d\leq3M-2$, so $x,x+d,x+2d,x+3d$ are distinct integer points below $N$. If $t=M/N$, then $\mathbb Ew=t^2$ and the sum of absolute values of its Fourier coefficients is $t$, by [Parseval identity on a finite group](#parseval-identity-on-a-finite-group). Expanding the four indicators around their [subset density](#density-of-a-finite-subset) leaves four terms with one balanced factor. Expand both weights in [Fourier series](fourier-series.md) and absorb each character $e(rx+sd)$ into the factors at $x$ and $x+d$. Character multiplication preserves the [Gowers U3 norm](#gowers-u3-norm), and the cyclic [four-term progression bound with torsion factors](#four-term-progression-bound-with-torsion-factors) bounds every error by $6^{1/8}\alpha$. Thus the weighted count is at least $\eta^4t^4-4\cdot6^{1/8}\alpha t^2$. Since $t\geq1/32$, positivity follows from $\alpha<\eta^4/(4096\cdot6^{1/8})$.

#### Generalized von Neumann inequality for four-term progressions

↑ **Parent:** [Gowers U3 norm](#gowers-u3-norm)

For functions bounded by one on a cyclic group of prime order greater than three, three applications of [Cauchy-Schwarz](probability-and-statistics.md#cauchy-schwarz-inequality) bound the four-term [arithmetic progression](arithmetic.md#arithmetic-progression) average by the smallest [Gowers U3 norm](#gowers-u3-norm) of its factors. Zero extension yields the corresponding interval bound with an absolute factor. This makes [Gowers U3 norm](#gowers-u3-norm) a measure of uniformity relevant to four-term [arithmetic progression](arithmetic.md#arithmetic-progression) counts.

##### Four-term progression bound with torsion factors

↑ **Parent:** [Generalized von Neumann inequality for four-term progressions](#generalized-von-neumann-inequality-for-four-term-progressions)

For a [finite abelian group](group.md#finite-abelian-group) $G$, put $t_j=|\{x\in G:jx=0\}|$. If $|f_i|\leq1$, then $|\mathbb E_{x,d}\prod_{i=0}^3f_i(x+id)|\leq(t_2t_3)^{1/8}\min_i\|f_i\|_{U^3}$. Three applications of [Cauchy-Schwarz](probability-and-statistics.md#cauchy-schwarz-inequality), eliminating the factors at slopes $3,2,1$, bound the eighth power by $\mathbb E_{h,k}|\mathbb E_x\Delta_{-3h}\Delta_{-2k}f_0(x)|^2$, where $\Delta_hf(x)=f(x)\overline{f(x+h)}$. The integrand is nonnegative; averaging over $3G$ and $2G$ costs at most their indices $t_3$ and $t_2$ compared with the unrestricted average defining $\|f_0\|_{U^3}^8$. Reversal treats slope three. For slope one, elimination at slopes $3,0,2$ produces increments $-2h,k,-r$, costing only $t_2$; reversal treats slope two. In a [cyclic group](group.md#cyclic-group), $t_2\leq2,t_3\leq3$, so the constant is at most $6^{1/8}$ independently of group size.

###### Unbounded torsion obstructs uniform control of four-term progressions

↑ **Parent:** [Four-term progression bound with torsion factors](#four-term-progression-bound-with-torsion-factors)

A bound tending to zero with one factor's [Gowers U3 norm](#gowers-u3-norm), uniformly over all finite abelian groups, is false. On $G=\mathbb F_2^m$, choose a random independent sign at each point. A cube with eight distinct vertices has sign product of [expectation](probability-theory.md#expected-value) zero. The [probability](probability-theory.md#probability) of a collision among its vertices is at most $\binom82/|G|$, since each equality of distinct vertices imposes a nonzero linear equation in the increments. Thus some sign [function](function.md) $f$ has $\|f\|_{U^3}^8\leq28/|G|$. But the four-term [arithmetic progression](arithmetic.md#arithmetic-progression) is $(x,x+d,x,x+d)$, so choosing factors $(f,1,f,1)$ gives correlation identically one. As $m\to\infty$, the [norm](functional-analysis.md#norm) tends to zero. Bounded torsion, as in cyclic groups, avoids this obstruction.

#### Gowers U3 norm on an interval

↑ **Parent:** [Gowers U3 norm](#gowers-u3-norm)

Normalize the conjugated cube average by the number of integer cubes whose vertices all lie in the interval. Equivalently, extend $f$ by zero to a cyclic group of order greater than $8N$ and divide its [Gowers U3 norm](#gowers-u3-norm) by that of the interval's [indicator function](measure-theory.md#indicator-function). A [quadratic phase](#quadratic-phase) then has norm one. Omitting the denominator gives a different but uniformly equivalent interval normalization.

#### Derivative identity for the Gowers U3 norm

↑ **Parent:** [Gowers U3 norm](#gowers-u3-norm)

For the multiplicative derivative $\partial_af(x)=f(x+a)\overline{f(x)}$,

$$
\|f\|_{U^3}^8=\mathbb E_a\|\partial_af\|_{U^2}^4
=\mathbb E_a\sum_{\gamma\in\widehat G}|\widehat{\partial_af}(\gamma)|^4.
$$

### Gowers inner product

↑ **Parent:** [Gowers uniformity norm](#gowers-uniformity-norm)

For functions indexed by $\epsilon\in\{0,1\}^k$, the Gowers inner product is

$$
\left\langle(f_\epsilon)\right\rangle_{U^k}
=\mathbb E_{x,h_1,\ldots,h_k}
\prod_{\epsilon\in\{0,1\}^k}
\mathcal C^{|\epsilon|}f_\epsilon(x+\epsilon\mathbin\cdot h),
$$

where $\mathcal C$ denotes complex conjugation.

#### Gowers-Cauchy-Schwarz inequality

↑ **Parent:** [Gowers inner product](#gowers-inner-product)

Repeated [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\left|\left\langle(f_\epsilon)\right\rangle_{U^k}\right|
\leq\prod_{\epsilon\in\{0,1\}^k}\|f_\epsilon\|_{U^k}.
$$

### Quadratic phase

↑ **Parent:** [Gowers uniformity norm](#gowers-uniformity-norm)

A quadratic phase on $\mathbb F_p^n$ is a function $x\mapsto e_p(q(x))$, where $q$ is a [quadratic form](linear-algebra.md#quadratic-form) and $e_p(t)=e^{2\pi it/p}$. Its third multiplicative derivative is one, so its $U^3$ norm is one.

### Inverse theorem for the Gowers U3 norm over a finite field

↑ **Parent:** [Gowers uniformity norm](#gowers-uniformity-norm)

For fixed prime $p$, a one-bounded function on $\mathbb F_p^n$ with $U^3$ norm at least $\delta$ has correlation bounded below in terms of $p$ and $\delta$ with a quadratic phase, with the usual nonclassical formulation in small characteristic.

#### Frequency graph extracted from a large Gowers U3 norm

↑ **Parent:** [Inverse theorem for the Gowers U3 norm over a finite field](#inverse-theorem-for-the-gowers-u3-norm-over-a-finite-field)

If $\|f\|_{U^3}^8\geq c$ and $\|f\|_\infty\leq1$, select for many $a$ a frequency $\phi(a)$ at which $\widehat{\partial_af}$ is large. A box-norm inequality shows that the graph $\{(a,\phi(a))\}$ has at least $(c/2)^8|G|^3$ additive quadruples. Additive-combinatorial structure in this graph is the first step toward recovering a quadratic phase.

#### Density-increment proof of the finite-field four-term progression theorem

↑ **Parent:** [Inverse theorem for the Gowers U3 norm over a finite field](#inverse-theorem-for-the-gowers-u3-norm-over-a-finite-field)

If a dense set has too few four-term arithmetic progressions, its balanced function has large $U^3$ norm. A [Frequency graph extracted from a large Gowers U3 norm](#frequency-graph-extracted-from-a-large-gowers-u3-norm), followed by the [Balog-Szemerédi-Gowers theorem](#balog-szemeredi-gowers-theorem) and a Freiman theorem, yields correlation with a quadratic phase. Restricting to a suitable level set gives a density increment, and iteration proves the [Finite-field Szemerédi theorem for four-term arithmetic progressions](#finite-field-szemeredi-theorem-for-four-term-arithmetic-progressions).

## Freiman homomorphism

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Freiman_homomorphism)

A Freiman homomorphism preserves additive quadruples: whenever $x_1+x_2=x_3+x_4$ in its domain, its values satisfy $\phi(x_1)+\phi(x_2)=\phi(x_3)+\phi(x_4)$.

### Freiman s-homomorphism

↑ **Parent:** [Freiman homomorphism](#freiman-homomorphism)

A map $\phi:A\to B$ is a Freiman $s$-homomorphism when

$$
a_1+\cdots+a_s=a'_1+\cdots+a'_s
$$

implies the corresponding equality between the $\phi(a_i)$. It is a Freiman $s$-isomorphism when it is bijective and the converse implication also holds.

#### Freiman s-isomorphism

↑ **Parent:** [Freiman s-homomorphism](#freiman-s-homomorphism)

A Freiman $s$-isomorphism is a bijection whose forward and inverse maps are both [Freiman s-homomorphisms](#freiman-s-homomorphism).

##### Freiman lifting of a progression

↑ **Parent:** [Freiman s-isomorphism](#freiman-s-isomorphism)

An eight-term Freiman isomorphism extends injectively to the two-sum/two-difference set by sending its representations to the corresponding integer differences. Independence of representation uses four-term relations, and additivity whenever $y,z,y+z$ lie in that difference set uses six-term relations. Thus a proper symmetric progression in the modeled difference set lifts, one coordinate step at a time, to a proper integer progression of the same rank and cardinality.

##### Freiman 2-isomorphism

↑ **Parent:** [Freiman s-isomorphism](#freiman-s-isomorphism)

A [Freiman 2-isomorphism](#freiman-2-isomorphism) is a [bijection](function.md#bijection) between subsets of [abelian groups](group.md#abelian-group) preserving additive quadruple relations in both directions. It need not extend to an ambient group homomorphism. Multiplication by a nonzero [scalar](vector-space.md#scalar) in a [finite field](algebra.md#finite-field) and [translation](geometry-and-topology.md#translation-geometry) are examples; reduction of an [integer](number-theory.md#integer) set modulo a prime is an example only when it creates no new additive relations.

###### Minimal binary Freiman models have full fourfold sumset

↑ **Parent:** [Freiman 2-isomorphism](#freiman-2-isomorphism)

If a [Freiman 2-isomorphism](#freiman-2-isomorphism) into $\mathbb F_2^m$ uses minimal $m$, every nonzero vector lies in the fourfold [sumset](#sumset). Otherwise quotienting by the line it spans would preserve all additive quadruple relations and would still be injective, contradicting minimality. Since zero also belongs to the fourfold [sumset](#sumset), that [sumset](#sumset) is the full model group. [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality) then bounds its size by $K^4|A|$. A finite subset of the [direct sum](vector-space.md#direct-sum) of countably many binary fields has a finite-dimensional model to start with.

#### Ruzsa modelling lemma

↑ **Parent:** [Freiman s-homomorphism](#freiman-s-homomorphism)

The Ruzsa modelling lemma says that a finite set with bounded doubling has a large subset Freiman $s$-isomorphic to a dense subset of a finite cyclic group, whose order is bounded by a constant depending only on the doubling constant and $s$ times the original set size.

##### Cardinality-controlled cyclic Freiman model

↑ **Parent:** [Ruzsa modelling lemma](#ruzsa-modelling-lemma)

A nonempty finite integer set has a subset of the displayed size [Freiman s-isomorphic](#freiman-s-isomorphism) to a subset of $\mathbb Z_N$. Embed in a sufficiently large auxiliary prime modulus and randomly dilate. Avoid the residues of every nonzero multiple of $N$ of absolute value less than that prime for all nonzero members of $kA-kA$; a [union bound](probability-inequality.md#boole-s-inequality) gives a successful dilation. Retain a most-populated one of $k+1$ short intervals of representatives. Its $k$-term sum differences have absolute value less than the auxiliary prime, so reduction modulo $N$ both preserves and reflects relations. Under $|kA-kA|\le C|A|$, this gives $N\le4C|A|+1$.

##### Cyclic Freiman model of a small-doubling integer set

↑ **Parent:** [Ruzsa modelling lemma](#ruzsa-modelling-lemma)

For $|A+A|\le K|A|$, one can take $q=8|8A-8A|\le8K^{16}|A|$. Embed in a much larger prime cyclic group and choose a dilation avoiding the residues of all nonzero multiples of $q$ of absolute value below that prime for every nonzero eightfold difference. A union bound ensures such a dilation. Retain a most-populated ninth-interval of representatives. Eight-term sums then have range shorter than the prime, and reduction modulo $q$ both preserves and reflects eight-term additive relations.

##### Half-size prime cyclic Freiman model

↑ **Parent:** [Ruzsa modelling lemma](#ruzsa-modelling-lemma)

For a nonempty [integer](number-theory.md#integer) set with [doubling constant](#doubling-constant) at most $K$, [Plünnecke-Ruzsa inequality](#plunnecke-ruzsa-inequality) bounds $|2A-2A|$ by $K^4|A|$. Embed the set modulo a sufficiently large auxiliary prime $q$, randomly dilate it, and select the more populated of two half-intervals of representatives. Differences of two pair sums on that half have absolute value less than $q$, so the lift preserves original relations. Every nonzero original difference is uniformly dilated among nonzero residues; avoiding all residues represented by nonzero multiples of $p$ of absolute value less than $q$ has positive [probability](probability-theory.md#probability) when $p>4|2A-2A|$. Reduction modulo $p$ then yields a [Freiman 2-isomorphism](#freiman-2-isomorphism) on the selected half.

###### Half-size cyclic Freiman model with a sharp difference-set bound

↑ **Parent:** [Half-size prime cyclic Freiman model](#half-size-prime-cyclic-freiman-model)

For a finite nonempty [integer](number-theory.md#integer) [set](set.md) $A$, put $D=2A-2A$. If an [integer](number-theory.md#integer) $N>|D|$, some $A'\subseteq A$ of size at least $|A|/2$ has a [Freiman 2-isomorphism](#freiman-2-isomorphism) into $\mathbb Z/N\mathbb Z$. Choose an auxiliary [prime](number-theory.md#prime-number) $P>N$ so large that reduction is [injective](algebra.md#injective-function) on $A$ and every nonzero element of $D$ remains nonzero. Dilate modulo $P$ by a uniformly chosen nonzero multiplier. The forbidden residues are those represented by nonzero multiples of $N$ of absolute value less than $P$, at most $2\lfloor(P-1)/N\rfloor$ residues. The nonzero elements of $D$ occur in opposite pairs; the two elements in each pair have the same bad event. The [union bound](probability-inequality.md#boole-s-inequality) therefore gives failure probability at most $(|D|-1)/N<1$. Choose a multiplier avoiding all these events. Select the more populated of two half-intervals of residues modulo $P$. Differences of two pair sums of representatives then have absolute value less than $P$. An original additive relation must therefore lift to equality in the [integers](number-theory.md#integer); conversely an equality modulo $N$ cannot have a nonzero lifted difference, by the forbidden-residue choice. Reduction modulo $N$ is the required isomorphism.

### Second-difference obstruction to a Freiman homomorphism

↑ **Parent:** [Freiman homomorphism](#freiman-homomorphism)

Let $X$ be the image of all additive second differences

$$
\phi(x)-\phi(x+a)-\phi(x+b)+\phi(x+a+b).
$$

If a subspace $V$ satisfies $V\cap X=\{0\}$, then the restriction of $\phi$ to the inverse image of every coset of $V$ is a Freiman homomorphism.

### Large Freiman-homomorphic restriction from bounded derivative images

↑ **Parent:** [Freiman homomorphism](#freiman-homomorphism)

Suppose every derivative $x\mapsto\phi(x+d)-\phi(x)$ on $\mathbb F_p^n$ takes at most $C$ values. Then $\phi$ restricts to a Freiman homomorphism on a set of density at least $p^{-1}C^{-5}$. The proof bounds the second-difference image by $C^5$ and chooses a random subspace avoiding its nonzero elements.

## Generalized arithmetic progression

↑ **Parent:** [Additive combinatorics](additive-combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_arithmetic_progression)

A generalized arithmetic progression of rank $r$ is a set

$$
P=\left\{x_0+n_1v_1+\cdots+n_rv_r:0\leq n_i<L_i\right\}.
$$

It is proper when every parameter tuple in the displayed box represents a different element.

### Abelian progression

↑ **Parent:** [Generalized arithmetic progression](#generalized-arithmetic-progression)

An abelian progression is a [generalized arithmetic progression](#generalized-arithmetic-progression) inside an [abelian group](group.md#abelian-group). It is the image of an integer box under a [group homomorphism](group-theory.md#group-homomorphism).

### Coset progression

↑ **Parent:** [Generalized arithmetic progression](#generalized-arithmetic-progression)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coset_progression)

A coset progression is a [sumset](#sumset) $H+P$, where $H$ is a finite [subgroup](group.md#subgroup) of an [abelian group](group.md#abelian-group) and $P$ is a [generalized arithmetic progression](#generalized-arithmetic-progression).

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Bertrand's postulate](number-theory.md#bertrand-s-postulate)
- [Roth theorem on three-term arithmetic progressions](#roth-theorem-on-three-term-arithmetic-progressions)
