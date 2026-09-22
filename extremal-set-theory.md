# Extremal set theory

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Extremal_set_theory)

Extremal set theory asks how large a family of finite sets can be under prescribed intersection or containment restrictions.

**Table of contents**

- [Eventown theorem](#eventown-theorem)
- [Oddtown theorem](#oddtown-theorem)
- [Separating set system](#separating-set-system)
- [Large family avoiding a high intersection](#large-family-avoiding-a-high-intersection)
- [Forbidden-intersection density increment](#forbidden-intersection-density-increment)
  - [Quantitative forbidden-intersection bound by widening](#quantitative-forbidden-intersection-bound-by-widening)
- [Effective ground-set parameter of a hereditary uniform layer](#effective-ground-set-parameter-of-a-hereditary-uniform-layer)
  - [Shadow ratio for a hereditary set family](#shadow-ratio-for-a-hereditary-set-family)
- [Coordinate shifts of a set family](#coordinate-shifts-of-a-set-family)
  - [Downward coordinate compression](#downward-coordinate-compression)
    - [Two cube edges in every direction force many vertices](#two-cube-edges-in-every-direction-force-many-vertices)
  - [Coordinate-shift shadow containment](#coordinate-shift-shadow-containment)
- [Constant-intersection family bound](#constant-intersection-family-bound)
  - [Constant t-wise intersection dichotomy](#constant-t-wise-intersection-dichotomy)
    - [Complement-of-singleton extremizers](#complement-of-singleton-extremizers)
- [Elementary set shift](#elementary-set-shift)
  - [Shifted set family](#shifted-set-family)
    - [Ballot reflection injection](#ballot-reflection-injection)
- [Odd cross-intersection bound](#odd-cross-intersection-bound)
- [Even cross-intersection bound](#even-cross-intersection-bound)
- [Weakly intersecting family in a product alphabet](#weakly-intersecting-family-in-a-product-alphabet)
- [Bollobas set-pairs inequality](#bollobas-set-pairs-inequality)
- [Separating family of disjoint set pairs](#separating-family-of-disjoint-set-pairs)
  - [Disjoint subcube packing inequality](#disjoint-subcube-packing-inequality)
- [Symmetric chain decomposition of a Boolean lattice](#symmetric-chain-decomposition-of-a-boolean-lattice)
  - [Symmetric chain in a Boolean lattice](#symmetric-chain-in-a-boolean-lattice)
  - [Adjacent-level matching in a Boolean lattice](#adjacent-level-matching-in-a-boolean-lattice)
  - [Minimum chain partition of a Boolean lattice](#minimum-chain-partition-of-a-boolean-lattice)
- [Lexicographic order](#lexicographic-order)
- [Colexicographic order](#colexicographic-order)
  - [Colexicographic initial segment](#colexicographic-initial-segment)
- [Set family shadow](#set-family-shadow)
  - [Lower shadow](#lower-shadow)
    - [Iterated lower shadow](#iterated-lower-shadow)
      - [Clique counting from iterated shadows](#clique-counting-from-iterated-shadows)
    - [Kruskal-Katona theorem](#kruskal-katona-theorem)
      - [Nonisomorphic colex shadow minimizers](#nonisomorphic-colex-shadow-minimizers)
      - [Lovász shadow bound](#lovasz-shadow-bound)
      - [Colexicographic section compression](#colexicographic-section-compression)
      - [Binomial-shadow arithmetic lemma](#binomial-shadow-arithmetic-lemma)
      - [UV-compression](#uv-compression)
        - [Intersection-preserving lexicographic UV-compression](#intersection-preserving-lexicographic-uv-compression)
        - [Left-compressed set family](#left-compressed-set-family)
        - [Shadow lemma for UV-compressions](#shadow-lemma-for-uv-compressions)
      - [UV-compression proof of the Kruskal-Katona theorem](#uv-compression-proof-of-the-kruskal-katona-theorem)
  - [Upper shadow](#upper-shadow)
- [Frankl-Wilson theorem](#frankl-wilson-theorem)
  - [Modular intersection graph](#modular-intersection-graph)
  - [Modular intersection polynomial](#modular-intersection-polynomial)
  - [Complement splitting for forbidden midpoint intersections](#complement-splitting-for-forbidden-midpoint-intersections)
    - [Fixed-core construction avoiding midpoint intersections](#fixed-core-construction-avoiding-midpoint-intersections)
  - [Prime-power modular intersection bound](#prime-power-modular-intersection-bound)
  - [Modular-size auxiliary polynomials](#modular-size-auxiliary-polynomials)
  - [Modular layer vanishing lemma](#modular-layer-vanishing-lemma)
  - [Nonuniform Frankl-Wilson theorem](#nonuniform-frankl-wilson-theorem)
  - [Ray-Chaudhuri–Wilson theorem](#ray-chaudhuri-wilson-theorem)
- [Set family](#set-family)
  - [Helly family](#helly-family)
  - [Incidence matrix of a set system](#incidence-matrix-of-a-set-system)
  - [Diagonal-intersection set-pair bound](#diagonal-intersection-set-pair-bound)
  - [Union and intersection of set families](#union-and-intersection-of-set-families)
  - [Ahlswede–Daykin inequality](#ahlswede-daykin-inequality)
    - [Two-point four-functions inequality](#two-point-four-functions-inequality)
  - [Biased measure of a set family](#biased-measure-of-a-set-family)
  - [Self-dual set family](#self-dual-set-family)
    - [Complementary-layer bound for biased measure](#complementary-layer-bound-for-biased-measure)
      - [Weighted Bernoulli majority bound](#weighted-bernoulli-majority-bound)
  - [Laminar family of sets](#laminar-family-of-sets)
  - [Union-intersection compression](#union-intersection-compression)
  - [Cross-Sperner family](#cross-sperner-family)
  - [Hitting set](#hitting-set)
    - [Bounded-size transversal kernel](#bounded-size-transversal-kernel)
  - [Boolean lattice](#boolean-lattice)
    - [Kleitman diametric theorem](#kleitman-diametric-theorem)
    - [Injectivity of inclusion between adjacent set layers](#injectivity-of-inclusion-between-adjacent-set-layers)
    - [Up-set](#up-set)
    - [Down-set](#down-set)
      - [Edge boundary of a down-set in a cube](#edge-boundary-of-a-down-set-in-a-cube)
        - [Largest edge boundary of a down-set](#largest-edge-boundary-of-a-down-set)
      - [Downward closure of a set family](#downward-closure-of-a-set-family)
    - [Antichain](#antichain)
      - [Maximal chain in a Boolean lattice](#maximal-chain-in-a-boolean-lattice)
        - [Uniformly random maximal chain in a Boolean lattice](#uniformly-random-maximal-chain-in-a-boolean-lattice)
      - [Lubell-Yamamoto-Meshalkin inequality](#lubell-yamamoto-meshalkin-inequality)
        - [Equality in the LYM inequality](#equality-in-the-lym-inequality)
        - [Lubell mass](#lubell-mass)
        - [Local LYM inequality](#local-lym-inequality)
          - [Connectedness of adjacent-level incidence in a Boolean lattice](#connectedness-of-adjacent-level-incidence-in-a-boolean-lattice)
          - [Iterated local LYM inequality](#iterated-local-lym-inequality)
        - [Sperner's theorem](#sperner-s-theorem)
          - [Littlewood-Offord inequality](#littlewood-offord-inequality)
            - [Two-level Littlewood-Offord bound](#two-level-littlewood-offord-bound)
            - [Separated block decomposition for vector subset sums](#separated-block-decomposition-for-vector-subset-sums)
          - [Equality in Sperner theorem](#equality-in-sperner-theorem)
      - [k-Sperner family](#k-sperner-family)
        - [Weighted theorem for k-Sperner families](#weighted-theorem-for-k-sperner-families)
          - [Number of maximizing weighted k-Sperner families](#number-of-maximizing-weighted-k-sperner-families)
        - [Erdős theorem on k-Sperner families](#erdos-theorem-on-k-sperner-families)
      - [Cross-Sperner inequality](#cross-sperner-inequality)
        - [Two-block extremisers for the cross-Sperner inequality](#two-block-extremisers-for-the-cross-sperner-inequality)
  - [Characteristic vector of a set](#characteristic-vector-of-a-set)
    - [Modular intersection method for set families](#modular-intersection-method-for-set-families)
  - [Incidence graph](#incidence-graph)
  - [Trace of a set family](#trace-of-a-set-family)
    - [Set shattering](#set-shattering)
      - [Unbounded finite shattering without an infinite universal trace](#unbounded-finite-shattering-without-an-infinite-universal-trace)
    - [Shearer trace inequality](#shearer-trace-inequality)
  - [Union-closed family](#union-closed-family)
    - [Union-closed sets conjecture](#union-closed-sets-conjecture)
      - [Binary entropy product inequality](#binary-entropy-product-inequality)
      - [Entropy bound for a union-closed family](#entropy-bound-for-a-union-closed-family)
  - [Entropy bound for pairwise-union tuples](#entropy-bound-for-pairwise-union-tuples)
  - [Intersecting family](#intersecting-family)
    - [Union bound for intersecting families](#union-bound-for-intersecting-families)
    - [Colexicographic replacement can destroy intersection](#colexicographic-replacement-can-destroy-intersection)
    - [Lexicographic initial segments preserve ordinary intersection](#lexicographic-initial-segments-preserve-ordinary-intersection)
    - [Maximal intersecting families choose one member of every complementary pair](#maximal-intersecting-families-choose-one-member-of-every-complementary-pair)
    - [t-intersecting family](#t-intersecting-family)
      - [Lexicographic replacement can destroy two-intersection](#lexicographic-replacement-can-destroy-two-intersection)
      - [Maximal intersection does not imply maximum size](#maximal-intersection-does-not-imply-maximum-size)
      - [Nonuniform t-intersecting family bound](#nonuniform-t-intersecting-family-bound)
      - [Ahlswede-Khachatrian theorem](#ahlswede-khachatrian-theorem)
      - [Complementation of uniform intersecting families](#complementation-of-uniform-intersecting-families)
      - [Complete-intersection candidate family](#complete-intersection-candidate-family)
    - [Intersecting two-element set family](#intersecting-two-element-set-family)
    - [Witness-pair concentration for an intersecting uniform family](#witness-pair-concentration-for-an-intersecting-uniform-family)
    - [Two-intersecting family](#two-intersecting-family)
      - [Pair-cover bound for a two-intersecting uniform family](#pair-cover-bound-for-a-two-intersecting-uniform-family)
      - [Nonuniform two-intersecting family bound](#nonuniform-two-intersecting-family-bound)
    - [Intersecting shadow lemma](#intersecting-shadow-lemma)
    - [Weighted intersecting family bound on an odd Boolean lattice](#weighted-intersecting-family-bound-on-an-odd-boolean-lattice)
    - [Intersecting family in a product alphabet](#intersecting-family-in-a-product-alphabet)
    - [Exactly one-intersecting family](#exactly-one-intersecting-family)
      - [Finite linear space](#finite-linear-space)
        - [De Bruijn--Erdos pair-covering inequality](#de-bruijn-erdos-pair-covering-inequality)
        - [Near-pencil](#near-pencil)
        - [Finite projective plane](#finite-projective-plane)
    - [Cross-intersecting family](#cross-intersecting-family)
      - [Finite intersection witness for cross-intersecting families](#finite-intersection-witness-for-cross-intersecting-families)
    - [Upward closure of a set family](#upward-closure-of-a-set-family)
    - [Dinur-Friedgut junta theorem for intersecting families](#dinur-friedgut-junta-theorem-for-intersecting-families)
  - [Uniform set family](#uniform-set-family)
    - [Generating family for a uniform set family](#generating-family-for-a-uniform-set-family)
      - [Tight pairs of left-compressed generators](#tight-pairs-of-left-compressed-generators)
      - [Maximum-support generator fibre](#maximum-support-generator-fibre)
      - [Compatibility bound for complementary generating families](#compatibility-bound-for-complementary-generating-families)
      - [Small-support generating lemma for extremal intersecting families](#small-support-generating-lemma-for-extremal-intersecting-families)
        - [Generator replacement proof of the small-support intersection lemma](#generator-replacement-proof-of-the-small-support-intersection-lemma)
    - [Intersection-free uniform set family](#intersection-free-uniform-set-family)
      - [Antichain trace bound for intersection-free families](#antichain-trace-bound-for-intersection-free-families)
    - [Uniform layer of the Boolean cube](#uniform-layer-of-the-boolean-cube)
      - [Low-degree evaluation rank on a uniform layer](#low-degree-evaluation-rank-on-a-uniform-layer)
    - [Erdős-Ko-Rado theorem](#erdos-ko-rado-theorem)
      - [Erdős-Ko-Rado theorem from shadows](#erdos-ko-rado-theorem-from-shadows)
      - [Katona circle method](#katona-circle-method)
        - [Cyclic interval antichain bound](#cyclic-interval-antichain-bound)
        - [Cyclic interval intersection bound](#cyclic-interval-intersection-bound)
    - [Steiner triple system](#steiner-triple-system)

## Eventown theorem

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

If every member of a [set family](#set-family) on $[n]$ and every distinct pairwise [intersection](set.md#set-intersection) has even size, its [characteristic vectors](#characteristic-vector-of-a-set) span a [self-orthogonal binary subspace](coding-theory.md#self-orthogonal-binary-subspace). The standard [dot product](linear-algebra.md#dot-product) is [nondegenerate](linear-algebra.md#nondegenerate-bilinear-form), so $W\subseteq W^\perp$ implies $2\dim W\leq n$. Thus the [set family](#set-family) has at most $2^{\lfloor n/2\rfloor}$ members. All unions of $\lfloor n/2\rfloor$ disjoint pairs of points attain this bound.

## Oddtown theorem

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

If all members of a [set family](#set-family) on $[n]$ have odd size and all distinct pairwise [intersections](set.md#set-intersection) have even size, its [characteristic vectors](#characteristic-vector-of-a-set) over the [finite field](algebra.md#finite-field) $\mathbb F_2$ are [linearly independent](vector-space.md#linear-independence). Their pairwise [dot products](linear-algebra.md#dot-product) are zero, and each vector has [dot product](linear-algebra.md#dot-product) one with itself. Taking the [dot product](linear-algebra.md#dot-product) of a [linear combination](vector-space.md#linear-combination) with each vector makes every coefficient vanish, so there are at most $n$ vectors. The [set family](#set-family) of all singleton [sets](set.md) attains this bound.

## Separating set system

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

A [set family](#set-family) on a finite [set](set.md) separates ordered pairs if each ordered pair of distinct points has a member containing the first point and omitting the second. If its members are $A_1,\ldots,A_m$, assign each point the [characteristic vector](#characteristic-vector-of-a-set) of its incidences, or equivalently $T_i=\{a:i\in A_a\}$. Separation in both directions says precisely that the $T_i$ form an [antichain](#antichain) in the [Boolean lattice](#boolean-lattice) on $m$ coordinates. Thus the [Sperner theorem](#sperner-s-theorem) gives $n\leq\binom m{\lfloor m/2\rfloor}$. Conversely, any [antichain](#antichain) of $n$ distinct subsets of $[m]$ supplies such a [set family](#set-family) by transposing its incidence table.

## Large family avoiding a high intersection

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

If a forbidden intersection size exceeds $n/2$, every subset of size at most $\lfloor n/2\rfloor$ avoids it, including on self-intersection. This [set family](#set-family) contains at least half the [Boolean lattice](#boolean-lattice). Consequently a fixed exponential bound $c^n$ with $c<2$ cannot hold uniformly as $n$ grows. Forbidden-intersection estimates below the middle rank therefore cannot simply be extrapolated to high intersections.

## Forbidden-intersection density increment

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

For two [set families](#set-family) forbidding all cross-intersections in $[a,b]$, split into absent and present coordinate sections. The section pairs $(\mathcal F_1,\mathcal G_1)$, $(\mathcal F_0,\mathcal G_0\cup\mathcal G_1)$, and $(\mathcal F_1,\mathcal G_0\cap\mathcal G_1)$ forbid, respectively, $[a-1,b-1]$, $[a,b]$, and $[a-1,b]$ in one fewer dimension. For $0<\delta\leq1/10$, either one of the first two pairs, allowing exchange of the [set family](#set-family) names, increases the density product by at least $1+\delta$, or the third widens the interval and retains at least $1-\delta-2\delta^2$ of that product. This converts a single forbidden intersection into a long forbidden interval while recording every density gain and loss.

### Quantitative forbidden-intersection bound by widening

↑ **Parent:** [Forbidden-intersection density increment](#forbidden-intersection-density-increment)

Let two [set families](#set-family) on $n$ coordinates forbid cross-intersection size $\ell$, and let $\rho$ be their density product. For $0<\delta\leq1/10$, put $g=\log(1+\delta)$, $h=-\log(1-\delta-2\delta^2)$, and $D=g+h$. Repeated [forbidden-intersection density increments](#forbidden-intersection-density-increment) terminate when one endpoint of the forbidden interval reaches zero or the remaining dimension. In the first case, if $v$ steps widened the interval, the [cross-intersection bound from cube separation](combinatorics.md#cross-intersection-bound-from-cube-separation) gives $\log\rho\leq-g\ell+Dv-v^2/n\leq-g\ell+D^2n/4$. In the second case, at least $n-\ell$ steps occurred and at most $\ell$ widened, giving $\log\rho\leq-gn+(2g+h)\ell$. For a single [set family](#set-family) take the square of its density. Choosing $\delta=1/50$ proves $|\mathcal A|\leq1.999^n$ for forbidden intersections $n/4$ and $\lfloor n/8\rfloor$, with small dimensions handled directly.

## Effective ground-set parameter of a hereditary uniform layer

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

For a nonempty degree-$m$ layer of a [down-set](#down-set) in an $N$-element [Boolean lattice](#boolean-lattice), the unique real number $x_m\geq m$ with $|\mathcal F_m|=\binom{x_m}m$ measures an effective number of available coordinates. The [Lovász shadow bound](#lovasz-shadow-bound) and $\partial\mathcal F_{m+1}\subseteq\mathcal F_m$ imply $x_{m+1}\leq x_m$ whenever the later layer is nonempty. It is a real parameter, not the actual size of the [set family](#set-family)'s support.

### Shadow ratio for a hereditary set family

↑ **Parent:** [Effective ground-set parameter of a hereditary uniform layer](#effective-ground-set-parameter-of-a-hereditary-uniform-layer)

For a [down-set](#down-set) on $N$ coordinates, let $p_m=|\mathcal F_m|/\binom Nm$. For $1\leq m<N$ with $p_m>0$, the [effective ground-set parameter of a hereditary uniform layer](#effective-ground-set-parameter-of-a-hereditary-uniform-layer) gives the displayed ratio bound. Iteration is valid up to the first empty layer. In particular, whenever $2m\leq N$, $p_{2m}\leq p_m^2$; if the later layer is empty this conclusion is immediate. Ratios with $p_m=0$ are undefined and must be replaced by the assertion that all later layers are empty.

## Coordinate shifts of a set family

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

For distinct coordinates $i,j$, replace a member containing $j$ but not $i$ by its partner with $j$ exchanged for $i$, provided that partner is absent. This [set family](#set-family) operation preserves [cardinality](set-theory.md#cardinality). Repeating shifts with $i<j$ terminates because every change decreases $\sum_{A\in\mathcal F}\sum_{a\in A}a$. Its effect on shadows is described by [coordinate-shift shadow containment](#coordinate-shift-shadow-containment).

### Downward coordinate compression

↑ **Parent:** [Coordinate shifts of a set family](#coordinate-shifts-of-a-set-family)

In a [set family](#set-family), replace a set containing $i$ by its deletion of $i$ only when that deletion is absent. This preserves cardinality and cannot increase maximum pairwise [Hamming distance](coding-theory.md#hamming-distance). If a new set and a retained set gave a larger distance, the retained set's deletion would already have been present; that deletion and the original uncompressed set would give the same distance. Repeated downward compressions yield a [down-set](#down-set).

#### Two cube edges in every direction force many vertices

↑ **Parent:** [Downward coordinate compression](#downward-coordinate-compression)

For a family in the $n$-dimensional [Boolean lattice](#boolean-lattice), the loss of trace cardinality on deleting coordinate $i$ equals the number of pairs $S,S\cup\{i\}$ both in the family. If every direction has at least two such edges, [downward coordinate compression](#downward-coordinate-compression) preserves that property. The resulting [down-set](#down-set) contains the empty set and all $n$ singletons. Each coordinate must also occur in a two-element member. Those pairs cover all $n$ coordinates and number at least $\lceil n/2\rceil$, giving the bound. For $n\ge2$, the empty set, all singletons and a minimum collection of pairs covering every coordinate attain it.

### Coordinate-shift shadow containment

↑ **Parent:** [Coordinate shifts of a set family](#coordinate-shifts-of-a-set-family)

For a [uniform set family](#uniform-set-family), the [lower shadow](#lower-shadow) of its shifted [set family](#set-family) is contained in the shifted [lower shadow](#lower-shadow). Check the witness in the four patterns of membership in coordinates $i,j$. A surviving shadow member containing only $j$ must have both old shadow partners; a member containing only $i$ needs either old partner. Taking complements exchanges $C_{ij}$ with $C_{ji}$ and gives the same containment for the [upper shadow](#upper-shadow). Thus [coordinate shifts of a set family](#coordinate-shifts-of-a-set-family) cannot increase either shadow or their disjoint union, the [external vertex boundary](graph-theory.md#external-vertex-boundary) of a [uniform set family](#uniform-set-family).

## Constant-intersection family bound

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

If distinct members of a [set family](#set-family) on $[n]$ have intersection size $\lambda$, then its size is at most $n$ for $\lambda>0$, and at most $n+1$ for $\lambda=0$, assuming $n\geq1$. In the positive case, use the [Gram matrix](linear-algebra.md#gram-matrix) of the [characteristic vectors of sets](#characteristic-vector-of-a-set); a member of size $\lambda$ is handled by disjoint remainders. In the zero case nonempty members are disjoint.

### Constant t-wise intersection dichotomy

↑ **Parent:** [Constant-intersection family bound](#constant-intersection-family-bound)

Let $m\geq t\geq3$ distinct sets have every $t$-fold intersection of size $\lambda$. Either all contain a common set of size $\lambda$, or $m\leq k+t-2$, where $k$ is the minimum size of a $(t-2)$-fold intersection. Fix such a minimum intersection and restrict the remaining sets to it. Equal traces give the common set; distinct traces satisfy the [constant-intersection family bound](#constant-intersection-family-bound). The qualification $m\geq t$ excludes vacuous counterexamples.

#### Complement-of-singleton extremizers

↑ **Parent:** [Constant t-wise intersection dichotomy](#constant-t-wise-intersection-dichotomy)

The sets $A_i=[m]\setminus\{i\}$ have every $t$-fold intersection of size $m-t$ and every $(t-2)$-fold intersection of size $m-t+2$. For $m\geq t+1$, their common intersection is empty and they attain $m=k+t-2$ in the [constant t-wise intersection dichotomy](#constant-t-wise-intersection-dichotomy).

## Elementary set shift

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

For $i<j$, replace a member $A$ containing $j$ but not $i$ by $(A\setminus\{j\})\cup\{i\}$ only when the replacement is absent. An [elementary set shift](#elementary-set-shift) preserves family size and the [intersecting family](#intersecting-family) property. The inclusion $\partial(S_{ij}\mathcal F)\subseteq S_{ij}(\partial\mathcal F)$ shows that it cannot increase the [lower shadow](#lower-shadow).

### Shifted set family

↑ **Parent:** [Elementary set shift](#elementary-set-shift)

A [set family](#set-family) is shifted if every [elementary set shift](#elementary-set-shift) leaves it unchanged. For a [uniform set family](#uniform-set-family), this is equivalent to downward closure under componentwise comparison of the increasing lists of its elements. Repeated [elementary set shifts](#elementary-set-shift) terminate at a [shifted set family](#shifted-set-family).

#### Ballot reflection injection

↑ **Parent:** [Shifted set family](#shifted-set-family)

For a member of a [shifted set family](#shifted-set-family) that is an [intersecting family](#intersecting-family), find the first prefix with more selected than unselected positions. Reflect membership in that prefix. The result has one fewer element and lies in the [lower shadow](#lower-shadow); the first prefix with more unselected positions gives the inverse. This injection proves the [intersecting shadow lemma](#intersecting-shadow-lemma).

## Odd cross-intersection bound

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

Appending a coordinate one to each [indicator vector](measure-theory.md#indicator-vector) changes every odd cross-intersection dot product into an even one in $\mathbb F_2^{n+1}$. The argument for the [even cross-intersection bound](#even-cross-intersection-bound) then gives the displayed bound. It is a valid bound without a claim that it is sharp.

## Even cross-intersection bound

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

If every cross-intersection of two [set families](#set-family) on $[n]$ has even size, the spans of their [indicator vectors](measure-theory.md#indicator-vector) are orthogonal in $\mathbb F_2^n$. The [orthogonal complement over the binary field](quantum-theory.md#orthogonal-complement-over-the-binary-field) dimension formula bounds the sum of their dimensions by $n$, giving the displayed cardinality bound.

## Weakly intersecting family in a product alphabet

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

Here two words must both have symbols greater than one in some common coordinate, without requiring the symbols to agree. Their supports $S(x)$ therefore form an [intersecting family](#intersecting-family). The fibre of a support of size $r$ contains $(k-1)^r$ words, relating this problem to a weighted [set family](#set-family) problem.

## Bollobas set-pairs inequality

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

For disjoint pairs $A_i,B_i$ such that $A_i\cap B_j\ne\varnothing$ whenever $i\ne j$, the displayed sum is at most one. In a uniformly random [permutation](combinatorics.md#permutation), the events that all of $A_i$ precedes all of $B_i$ are [disjoint events](probability-theory.md#disjoint-events), and their probabilities are the summands. Taking $B_i$ to be the complement of the members $A_i$ of an [antichain](#antichain) recovers the [LYM inequality](#lubell-yamamoto-meshalkin-inequality).

## Separating family of disjoint set pairs

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

A family $(A_i,B_i)_{i=1}^m$ of pairs of disjoint subsets of a finite set separates its points if each two distinct points lie on opposite sides of at least one pair. Empty sides are allowed by this definition. Let $d(x)$ count pairs containing $x$. Associate to $x$ the subcube of $\{0,1\}^m$ fixing coordinate $i$ to zero on $A_i$ and one on $B_i$. Separation makes these subcubes disjoint and yields the [disjoint subcube packing inequality](#disjoint-subcube-packing-inequality).

### Disjoint subcube packing inequality

↑ **Parent:** [Separating family of disjoint set pairs](#separating-family-of-disjoint-set-pairs)

Pairwise disjoint subcubes of $\{0,1\}^m$ fixing $d_1,\ldots,d_n$ coordinates satisfy $\sum_{x=1}^n2^{-d_x}\leq1$. By [Jensen inequality](real-analysis.md#jensen-s-inequality), their average codimension is at least $\log_2n$. Consequently a [separating family of disjoint set pairs](#separating-family-of-disjoint-set-pairs) of total incidence at most $\lambda mn$, with $\lambda>0$, has $m\geq\lceil\log_2n/\lambda\rceil$.

## Symmetric chain decomposition of a Boolean lattice

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

A symmetric chain in the Boolean lattice $\mathcal P([n])$ contains one set of each size from $r$ through $n-r$. A symmetric chain decomposition partitions the Boolean lattice into such chains.

### Symmetric chain in a Boolean lattice

↑ **Parent:** [Symmetric chain decomposition of a Boolean lattice](#symmetric-chain-decomposition-of-a-boolean-lattice)

A [symmetric chain](#symmetric-chain-in-a-boolean-lattice) contains one subset of each size from $k$ to $n-k$, nested by inclusion. Its endpoint ranks sum to $n$. A [symmetric chain decomposition of a Boolean lattice](#symmetric-chain-decomposition-of-a-boolean-lattice) partitions all subsets into such chains.

### Adjacent-level matching in a Boolean lattice

↑ **Parent:** [Symmetric chain decomposition of a Boolean lattice](#symmetric-chain-decomposition-of-a-boolean-lattice)

For $1\leq i\leq n/2$, the inclusion graph between ranks $i-1$ and $i$ of $\mathcal P([n])$ has a matching saturating rank $i-1$. Indeed, each lower vertex has degree $n-i+1$, each upper vertex has degree $i$, and edge counting gives

$$
(n-i+1)|\mathcal A|\leq i|N(\mathcal A)|
$$

for every family $\mathcal A$ in the lower rank. This verifies the condition of the [Hall marriage theorem](graph-theory.md#hall-s-marriage-theorem).

### Minimum chain partition of a Boolean lattice

↑ **Parent:** [Symmetric chain decomposition of a Boolean lattice](#symmetric-chain-decomposition-of-a-boolean-lattice)

The least number of chains partitioning $\mathcal P([n])$ is the size of its largest rank:

$$
\binom n{\lfloor n/2\rfloor}.
$$

The middle rank gives the lower bound because a chain contains at most one member of any rank. Compatible adjacent-level matchings give a symmetric chain decomposition attaining the bound.

## Lexicographic order

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lexicographic_order)

For equal-size subsets $A$ and $B$ of an ordered ground set, $A$ precedes $B$ in lexicographic order when the smallest element of their symmetric difference belongs to $A$.

## Colexicographic order

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Colexicographic_order)

For equal-size finite subsets $A$ and $B$, $A$ precedes $B$ in colexicographic order when the largest element of their symmetric difference belongs to $B$.

### Colexicographic initial segment

↑ **Parent:** [Colexicographic order](#colexicographic-order)

The first $a$ sets of a fixed size in [colexicographic order](#colexicographic-order) form a [colexicographic initial segment](#colexicographic-initial-segment). Its [lower shadow](#lower-shadow) is again a [colexicographic initial segment](#colexicographic-initial-segment) at the next smaller size.

## Set family shadow

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

A shadow moves a uniform set family to an adjacent level of the subset lattice by deleting or adding one element.

### Lower shadow

↑ **Parent:** [Set family shadow](#set-family-shadow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lower_shadow)

The lower shadow of $\mathcal A\subseteq[n]^{(r)}$ is

$$
\partial\mathcal A=\{B\in[n]^{(r-1)}:B\subset A\text{ for some }A\in\mathcal A\}.
$$

#### Iterated lower shadow

↑ **Parent:** [Lower shadow](#lower-shadow)

Repeatedly take the [lower shadow](#lower-shadow) of a [uniform set family](#uniform-set-family). After $j$ steps the result consists of all subsets of its members whose size is $j$ smaller. Iterating the [Kruskal-Katona theorem](#kruskal-katona-theorem) shows that [colexicographic initial segments](#colexicographic-initial-segment) minimize every [iterated lower shadow](#iterated-lower-shadow).

##### Clique counting from iterated shadows

↑ **Parent:** [Iterated lower shadow](#iterated-lower-shadow)

For the [uniform set family](#uniform-set-family) of vertex sets of $r$-cliques, its $(r-2)$-fold [lower shadow](#lower-shadow) consists of graph edges. Repeated use of the [Kruskal-Katona theorem](#kruskal-katona-theorem) bounds clique count from edge count. Sixteen four-cliques have at least twenty-three triples in their shadow and at least eighteen edges in their second shadow, by the expansions $16=\binom64+\binom33$ and $23=\binom63+\binom32$. Hence a graph with fifteen edges has at most fifteen four-cliques, attained by the [complete graph](graph-theory.md#complete-graph) on six vertices.

#### Kruskal-Katona theorem

↑ **Parent:** [Lower shadow](#lower-shadow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kruskal-Katona_theorem)

If

$$
|\mathcal A|=\binom{a_r}{r}+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_s}{s},
\qquad a_r>\cdots>a_s\geq s,
$$

then

$$
|\partial\mathcal A|\geq
\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_s}{s-1}.
$$

Initial segments of [colexicographic order](#colexicographic-order) attain equality.

##### Nonisomorphic colex shadow minimizers

↑ **Parent:** [Kruskal-Katona theorem](#kruskal-katona-theorem)

Minimum-shadow families need not be unique up to permutation. Four edges of a four-cycle and the first four pairs in [colexicographic order](#colexicographic-order) both have four vertices in their [lower shadow](#lower-shadow), but the latter graph has a triangle. For triples, the six sets consisting of two points from $\{1,2,3\}$ and one from $\{4,5\}$ have a nine-pair shadow. The initial six colex triples also have shadow size nine, but their point degrees are $5,4,4,3,2$ instead of $4,4,4,3,3$.

<h5 id="lovasz-shadow-bound">Lovász shadow bound</h5>

↑ **Parent:** [Kruskal-Katona theorem](#kruskal-katona-theorem)

For a nonempty $r$-[uniform set family](#uniform-set-family), define $x>r-1$ by $|\mathcal F|=\binom xr$ using real [binomial coefficients](combinatorics.md#binomial-coefficient). Then its [lower shadow](#lower-shadow) has at least $\binom{x}{r-1}$ members. This continuous estimate is often easier to use than the exact integer expansion in the [Kruskal-Katona theorem](#kruskal-katona-theorem).

A short proof uses [coordinate shifts of a set family](#coordinate-shifts-of-a-set-family). In a fully left-shifted [set family](#set-family) split at coordinate one into $\mathcal F_0$ and $\mathcal F_1$, deleting one in the present section. The shifting property implies $\partial\mathcal F_0\subseteq\mathcal F_1$, and the total [lower shadow](#lower-shadow) has size $|\mathcal F_1|+|\partial\mathcal F_1|$. Induct on uniformity and, at fixed uniformity, on [set family](#set-family) size. If $|\mathcal F_1|<\binom{x-1}{r-1}$, the [Pascal's identity](combinatorics.md#pascal-s-rule) and the size [mathematical induction](foundations-of-mathematics.md#mathematical-induction) force $|\partial\mathcal F_0|>\binom{x-1}{r-1}$, a contradiction. The uniformity [mathematical induction](foundations-of-mathematics.md#mathematical-induction) applied to $\mathcal F_1$, followed by the [Pascal's identity](combinatorics.md#pascal-s-rule), proves the estimate. Integer $x$ is sharp for the full $r$-level on $x$ coordinates.

##### Colexicographic section compression

↑ **Parent:** [Kruskal-Katona theorem](#kruskal-katona-theorem)

Split a [uniform set family](#uniform-set-family) into the section avoiding a coordinate and the section containing it, with that coordinate removed. Replace each section by a [colexicographic initial segment](#colexicographic-initial-segment) of the same size. Induction on the ground-set size, and nesting of initial segments, show that this operation cannot enlarge the [lower shadow](#lower-shadow).

##### Binomial-shadow arithmetic lemma

↑ **Parent:** [Kruskal-Katona theorem](#kruskal-katona-theorem)

Let $f_r(m)$ be the lower-shadow size prescribed by the binomial representation in the [Kruskal-Katona theorem](#kruskal-katona-theorem). Then

$$
f_r(a+b)\leq\max\{f_r(a),b\}+f_{r-1}(b).
$$

Induction using [Pascal's identity](combinatorics.md#pascal-s-rule) proves the inequality and drives the standard ground-set induction for the theorem.

##### UV-compression

↑ **Parent:** [Kruskal-Katona theorem](#kruskal-katona-theorem)

Let $U,V\subseteq[n]$ be disjoint and have the same [cardinality](set-theory.md#cardinality). For a set $A$, its $UV$-compression is

$$
C_{U,V}(A)=
\begin{cases}
(A\setminus V)\cup U,&A\cap(U\cup V)=V,\\
A,&\text{otherwise}.
\end{cases}
$$

For a [uniform set family](#uniform-set-family) $\mathcal A$, a member is replaced only when its image is absent from $\mathcal A$; this convention preserves the family's cardinality.

###### Intersection-preserving lexicographic UV-compression

↑ **Parent:** [UV-compression](#uv-compression)

Let $U,V$ be disjoint, equally sized, nonempty [sets](set.md), with $\min U<\min V$. Suppose an [intersecting family](#intersecting-family) is unchanged by all such [UV-compressions](#uv-compression) of smaller size. Then its $(U,V)$-[UV-compression](#uv-compression) is still an [intersecting family](#intersecting-family). Indeed, a newly moved member $A'=(A\setminus V)\cup U$ can only be disjoint from a retained old member $B$, since two newly moved members share $U$. Here $B\cap U=\varnothing$ and $V'=B\cap V\ne\varnothing$. If $V'=V$, retaining $B$ forces $(B\setminus V)\cup U$ to have been present, contradicting the old [intersection](set.md#set-intersection) property with $A$. Otherwise choose $U'\subset U$ with $|U'|=|V'|$ and $\min U\in U'$. Stability under the smaller $(U',V')$-[UV-compression](#uv-compression) forces $(A\setminus V')\cup U'$ to be present; this member is disjoint from $B$, again a contradiction. Repeatedly applying a changing [UV-compression](#uv-compression) of smallest size terminates, since the sum of [lexicographic order](#lexicographic-order) positions decreases. A terminal [set family](#set-family) is a [lexicographic](#lexicographic-order) initial segment: a missing earlier member $X$ and present later member $Y$ would be moved by $U=X\setminus Y$, $V=Y\setminus X$.

###### Left-compressed set family

↑ **Parent:** [UV-compression](#uv-compression)

A set family is left-compressed when replacing a member $j$ by a missing smaller element $i<j$ always produces another member. Equivalently, it is fixed by every $\{i\},\{j\}$-compression with $i<j$.

###### Shadow lemma for UV-compressions

↑ **Parent:** [UV-compression](#uv-compression)

Suppose that for every $x\in U$ there is a $y\in V$ such that $\mathcal A$ is fixed by the smaller compression $C_{U\setminus\{x\},V\setminus\{y\}}$. Then

$$
\left|\partial C_{U,V}(\mathcal A)\right|\leq|\partial\mathcal A|.
$$

Indeed, deleting an element outside $U$ from a newly compressed member gives the $UV$-compression of an old shadow member. If the deleted element is $x\in U$, stability under the chosen smaller compression shows that the resulting set already belongs to the old [lower shadow](#lower-shadow). Thus

$$
\partial C_{U,V}(\mathcal A)\subseteq C_{U,V}(\partial\mathcal A),
$$

and compression preserves cardinality.

##### UV-compression proof of the Kruskal-Katona theorem

↑ **Parent:** [Kruskal-Katona theorem](#kruskal-katona-theorem)

If a uniform family is not an initial [colexicographic](#colexicographic-order) segment, choose a nontrivial $UV$-compression with $\max U<\max V$ and with $|U|$ minimal. The minimal choice supplies the smaller-compression hypotheses of the [Shadow lemma for UV-compressions](#shadow-lemma-for-uv-compressions), so the operation does not increase the [lower shadow](#lower-shadow). It strictly decreases the integer weight

$$
\sum_{A\in\mathcal A}\sum_{i\in A}2^i,
$$

because the largest element of $U\cup V$ belongs to $V$. Iteration therefore terminates. A terminal family must be an initial colexicographic segment: otherwise an earlier absent set and a later present set supply one more admissible compression. The shadow of that segment has the size in the [Kruskal-Katona theorem](#kruskal-katona-theorem), proving the theorem.

### Upper shadow

↑ **Parent:** [Set family shadow](#set-family-shadow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Upper_shadow)

The upper shadow of $\mathcal A\subseteq[n]^{(r)}$ is

$$
\nabla\mathcal A=\{B\in[n]^{(r+1)}:A\subset B\text{ for some }A\in\mathcal A\}.
$$

Among families of fixed size, an initial [lexicographic](#lexicographic-order) segment minimizes its upper shadow.

## Frankl-Wilson theorem

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

Let $p$ be a [prime number](number-theory.md#prime-number), let $L\subseteq\mathbb F_p$ have $s\leq\min\{k,n-k\}$ elements, and suppose $\mathcal A\subseteq[n]^{(k)}$ satisfies $|A\cap B|\bmod p\in L$ for distinct members while $k\bmod p\notin L$. The Frankl-Wilson theorem gives

$$
|\mathcal A|\leq\binom ns.
$$

Its [polynomial method in combinatorics](combinatorics.md#polynomial-method-in-combinatorics) turns modular intersection restrictions into linearly independent functions represented by square-free monomials of degree $s$.

### Modular intersection graph

↑ **Parent:** [Frankl-Wilson theorem](#frankl-wilson-theorem)

For a [prime number](number-theory.md#prime-number) $p$, the [vertices](graph.md#vertex-graph-theory) are $k$-subsets of $[N]$. An [independent set](graph-theory.md#independent-set-graph-theory) avoids the only off-diagonal intersection congruent to $k$ modulo $p$, so the [Frankl-Wilson theorem](#frankl-wilson-theorem) bounds its size by $\binom N{p-1}$. A [clique](graph-theory.md#clique-graph-theory) has constant intersection $p-1$ and has size at most $N$, by the same theorem modulo a prime larger than $k$. This explicit [graph](graph.md) gives an asymmetric [Ramsey number](ramsey-theory.md#ramsey-number) lower bound and an exponential [chromatic number](graph-theory.md#chromatic-number) lower bound.

### Modular intersection polynomial

↑ **Parent:** [Frankl-Wilson theorem](#frankl-wilson-theorem)

If member sizes modulo a [prime number](number-theory.md#prime-number) $p$ avoid $L$ while distinct intersections lie in $L$, evaluation at [characteristic vectors of sets](#characteristic-vector-of-a-set) gives a diagonal matrix with nonzero diagonal. After [multilinear reduction on the Boolean cube](polynomial.md#multilinear-reduction-on-the-boolean-cube), these [polynomials](polynomial.md) remain [linearly independent](vector-space.md#linear-independence) and have degree at most $|L|$. Counting square-free [monomials](polynomial.md#monomial) proves $|\mathcal F|\leq\sum_{j=0}^{|L|}\binom nj$. On a fixed uniform layer, the [low-degree evaluation rank on a uniform layer](#low-degree-evaluation-rank-on-a-uniform-layer) sharpens this to $\binom n{|L|}$ when $|L|$ does not exceed the layer rank.

### Complement splitting for forbidden midpoint intersections

↑ **Parent:** [Frankl-Wilson theorem](#frankl-wilson-theorem)

For a prime $p$, take rank-$2p$ subsets of $[4p]$ with no distinct pair meeting in $p$ points. Split by membership of coordinate one. In the containing part, remove that coordinate; in the avoiding part, first take complements and then remove it. Both transformed families have rank $2p-1$ on $4p-1$ points. Their distinct intersections avoid residue $p-1$ modulo $p$. The uniform [Frankl-Wilson theorem](#frankl-wilson-theorem) bounds each by $\binom{4p-1}{p-1}$, yielding the displayed stronger form of the requested bound.

#### Fixed-core construction avoiding midpoint intersections

↑ **Parent:** [Complement splitting for forbidden midpoint intersections](#complement-splitting-for-forbidden-midpoint-intersections)

Fix a $(p+1)$-set $B\subseteq[4p]$. Take every $2p$-set $B\cup X$ with $X$ a $(p-1)$-subset of the remaining $3p-1$ points, together with the complements of all these sets. Within either half, intersections have size at least $p+1$. Across the halves they have size $|X\setminus Y|\leq p-1$. Thus no intersection has size $p$, and the two disjoint halves give the displayed family size.

### Prime-power modular intersection bound

↑ **Parent:** [Frankl-Wilson theorem](#frankl-wilson-theorem)

Let $m=p^a$ and let an $r$-[uniform set family](#uniform-set-family) have no distinct pair whose intersection is congruent to $r$ modulo $m$. Its size is bounded as displayed; the customary nontrivial form $\binom n{m-1}$ requires $m-1\le r$. The [Lucas theorem](combinatorics.md#lucas-s-theorem) makes $\binom{z-r+m-1}{m-1}$ a residue detector modulo $p$, equal to one exactly when $z\equiv r\pmod m$. Its Boolean evaluation functions have degree at most $m-1$ and a diagonal evaluation matrix on the family. The [low-degree evaluation rank on a uniform layer](#low-degree-evaluation-rank-on-a-uniform-layer) supplies the sharp dimension bound. Without the size qualification, three singletons with $n=3,r=1,m=4$ contradict the customary printed form, since $3>\binom33$.

### Modular-size auxiliary polynomials

↑ **Parent:** [Frankl-Wilson theorem](#frankl-wilson-theorem)

In the [polynomial method in combinatorics](combinatorics.md#polynomial-method-in-combinatorics), a [set family](#set-family) of sets with common size residue $r$ modulo a [prime number](number-theory.md#prime-number) $p$ annihilates the displayed auxiliary functions. After [multilinear reduction on the Boolean cube](polynomial.md#multilinear-reduction-on-the-boolean-cube), functions with $|S|\leq s-1$ have degree at most $s$. If $r$ avoids every $j=0,\ldots,s-1$ modulo $p$, these functions are [linearly independent](vector-space.md#linear-independence): evaluation at a set $T$ gives $(|T|-r)\sum_{S\subseteq T}c_S$, and increasing $|T|$ eliminates coefficients. Combining them with diagonal [intersection polynomials](combinatorics.md#intersection-polynomial) removes the lower-degree monomial count and strengthens the dimension bound from $\sum_{j\leq s}\binom nj$ to $\binom ns$.

### Modular layer vanishing lemma

↑ **Parent:** [Frankl-Wilson theorem](#frankl-wilson-theorem)

Let $p$ be a [prime number](number-theory.md#prime-number), $0\leq a<p$, $1\leq s<p$, and $n\geq a+s$. A [multilinear polynomial](polynomial.md#multilinear-polynomial) over $\mathbb F_p$ of degree less than $s$ that vanishes on every Boolean vertex whose weight is not congruent to $a$ modulo $p$ vanishes everywhere. Alternating sums over intervals of $s$ free coordinates eliminate the possible nonzero weight levels one at a time. This proves independence of the auxiliary functions used for the uniform [Frankl-Wilson theorem](#frankl-wilson-theorem) bound.

### Nonuniform Frankl-Wilson theorem

↑ **Parent:** [Frankl-Wilson theorem](#frankl-wilson-theorem)

Let $p$ be a [prime number](number-theory.md#prime-number) and $L\subseteq\mathbb F_p$ have $s$ elements. A [set family](#set-family) whose member sizes modulo $p$ avoid $L$, and whose distinct pairwise intersection sizes modulo $p$ belong to $L$, has at most $\sum_{j=0}^{\min(s,n)}\binom nj$ members. The [intersection polynomials](combinatorics.md#intersection-polynomial) $\prod_{\ell\in L}(\sum_{i\in A}x_i-\ell)$ have a diagonal, nonzero evaluation matrix on the family's [characteristic vectors of sets](#characteristic-vector-of-a-set). [Multilinear reduction on the Boolean cube](polynomial.md#multilinear-reduction-on-the-boolean-cube) places these [linearly independent](vector-space.md#linear-independence) functions in the space spanned by square-free [monomials](polynomial.md#monomial) of degree at most $s$.

<h3 id="ray-chaudhuri-wilson-theorem">Ray-Chaudhuri–Wilson theorem</h3>

↑ **Parent:** [Frankl-Wilson theorem](#frankl-wilson-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ray-Chaudhuri–Wilson_theorem)

If a $k$-uniform set family on an $n$-element ground set has at most $s$ possible intersection sizes between distinct members, then its size is at most $\binom ns$. The proof uses the linear independence of incidence polynomials on the $k$-slice.

## Set family

↑ **Parent:** [Extremal set theory](extremal-set-theory.md)

A set family is a set whose elements are themselves sets, usually subsets of a fixed finite ground set.

### Helly family

↑ **Parent:** [Set family](#set-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helly_family)

A [Helly family](#helly-family) of order $k$ is a [set family](#set-family) for which every finite subfamily has nonempty total intersection whenever each of its subfamilies with at most $k$ members has nonempty intersection. Convex subtrees of a tree have Helly order two.

### Incidence matrix of a set system

↑ **Parent:** [Set family](#set-family)

For a finite ground [set](set.md) and an indexed [set family](#set-family), this zero-one [matrix](vector-space.md#matrix) records membership of points in members. The diagonal entries of $B^TB$ are member sizes, and its off-diagonal entries count pairwise [intersections](set.md#set-intersection). For the [Fano plane](projective-space.md#fano-plane), either point-line orientation gives the identity $B^TB=2I+J$, since every point lies on three lines and each distinct point pair lies on one line.

### Diagonal-intersection set-pair bound

↑ **Parent:** [Set family](#set-family)

Suppose $|R_i|=r$, $|S_i|=s$ and $R_i\cap S_j$ is nonempty exactly when $i=j$. Choose $x_i\in R_i\cap S_i$. Each witness lies in neither set of any other pair, so the witnesses are distinct. For two distinct indices, $R_i\setminus\{x_i\}$ and $S_j\setminus\{x_j\}$ are disjoint subsets outside the witness set. Thus $n-|I|\geq r+s-2$. Equality is attained by disjoint fixed cores $P,Q$ of sizes $r-1,s-1$ and distinct remaining witnesses, with $R_i=P\cup\{x_i\}$ and $S_i=Q\cup\{x_i\}$.

### Union and intersection of set families

↑ **Parent:** [Set family](#set-family)

For [set families](#set-family), $\mathcal A\vee\mathcal B=\{A\cup B:A\in\mathcal A,B\in\mathcal B\}$ and $\mathcal A\wedge\mathcal B=\{A\cap B:A\in\mathcal A,B\in\mathcal B\}$. These are families of distinct sets, rather than multisets indexed by pairs. The [four functions theorem](#ahlswede-daykin-inequality) gives $|\mathcal A\vee\mathcal B|\,|\mathcal A\wedge\mathcal B|\ge|\mathcal A|\,|\mathcal B|$. Complementing one input family yields the analogous product bound for pairwise [set differences](set.md#set-difference).

<h3 id="ahlswede-daykin-inequality">Ahlswede–Daykin inequality</h3>

↑ **Parent:** [Set family](#set-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ahlswede–Daykin_inequality)

For nonnegative functions on a finite [Boolean lattice](#boolean-lattice), the condition $\alpha(A)\beta(B)\le\gamma(A\cup B)\delta(A\cap B)$ for all pairs implies $(\sum\alpha)(\sum\beta)\le(\sum\gamma)(\sum\delta)$. Coordinate elimination and the [two-point four-functions inequality](#two-point-four-functions-inequality) prove it by induction. Indicators give inequalities for the [union and intersection of set families](#union-and-intersection-of-set-families). The Boolean-lattice statement appears in [Theorem 3.1 of Nicholas Ruozzi's paper](https://proceedings.neurips.cc/paper_files/paper/2012/file/03afdbd66e7929b125f8597834fa83a4-Paper.pdf).

#### Two-point four-functions inequality

↑ **Parent:** [Ahlswede–Daykin inequality](#ahlswede-daykin-inequality)

Suppose nonnegative numbers satisfy $a_0b_0\le c_0d_0$, $a_1b_1\le c_1d_1$, and $a_0b_1,a_1b_0\le c_1d_0$. Set $x=a_0b_1$, $y=a_1b_0$, $M=c_1d_0$, $N=c_0d_1$. Then $x,y\le M$ and $xy\le MN$. For $M>0$, $(M-x)(M-y)\ge0$ gives $x+y\le M+xy/M\le M+N$; for $M=0$, $x=y=0$. Adding the two diagonal bounds proves $(a_0+a_1)(b_0+b_1)\le(c_0+c_1)(d_0+d_1)$. This lets the [four functions theorem](#ahlswede-daykin-inequality) sum out one Boolean coordinate while preserving its pointwise hypothesis.

### Biased measure of a set family

↑ **Parent:** [Set family](#set-family)

The [biased measure of a set family](#biased-measure-of-a-set-family) is its probability when each ground-set element is independently included with probability $p$. If $a_j$ is the proportion of the $j$th level occupied by the family, then $\mu_p(\mathcal F)=\sum_j\binom nj a_jp^j(1-p)^{n-j}$. This translates a combinatorial level bound into a probability inequality for independent [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution).

### Self-dual set family

↑ **Parent:** [Set family](#set-family)

A [self-dual set family](#self-dual-set-family) on $[n]$ contains exactly one of $A,A^c$ for every subset $A$. Its relative proportions $a_j$ in complementary uniform levels satisfy $a_{n-j}=1-a_j$. In particular its measure under a uniform random subset is $1/2$.

#### Complementary-layer bound for biased measure

↑ **Parent:** [Self-dual set family](#self-dual-set-family)

Suppose a [self-dual set family](#self-dual-set-family) has level proportions $a_j\le j/n$ for $j<n/2$. Subtract the binomial identity $p=\sum_j\binom nj(j/n)p^j(1-p)^{n-j}$ from its [biased measure of a set family](#biased-measure-of-a-set-family) and pair levels $j,n-j$. The difference is

$$
\mu_p(\mathcal F)-p=\sum_{j<n/2}\binom nj(j/n-a_j)[p^{n-j}(1-p)^j-p^j(1-p)^{n-j}].
$$

Every term is nonnegative for $p\ge1/2$. A self-dual [intersecting family](#intersecting-family) has the required level bounds by the [Erdős-Ko-Rado theorem](#erdos-ko-rado-theorem).

##### Weighted Bernoulli majority bound

↑ **Parent:** [Complementary-layer bound for biased measure](#complementary-layer-bound-for-biased-measure)

Let $c_i\ge0$ sum to one, with no subset sum equal to $1/2$, and let independent [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) $Z_i$ all have parameter $p\ge1/2$. The subsets of weight greater than $1/2$ form an intersecting [self-dual set family](#self-dual-set-family). The [complementary-layer bound for biased measure](#complementary-layer-bound-for-biased-measure) proves $\mathbb P(\sum_ic_iZ_i\ge1/2)\ge p$. Nonnegative weights ensure that disjoint sets cannot both have weight greater than $1/2$; the no-tie condition supplies self-duality.

### Laminar family of sets

↑ **Parent:** [Set family](#set-family)

A [set family](#set-family) is laminar if any two members are disjoint or one contains the other. Its distinct inclusion-maximal members are therefore disjoint. Applied to the true sets in a hierarchical family of [intersection hypotheses](statistical-modelling.md#intersection-hypothesis), this gives the disjoint-block bound used for [familywise error control for a laminar hypothesis family](statistical-modelling.md#familywise-error-control-for-a-laminar-hypothesis-family).

### Union-intersection compression

↑ **Parent:** [Set family](#set-family)

An elementary union-intersection compression of a finite [multiset](set.md#multiset) of subsets replaces occurrences of $A,B$ by $A\cup B,A\cap B$. A compression is a finite sequence of these moves. The move preserves every coordinate multiplicity. On incomparable sets it increases $\sum_S|S|^2$ by $2|A\setminus B||B\setminus A|$, so repeated compression reaches a chain under inclusion. For any [submodular set function](function.md#submodular-set-function), the sum of its values cannot increase.

### Cross-Sperner family

↑ **Parent:** [Set family](#set-family)

Two [set families](#set-family) $\mathcal A,\mathcal B$ are cross-Sperner when no member of either is a [subset](set.md#subset) of a member of the other, including equality. Thus $\mathcal A\cap\mathcal B=\varnothing$. Neither family need itself be an [antichain](#antichain). On the [Boolean lattice](#boolean-lattice) of [subsets](set.md#subset) of $[n]$, the [Cross-Sperner inequality](#cross-sperner-inequality) bounds $\sqrt{|\mathcal A|}+\sqrt{|\mathcal B|}$ by $2^{n/2}$.

### Hitting set

↑ **Parent:** [Set family](#set-family)

A [set](set.md) $H$ is a hitting set for a [set family](#set-family) $\mathcal F$ if $H\cap A\ne\varnothing$ for every $A\in\mathcal F$. Every [set](set.md) is a hitting set for an empty [set family](#set-family); none is a hitting set for a family containing the empty [set](set.md). Bounded hitting sets permit finite certificates for some infinite [set families](#set-family), as in the [bounded-size transversal kernel](#bounded-size-transversal-kernel).

#### Bounded-size transversal kernel

↑ **Parent:** [Hitting set](#hitting-set)

If the members of a possibly infinite [set family](#set-family) $\mathcal F$ have size at most $r$, there is a finite [subset](set.md#subset) $\mathcal F_0\subseteq\mathcal F$ of size at most $M(r,s)$ with exactly the same [hitting sets](#hitting-set) of size at most $s$. Use [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on $s$. For nonempty $\mathcal F$, choose $A_0\in\mathcal F$. When $s=0$ this one member suffices. Otherwise, for each $x\in A_0$, retain an inductive kernel for $\mathcal F_x=\{A\in\mathcal F:x\notin A\}$ at parameter $s-1$, and take their [set union](set.md#set-union) together with $A_0$. Its size is at most $1+rM(r,s-1)=M(r,s)$. A [hitting set](#hitting-set) $H$ for this kernel meets $A_0$ at some $x$; $H\setminus\{x\}$ meets the kernel for $\mathcal F_x$, hence all of $\mathcal F_x$, while $x$ meets the other members of $\mathcal F$. If $A_0$ is empty no [hitting set](#hitting-set) exists, and if $\mathcal F$ is empty its kernel is empty. Only finite branching is used, so no finiteness assumption on $\mathcal F$ is needed.

### Boolean lattice

↑ **Parent:** [Set family](#set-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boolean_lattice)

The Boolean lattice is the [power set](set.md#power-set) of a finite set ordered by inclusion. Its rank-$h$ level consists of all $h$-element subsets.

#### Kleitman diametric theorem

↑ **Parent:** [Boolean lattice](#boolean-lattice)

A family in the Boolean lattice whose pairwise Hamming distances are at most $d<n$ has size at most $D(n,d)$. Downward compression followed by [elementary set shifts](#elementary-set-shift) preserves the distance bound. In the resulting down-set, the section containing the last coordinate has diameter at most $d-2$: two members leave a coordinate free, and shifting the last coordinate to it creates a pair with two additional disagreements. This gives the recurrence $D(n,d)=D(n-1,d)+D(n-1,d-2)$. The boundary case $d=n-1$ follows by pairing complementary sets. Hamming balls attain the even case; the union of two radius-$q$ balls with adjacent centers attains the odd case.

#### Injectivity of inclusion between adjacent set layers

↑ **Parent:** [Boolean lattice](#boolean-lattice)

If $n\geq2d+1$ and the [field characteristic](algebra.md#characteristic-of-a-field) is zero or greater than $d+1$, the matrix recording inclusion of $d$-sets in $(d+1)$-sets has full row [rank](linear-algebra.md#rank-one-quadratic-form). Subtracting equations on sets differing in one coordinate reduces the kernel problem to degree $d-1$ on $n-2$ coordinates. [Mathematical induction](foundations-of-mathematics.md#mathematical-induction) then makes all coefficients equal, and the factor $d+1$ forces them to vanish. This gives the auxiliary-polynomial independence used in the uniform [Frankl-Wilson theorem](#frankl-wilson-theorem).

#### Up-set

↑ **Parent:** [Boolean lattice](#boolean-lattice)

An up-set is a family $\mathcal U$ such that $A\in\mathcal U$ and $A\subseteq B$ imply $B\in\mathcal U$.

An up-set is upward closed under inclusion: if $A$ belongs and $A\subseteq B$, then $B$ belongs. This is the Boolean-lattice case of [upper and lower sets](set.md#upper-and-lower-sets).

#### Down-set

↑ **Parent:** [Boolean lattice](#boolean-lattice)

A down-set is a family $\mathcal D$ such that $A\in\mathcal D$ and $B\subseteq A$ imply $B\in\mathcal D$. It is the complement of an up-set within the same Boolean lattice.

This is the downward-closed Boolean-lattice case of [upper and lower sets](set.md#upper-and-lower-sets).

##### Edge boundary of a down-set in a cube

↑ **Parent:** [Down-set](#down-set)

For a [down-set](#down-set) $D$ in the [Boolean lattice](#boolean-lattice), every member $A$ has all its $|A|$ immediate lower neighbors in $D$. Counting an internal edge at its upper endpoint gives $e(D)=\sum_{A\in D}|A|$. The degree identity for the [edge boundary](combinatorics.md#edge-boundary-in-a-graph) of the [hypercube graph](graph.md#hypercube-graph) then gives the displayed formula.

###### Largest edge boundary of a down-set

↑ **Parent:** [Edge boundary of a down-set in a cube](#edge-boundary-of-a-down-set-in-a-cube)

For a [down-set](#down-set) of size $m$, maximize its [edge boundary](combinatorics.md#edge-boundary-in-a-graph) by minimizing the sum of the sizes of its members. Choose all sets in the smallest ranks, followed by any needed part of the next rank; this minimizes that sum among all families and is itself a down-set. With $M_j=\sum_{i=0}^j\binom ni$, $M_{-1}=0$, and $M_{r-1}\le m\le M_r$, the exact maximum is $h(m)=nm-2[\sum_{j<r}j\binom nj+r(m-M_{r-1})]$.

##### Downward closure of a set family

↑ **Parent:** [Down-set](#down-set)

For a [set family](#set-family) $\mathcal A\subseteq\mathcal P([n])$, its downward closure is $\downarrow\mathcal A=\{S:\text{some }A\in\mathcal A\text{ has }S\subseteq A\}$. It is the smallest [down-set](#down-set) containing $\mathcal A$, just as the [upward closure of a set family](#upward-closure-of-a-set-family) is the smallest [up-set](#up-set) containing it. The two closures allow [Harris' inequality](probability-inequality.md#harris-inequality) to control sizes of a [cross-Sperner family](#cross-sperner-family) pair.

#### Antichain

↑ **Parent:** [Boolean lattice](#boolean-lattice)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antichain)

An antichain is a family of sets no one of which contains another.

##### Maximal chain in a Boolean lattice

↑ **Parent:** [Antichain](#antichain)

A maximal chain in $\mathcal P([n])$ contains one set of every cardinality from zero to $n$, with each set obtained from the preceding one by adding a single element.

###### Uniformly random maximal chain in a Boolean lattice

↑ **Parent:** [Maximal chain in a Boolean lattice](#maximal-chain-in-a-boolean-lattice)

A uniformly random maximal chain is obtained from a uniformly random ordering of the ground set by taking its successive initial segments. A fixed $h$-element set occurs with probability $\binom nh^{-1}$.

##### Lubell-Yamamoto-Meshalkin inequality

↑ **Parent:** [Antichain](#antichain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lubell–Yamamoto–Meshalkin_inequality)

If $\mathcal A$ is an antichain in $\mathcal P([n])$ and $\mathcal A_h$ is its rank-$h$ part, then

$$
\sum_{h=0}^n\frac{|\mathcal A_h|}{\binom nh}\leq1.
$$

The left side is the expected number of members of $\mathcal A$ on a [Uniformly random maximal chain in a Boolean lattice](#uniformly-random-maximal-chain-in-a-boolean-lattice).

###### Equality in the LYM inequality

↑ **Parent:** [Lubell-Yamamoto-Meshalkin inequality](#lubell-yamamoto-meshalkin-inequality)

An [antichain](#antichain) in the [Boolean lattice](#boolean-lattice) has [Lubell mass](#lubell-mass) one if and only if it is a full rank level. Equality means every [maximal chain in a Boolean lattice](#maximal-chain-in-a-boolean-lattice) meets the family exactly once. Swapping two adjacent entries in the defining [permutation](combinatorics.md#permutation) then forces the family to contain every set obtained from one member by exchanging an included and an excluded element, hence every set of that rank.

###### Lubell mass

↑ **Parent:** [Lubell-Yamamoto-Meshalkin inequality](#lubell-yamamoto-meshalkin-inequality)

The Lubell mass of a set family $\mathcal A\subseteq\mathcal P([n])$ is

$$
\lambda(\mathcal A)=\sum_{A\in\mathcal A}\binom n{|A|}^{-1}.
$$

It is the [expected value](probability-theory.md#expected-value) of the number of members of $\mathcal A$ on a [Uniformly random maximal chain in a Boolean lattice](#uniformly-random-maximal-chain-in-a-boolean-lattice).

###### Local LYM inequality

↑ **Parent:** [Lubell-Yamamoto-Meshalkin inequality](#lubell-yamamoto-meshalkin-inequality)

For $\mathcal A\subseteq[n]^{(r)}$, the local LYM inequality says

$$
\frac{|\partial\mathcal A|}{\binom n{r-1}}
\geq\frac{|\mathcal A|}{\binom nr}.
$$

It follows by counting pairs $(B,A)$ with $B\subset A$, $|B|=r-1$, and $A\in\mathcal A$.

###### Connectedness of adjacent-level incidence in a Boolean lattice

↑ **Parent:** [Local LYM inequality](#local-lym-inequality)

The bipartite inclusion [graph](graph.md) between consecutive nonempty ranks of the [Boolean lattice](#boolean-lattice) is connected. Two rank-$r$ sets differing by one exchanged element share their rank-$(r+1)$ union as a neighbour; successive exchanges connect any two rank-$r$ sets. Every upper vertex has a lower neighbour. For the two middle ranks of an odd-dimensional [Boolean lattice](#boolean-lattice) the [graph](graph.md) is regular, so equality in the [Local LYM inequality](#local-lym-inequality) for a nonempty upper family forces the whole upper rank: equality admits no [edges](graph-theory.md#edge-of-a-graph) from its [lower shadow](#lower-shadow) to the remaining upper [vertices](graph.md#vertex-graph-theory).

###### Iterated local LYM inequality

↑ **Parent:** [Local LYM inequality](#local-lym-inequality)

Repeatedly applying the [Local LYM inequality](#local-lym-inequality) to upper shadows gives

$$
\frac{|\nabla^s\mathcal A|}{\binom n{r+s}}
\geq\frac{|\mathcal A|}{\binom nr}
$$

for $\mathcal A\subseteq[n]^{(r)}$ and $0\leq s\leq n-r$. The analogous statement for iterated lower shadows follows directly from the stated lower-shadow form.

<h6 id="sperner-s-theorem">Sperner's theorem</h6>

↑ **Parent:** [Lubell-Yamamoto-Meshalkin inequality](#lubell-yamamoto-meshalkin-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sperner's_theorem)

Every antichain in $\mathcal P([n])$ has at most $\binom n{\lfloor n/2\rfloor}$ members. Equality is attained only by a full middle level, with either middle level possible when $n$ is odd.

###### Littlewood-Offord inequality

↑ **Parent:** [Sperner's theorem](#sperner-s-theorem)

For vectors of norm at least one, the number of signed sums in an open unit ball is at most the central binomial coefficient. In one dimension this follows from the [antichain](#antichain) bound. In Euclidean spaces a [separated block decomposition for vector subset sums](#separated-block-decomposition-for-vector-subset-sums) supplies the same bound without assuming all vectors have positive projection in one common direction. Signed sums are counted with multiplicity, by their sign choices.

###### Two-level Littlewood-Offord bound

↑ **Parent:** [Littlewood-Offord inequality](#littlewood-offord-inequality)

For real coefficients of absolute value at least one, an open interval of length four contains at most the sum of the two largest binomial coefficients of signed sums. The corresponding subset family has no three-element inclusion chain. Its [Lubell mass](#lubell-mass) is therefore at most two, giving the bound by allocating mass to the two largest levels. Unit coefficients attain it at a center midway between the two chosen sum levels.

###### Separated block decomposition for vector subset sums

↑ **Parent:** [Littlewood-Offord inequality](#littlewood-offord-inequality)

For Euclidean vectors $x_i$ of length at least one, their labeled subset sums can be partitioned into pairwise distance-at-least-one blocks, with $\binom nr-\binom n{r-1}$ blocks of size $n-2r+1$. To extend a separated block by a vector $x$, choose its member $y$ minimizing inner product with $x$. The translated block together with $y$ remains separated, since $(z+x-y)\cdot x\geq\|x\|^2$. The untransformed block with $y$ removed remains separated too. Block sizes change from $\ell$ to $\ell+1,\ell-1$, the same recurrence as a [symmetric chain decomposition of a Boolean lattice](#symmetric-chain-decomposition-of-a-boolean-lattice). There are exactly $\binom n{\lfloor n/2\rfloor}$ nonempty blocks.

###### Equality in Sperner theorem

↑ **Parent:** [Sperner's theorem](#sperner-s-theorem)

The maximum [antichains](#antichain) in the [Boolean lattice](#boolean-lattice) are exactly its full middle levels. For even $n$ there is one such level, and for odd $n$ either middle level works. The [LYM inequality](#lubell-yamamoto-meshalkin-inequality) first confines a maximum antichain to those levels; connectedness of the regular inclusion [bipartite graph](graph-theory.md#bipartite-graph) rules out a mixture of the two odd middle levels.

##### k-Sperner family

↑ **Parent:** [Antichain](#antichain)

A $k$-Sperner family contains no inclusion chain of length $k+1$. Every [maximal chain in a Boolean lattice](#maximal-chain-in-a-boolean-lattice) therefore meets it in at most $k$ members, so its [Lubell mass](#lubell-mass) is at most $k$.

###### Weighted theorem for k-Sperner families

↑ **Parent:** [k-Sperner family](#k-sperner-family)

For positive weights $w(i)$ depending only on rank, put $u_i=\binom ni w(i)$. The largest weight of a [k-Sperner family](#k-sperner-family) in $\mathcal P([n])$ is the sum of the $k$ largest $u_i$. Every maximizing family is a union of $k$ full rank levels. To see the equality assertion, its [Lubell mass](#lubell-mass) must be $k$; decomposing it into $k$ [antichains](#antichain) by chain height and using [equality in the LYM inequality](#equality-in-the-lym-inequality) forces each part to be a full level.

###### Number of maximizing weighted k-Sperner families

↑ **Parent:** [Weighted theorem for k-Sperner families](#weighted-theorem-for-k-sperner-families)

If $t$ is the $k$th largest rank weight $u_i$, exactly $h$ levels have weight greater than $t$, and exactly $s$ have weight $t$, then there are $\binom{s}{k-h}$ maximizing families. For fixed $n,k$, the possible counts are exactly $\binom{s}{j}$ with $1\leq j\leq k$ and $j\leq s\leq n+1-k+j$.

<h6 id="erdos-theorem-on-k-sperner-families">Erdős theorem on k-Sperner families</h6>

↑ **Parent:** [k-Sperner family](#k-sperner-family)

Among $k$-Sperner subfamilies of $\mathcal P([n])$, the maximum cardinality is the sum of the $k$ largest [binomial coefficients](combinatorics.md#binomial-coefficient) $\binom nj$. The union of the corresponding levels attains the bound. For the upper bound, the [Lubell mass](#lubell-mass) is at most $k$, and assigning its available mass to the levels with largest binomial coefficients maximizes cardinality.

##### Cross-Sperner inequality

↑ **Parent:** [Antichain](#antichain)

If set families $\mathcal A,\mathcal B\subseteq\mathcal P([n])$ are cross-incomparable, meaning no member of either contains a member of the other, then

$$
\sqrt{|\mathcal A|}+\sqrt{|\mathcal B|}\leq2^{n/2}.
$$

The proof applies the [Harris-Kleitman inequality](probability-inequality.md#harris-inequality) to the upward closures generated by the two families.

###### Two-block extremisers for the cross-Sperner inequality

↑ **Parent:** [Cross-Sperner inequality](#cross-sperner-inequality)

Choose disjoint [subsets](set.md#subset) $K_1,K_2\subseteq[n]$ of size $k\geq1$ with $2k\leq n$. Let $\mathcal A$ consist of [subsets](set.md#subset) containing all of $K_1$ and none of $K_2$; let $\mathcal B$ consist of [subsets](set.md#subset) omitting at least one point of $K_1$ and containing at least one point of $K_2$. These form a [cross-Sperner family](#cross-sperner-family) pair, with sizes $2^{n-2k}$ and $(2^k-1)^2 2^{n-2k}$. Their square roots sum to $2^{n/2}$, proving sharpness of the [Cross-Sperner inequality](#cross-sperner-inequality). The free coordinates outside the two blocks account for the factor $2^{n-2k}$.

### Characteristic vector of a set

↑ **Parent:** [Set family](#set-family)

For $A\subseteq[n]$, the characteristic vector $\mathbf1_A\in\{0,1\}^n$ has coordinate $i$ equal to one exactly when $i\in A$. Under this identification, [set union](set.md#set-union) becomes coordinatewise Boolean OR.

#### Modular intersection method for set families

↑ **Parent:** [Characteristic vector of a set](#characteristic-vector-of-a-set)

Over $\mathbb F_2$, characteristic vectors satisfy $\mathbf1_A\mathbin\cdot\mathbf1_B=|A\cap B|\bmod2$. Parity restrictions on sizes and intersections therefore become diagonal and off-diagonal conditions on a [Gram matrix](linear-algebra.md#gram-matrix), allowing rank and linear-independence arguments.

### Incidence graph

↑ **Parent:** [Set family](#set-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Incidence_graph)

The incidence graph of a set family is the bipartite graph whose two vertex classes are the family members and the ground points, with an edge for each containment relation.

### Trace of a set family

↑ **Parent:** [Set family](#set-family)

For a set family $\mathcal A\subseteq\mathcal P([n])$ and $F\subseteq[n]$, its trace on $F$ is

$$
T_F(\mathcal A)=\{A\cap F:A\in\mathcal A\}.
$$

#### Set shattering

↑ **Parent:** [Trace of a set family](#trace-of-a-set-family)

A [set family](#set-family) shatters $Z$ when every subset of $Z$ occurs as a [trace of a set family](#trace-of-a-set-family). The largest finite shattered-set size is its [VC dimension](foundations-of-mathematics.md#vc-dimension). The [Sauer-Shelah lemma](foundations-of-mathematics.md#sauer-shelah-lemma) bounds the number of traces when no set of a given size is shattered.

##### Unbounded finite shattering without an infinite universal trace

↑ **Parent:** [Set shattering](#set-shattering)

Partition an infinite countable set into disjoint finite blocks of unbounded size. The union of their power sets consists entirely of finite sets and shatters each block, so it has unbounded finite [VC dimension](foundations-of-mathematics.md#vc-dimension). Every infinite set meets two different blocks. The pair formed by one point from each can never occur as a trace, since each family member stays in one block. Thus no infinite set has traces realizing all its finite subsets.

#### Shearer trace inequality

↑ **Parent:** [Trace of a set family](#trace-of-a-set-family)

If every ground element belongs to at least $t$ members of a family $\mathcal F\subseteq\mathcal P([n])$, then

$$
|\mathcal A|\leq
\left(\prod_{F\in\mathcal F}|T_F(\mathcal A)|\right)^{1/t}.
$$

Apply [Shearer's inequality](information-theory.md#shearer-s-inequality) to the characteristic vector of a uniformly random member of $\mathcal A$.

### Union-closed family

↑ **Parent:** [Set family](#set-family)

A set family $\mathcal A$ is union-closed when $A\cup B\in\mathcal A$ for every $A,B\in\mathcal A$.

#### Union-closed sets conjecture

↑ **Parent:** [Union-closed family](#union-closed-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Union-closed_sets_conjecture)

The union-closed sets conjecture states that every finite nontrivial [union-closed family](#union-closed-family) has an element contained in at least half of its members.

##### Binary entropy product inequality

↑ **Parent:** [Union-closed sets conjecture](#union-closed-sets-conjecture)

For $x,y\in[0,1]$, the [binary entropy](information-theory.md#binary-entropy) and the [golden ratio](algebra.md#golden-ratio) $\varphi$ satisfy

$$
h_2(xy)\geq\frac{\varphi}{2}\bigl(xh_2(y)+yh_2(x)\bigr).
$$

##### Entropy bound for a union-closed family

↑ **Parent:** [Union-closed sets conjecture](#union-closed-sets-conjecture)

Every finite [union-closed family](#union-closed-family) other than $\{\varnothing\}$ has an element belonging to at least

$$
\frac{3-\sqrt5}{2}
$$

of its members. The proof applies the [binary entropy product inequality](#binary-entropy-product-inequality) coordinate by coordinate to the union of two independent uniform members of the family.

### Entropy bound for pairwise-union tuples

↑ **Parent:** [Set family](#set-family)

Let $A_1,\ldots,A_m$ be random subsets of a common ground set. If every pairwise union $A_i\cup A_j$ takes values in a fixed family $\mathcal A$ of sets of cardinality at most $k$, then [Shearer's inequality](information-theory.md#shearer-s-inequality) and the fact that a pair of bits with prescribed OR has at most three possibilities give

$$
(m-1)H(A_1,\ldots,A_m)
\leq\sum_{i<j}\bigl(\log|\mathcal A|+k\log3\bigr).
$$

### Intersecting family

↑ **Parent:** [Set family](#set-family)

A family of sets is intersecting when every two of its members have nonempty intersection.

This is a property of a [set family](#set-family), distinct from extremal theorems bounding its size.

#### Union bound for intersecting families

↑ **Parent:** [Intersecting family](#intersecting-family)

For [intersecting families](#intersecting-family) of subsets of $[n]$, take each [upward closure of a set family](#upward-closure-of-a-set-family). It remains intersecting and contains at most one set in each complementary pair, so its complement as a family has density at least one half. Those complements are decreasing [set families](#set-family). Repeated [Harris-Kleitman inequality](probability-inequality.md#harris-inequality) gives intersection density at least $2^{-k}$, proving the displayed bound. For $k\leq n$, the families of sets containing coordinate $i$, for $1\leq i\leq k$, attain equality.

#### Colexicographic replacement can destroy intersection

↑ **Parent:** [Intersecting family](#intersecting-family)

On five points, the four sets $12,13,14,15$ are an [intersecting family](#intersecting-family). The first four two-element sets in [colexicographic order](#colexicographic-order) are $12,13,23,14$, containing the disjoint pair $23,14$. Thus replacing a family by an equally large [colexicographic initial segment](#colexicographic-initial-segment) can destroy intersection, even though it minimizes the [lower shadow](#lower-shadow).

#### Lexicographic initial segments preserve ordinary intersection

↑ **Parent:** [Intersecting family](#intersecting-family)

For $1\le r\le n/2$, the [Erdős-Ko-Rado theorem](#erdos-ko-rado-theorem) bounds an [intersecting family](#intersecting-family) by the displayed size. The first that many rank-$r$ sets in [lexicographic order](#lexicographic-order) all contain coordinate one. Therefore the lexicographic [initial segment](set.md#initial-segment) of the same size as any [intersecting family](#intersecting-family) is also intersecting. This statement concerns ordinary one-element intersection and does not extend to higher intersection requirements.

#### Maximal intersecting families choose one member of every complementary pair

↑ **Parent:** [Intersecting family](#intersecting-family)

A maximal intersecting family is an [up-set](#up-set). It cannot contain both a set and its complement. If neither were present, maximality would supply a member disjoint from the first set, and upward closure would then include its complement. Thus precisely one member of each complementary pair occurs, so the family has $2^{n-1}$ members for $n\geq1$.

#### t-intersecting family

↑ **Parent:** [Intersecting family](#intersecting-family)

A [set family](#set-family) is t-intersecting if every pair of its members has at least $t$ common elements. For $r$-sets on an $n$-point ground set, the whole level is t-intersecting when $n\leq2r-t$. Ordinary [intersecting families](#intersecting-family) are the case $t=1$.

##### Lexicographic replacement can destroy two-intersection

↑ **Parent:** [T-intersecting family](#t-intersecting-family)

On eight points, the rank-four [Frankl family](#complete-intersection-candidate-family) consisting of sets containing at least three of $1,2,3,4$ has seventeen members and is two-intersecting. The first fifteen rank-four sets in [lexicographic order](#lexicographic-order) contain $1,2$, while the sixteenth is $1345$. The earlier set $1278$ meets it only at one. This disproves preservation of two-intersection by lexicographic replacement even when the rank is half the ground-set size.

##### Maximal intersection does not imply maximum size

↑ **Parent:** [T-intersecting family](#t-intersecting-family)

For two-intersecting families on four points, all supersets of a fixed pair form a maximal family of size four: any set missing part of that pair fails its intersection test with the pair itself. The maximum instead has size five, attained by all sets of size at least three. Thus maximality and maximum cardinality diverge for intersection parameter two.

##### Nonuniform t-intersecting family bound

↑ **Parent:** [T-intersecting family](#t-intersecting-family)

If $|A\cap B|\geq t$, then $|A\triangle B|=|A\cup B|-|A\cap B|\leq n-t$. The [Kleitman diametric theorem](#kleitman-diametric-theorem) therefore gives the sharp nonuniform intersection bound. For $n-t=2q$, all sets of size at least $n-q$ attain it. For $n-t=2q+1$, take all sets of size at least $n-q$, together with all $(n-q-1)$-sets avoiding one fixed point.

##### Ahlswede-Khachatrian theorem

↑ **Parent:** [T-intersecting family](#t-intersecting-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ahlswede–Khachatrian_theorem)

The maximum size of a [t-intersecting family](#t-intersecting-family) of $r$-sets on $[n]$ is the largest [complete-intersection candidate family](#complete-intersection-candidate-family). In strict nontrivial intervals $n_{k+1}<n<n_k$, the maximizing index is $k$, where $n_k=(r-t+1)(2+(t-1)/k)$ and $n_0=\infty$. At admissible interior boundaries the consecutive candidates tie. If $n\leq2r-t$, the whole level is optimal. A proof uses left compression, the [small-support generating lemma for extremal intersecting families](#small-support-generating-lemma-for-extremal-intersecting-families) for the original and complement families, and the [compatibility bound for complementary generating families](#compatibility-bound-for-complementary-generating-families). The latter forces one generator family to have the candidate threshold size, placing the original family inside a candidate.

##### Complementation of uniform intersecting families

↑ **Parent:** [T-intersecting family](#t-intersecting-family)

Complementing all members preserves [cardinality](set-theory.md#cardinality) and gives $|A^c\cap B^c|=n-2r+|A\cap B|$. Thus complementation bijects [t-intersecting families](#t-intersecting-family) of $r$-sets with $(n-2r+t)$-intersecting families of $(n-r)$-sets. It swaps left and right [coordinate shifts of a set family](#coordinate-shifts-of-a-set-family). When the transformed intersection parameter is positive, extremal families and their generating-support lemmas can therefore be compared in opposite compression directions.

##### Complete-intersection candidate family

↑ **Parent:** [T-intersecting family](#t-intersecting-family)

Two members of this [uniform set family](#uniform-set-family) have at least $2(t+i)-(t+2i)=t$ common points in its distinguished prefix, so it is a [t-intersecting family](#t-intersecting-family). Nonempty indices satisfy $0\leq i\leq r-t$. Consecutive-family size comparison reduces to the threshold $n_{i+1}=(r-t+1)(2+(t-1)/(i+1))$: gain sets contain both newly introduced coordinates and $t+i-1$ earlier points; loss sets contain neither and $t+i$ earlier points. Counting these sets with [binomial coefficients](combinatorics.md#binomial-coefficient) proves increase below, equality at and decrease above this threshold.

#### Intersecting two-element set family

↑ **Parent:** [Intersecting family](#intersecting-family)

A pairwise [intersecting family](#intersecting-family) of two-element sets is contained in a [star graph](graph-theory.md#star-graph-theory) or in the three [edges](graph-theory.md#edge-of-a-graph) of a [triangle in a graph](graph.md#triangle-in-a-graph). If two members are $\{a,b\},\{a,c\}$ and a third avoids $a$, the third must be $\{b,c\}$. Every member meeting all three belongs to that triangle.

#### Witness-pair concentration for an intersecting uniform family

↑ **Parent:** [Intersecting family](#intersecting-family)

For an [intersecting family](#intersecting-family) of $r$-sets, some element $x$ is avoided by at most $(r-1)^2\binom{n-2}{r-2}$ members. If two members meet exactly at $x$, every member avoiding $x$ contains one element from each of their disjoint remainders. If no such pair exists, apply the [pair-cover bound for a two-intersecting uniform family](#pair-cover-bound-for-a-two-intersecting-uniform-family).

#### Two-intersecting family

↑ **Parent:** [Intersecting family](#intersecting-family)

A [set family](#set-family) is two-intersecting if $|A\cap B|\geq2$ for all of its members, including $A=B$. In particular its members all have at least two elements. This is stronger than being an [intersecting family](#intersecting-family).

##### Pair-cover bound for a two-intersecting uniform family

↑ **Parent:** [Two-intersecting family](#two-intersecting-family)

Fix a member of size $r$. Every other member of a [two-intersecting family](#two-intersecting-family) contains a pair from that fixed member. Counting all $r$-sets containing these pairs gives $|\mathcal F|\leq\binom r2\binom{n-2}{r-2}$ for a [uniform set family](#uniform-set-family).

##### Nonuniform two-intersecting family bound

↑ **Parent:** [Two-intersecting family](#two-intersecting-family)

On an even ground set $n=2h$, a [two-intersecting family](#two-intersecting-family) has size at most $\sum_{j=h+1}^n\binom nj$. On an odd ground set $n=2h+1$, the bound is $\binom{2h}{h+1}+\sum_{j=h+2}^n\binom nj$. Pair lower levels with complements of upper levels using the [intersecting shadow lemma](#intersecting-shadow-lemma); apply the [Erdős-Ko-Rado theorem](#erdos-ko-rado-theorem) to the remaining middle level in the odd case.

#### Intersecting shadow lemma

↑ **Parent:** [Intersecting family](#intersecting-family)

For an [intersecting family](#intersecting-family) of $r$-sets with $r\geq1$, its [lower shadow](#lower-shadow) has at least as many members as the family. Apply [elementary set shifts](#elementary-set-shift) and then the [ballot reflection injection](#ballot-reflection-injection) to obtain this bound.

#### Weighted intersecting family bound on an odd Boolean lattice

↑ **Parent:** [Intersecting family](#intersecting-family)

For odd $n$ and $w\geq1$, an [intersecting family](#intersecting-family) contains at most one set from each complementary pair in the [Boolean lattice](#boolean-lattice). Choosing the larger member in every pair gives the displayed bound and is feasible, because all sets of size greater than $n/2$ intersect. For $w>1$ it is the unique maximizer; for $w=1$ other maximizing families can exist.

#### Intersecting family in a product alphabet

↑ **Parent:** [Intersecting family](#intersecting-family)

A family of words in $[k]^n$ is intersecting if any two words agree in some coordinate. For positive $n,k$, its maximum size is $k^{n-1}$: simultaneous cyclic shifts partition the words into classes in which distinct words never agree, and fixing one coordinate attains the resulting bound.

#### Exactly one-intersecting family

↑ **Parent:** [Intersecting family](#intersecting-family)

An exactly one-intersecting family satisfies $|A\cap B|=1$ for every two distinct members. It is nontrivial when the intersection of all its members is empty.

##### Finite linear space

↑ **Parent:** [Exactly one-intersecting family](#exactly-one-intersecting-family)

A finite linear space consists of finitely many points and proper subsets called lines such that every two points lie on exactly one line. The sets of family indices containing each ground point turn a nontrivial exactly one-intersecting family into a finite linear space.

It is a finite nontrivial instance of a [Linear space](combinatorics.md#linear-space-geometry).

<h6 id="de-bruijn-erdos-pair-covering-inequality">De Bruijn--Erdos pair-covering inequality</h6>

↑ **Parent:** [Finite linear space](#finite-linear-space)

If $r_x$ denotes the number of lines through $x$ in a nontrivial finite linear space on $v$ points, then

$$
\sum_x\binom{r_x}{2}\geq\binom v2.
$$

To prove it, let $k_L$ be the line sizes. The inequalities $k_L\leq r_x$ whenever $x\notin L$, counted at each integer threshold, give

$$
\sum_x(r_x-t)_+\geq\sum_L(k_L-t)_+
$$

for every $t\geq1$. Summing in $t$ and using $\binom s2=\sum_{t\geq1}(s-t)_+$ gives

$$
\sum_x\binom{r_x}{2}\geq\sum_L\binom{k_L}{2}=\binom v2,
$$

where the last identity counts pairs of points by their unique line.

###### Near-pencil

↑ **Parent:** [Finite linear space](#finite-linear-space)

A near-pencil on $v$ points has one line containing $v-1$ points and $v-1$ two-point lines joining the remaining point to each point of the large line.

This is a particular [finite linear space](#finite-linear-space) configuration, rather than a synonym for every pencil of lines.

###### Finite projective plane

↑ **Parent:** [Finite linear space](#finite-linear-space)

A finite projective plane of order $q$ has $q^2+q+1$ points and the same number of lines. Every line contains $q+1$ points, every point lies on $q+1$ lines, and every two points or two lines determine a unique line or intersection point respectively.

#### Cross-intersecting family

↑ **Parent:** [Intersecting family](#intersecting-family)

Two set families $\mathcal A$ and $\mathcal B$ are cross-intersecting when $A\cap B\ne\varnothing$ for every $A\in\mathcal A$ and $B\in\mathcal B$.

##### Finite intersection witness for cross-intersecting families

↑ **Parent:** [Cross-intersecting family](#cross-intersecting-family)

For [cross-intersecting families](#cross-intersecting-family) $\mathcal A,\mathcal B$ with member sizes at most $r,s$ respectively, there is a finite [set](set.md) $X$ with $|X|\leq r\sum_{j=0}^s r^j$ such that $A\cap B\cap X\ne\varnothing$ for every $A\in\mathcal A,B\in\mathcal B$. Take a [bounded-size transversal kernel](#bounded-size-transversal-kernel) $\mathcal A_0$ preserving [hitting sets](#hitting-set) of size at most $s$ and set $X=\bigcup_{A\in\mathcal A_0}A$. For each $B$, the [set](set.md) $B\cap X$ is a [hitting set](#hitting-set) for $\mathcal A_0$, hence for all of $\mathcal A$. This proves the assertion even for infinite [set families](#set-family); if either family is empty, take $X=\varnothing$.

#### Upward closure of a set family

↑ **Parent:** [Intersecting family](#intersecting-family)

The upward closure of $\mathcal B$ is $\overline{\mathcal B}=\{A:\text{some }B\in\mathcal B\text{ satisfies }B\subseteq A\}$.

#### Dinur-Friedgut junta theorem for intersecting families

↑ **Parent:** [Intersecting family](#intersecting-family)

For $0<p<1/2$ and $\varepsilon>0$, every intersecting family is, up to $\mu_p$-measure $\varepsilon$, contained in the [upward closure of a set family](#upward-closure-of-a-set-family) generated by an intersecting family on a bounded set of coordinates.

### Uniform set family

↑ **Parent:** [Set family](#set-family)

A $k$-uniform set family consists entirely of $k$-element subsets of a common ground set.

#### Generating family for a uniform set family

↑ **Parent:** [Uniform set family](#uniform-set-family)

A generating family consists of sets of size at most $r$ whose $r$-element supersets are exactly the prescribed [uniform set family](#uniform-set-family). Small-support generators express dependence on a bounded prefix rather than on the full ground set. Taking the entire family itself as generators always works, but extremal intersection problems admit much smaller supporting intervals.

##### Tight pairs of left-compressed generators

↑ **Parent:** [Generating family for a uniform set family](#generating-family-for-a-uniform-set-family)

For a [t-intersecting family](#t-intersecting-family) with left-compressed generators supported on $[m]$, a tight pair containing $m$ cannot both miss an earlier coordinate $i$. Replacing $m$ by $i$ in one generator gives a shifted set containing a generator, whose intersection with the other has at most $t-1$ points. Thus the union is $[m]$, and their sizes sum to $m+t$. This identifies precisely which size classes conflict when the largest support coordinate is removed.

##### Maximum-support generator fibre

↑ **Parent:** [Generating family for a uniform set family](#generating-family-for-a-uniform-set-family)

Suppose a [left-compressed set family](#left-compressed-set-family) of $k$-sets has an [antichain](#antichain) of generators on $[m]$, closed under left shifts followed by taking inclusion-minimal members. For a generator $G$ containing $m$, the members generated only by $G$ have intersection with $[m]$ exactly $G$. If another prefix coordinate $i$ occurred, the left shift $G-\{m\}+\{i\}$ would supply another generator. Conversely, an exact prefix $G$ contains no other generator by the [antichain](#antichain) condition. The free tail gives the displayed [binomial coefficient](combinatorics.md#binomial-coefficient).

##### Compatibility bound for complementary generating families

↑ **Parent:** [Generating family for a uniform set family](#generating-family-for-a-uniform-set-family)

Let $n>2r-t$ and let $G,H$ generate respectively a [t-intersecting family](#t-intersecting-family) of $r$-sets and its complement family. If their union had size at most $n-r+t-1$, contain it in a set $T$ of that size. Since $|T|\geq r,n-r$, extend $G,H$ within $T$ to an $r$-set $A$ and an $(n-r)$-set $B$. Both $A$ and $B^c$ belong to the original family, but $|A\cap B^c|=|A\cup B|-|B|\leq t-1$. This contradiction proves the bound.

##### Small-support generating lemma for extremal intersecting families

↑ **Parent:** [Generating family for a uniform set family](#generating-family-for-a-uniform-set-family)

Assume $1\leq t\leq r\leq n$, $n>2r-t$, and $j\geq0$. A maximum-cardinality [left-compressed set family](#left-compressed-set-family) of $r$-sets that is [t-intersecting](#t-intersecting-family) has a [generating family for a uniform set family](#generating-family-for-a-uniform-set-family) supported on $[t+2j]$ under the displayed strict inequality. Reflection gives a right-end supporting interval for a right-compressed optimum. The strict threshold is important: at a tie between consecutive candidate families, use the next larger support bound. This auxiliary generating result, combined with the [compatibility bound for complementary generating families](#compatibility-bound-for-complementary-generating-families), supplies the upper bound in the [Ahlswede-Khachatrian theorem](#ahlswede-khachatrian-theorem).

###### Generator replacement proof of the small-support intersection lemma

↑ **Parent:** [Small-support generating lemma for extremal intersecting families](#small-support-generating-lemma-for-extremal-intersecting-families)

Let $m$ be the smallest supporting prefix for a maximum [left-compressed set family](#left-compressed-set-family) of $k$-sets that is [t-intersecting](#t-intersecting-family), and set $N=n-m$. The [maximum-support generator fibre](#maximum-support-generator-fibre) gives exclusive count $\binom N{k-a}$ for a size-$a$ generator containing $m$. By [tight pairs of left-compressed generators](#tight-pairs-of-left-compressed-generators), only classes $a,b$ with $a+b=m+t$ can conflict after deleting $m$. For unequal such sizes, replacing both classes by the shortened generators of either class would imply

$$
\binom N{k-a+1}\binom N{k-b+1}\leq\binom N{k-a}\binom N{k-b}.
$$

When $n\geq2k-t+2$ and the classes have positive fibres, the reverse inequality is strict. For the remaining central class $a=t+j$, $m=t+2j$, some earlier coordinate is absent from at least $j/(m-1)$ of its shortened generators. Those generators are mutually t-intersecting. Replacing the central class by that subfamily has gain-to-loss ratio at least

$$
\frac{j}{m-1}\frac{N+1}{k-t-j+1},
$$

which exceeds one exactly when $n>(k-t+1)(2+(t-1)/j)$. This forces the support bound in the [small-support generating lemma for extremal intersecting families](#small-support-generating-lemma-for-extremal-intersecting-families).

#### Intersection-free uniform set family

↑ **Parent:** [Uniform set family](#uniform-set-family)

An [intersection-free uniform set family](#intersection-free-uniform-set-family) is a [uniform set family](#uniform-set-family) $\mathcal F$ with no three distinct members $A,B,C$ satisfying $A\cap B\subseteq C$. For distinct members of a rank-$r$ family, $|A\cap B|<r$, so using strict containment gives the same restriction. Fixing one member turns the other members' intersections with it into distinct [antichain](#antichain) traces, giving the [antichain trace bound for intersection-free families](#antichain-trace-bound-for-intersection-free-families).

##### Antichain trace bound for intersection-free families

↑ **Parent:** [Intersection-free uniform set family](#intersection-free-uniform-set-family)

For an [intersection-free uniform set family](#intersection-free-uniform-set-family) of rank $r$, fix $X\in\mathcal F$. The map $A\mapsto X\cap A$ on $\mathcal F\setminus\{X\}$ is injective and its image is an [antichain](#antichain) in $\mathcal P(X)$: a containment $X\cap A\subseteq X\cap B$ would violate intersection-freeness on the distinct members $X,A,B$. The [Sperner theorem](#sperner-s-theorem) then proves the displayed bound.

#### Uniform layer of the Boolean cube

↑ **Parent:** [Uniform set family](#uniform-set-family)

The uniform layer consists of the [characteristic vectors of sets](#characteristic-vector-of-a-set) of size $r$ in $[n]$. It has size $\binom nr$, a [binomial coefficient](combinatorics.md#binomial-coefficient). Restricting [polynomials](polynomial.md) to a uniform layer introduces identities absent on the entire [Boolean lattice](#boolean-lattice), since the coordinate sum is fixed. In particular, [homogenisation on a uniform layer](polynomial.md#homogenisation-on-a-uniform-layer) spans all restricted [multilinear polynomials](polynomial.md#multilinear-polynomial) of degree at most $s\leq r$ using just the degree-$s$ [monomials](polynomial.md#monomial).

##### Low-degree evaluation rank on a uniform layer

↑ **Parent:** [Uniform layer of the Boolean cube](#uniform-layer-of-the-boolean-cube)

Let $0\leq s\leq k\leq n$ and form the integer [matrix](vector-space.md#matrix) with rows indexed by $S\subseteq[n]$, $|S|\leq s$, columns indexed by $k$-subsets $T$, and entry $M_{S,T}=\mathbf1_{S\subseteq T}$. Its [matrix rank](vector-space.md#matrix-rank) over any [finite field](algebra.md#finite-field) $\mathbb F_p$ is at most $\binom ns$. Over the [rational numbers](number-theory.md#rational-number), the row of a $j$-subset $S$ is $\binom{k-j}{s-j}^{-1}$ times the sum of the rows of all $s$-subsets containing $S$. Thus the rows of degree exactly $s$ span, giving the bound over the [rational numbers](number-theory.md#rational-number). Every larger square minor therefore has integer [determinant](linear-algebra.md#determinant) zero, and remains zero modulo $p$. The [matrix rank](vector-space.md#matrix-rank) cannot increase under this reduction. This argument avoids dividing by an integer that might vanish in the [finite field](algebra.md#finite-field), and gives the sharp uniform-layer step in the [Frankl-Wilson theorem](#frankl-wilson-theorem).

<h4 id="erdos-ko-rado-theorem">Erdős-Ko-Rado theorem</h4>

↑ **Parent:** [Uniform set family](#uniform-set-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Erdős–Ko–Rado_theorem)

If $n\geq2k$ and $\mathcal A\subseteq[n]^{(k)}$ is intersecting, then $|\mathcal A|\leq\binom{n-1}{k-1}$.

<h5 id="erdos-ko-rado-theorem-from-shadows">Erdős-Ko-Rado theorem from shadows</h5>

↑ **Parent:** [Erdős-Ko-Rado theorem](#erdos-ko-rado-theorem)

For an [intersecting family](#intersecting-family) of $r$-sets with $n\geq2r$, the rank-$r$ [lower shadow](#lower-shadow) of its complement family is disjoint from the original family. Iterating the [Kruskal-Katona theorem](#kruskal-katona-theorem) shows that exceeding $\binom{n-1}{r-1}$ original members would force this shadow to have more than $\binom{n-1}r$ members, contradicting the total number $\binom nr$ of $r$-sets.

##### Katona circle method

↑ **Parent:** [Erdős-Ko-Rado theorem](#erdos-ko-rado-theorem)

Katona's circle method places a finite ground set in a uniformly counted cyclic order, proves a bound for the members of a set family that appear as cyclic intervals, and double-counts pairs of a member and a compatible cyclic order.

###### Cyclic interval antichain bound

↑ **Parent:** [Katona circle method](#katona-circle-method)

In any [cyclic ordering](combinatorics.md#cyclic-ordering) on $n$ points, an [antichain](#antichain) contains at most $n$ nonempty proper [cyclic intervals](combinatorics.md#cyclic-interval). The intervals with one prescribed final position are nested, so at most one belongs to the [antichain](#antichain). Summing over final positions proves the bound. Averaging it over [cyclic orderings](combinatorics.md#cyclic-ordering) proves the [LYM inequality](#lubell-yamamoto-meshalkin-inequality); the empty set and full set must be handled separately.

###### Cyclic interval intersection bound

↑ **Parent:** [Katona circle method](#katona-circle-method)

An [intersecting family](#intersecting-family) of cyclic intervals of length $r$ in a cyclic order of $n$ positions has at most $r$ members when $1\leq r\leq n/2$. Rotate one selected interval to end at position $n$. Intervals ending at $r,\ldots,n-r$ miss it. Pair the remaining endpoints, other than $n$, as $(j,j+n-r)$ for $1\leq j\leq r-1$; each pair represents two disjoint intervals, hence contributes at most one member. This gives $1+(r-1)=r$. Counting such intervals over all [permutations](combinatorics.md#permutation) proves the [Erdős-Ko-Rado theorem](#erdos-ko-rado-theorem).

#### Steiner triple system

↑ **Parent:** [Uniform set family](#uniform-set-family)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Steiner_triple_system)

A Steiner triple system is a collection of three-element subsets, called blocks, in which every pair of points belongs to exactly one block. Distinct blocks consequently meet in at most one point, and a system on $v$ points has $v(v-1)/6$ blocks.

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
