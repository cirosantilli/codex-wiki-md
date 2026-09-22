# Ramsey theory

↑ **Parent:** [Combinatorics](combinatorics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ramsey_theory)

Ramsey theory studies the ordered configurations that every [finite coloring](#finite-coloring) of a sufficiently large structure must contain.

**Table of contents**

- [Square-difference recurrence for finite colourings](#square-difference-recurrence-for-finite-colourings)
- [Multicolour Ramsey bound](#multicolour-ramsey-bound)
- [Homogeneous set for a colouring](#homogeneous-set-for-a-colouring)
  - [Computable colouring](#computable-colouring)
    - [Finite-injury computable colouring of pairs](#finite-injury-computable-colouring-of-pairs)
    - [Halting-stage colouring of triples](#halting-stage-colouring-of-triples)
- [Dyadic valuation and scale colouring](#dyadic-valuation-and-scale-colouring)
- [Space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers)
  - [Finite stem of an infinite subset](#finite-stem-of-an-infinite-subset)
  - [Ramsey family in the homogeneous-cone sense](#ramsey-family-in-the-homogeneous-cone-sense)
  - [Ramsey cone topology](#ramsey-cone-topology)
    - [Meagreness of the Ramsey cone topology](#meagreness-of-the-ramsey-cone-topology)
  - [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets)
    - [Open Ramsey theorem](#open-ramsey-theorem)
    - [Finite-symmetric-difference parity colouring](#finite-symmetric-difference-parity-colouring)
    - [Non-Ramsey set from transfinite selection](#non-ramsey-set-from-transfinite-selection)
    - [Completely Ramsey set](#completely-ramsey-set)
      - [Stem-supported Ramsey family need not be completely Ramsey](#stem-supported-ramsey-family-need-not-be-completely-ramsey)
      - [Completely Ramsey-null set](#completely-ramsey-null-set)
        - [Ellentuck meagre-set fusion lemma](#ellentuck-meagre-set-fusion-lemma)
      - [Fusion proof for open Ellentuck sets](#fusion-proof-for-open-ellentuck-sets)
        - [Acceptance and rejection of finite stems](#acceptance-and-rejection-of-finite-stems)
          - [Finitely many accepting extensions of a rejected stem](#finitely-many-accepting-extensions-of-a-rejected-stem)
          - [Deciding all finite stems by fusion](#deciding-all-finite-stems-by-fusion)
  - [Ellentuck topology](#ellentuck-topology)
    - [Ellentuck Borel sets are completely Ramsey](#ellentuck-borel-sets-are-completely-ramsey)
      - [Baire-property reduction for completely Ramsey families](#baire-property-reduction-for-completely-ramsey-families)
    - [Cone on an infinite coinfinite ground set](#cone-on-an-infinite-coinfinite-ground-set)
      - [Ordinarily nowhere-dense sets need not be completely Ramsey](#ordinarily-nowhere-dense-sets-need-not-be-completely-ramsey)
    - [Countable unions of Ellentuck clopen sets need not be closed](#countable-unions-of-ellentuck-clopen-sets-need-not-be-closed)
    - [Baire property in the Ellentuck topology](#baire-property-in-the-ellentuck-topology)
  - [Ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets)
    - [Dense countable family of cofinite infinite subsets](#dense-countable-family-of-cofinite-infinite-subsets)
    - [Gap-doubling closed family of infinite subsets](#gap-doubling-closed-family-of-infinite-subsets)
      - [Meagre set meeting every Ramsey cone in both colours](#meagre-set-meeting-every-ramsey-cone-in-both-colours)
    - [Baire property in the ordinary infinite-subset topology](#baire-property-in-the-ordinary-infinite-subset-topology)
- [Matching Ramsey number](#matching-ramsey-number)
- [Triangle-packing Ramsey number](#triangle-packing-ramsey-number)
- [Finite coloring](#finite-coloring)
  - [Colour profile of a finite block](#colour-profile-of-a-finite-block)
  - [Colour class](#colour-class)
  - [Cyclic logarithmic coloring](#cyclic-logarithmic-coloring)
  - [Refinement of a finite coloring](#refinement-of-a-finite-coloring)
  - [Monochromatic set](#monochromatic-set)
- [Ramsey's theorem](#ramsey-s-theorem)
  - [Simultaneous coefficient patterns from a homogeneous four-set colouring](#simultaneous-coefficient-patterns-from-a-homogeneous-four-set-colouring)
  - [Successive thinning proof of the infinite Ramsey theorem](#successive-thinning-proof-of-the-infinite-ramsey-theorem)
  - [Finite Ramsey theorem](#finite-ramsey-theorem)
    - [Ramsey number](#ramsey-number)
- [Modular-intersection graph Ramsey lower bound](#modular-intersection-graph-ramsey-lower-bound)
- [Combinatorial line](#combinatorial-line)
  - [Fixed-active-size obstruction for combinatorial lines](#fixed-active-size-obstruction-for-combinatorial-lines)
  - [Run-count obstruction to interval-active lines](#run-count-obstruction-to-interval-active-lines)
  - [Coordinate duplication for combinatorial lines](#coordinate-duplication-for-combinatorial-lines)
  - [Adequate family of active coordinate sets](#adequate-family-of-active-coordinate-sets)
  - [Hales-Jewett theorem](#hales-jewett-theorem)
    - [Letter-merging proof of the Hales-Jewett theorem](#letter-merging-proof-of-the-hales-jewett-theorem)
    - [Alphabet insensitivity lemma](#alphabet-insensitivity-lemma)
      - [Explicit block bound for alphabet insensitivity](#explicit-block-bound-for-alphabet-insensitivity)
  - [Combinatorial subspace](#combinatorial-subspace)
    - [Extended Hales-Jewett theorem](#extended-hales-jewett-theorem)
- [Hilbert cube](#hilbert-cube)
  - [Hilbert cube theorem](#hilbert-cube-theorem)
- [Van der Waerden theorem](#van-der-waerden-theorem)
  - [Colour-focusing proof of Van der Waerden theorem](#colour-focusing-proof-of-van-der-waerden-theorem)
  - [Brauer progression theorem](#brauer-progression-theorem)
  - [Strengthened Van der Waerden theorem](#strengthened-van-der-waerden-theorem)
  - [Color-focused arithmetic progression](#color-focused-arithmetic-progression)
- [Gallai theorem for an integer lattice](#gallai-theorem-for-an-integer-lattice)
  - [Canonical arithmetic progression dichotomy](#canonical-arithmetic-progression-dichotomy)
  - [Sum map from words to homothetic copies](#sum-map-from-words-to-homothetic-copies)
  - [Arithmetic-progression bipartite Ramsey dichotomy](#arithmetic-progression-bipartite-ramsey-dichotomy)
- [Partition regular matrix](#partition-regular-matrix)
  - [Scaling invariance of homogeneous partition regularity](#scaling-invariance-of-homogeneous-partition-regularity)
  - [Reciprocal partition regularity](#reciprocal-partition-regularity)
  - [Compactness bound for partition regularity](#compactness-bound-for-partition-regularity)
  - [Partition regularity dichotomy under an extra constraint](#partition-regularity-dichotomy-under-an-extra-constraint)
  - [Columns property](#columns-property)
    - [Rado's theorem](#rado-s-theorem)
      - [Partition-regular system forcing an ordered Schur relation](#partition-regular-system-forcing-an-ordered-schur-relation)
      - [Rado theorem for one equation](#rado-theorem-for-one-equation)
        - [Brauer configuration for a one-row zero-sum equation](#brauer-configuration-for-a-one-row-zero-sum-equation)
        - [Leading-residue obstruction to partition regularity](#leading-residue-obstruction-to-partition-regularity)
        - [One-equation partition regularity over odd integers](#one-equation-partition-regularity-over-odd-integers)
    - [P-adic columns lemma](#p-adic-columns-lemma)
      - [Finite separating-functional proof of the columns condition](#finite-separating-functional-proof-of-the-columns-condition)
      - [Last nonzero digit coloring](#last-nonzero-digit-coloring)
    - [M-p-c set](#m-p-c-set)
      - [Rado solution inside an m-p-c set](#rado-solution-inside-an-m-p-c-set)
      - [Monochromatic m-p-c set theorem](#monochromatic-m-p-c-set-theorem)
        - [Finite sums theorem](#finite-sums-theorem)
          - [Columns partition for finite-sums systems](#columns-partition-for-finite-sums-systems)
- [Hindman theorem](#hindman-theorem)
  - [Dynamical proof of Hindman's theorem](#dynamical-proof-of-hindman-s-theorem)
  - [Idempotent-ultrafilter proof of Hindman's theorem](#idempotent-ultrafilter-proof-of-hindman-s-theorem)
  - [Finite-sums set](#finite-sums-set)
    - [Divisibility chain inside a finite-sums set](#divisibility-chain-inside-a-finite-sums-set)
    - [IP set](#ip-set)
      - [Alternating dyadic intervals contain disjoint IP sets](#alternating-dyadic-intervals-contain-disjoint-ip-sets)
      - [IP-star set](#ip-star-set)
        - [IP-star filter](#ip-star-filter)
      - [Partition regularity of IP sets](#partition-regularity-of-ip-sets)
  - [Milliken–Taylor theorem](#milliken-taylor-theorem)
- [Monochromatic sums-and-products obstruction](#monochromatic-sums-and-products-obstruction)
- [Euclidean Ramsey set](#euclidean-ramsey-set)
  - [Spherical point set](#spherical-point-set)
  - [Product theorem for Euclidean Ramsey sets](#product-theorem-for-euclidean-ramsey-sets)
  - [Three-term unit arithmetic progression is not Euclidean Ramsey](#three-term-unit-arithmetic-progression-is-not-euclidean-ramsey)
  - [Triangle is a Euclidean Ramsey set](#triangle-is-a-euclidean-ramsey-set)
  - [Line segment is a Euclidean Ramsey set](#line-segment-is-a-euclidean-ramsey-set)
  - [Regular polygon is a Euclidean Ramsey set](#regular-polygon-is-a-euclidean-ramsey-set)
  - [Approximately Euclidean Ramsey set](#approximately-euclidean-ramsey-set)
  - [Edge Ramsey set](#edge-ramsey-set)
  - [Cyclic transitive point set](#cyclic-transitive-point-set)
    - [Kriz theorem for cyclic transitive point sets](#kriz-theorem-for-cyclic-transitive-point-sets)
      - [A-invariant coloring of a Cartesian power](#a-invariant-coloring-of-a-cartesian-power)

## Square-difference recurrence for finite colourings

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

Every finite colouring of the positive integers contains a pair with nonzero square difference. One proof takes limits of the colour autocorrelations and represents the resulting positive-definite sequence by a positive spectral measure. Its atom at zero has mass at least the sum of squared colour densities. Averaging along squares kills irrational frequencies; a common multiple makes finitely many rational atomic frequencies equal to one. The remaining rational atomic mass can be made arbitrarily small, leaving a positive average correlation.

## Multicolour Ramsey bound

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

Let $R_k(3)$ be the least order of a [complete graph](graph-theory.md#complete-graph) whose every $k$-edge-colouring has a [monochromatic](#monochromatic-set) [triangle in a graph](graph.md#triangle-in-a-graph). At a vertex of a graph of order $k(R_{k-1}(3)-1)+2$, some colour joins at least $R_{k-1}(3)$ neighbours. An edge of that colour among these neighbours completes a triangle; otherwise the neighbours use at most $k-1$ colours and contain a triangle by induction. This proves the recurrence and the weaker explicit bound $R_k(3)\le3k!$.

## Homogeneous set for a colouring

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

For a colouring $\chi:[S]^r\to\{0,\ldots,k-1\}$ of the $r$-element subsets of a [set](set.md) $S$, a subset $H\subseteq S$ is homogeneous if all its $r$-element subsets receive the same colour. The infinite [Ramsey theorem for r-sets](#ramsey-s-theorem) guarantees an infinite homogeneous subset when $S=\mathbb N$, $r$ is positive and the number of colours is finite. This does not guarantee a [computable set](foundations-of-mathematics.md#computable-set) when the colouring is computable.

### Computable colouring

↑ **Parent:** [Homogeneous set for a colouring](#homogeneous-set-for-a-colouring)

A colouring is computable when an [algorithm](computer-science.md#algorithm) sorts the finite input subset, computes its colour and terminates. Its colour classes are uniformly [computable sets](foundations-of-mathematics.md#computable-set). The distinction between existence of an infinite [homogeneous set for a colouring](#homogeneous-set-for-a-colouring) and effective construction of one is a basic phenomenon in [computability theory](foundations-of-mathematics.md#computability-theory).

#### Finite-injury computable colouring of pairs

↑ **Parent:** [Computable colouring](#computable-colouring)

There is a two-colour [computable colouring](#computable-colouring) of pairs with no infinite [computably enumerable set](foundations-of-mathematics.md#recursively-enumerable-set) homogeneous for it. Enumerate these [sets](set.md) as $W_e$. In stages, give each eligible requirement two markers from its enumerated [set](set.md), avoiding markers of higher priority, and cancel all lower-priority markers whenever a new assignment is made. Colour $(x,y)$ by the marker status of $x$ at stage $y$: first markers have colour zero, second markers colour one, and unmarked points colour zero. Each requirement is injured only finitely often by induction on its index. If $W_e$ is infinite it eventually has permanent distinct markers $a_e,b_e$; for every sufficiently large $y\in W_e$, the pairs $(a_e,y)$ and $(b_e,y)$ have different colours. Simulating finitely many stages computes each pair's colour, proving both effectiveness and the obstruction.

#### Halting-stage colouring of triples

↑ **Parent:** [Computable colouring](#computable-colouring)

Let $K_s$ be an increasing uniformly computable finite approximation to the [diagonal halting set](foundations-of-mathematics.md#diagonal-halting-set). For $a<b<c$, colour the triple $0$ if $K_b\restriction a=K_c\restriction a$, and $1$ otherwise. No infinite [homogeneous set for a colouring](#homogeneous-set-for-a-colouring) can have colour $1$, since the finitely many bits below its first element eventually stabilize. Every infinite homogeneous set $H$ of colour $0$ computes the [diagonal halting set](foundations-of-mathematics.md#diagonal-halting-set): choose $n<a<b$ in $H$ and read membership of $n$ in $K_b$. Homogeneity and unboundedness make this answer final. Thus the colouring has no infinite computable homogeneous set.

## Dyadic valuation and scale colouring

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

Colour $n>0$ by $(v_2(n)\bmod2,\lfloor\log_2n\rfloor\bmod2)$. No increasing infinite sequence can make all its sums $x_i+x_j$ and $x_i+2x_j$, $i<j$, one colour. If its [2-adic valuations](number-theory.md#2-adic-valuation) are bounded, two terms of equal valuation and equal odd part modulo four give pair sums of different valuation parity. If they are unbounded, a later term divisible by a sufficiently large power of two prevents adding a fixed earlier term from crossing either dyadic boundary; the two resulting sums have adjacent logarithmic scale indices.

## Space of infinite subsets of the natural numbers

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

The space $[\mathbb N]^\omega$, also written $\mathbb N^{(\omega)}$, consists of all infinite subsets of the [positive integers](number-theory.md#positive-integer). An element is identified with its strictly increasing enumeration. If $s$ is finite, write $s\sqsubset X$ when $s$ is the finite [initial segment](set.md#initial-segment) of this enumeration.

### Finite stem of an infinite subset

↑ **Parent:** [Space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers)

A [finite stem](#finite-stem-of-an-infinite-subset) is a finite initial segment $s$ of an infinite [subset](set.md#subset) of $\mathbb N$. The associated [neighbourhood](topology.md#neighbourhood-mathematics) in the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets) is $[s]=\{X:s\text{ is an initial segment of }X\}$. For an infinite tail $A$ above $\max s$, the [neighbourhood](topology.md#neighbourhood-mathematics) $[s,A]=\{s\cup B:B\in[A]^\omega\}$ is basic in the [Ellentuck topology](#ellentuck-topology). [Finite stems](#finite-stem-of-an-infinite-subset) allow a fusion argument to fix initial choices while successively thinning the remaining infinite tail.

### Ramsey family in the homogeneous-cone sense

↑ **Parent:** [Space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers)

A family $\mathcal A\subseteq[\mathbb N]^\omega$ is Ramsey in the homogeneous-cone sense if there is an infinite $M\subseteq\mathbb N$ such that either $[M]^\omega\subseteq\mathcal A$ or $[M]^\omega\cap\mathcal A=\varnothing$. This is the existence of one infinite homogeneous cone. Requiring such a refinement inside every infinite initial ground [set](set.md) gives the stronger definition used for a [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets); requiring a homogeneous refinement in every finite-stem [neighbourhood](topology.md#neighbourhood-mathematics) gives a [completely Ramsey set](#completely-ramsey-set).

These quantifiers should be distinguished. For example, the existence of a homogeneous cone on the even numbers does not constrain a family's restriction to the odd numbers. If $\mathcal E$ is the [finite-symmetric-difference parity colouring](#finite-symmetric-difference-parity-colouring) class on the odd numbers, the family consisting of $\mathcal E$ alone has a homogeneous cone disjoint from it on the even numbers, but no homogeneous cone on the odd numbers. Every [open set](topology.md#open-set) in the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets) has homogeneous cones inside all infinite ground [sets](set.md), as follows by deciding [finite stems](#finite-stem-of-an-infinite-subset) through fusion.

### Ramsey cone topology

↑ **Parent:** [Space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers)

This topology has basic open sets $[A]^\omega$ for infinite ground sets $A$, without fixed finite stems. It is coarser than the [Ellentuck topology](#ellentuck-topology) and differs from the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets), whose basic cylinders fix an initial segment. The symbol $\tau$ is sometimes used for either coarser convention, so it should be accompanied by a definition.

#### Meagreness of the Ramsey cone topology

↑ **Parent:** [Ramsey cone topology](#ramsey-cone-topology)

The whole [space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers) is a [meagre set](topological-analysis.md#meagre-set) in the [Ramsey cone topology](#ramsey-cone-topology). For $D_j=\{X:\min X=j\}$, the closure is $\{X:j\in X\}$, which has empty interior: every infinite ground set can be thinned to omit $j$. Thus all $D_j$ are [nowhere dense](topological-analysis.md#nowhere-dense-set), while their countable union is the whole space. In contrast, the whole space is not meagre in either the [Ellentuck topology](#ellentuck-topology) or the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets).

### Ramsey set of infinite subsets

↑ **Parent:** [Space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers)

A set $E\subseteq[\mathbb N]^\omega$ is Ramsey if every infinite $A$ has an infinite subset $B$ such that $[B]^\omega\subseteq E$ or $[B]^\omega\cap E=\varnothing$.

#### Open Ramsey theorem

↑ **Parent:** [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets)

Every [open set](topology.md#open-set) $O$ in the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets) is a [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets): some infinite $B$ has $[B]^\omega\subseteq O$ or $[B]^\omega\cap O=\varnothing$. Use [acceptance and rejection of finite stems](#acceptance-and-rejection-of-finite-stems) and fusion to decide every finite stem. If the empty stem is rejected, each rejected stem has only finitely many accepting one-point extensions. Successive avoidance of these finite obstructions gives an infinite set all of whose finite stems are rejected; openness then excludes every infinite subset from $O$. This concerns increasing enumerations of infinite subsets, rather than unrestricted sequences with repetitions.

#### Finite-symmetric-difference parity colouring

↑ **Parent:** [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets)

Choose one representative $R$ for each equivalence class of infinite sets under finite [symmetric difference](set.md#symmetric-difference). The colour $|A\triangle R|\bmod2$ changes on removing one point. Every cone $[M]^\omega$ therefore contains opposite-coloured sets $M$ and $M\setminus\{\min M\}$. Either colour family is a non-[Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets). Choice of representatives is essential to this construction, which does not claim a definable regular family.

#### Non-Ramsey set from transfinite selection

↑ **Parent:** [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets)

Using the [axiom of choice](set-theory.md#axiom-of-choice), enumerate all infinite subsets $A_\alpha$ of the [positive integers](number-theory.md#positive-integer) in order type $2^{\aleph_0}$. By [transfinite recursion](set-theory.md#transfinite-recursion), choose two previously unused infinite subsets $X_\alpha,Y_\alpha$ of each $A_\alpha$. This is possible because each $[A_\alpha]^\omega$ has cardinality $2^{\aleph_0}$ and fewer choices have been made at stage $\alpha$. The set $\{X_\alpha\}$ is not a [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets), since every $[A_\alpha]^\omega$ meets both it and its complement.

#### Completely Ramsey set

↑ **Parent:** [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets)

A set $E\subseteq[\mathbb N]^\omega$ is completely Ramsey if every basic [Ellentuck topology](#ellentuck-topology) neighborhood $[s,A]$ admits an infinite $B\subseteq A$ with $[s,B]\subseteq E$ or $[s,B]\cap E=\varnothing$. Keeping the finite stem $s$ makes this stronger than being a [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets).

##### Stem-supported Ramsey family need not be completely Ramsey

↑ **Parent:** [Completely Ramsey set](#completely-ramsey-set)

Let E be the even [positive integers](number-theory.md#positive-integer), and take a [finite-symmetric-difference parity colouring](#finite-symmetric-difference-parity-colouring) $\varepsilon$ of $[E]^\omega$. The family $\{\{1\}\cup X:X\in[E]^\omega,\ \varepsilon(X)=0\}$ is Ramsey even under the every-ground-set convention, since every infinite ground set can be thinned to omit 1. It is not [completely Ramsey](#completely-ramsey-set): inside $[\{1\},E]$, every infinite tail has two subfamilies of opposite parity. Its supporting [neighbourhood](topology.md#neighbourhood-mathematics) is closed and [nowhere dense](topological-analysis.md#nowhere-dense-set) in the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets), but open in the [Ellentuck topology](#ellentuck-topology).

##### Completely Ramsey-null set

↑ **Parent:** [Completely Ramsey set](#completely-ramsey-set)

A set $N$ is completely Ramsey-null when every [Ellentuck topology](#ellentuck-topology) neighborhood $[s,A]$ has a refinement $[s,B]$ disjoint from $N$, with the same finite stem $s$. Assuming open Ellentuck sets are [completely Ramsey](#completely-ramsey-set), every star-[nowhere dense set](topological-analysis.md#nowhere-dense-set) is completely Ramsey-null: apply the open-set property to the dense complement of its closure. The [Ellentuck meagre-set fusion lemma](#ellentuck-meagre-set-fusion-lemma) shows that countable unions retain this avoidance property.

###### Ellentuck meagre-set fusion lemma

↑ **Parent:** [Completely Ramsey-null set](#completely-ramsey-null-set)

Countably many [completely Ramsey-null](#completely-ramsey-null-set) sets can be avoided simultaneously in a stem-preserving [Ellentuck topology](#ellentuck-topology) refinement. Select an increasing sequence $b_j$ with nested infinite remaining tails. At stage $j$, thin the tail to avoid the $j$th set for every stem $s\cup t$, where $t$ ranges over all subsets of the first $j$ selected points. There are only finitely many such stems. Any infinite subset of the final selected sequence uses some such $t$ before stage $j$ and has all remaining points in the thinned tail. Thus it avoids every forbidden set. This explains why an argument checking only the full selected prefix is insufficient.

##### Fusion proof for open Ellentuck sets

↑ **Parent:** [Completely Ramsey set](#completely-ramsey-set)

Every [open set](topology.md#open-set) in the [Ellentuck topology](#ellentuck-topology) is a [completely Ramsey set](#completely-ramsey-set). Fix a finite stem $s$. An infinite tail accepts a finite extension $a$ if its entire basic neighborhood $[s\cup a,A]$ lies in the open set; it rejects $a$ if no infinite subtail accepts it. Decisions persist under thinning. A fusion chooses an infinite set deciding every finite extension. For any rejected extension, only finitely many possible next elements can yield accepted extensions, since infinitely many would themselves provide an accepting tail. A second thinning therefore makes all finite extensions rejected. Openness then rules out any point of the set in the resulting neighborhood.

###### Acceptance and rejection of finite stems

↑ **Parent:** [Fusion proof for open Ellentuck sets](#fusion-proof-for-open-ellentuck-sets)

Relative to a family $Y$, an infinite reservoir accepts a finite stem $s$ when its entire [Ellentuck topology](#ellentuck-topology) neighbourhood $[s,A]$ lies in $Y$. It rejects $s$ when no infinite refinement accepts it. Every reservoir has a refinement deciding a prescribed stem, and both outcomes are hereditary under further infinite thinning. These definitions turn open-set homogeneity into a fusion construction.

###### Finitely many accepting extensions of a rejected stem

↑ **Parent:** [Acceptance and rejection of finite stems](#acceptance-and-rejection-of-finite-stems)

Suppose a reservoir rejects $s$ and decides every extension $s\cup\{a\}$. Only finitely many of those one-point extensions can have accepting tails. If infinitely many did, collect their new points into $C$; every infinite subset of $C$ begins with an accepting successor, so $[s,C]$ would lie in the family. That would make $C$ accept $s$, contradicting rejection. This finite-obstruction fact lets a second fusion preserve rejection of every finite stem.

###### Deciding all finite stems by fusion

↑ **Parent:** [Acceptance and rejection of finite stems](#acceptance-and-rejection-of-finite-stems)

Choose successive points and, after each choice, thin the unused reservoir to decide all subsets of the finite chosen prefix. There are only finitely many stems to handle at each stage. The final diagonal infinite set decides every one of its finite stems, because its relevant tail lies in the reservoir chosen when the stem's largest point was selected. The argument uses the hereditary decisions from [acceptance and rejection of finite stems](#acceptance-and-rejection-of-finite-stems).

### Ellentuck topology

↑ **Parent:** [Space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ellentuck_topology)

For a finite set $s$ and an infinite set $A$ lying above $\max s$, put

$$
[s,A]=\{s\cup B:B\in[A]^\omega\}.
$$

These sets form the basic neighborhoods of the Ellentuck topology, also called the star topology. It is finer than the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets). Every basic neighborhood is a [clopen set](topology.md#clopen-set) in the Ellentuck topology, and a [closed set](topology.md#closed-set) in the ordinary topology.

#### Ellentuck Borel sets are completely Ramsey

↑ **Parent:** [Ellentuck topology](#ellentuck-topology)

Every [Borel set](measure-theory.md#borel-set) for the [Ellentuck topology](#ellentuck-topology) is [completely Ramsey](#completely-ramsey-set). First, an acceptance-and-rejection fusion makes every open set homogeneous after thinning the infinite reservoir while keeping its finite stem. Every nowhere-dense set is consequently [completely Ramsey-null](#completely-ramsey-null-set), and a fusion handling all subsets of each finite selected prefix shows that countable unions of such null sets remain null. Finally, sets differing from an open set by a [meagre set](topological-analysis.md#meagre-set) form a [sigma-algebra](measure-theory.md#sigma-algebra) containing the open sets. Thus every Borel set has the required stem-preserving homogeneous refinement.

##### Baire-property reduction for completely Ramsey families

↑ **Parent:** [Ellentuck Borel sets are completely Ramsey](#ellentuck-borel-sets-are-completely-ramsey)

In the [Ellentuck topology](#ellentuck-topology), suppose every [open set](topology.md#open-set) is [completely Ramsey](#completely-ramsey-set) and every [meagre set](topological-analysis.md#meagre-set) is [completely Ramsey-null](#completely-ramsey-null-set). If $E\triangle U$ is contained in a meagre set for some open $U$, first refine a basic [neighbourhood](topology.md#neighbourhood-mathematics) without changing its stem to avoid that exceptional set, and then refine again to be homogeneous for $U$. The resulting neighbourhood is homogeneous for $E$. Sets with such an open representative form a [sigma-algebra](measure-theory.md#sigma-algebra): countable unions collect the meagre errors, and complements replace $U^c$ by its interior, differing only on the nowhere-dense boundary of $U$. This proves that all star-[Borel sets](measure-theory.md#borel-set) are completely Ramsey.

#### Cone on an infinite coinfinite ground set

↑ **Parent:** [Ellentuck topology](#ellentuck-topology)

For an infinite [coinfinite set](set.md#coinfinite-set) $A\subseteq\mathbb N$, let $E_A=[A]^\omega$ in the [space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers). This cone is a nonempty [clopen set](topology.md#clopen-set) in the [Ellentuck topology](#ellentuck-topology), because it is the basic [neighbourhood](topology.md#neighbourhood-mathematics) $[\varnothing,A]$, and any $X\notin E_A$ has a finite initial segment containing a point outside $A$ and hence a basic [neighbourhood](topology.md#neighbourhood-mathematics) disjoint from $E_A$.

The cone is a [closed set](topology.md#closed-set) with empty [interior](topology.md#interior-topology) in the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets): membership of a point outside $A$ witnesses its complement as an [open set](topology.md#open-set), while every ordinary finite-stem [neighbourhood](topology.md#neighbourhood-mathematics) can be extended by an arbitrarily large point outside $A$. Thus $E_A$ is an ordinary [nowhere dense set](topological-analysis.md#nowhere-dense-set), but it is neither ordinary open nor Ellentuck nowhere dense. It provides both distinctions between these two [topologies](topology.md).

##### Ordinarily nowhere-dense sets need not be completely Ramsey

↑ **Parent:** [Cone on an infinite coinfinite ground set](#cone-on-an-infinite-coinfinite-ground-set)

The cone $[E]^\omega$ on the even [integers](number-theory.md#integer) is nonempty and [Ellentuck topology](#ellentuck-topology) open, while it is closed and [nowhere dense](topological-analysis.md#nowhere-dense-set) in the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets). Choose a [finite-symmetric-difference parity colouring](#finite-symmetric-difference-parity-colouring) on that cone and take one colour class. The class is still ordinarily [nowhere dense](topological-analysis.md#nowhere-dense-set) because its [closure](topology.md#closure-topology) lies in the cone, but every stem-free refinement inside the cone meets both colours. Hence it is not [completely Ramsey](#completely-ramsey-set).

#### Countable unions of Ellentuck clopen sets need not be closed

↑ **Parent:** [Ellentuck topology](#ellentuck-topology)

In the [space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers), the families $C_n=\{X:n\notin X\}$ are [clopen sets](topology.md#clopen-set) in the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets) and thus in the finer [Ellentuck topology](#ellentuck-topology). Their union is $[\mathbb N]^\omega\setminus\{\mathbb N\}$. Every basic [Ellentuck topology](#ellentuck-topology) neighborhood of $\mathbb N$ contains $\mathbb N\setminus\{n\}$ for some sufficiently large $n$, so this union is not a [closed set](topology.md#closed-set).

#### Baire property in the Ellentuck topology

↑ **Parent:** [Ellentuck topology](#ellentuck-topology)

A subset of the [space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers) has this property when it differs from an [Ellentuck topology](#ellentuck-topology) open set by a [meagre set](topological-analysis.md#meagre-set) in the same topology. By the complete-Ramsey characterization, these are precisely the [completely Ramsey sets](#completely-ramsey-set). Using meagreness from a different topology changes the definition.

### Ordinary topology on infinite subsets

↑ **Parent:** [Space of infinite subsets of the natural numbers](#space-of-infinite-subsets-of-the-natural-numbers)

The ordinary topology on $[\mathbb N]^\omega$ has basic sets $[s]=\{X:s\sqsubset X\}$ for finite $s$. It is the [product topology](geometry-and-topology.md#product-topology) on increasing enumerations, and also the subspace topology on infinite-subset [indicator functions](measure-theory.md#indicator-function) in $\{0,1\}^{\mathbb N}$.

#### Dense countable family of cofinite infinite subsets

↑ **Parent:** [Ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets)

In the [ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets), the family $D$ of [cofinite sets](set-theory.md#cofinite-set) is a [countable set](set-theory.md#countable-set), a [dense](topology.md#dense-set) and a [meagre set](topological-analysis.md#meagre-set). Countability follows by indexing its members by their finite complements. Each singleton is closed with empty interior, while every basic cylinder with finite initial segment $s$ contains $s\cup\{n:n>\max s\}$. Consequently $D$ is not a [nowhere dense set](topological-analysis.md#nowhere-dense-set). This example uses the ordinary cylinder topology, rather than the [Ramsey cone topology](#ramsey-cone-topology).

#### Gap-doubling closed family of infinite subsets

↑ **Parent:** [Ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets)

The family $D=\{\{a_1<a_2<\cdots\}:a_{n+1}>2a_n\text{ for all }n\}$ is ordinarily closed and [nowhere dense](topological-analysis.md#nowhere-dense-set). A failed gap is witnessed by a finite prefix, and any cylinder can be refined by adjoining consecutive large integers that fail the gap. Nevertheless $D$ intersects every infinite-subset cone in continuum many sets: a binary tree chooses two sufficiently large next points inside its reservoir at each step.

##### Meagre set meeting every Ramsey cone in both colours

↑ **Parent:** [Gap-doubling closed family of infinite subsets](#gap-doubling-closed-family-of-infinite-subsets)

A closed [nowhere dense](topological-analysis.md#nowhere-dense-set) family can meet every cone $[M]^\omega$ in continuum many sets, as the [gap-doubling closed family of infinite subsets](#gap-doubling-closed-family-of-infinite-subsets) does. Well-order the cones and choose two fresh candidates in each, permanently reserving one of each colour. The red family meets every cone and its complement contains every reserved blue candidate, so it is not Ramsey. As a subset of the closed nowhere dense family, it is still nowhere dense and has the [Baire property in the ordinary infinite-subset topology](#baire-property-in-the-ordinary-infinite-subset-topology). This recursion requires no regularity assumption on the continuum cardinal.

#### Baire property in the ordinary infinite-subset topology

↑ **Parent:** [Ordinary topology on infinite subsets](#ordinary-topology-on-infinite-subsets)

A family $Y\subseteq[\mathbb N]^\omega$ is $\tau$-Baire when $Y\triangle O$ is [meagre](topological-analysis.md#meagre-set) for some ordinarily open family $O$. This is weaker than the corresponding regularity in the [star topology](#ellentuck-topology). A [meagre set meeting every Ramsey cone in both colours](#meagre-set-meeting-every-ramsey-cone-in-both-colours) has the ordinary Baire property while failing to be a [Ramsey set of infinite subsets](#ramsey-set-of-infinite-subsets).

## Matching Ramsey number

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

For $r\geq s\geq1$, the two-colour Ramsey number for disjoint edge matchings is

$$
R(rK_2,sK_2)=2r+s-1.
$$

Thus every red-blue colouring of $K_{2r+s-1}$ contains either a red matching of size $r$ or a blue matching of size $s$, and the order is sharp.

## Triangle-packing Ramsey number

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

For $t\geq2$, the two-colour Ramsey number for $t$ vertex-disjoint triangles is

$$
R(tK_3,tK_3)=5t.
$$

Every red-blue colouring of $K_{5t}$ therefore contains $t$ vertex-disjoint triangles of one colour, while a colouring of $K_{5t-1}$ can avoid such a packing in both colours.

## Finite coloring

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

A finite coloring of a set $X$ is a [function](function.md) $c:X\to C$ into a [finite set](set.md#finite-set) $C$ of colors. A subset is monochromatic when the restriction of $c$ to it is [constant](function.md#constant-function).

### Colour profile of a finite block

↑ **Parent:** [Finite coloring](#finite-coloring)

The [colour profile](#colour-profile-of-a-finite-block) of a length-$N$ block $b_1,\ldots,b_N$ under a [finite colouring](#finite-coloring) $c$ is the ordered tuple $(c(b_1),\ldots,c(b_N))$. There are at most $r^N$ profiles when $c$ uses at most $r$ colours. Equally profiled blocks reproduce every colour configuration at the same relative positions; this converts a colouring of points into a [finite colouring](#finite-coloring) of blocks in the [colour-focusing proof of Van der Waerden theorem](#colour-focusing-proof-of-van-der-waerden-theorem).

### Colour class

↑ **Parent:** [Finite coloring](#finite-coloring)

A [colour class](#colour-class) of a [finite colouring](#finite-coloring) $c:X\to\{1,\ldots,r\}$ is a fibre $c^{-1}(i)$. Each [colour class](#colour-class) is a [monochromatic set](#monochromatic-set), and these fibres give a finite [set partition](combinatorics.md#set-partition) of $X$ after empty fibres are omitted.

### Cyclic logarithmic coloring

↑ **Parent:** [Finite coloring](#finite-coloring)

For $b>1$ and an [integer](number-theory.md#integer) $q\geq2$, assign $x\geq1$ the color $\lfloor\log_b x\rfloor\bmod q$. The [floor function](calculus.md#floor-function) partitions the domain into half-open geometric bins. If $1<\log_b(y/x)<q-1$, their bin indices differ by an [integer](number-theory.md#integer) in $\{1,\ldots,q-1\}$, so their colors differ. For example, $b=3/2$ and $q=3$ separates every ratio in $[1.9,2]$. Composing this [finite coloring](#finite-coloring) with another [logarithm](calculus.md#logarithm) can obstruct [monochromatic](#monochromatic-set) multiplicative configurations whose [logarithms](calculus.md#logarithm) have such ratios.

### Refinement of a finite coloring

↑ **Parent:** [Finite coloring](#finite-coloring)

A refinement of a [finite coloring](#finite-coloring) assigns different new colors whenever the original colors differ. A set [monochromatic](#monochromatic-set) for the refinement is therefore [monochromatic](#monochromatic-set) for the original coloring. Given colorings $\chi,\psi$, the product coloring $n\mapsto(\chi(n),\psi(n))$ refines both. This makes it possible to impose finitely many coloring obstructions simultaneously.

### Monochromatic set

↑ **Parent:** [Finite coloring](#finite-coloring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monochromatic_set)

<h2 id="ramsey-s-theorem">Ramsey's theorem</h2>

↑ **Parent:** [Ramsey theory](ramsey-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ramsey's_theorem)

The infinite form of Ramsey's theorem says that if the $r$-element subsets of an infinite set are finitely colored, then some infinite subset has all its $r$-element subsets in one color.

### Simultaneous coefficient patterns from a homogeneous four-set colouring

↑ **Parent:** [Ramsey's theorem](#ramsey-s-theorem)

Take increasing even $u_i$ for which every ordered four-index expression $u_i+u_j+2u_k+2u_l$ has one colour. The [Ramsey theorem for r-sets](#ramsey-s-theorem) supplies them. Set $x_i=u_{2i-1}+u_{2i}$ and $y_i=(u_1+u_2)/2+2u_{i+2}$. Then both $x_i+2x_j$ and $y_i+y_j$ use the same ordered coefficient pattern $(1,1,2,2)$, so their union is monochromatic. The shared half-prefix makes the unweighted pair family possible without asking the two families to use the same generating sequence.

### Successive thinning proof of the infinite Ramsey theorem

↑ **Parent:** [Ramsey's theorem](#ramsey-s-theorem)

For finitely coloured $(r+1)$-element subsets, choose successive least points and use the inductive $r$-set theorem to thin the remaining reservoir after each choice. Every tuple with that least point then has one assigned colour. The [infinite pigeonhole principle](algebra.md#infinite-pigeonhole-principle) retains infinitely many least points with the same assigned colour, giving an infinite homogeneous set. The $r=1$ base case is the same pigeonhole principle. This proves the [Ramsey theorem for r-sets](#ramsey-s-theorem) for all finite $r$.

### Finite Ramsey theorem

↑ **Parent:** [Ramsey's theorem](#ramsey-s-theorem)

For positive integers $r,k,m$, there is $n$ such that every $k$-coloring of the $r$-element subsets of $[n]$ has a monochromatic $m$-element subset. A diagonal [compactness](topology.md#compact-space) argument deduces this from [Ramsey's theorem](#ramsey-s-theorem).

#### Ramsey number

↑ **Parent:** [Finite Ramsey theorem](#finite-ramsey-theorem)

The Ramsey number $R(s,t)$ is the least integer $n$ such that every red–blue coloring of the edges of $K_n$ contains a red $K_s$ or a blue $K_t$. The neighbor split at one vertex gives $R(s,t)\le R(s-1,t)+R(s,t-1)$, with $R(1,t)=R(s,1)=1$. This proves finite existence and gives quantitative bounds.

## Modular-intersection graph Ramsey lower bound

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

Let $p$ be prime and join two $p^2$-subsets of a $p^3$-element set when their intersection size is divisible by $p$. The [modular intersection bound for a set family](combinatorics.md#modular-intersection-bound-for-a-set-family) bounds both its independence and clique numbers by a quantity strictly below $p^{3p}$. Since the graph has $\binom{p^3}{p^2}\geq p^{p^2}$ vertices,

$$
R(p^{3p},p^{3p})\geq p^{p^2},
$$

a lower bound larger than every fixed power of $p^{3p}$ as $p\to\infty$.

## Combinatorial line

↑ **Parent:** [Ramsey theory](ramsey-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Combinatorial_line)

Let $X$ be a finite alphabet. A combinatorial line in $X^n$ is obtained by fixing some coordinates and replacing every coordinate in one nonempty active set by the same variable letter. It therefore contains one word for each letter of $X$.

### Fixed-active-size obstruction for combinatorial lines

↑ **Parent:** [Combinatorial line](#combinatorial-line)

For any proposed positive active size $d$, the displayed two-colour [finite colouring](#finite-coloring) of binary words gives opposite colours to the two points of every [combinatorial line](#combinatorial-line) with exactly $d$ active coordinates. Their counts of the letter $2$ differ by $d$. Thus no dimension can guarantee a [monochromatic](#monochromatic-set) line of one universally prescribed active size, even though the [Hales-Jewett theorem](#hales-jewett-theorem) guarantees some active size. The colouring is allowed to depend on $d$ because $d$ is chosen before the colouring.

### Run-count obstruction to interval-active lines

↑ **Parent:** [Combinatorial line](#combinatorial-line)

For any $N\geq1$, color $w\in[3]^N$ by its first letter together with its number of [runs of a word](foundations-of-mathematics.md#run-of-a-word) modulo $3$. This [finite coloring](#finite-coloring) uses at most nine colors and has no [monochromatic](#monochromatic-set) [combinatorial line](#combinatorial-line) whose active coordinates form an interval. An active interval starting at the first coordinate changes the first letter. Otherwise, its left boundary and optional right boundary contribute $0$ versus $1$, $0$ versus $2$, or $1$ versus $2$ to the run count as the active letter varies. These differences remain nonzero modulo $3$. The first-letter component is essential for intervals that occupy the entire word.

### Coordinate duplication for combinatorial lines

↑ **Parent:** [Combinatorial line](#combinatorial-line)

Repeat every coordinate of a word $q$ times. A [combinatorial line](#combinatorial-line) maps to a [combinatorial line](#combinatorial-line) whose active-set size is multiplied by $q$. Pulling back a [finite coloring](#finite-coloring) along this map and using the [Hales-Jewett theorem](#hales-jewett-theorem) forces [monochromatic](#monochromatic-set) lines with active-set size divisible by any prescribed positive integer $q$.

### Adequate family of active coordinate sets

↑ **Parent:** [Combinatorial line](#combinatorial-line)

For a fixed alphabet size $m>1$, a family $\mathcal F\subseteq\mathcal P([n])$ is adequate if every two-color [finite coloring](#finite-coloring) of $[m]^n$ has a [monochromatic](#monochromatic-set) [combinatorial line](#combinatorial-line) whose nonempty active coordinate set belongs to $\mathcal F$.

An [intersecting family](extremal-set-theory.md#intersecting-family) is never adequate. Color a word red when the coordinates carrying letter $1$ contain a member of $\mathcal F$, and blue otherwise. For a line with active set $A\in\mathcal F$, its letter-$1$ word is red and its letter-$2$ word is blue, because no member of an [intersecting family](extremal-set-theory.md#intersecting-family) can lie wholly outside $A$.

### Hales-Jewett theorem

↑ **Parent:** [Combinatorial line](#combinatorial-line)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hales–Jewett_theorem)

For every finite alphabet $X$ and every positive integer $k$, there is $n$ such that every $k$-coloring of $X^n$ contains a monochromatic [combinatorial line](#combinatorial-line).

#### Letter-merging proof of the Hales-Jewett theorem

↑ **Parent:** [Hales-Jewett theorem](#hales-jewett-theorem)

Induct on the alphabet size $k$. For an $r$-colouring, choose an $(k-1,k)$-insensitive [combinatorial subspace](#combinatorial-subspace) whose dimension forces a [monochromatic](#monochromatic-set) [combinatorial line](#combinatorial-line) over the first $k-1$ letters. The inductive [Hales-Jewett theorem](#hales-jewett-theorem) supplies that line. Changing all of its active parameters from $k-1$ to $k$, one at a time, preserves the colour by the [alphabet insensitivity lemma](#alphabet-insensitivity-lemma). Thus the line extends to all $k$ letters. The one-letter alphabet is the base case.

#### Alphabet insensitivity lemma

↑ **Parent:** [Hales-Jewett theorem](#hales-jewett-theorem)

For a [finite coloring](#finite-coloring) of $[m]^N$, a [combinatorial subspace](#combinatorial-subspace) is $(a,b)$-insensitive if replacing $a$ by $b$, or conversely, in any of its variable coordinates leaves the color unchanged. For every number of colors, alphabet size $m\geq2$, and dimension $d$, sufficiently large $N$ guarantees such a $d$-dimensional [combinatorial subspace](#combinatorial-subspace) for any specified distinct letters $a,b$.

A proof uses the [pigeonhole principle](algebra.md#pigeonhole-principle) on chains $a^j b^{L-j}$ in consecutive coordinate blocks. Choose block lengths from left to right, making each long enough to pigeonhole the vector of colors for every earlier word and every later variable assignment. Process the blocks from right to left. Two equal color vectors give a nonempty variable interval insensitive to $a,b$. Insensitivity already obtained in later blocks survives all restrictions of earlier coordinates. This lemma proves the [Hales-Jewett theorem](#hales-jewett-theorem) by induction on alphabet size.

##### Explicit block bound for alphabet insensitivity

↑ **Parent:** [Alphabet insensitivity lemma](#alphabet-insensitivity-lemma)

For r colours, k letters and d variable blocks, set $P_i=\sum_{j<i}L_j$ and $L_i=r^{k^{P_i+d-i}}$. Process blocks from right to left. In block i, the $L_i+1$ words $a^t b^{L_i-t}$ have [colour profiles](#colour-profile-of-a-finite-block) indexed by all $k^{P_i}$ earlier words and $k^{d-i}$ later variable assignments. Two profiles agree, giving a nonempty variable interval insensitive to exchanging a and b. Previously obtained insensitivity holds for all earlier words and survives their restriction. This constructs the [combinatorial subspace](#combinatorial-subspace) required by the [alphabet insensitivity lemma](#alphabet-insensitivity-lemma).

### Combinatorial subspace

↑ **Parent:** [Combinatorial line](#combinatorial-line)

A $d$-dimensional combinatorial subspace, also called a $d$-parameter set, has $d$ pairwise disjoint nonempty active coordinate sets. Coordinates in the $j$th active set all receive one freely chosen alphabet letter, independently for each $j$, while the remaining coordinates stay fixed.

#### Extended Hales-Jewett theorem

↑ **Parent:** [Combinatorial subspace](#combinatorial-subspace)

For every alphabet size $m$, number of colors $k$, and dimension $d$, some $n$ has the property that every $k$-coloring of $[m]^n$ contains a monochromatic $d$-dimensional [combinatorial subspace](#combinatorial-subspace). It follows from the [Hales-Jewett theorem](#hales-jewett-theorem) by identifying $[m]^{dN}$ with the word space over the alphabet $[m]^d$.

## Hilbert cube

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

A Hilbert $n$-cube in the [positive integers](number-theory.md#positive-integer) is a set

$$
\left\{a+\sum_{i\in I}x_i:I\subseteq[n]\right\},
$$

where $a,x_1,\ldots,x_n$ are positive integers.

### Hilbert cube theorem

↑ **Parent:** [Hilbert cube](#hilbert-cube)

Every [finite coloring](#finite-coloring) of the [positive integers](number-theory.md#positive-integer) contains a monochromatic [Hilbert cube](#hilbert-cube) of every prescribed finite dimension.

## Van der Waerden theorem

↑ **Parent:** [Ramsey theory](ramsey-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Van_der_Waerden_theorem)

Every [finite coloring](#finite-coloring) of the [positive integers](number-theory.md#positive-integer) contains monochromatic [arithmetic progressions](arithmetic.md#arithmetic-progression) of every prescribed finite length.

### Colour-focusing proof of Van der Waerden theorem

↑ **Parent:** [Van der Waerden theorem](#van-der-waerden-theorem)

For positive $r,k$, let $W(r,k)$ bound the interval needed to force a [monochromatic](#monochromatic-set) length-$k$ [arithmetic progression](arithmetic.md#arithmetic-progression) in every [finite colouring](#finite-coloring) using at most $r$ colours. The [colour-focusing proof of Van der Waerden theorem](#colour-focusing-proof-of-van-der-waerden-theorem) inducts on $k$, simultaneously for every number of colours, and then creates progressions of distinct colours with a common next point.

Assume $W(r,k)$ exists for every $r$. For fixed $r$, construct $F_t$ such that a [finite colouring](#finite-coloring) of $[F_t]$ using at most $r$ colours contains either a [monochromatic](#monochromatic-set) length-$(k+1)$ [arithmetic progression](arithmetic.md#arithmetic-progression), or $t$ length-$k$ [arithmetic progressions](arithmetic.md#arithmetic-progression) of pairwise distinct colours of the form $f-hd_i$, $1\le h\le k$, with a common focus $f\in[F_t]$. Take $F_1=2W(r,k)$: a length-$k$ [arithmetic progression](arithmetic.md#arithmetic-progression) in its first half has its next point inside the whole interval. For $k=1$, give a singleton step $1$.

Given $N=F_t$, put $M=W(r^N,k)$ and $F_{t+1}=2NM$. Regard the first $M$ length-$N$ blocks as coloured by their full [colour profiles](#colour-profile-of-a-finite-block). Some block indices $j_0,j_0+D,\ldots,j_0+(k-1)D$ share a profile. If there is no [monochromatic](#monochromatic-set) length-$(k+1)$ [arithmetic progression](arithmetic.md#arithmetic-progression), this profile supplies $t$ focused progressions with focus position $f$, steps $d_i$, and distinct colours $q_i$. The colour $q$ of position $f$ differs from every $q_i$. In the later block $j_*=j_0+kD\le2M$, put $F=N(j_*-1)+f$. For each $i$, the points $F-h(ND+d_i)$ have colour $q_i$: they lie in the selected block $j_*-hD$ at position $f-hd_i$. The points $F-hND$ have colour $q$. Thus $t+1$ distinct colours focus at $F$. For $t=r$, its own colour completes one of the $r$ focused progressions. The base case $W(r,1)=1$ completes the [mathematical induction](foundations-of-mathematics.md#mathematical-induction).

### Brauer progression theorem

↑ **Parent:** [Van der Waerden theorem](#van-der-waerden-theorem)

For [positive integers](number-theory.md#positive-integer) $k,s,\ell$, some $N$ ensures that every $k$-color [finite coloring](#finite-coloring) of $[N]$ contains a [monochromatic](#monochromatic-set) set

$$
\{sd,a,a+d,\ldots,a+(\ell-1)d\},\qquad a,d>0.
$$

It follows from the [Van der Waerden theorem](#van-der-waerden-theorem) by [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on the number of colors. If $M$ is a bound for $k-1$ colors, take a long one-color [arithmetic progression](arithmetic.md#arithmetic-progression) of length $(\ell-1)M+1$ and step $d$. Either one of $sd,2sd,\ldots,Msd$ has its color, giving the result immediately, or these multiples use only $k-1$ colors. Pull back their [finite coloring](#finite-coloring) to $[M]$ and use [mathematical induction](foundations-of-mathematics.md#mathematical-induction), then multiply the resulting configuration by $sd$. Enlarge the ambient finite [integer interval](number-theory.md#integer-interval) to include all these multiples. The cases $k=1$ and $\ell=1$ are immediate. The parameter $s$ makes this useful for positive [monochromatic](#monochromatic-set) solutions of a [partition regular equation](graph-theory.md#partition-regular-equation) with arbitrary [integer](number-theory.md#integer) coefficients.

### Strengthened Van der Waerden theorem

↑ **Parent:** [Van der Waerden theorem](#van-der-waerden-theorem)

For all positive integers $k,m$, some $n$ has the following property: every $k$-coloring of $[n]$ contains $a,d>0$ for which

$$
\{d,a,a+d,\ldots,a+(m-1)d\}
$$

is monochromatic. Thus the [common difference](arithmetic.md#common-difference) has the same color as the progression.

### Color-focused arithmetic progression

↑ **Parent:** [Van der Waerden theorem](#van-der-waerden-theorem)

Several monochromatic [arithmetic progressions](arithmetic.md#arithmetic-progression) are color-focused when they have different colors and extend by one further term to the same point. Such focused families give an elementary induction proof of the length-three case of the [Van der Waerden theorem](#van-der-waerden-theorem).

## Gallai theorem for an integer lattice

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

For every finite $S\subseteq\mathbb N^d$, every [finite coloring](#finite-coloring) of $\mathbb N^d$ contains a monochromatic homothetic copy $a+rS$. The theorem follows from the [Hales-Jewett theorem](#hales-jewett-theorem) by coloring a word according to the sum of the points indexed by its letters.

### Canonical arithmetic progression dichotomy

↑ **Parent:** [Gallai theorem for an integer lattice](#gallai-theorem-for-an-integer-lattice)

Every colouring of the [positive integers](number-theory.md#positive-integer), even with infinitely many colours, has an [arithmetic progression](arithmetic.md#arithmetic-progression) of any prescribed finite length on which the colouring is constant or [injective](algebra.md#injective-function). Encode a progression by the [equivalence relation](set-theory.md#equivalence-relation) of equality of its colours. This gives a [finite colouring](#finite-coloring) of its starting point and step. A [Gallai theorem for an integer lattice](#gallai-theorem-for-an-integer-lattice) copy of a suitable two-dimensional pattern makes either all indices inequivalent, or one equal-colour pair range independently over two whole progressions. In the second case, one of those progressions is [monochromatic](#monochromatic-set).

### Sum map from words to homothetic copies

↑ **Parent:** [Gallai theorem for an integer lattice](#gallai-theorem-for-an-integer-lattice)

For a finite pattern $\{v_1,\ldots,v_k\}$ in a [real vector space](vector-space.md#real-vector-space), pull a [finite colouring](#finite-coloring) back to words through the displayed sum map. A [combinatorial line](#combinatorial-line) with active coordinates J maps to $a+|J|\{v_1,\ldots,v_k\}$. The [Hales-Jewett theorem](#hales-jewett-theorem) therefore forces a [monochromatic](#monochromatic-set) [homothetic copy](geometry-and-topology.md#homothetic-copy-of-a-finite-configuration). [Integer](number-theory.md#integer) patterns remain in the [integer lattice](geometry-and-topology.md#integer-lattice); choosing b sufficiently large gives the positive-lattice version.

### Arithmetic-progression bipartite Ramsey dichotomy

↑ **Parent:** [Gallai theorem for an integer lattice](#gallai-theorem-for-an-integer-lattice)

Every red-blue [finite coloring](#finite-coloring) of the pairs of [positive integers](number-theory.md#positive-integer) has either a blue complete [arithmetic progression](arithmetic.md#arithmetic-progression) of any prescribed finite length $m$, or two disjoint $m$-term [arithmetic progressions](arithmetic.md#arithmetic-progression) with all cross-pairs red. To see the geometry, assign $(a,d)$ a chosen red pair of indices $(r,s)$ in its progression, assuming the first alternative fails. Apply the [Gallai theorem for an integer lattice](#gallai-theorem-for-an-integer-lattice) to the fixed finite pattern

$$
\bigcup_{0\leq r<s<m}\{(si-rj,j-i):0\leq i,j<m\}.
$$

In a [monochromatic](#monochromatic-set) copy $(a_0,d_0)+qF$ with common label $(r,s)$, the selected red pairs are precisely

$$
\bigl(a_0+rd_0+q(s-r)i,\ a_0+sd_0+q(s-r)j\bigr).
$$

The copy lies in the positive quadrant, so $d_0>q(m-1)$. Consequently the two displayed [arithmetic progressions](arithmetic.md#arithmetic-progression) are disjoint. Translating the finite pattern before applying the lattice theorem permits its initially negative coordinates.

## Partition regular matrix

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

A matrix $A$ over the [rational numbers](number-theory.md#rational-number) is partition regular when every [finite coloring](#finite-coloring) of the [positive integers](number-theory.md#positive-integer) admits a [monochromatic](#monochromatic-set) vector $x$ satisfying $Ax=0$, with every coordinate a positive integer. Repeated coordinates are permitted.

### Scaling invariance of homogeneous partition regularity

↑ **Parent:** [Partition regular matrix](#partition-regular-matrix)

For any positive integer $c$, a homogeneous rational matrix is [partition regular](#partition-regular-matrix) over $c\mathbb N$ if and only if it is [partition regular](#partition-regular-matrix) over $\mathbb N$. Pull a colouring of $c\mathbb N$ back along $n\mapsto cn$ and scale the resulting solution. Conversely, restrict a colouring of all positive integers to $c\mathbb N$. The argument depends on homogeneity and does not automatically extend to inhomogeneous equations or prescribed distinctness conditions.

### Reciprocal partition regularity

↑ **Parent:** [Partition regular matrix](#partition-regular-matrix)

If a [rational matrix](vector-space.md#rational-matrix) $A$ is a [partition regular matrix](#partition-regular-matrix), every [finite coloring](#finite-coloring) of the [positive integers](number-theory.md#positive-integer) admits [monochromatic](#monochromatic-set) $y_1,\ldots,y_n$ such that

$$
A(1/y_1,\ldots,1/y_n)^{\mathsf T}=0.
$$

Choose a [compactness bound for partition regularity](#compactness-bound-for-partition-regularity) $T$ for the number of colors, put $S=\operatorname{lcm}(1,\ldots,T)$, and pull back the coloring by $t\mapsto S/t$ on $[T]$. A [monochromatic](#monochromatic-set) positive solution $x$ of $Ax=0$ gives $y_i=S/x_i$; then $(1/y_i)=x_i/S$. The [least common multiple](number-theory.md#least-common-multiple) guarantees that every $y_i$ is a [positive integer](number-theory.md#positive-integer).

### Compactness bound for partition regularity

↑ **Parent:** [Partition regular matrix](#partition-regular-matrix)

If a [rational matrix](vector-space.md#rational-matrix) is a [partition regular matrix](#partition-regular-matrix), then for each fixed number of colors $k$ some finite [integer interval](number-theory.md#integer-interval) $[T]$ already forces a [monochromatic](#monochromatic-set) positive solution. Otherwise the solution-free [finite colorings](#finite-coloring) of successive intervals form a finitely branching [tree](combinatorics.md#tree-graph-theory) with every level nonempty. The [König infinity lemma](combinatorics.md#konig-s-lemma) gives an infinite branch, contradicting partition regularity. More generally, this argument applies to any family of configurations each using finitely many [positive integers](number-theory.md#positive-integer).

### Partition regularity dichotomy under an extra constraint

↑ **Parent:** [Partition regular matrix](#partition-regular-matrix)

For a [partition regular matrix](#partition-regular-matrix) $A$ and any property $P$ of its positive solution vectors, either every [finite coloring](#finite-coloring) admits a [monochromatic](#monochromatic-set) solution with $P$, or every [finite coloring](#finite-coloring) admits one without $P$. If the first alternative fails, take a witnessing coloring and pair it with any other coloring. Partition regularity of the product coloring forces a solution avoiding $P$ in the other coloring. The alternatives need not be exclusive.

### Columns property

↑ **Parent:** [Partition regular matrix](#partition-regular-matrix)

If $c_1,\ldots,c_n$ are the columns of a matrix, the matrix has the columns property when $[n]$ has an ordered partition $B_1\sqcup\cdots\sqcup B_s$ such that

$$
\sum_{i\in B_1}c_i=0
$$

and, for $j>1$, $\sum_{i\in B_j}c_i$ belongs to the [linear span](vector-space.md#linear-span) of the columns indexed by $B_1\cup\cdots\cup B_{j-1}$.

<h4 id="rado-s-theorem">Rado's theorem</h4>

↑ **Parent:** [Columns property](#columns-property)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rado's_theorem_(Ramsey_theory))

Rado's theorem states that a rational matrix is [partition regular](#partition-regular-matrix) if and only if it has the [columns property](#columns-property).

##### Partition-regular system forcing an ordered Schur relation

↑ **Parent:** [Rado's theorem](#rado-s-theorem)

The positive-variable system $3x+y=3z$, $x-2y=w$ is [partition regular](#partition-regular-matrix). Its columns for $x,z,w$ sum to zero, and the remaining $y$ column lies in their rational span, satisfying the [columns condition](#columns-property). Thus every finite colouring has monochromatic positive $x,y,z,w$ with $2y<x$. A triangular [m-p-c set](#m-p-c-set) gives the explicit solution $x=3u$, $y=3v$, $z=3u+v$, $w=3u-6v$, with positivity guaranteed by membership in that set.

##### Rado theorem for one equation

↑ **Parent:** [Rado's theorem](#rado-s-theorem)

For nonzero rational coefficients $a_1,\ldots,a_n$, the equation

$$
a_1x_1+\cdots+a_nx_n=0
$$

is [partition regular](graph-theory.md#partition-regular-equation) exactly when some nonempty subset of the coefficients has sum zero. This is the one-row form of the [columns property](#columns-property).

###### Brauer configuration for a one-row zero-sum equation

↑ **Parent:** [Rado theorem for one equation](#rado-theorem-for-one-equation)

Suppose nonzero integer coefficients have a nonempty zero-sum subset $I$, and fix $i_0\in I$. Put $s=|a_{i_0}|$ and $C=\sum_{j\notin I}a_j$. A [Brauer progression theorem](#brauer-progression-theorem) configuration containing a sufficiently long [monochromatic](#monochromatic-set) progression of step $d$ and the point $sd$ gives a positive solution: take every outside variable equal to $sd$, and the inside variables from the progression with offsets $\lambda_i$, where $\lambda_{i_0}=-\operatorname{sgn}(a_{i_0})C$ and the other offsets are zero. Shifting all inside offsets by the same integer keeps their weighted sum unchanged, because $\sum_{i\in I}a_i=0$. This removes negative offsets while preserving the equation.

###### Leading-residue obstruction to partition regularity

↑ **Parent:** [Rado theorem for one equation](#rado-theorem-for-one-equation)

For nonzero [integer](number-theory.md#integer) coefficients $a_i$, choose a [prime number](number-theory.md#prime-number) $p>\sum_i|a_i|$ and colour each positive integer by its nonzero leading residue after removing its power of $p$. In a [monochromatic](#monochromatic-set) zero-sum solution, divide by the least occurring power of $p$. Reduction modulo $p$ then makes the sum of the coefficients attached to the least-valuation variables vanish modulo $p$. Its absolute value is less than $p$, so that sum vanishes as an integer. This gives the necessity direction of the one-equation [partition regularity](#partition-regular-matrix) criterion without using the general [Rado theorem](#rado-s-theorem).

###### One-equation partition regularity over odd integers

↑ **Parent:** [Rado theorem for one equation](#rado-theorem-for-one-equation)

A rational homogeneous equation $\sum_i a_ix_i=0$ has a [monochromatic](#monochromatic-set) positive odd solution in every [finite colouring](#finite-coloring) of the odd integers exactly when its full coefficient sum is zero. Sufficiency uses a constant odd vector. For necessity, clear denominators and, if the total $S$ is nonzero, colour by odd [residue classes](number-theory.md#residue-class) modulo $2^K>|S|$. A common odd residue is invertible, so a solution would require $2^K\mid S$, impossible. This is stronger than the zero-sum-subset criterion for unrestricted [partition regularity](#partition-regular-matrix).

#### P-adic columns lemma

↑ **Parent:** [Columns property](#columns-property)

The necessity direction in [Rado's theorem](#rado-s-theorem) colors an integer using initial data from a [P-adic valuation](number-theory.md#p-adic-valuation). Applying partition regularity and grouping the coordinates of a monochromatic solution by valuation yields the blocks in the [columns property](#columns-property); reduction modulo successively higher powers of $p$ supplies the required linear dependences.

##### Finite separating-functional proof of the columns condition

↑ **Parent:** [P-adic columns lemma](#p-adic-columns-lemma)

After clearing denominators in a [matrix](vector-space.md#matrix), for every disjoint pair of index sets $I,B$ with $B$ nonempty and $\sum_{i\in B}a_i$ outside the [linear span](vector-space.md#linear-span) of the $I$-columns, choose an integer [linear functional](linear-algebra.md#linear-functional) vanishing on those columns but not on the indicated sum. Choose a [prime number](number-theory.md#prime-number) dividing none of the finitely many nonzero evaluations. The [last nonzero digit coloring](#last-nonzero-digit-coloring) for this prime, applied to a [monochromatic](#monochromatic-set) positive solution, groups coordinates into blocks by [P-adic valuation](number-theory.md#p-adic-valuation). Applying the appropriate functional and reducing modulo the prime shows that each block sum lies in the [linear span](vector-space.md#linear-span) of all earlier columns. This proves necessity in [Rado's theorem](#rado-s-theorem) without an asymptotic limiting argument.

##### Last nonzero digit coloring

↑ **Parent:** [P-adic columns lemma](#p-adic-columns-lemma)

For a [prime number](number-theory.md#prime-number) $p$, write a positive integer as $x=p^{v_p(x)}u$ with $p\nmid u$. Its last nonzero base-$p$ digit is $u\bmod p$, an element of $\{1,\ldots,p-1\}$. Assigning this digit as the color gives the last nonzero digit coloring used in the necessity proof of [Rado's theorem](#rado-s-theorem).

#### M-p-c set

↑ **Parent:** [Columns property](#columns-property)

An $(m,p,c)$-set has positive integer generators $z_1,\ldots,z_m$ chosen so that every expression below is positive, and consists of all their values:

$$
cz_j+\sum_{s>j}\lambda_s z_s,
\qquad \lambda_s\in\mathbb Z,\quad |\lambda_s|\leq p.
$$

The required positivity is equivalent to $cz_j>p\sum_{s>j}z_s$ for each $j$; it is not defined by discarding nonpositive values from the displayed family.

##### Rado solution inside an m-p-c set

↑ **Parent:** [M-p-c set](#m-p-c-set)

Suppose the columns $a_i$ of a [matrix](vector-space.md#matrix) over the [rational numbers](number-theory.md#rational-number) satisfy the [columns condition](#columns-property) with blocks $B_1,\ldots,B_s$. Choose rational coefficients $\lambda_{ij}$ such that

$$
\sum_{i\in B_j}a_i+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i=0.
$$

Choose a positive integer $c$ clearing all denominators and $p\geq\max|c\lambda_{ij}|$. For generators of any full positive [M-p-c set](#m-p-c-set), the coordinates

$$
x_i=cz_h+\sum_{j>h}c\lambda_{ij}z_j\qquad(i\in B_h)
$$

lie in that set and satisfy $Ax=0$. Thus the [monochromatic m-p-c set theorem](#monochromatic-m-p-c-set-theorem) supplies the sufficiency direction of [Rado's theorem](#rado-s-theorem).

##### Monochromatic m-p-c set theorem

↑ **Parent:** [M-p-c set](#m-p-c-set)

For every positive $m,p,c$, every [finite coloring](#finite-coloring) of the [positive integers](number-theory.md#positive-integer) contains a monochromatic [M-p-c set](#m-p-c-set).

###### Finite sums theorem

↑ **Parent:** [Monochromatic m-p-c set theorem](#monochromatic-m-p-c-set-theorem)

For every dimension $m$, every [finite coloring](#finite-coloring) of the [positive integers](number-theory.md#positive-integer) contains $x_1,\ldots,x_m$ for which all nonempty sums of distinct $x_i$ have one color. This is the case $p=c=1$ of the [monochromatic m-p-c set theorem](#monochromatic-m-p-c-set-theorem).

###### Columns partition for finite-sums systems

↑ **Parent:** [Finite sums theorem](#finite-sums-theorem)

Introduce a variable $z_I$ for every nonempty $I\subseteq[k]$ and the homogeneous equations $z_I-\sum_{i\in I}z_{\{i\}}=0$ for $|I|\ge2$. In their [matrix](vector-space.md#matrix) $A$, partition the columns by the displayed blocks. For each $j$, the vector with coordinate $1$ exactly when $j\in I$ lies in the [kernel of a linear map](linear-algebra.md#kernel-of-a-linear-map) of $A$. Its nonzero coordinates occur in $B_j$ and earlier blocks only; every coordinate in $B_j$ is one. Hence the first block's column sum is zero and every subsequent block sum is in the [linear span](vector-space.md#linear-span) of earlier columns. The [columns condition](#columns-property) holds, so [Rado's theorem](#rado-s-theorem) forces a positive [monochromatic](#monochromatic-set) solution, and all nonempty finite sums of its singleton coordinates have the same colour.

## Hindman theorem

↑ **Parent:** [Ramsey theory](ramsey-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hindman_theorem)

Every [finite coloring](#finite-coloring) of the [positive integers](number-theory.md#positive-integer) has an infinite sequence $(x_i)$ for which all nonempty finite sums of distinct terms have one color.

<h3 id="dynamical-proof-of-hindman-s-theorem">Dynamical proof of Hindman's theorem</h3>

↑ **Parent:** [Hindman theorem](#hindman-theorem)

Extend a [finite coloring](#finite-coloring) of the [positive integers](number-theory.md#positive-integer) to a point $x$ of a two-sided [full shift](dynamical-systems.md#full-shift). A [minimal subsystem](dynamical-systems.md#minimal-subsystem) of its forward [orbit closure](dynamical-systems.md#orbit-closure), together with the proximal-minimal existence theorem, supplies a [minimal point](dynamical-systems.md#minimal-point) $y$ [proximal](dynamical-systems.md#proximality) to $x$. Put $q=y(0)$. If all sums in $\{0\}\cup\operatorname{FS}(a_1,\ldots,a_r)$, the augmented [finite-sums set](#finite-sums-set), have color $q$ in $y$, their coordinate constraints define a [cylinder set](geometry-and-topology.md#cylinder-set) containing $y$. The [joint return lemma for a proximal minimal pair](dynamical-systems.md#joint-return-lemma-for-a-proximal-minimal-pair) chooses a new positive term so that all new sums have color $q$ in both $x$ and $y$. [Mathematical induction](foundations-of-mathematics.md#mathematical-induction) gives an infinite [monochromatic](#monochromatic-set) [finite-sums set](#finite-sums-set). The new term can exceed the sum of all previous terms, giving unique representations. The proximal-minimal existence theorem is a substantive input to this proof.

<h3 id="idempotent-ultrafilter-proof-of-hindman-s-theorem">Idempotent-ultrafilter proof of Hindman's theorem</h3>

↑ **Parent:** [Hindman theorem](#hindman-theorem)

Choose an [idempotent ultrafilter on the natural numbers](set-theory.md#idempotent-ultrafilter-on-the-natural-numbers) $\mathcal U$ and a color class $A\in\mathcal U$. The set

$$
A^*=\{x\in A:A-x\in\mathcal U\}
$$

also belongs to $\mathcal U$, and $A^*-x\in\mathcal U$ for every $x\in A^*$. Recursively choosing each new term from the finitely many required translates of $A^*$ puts every nonempty finite sum in $A$.

### Finite-sums set

↑ **Parent:** [Hindman theorem](#hindman-theorem)

For a sequence $(x_i)$, its finite-sums set is

$$
\operatorname{FS}(x_i)=\left\{\sum_{i\in F}x_i: \varnothing\ne F\subseteq\mathbb N\text{ finite}\right\}.
$$

#### Divisibility chain inside a finite-sums set

↑ **Parent:** [Finite-sums set](#finite-sums-set)

Every [finite-sums set](#finite-sums-set) generated by an infinite [sequence](real-analysis.md#sequence) of positive [integers](number-theory.md#integer) contains another [finite-sums set](#finite-sums-set) generated by a strictly increasing [sequence](real-analysis.md#sequence) $x_i$ satisfying $x_i\mid x_{i+1}$. Consequently the divisibility requirement can be added to the conclusion of [Hindman theorem](#hindman-theorem).

Choose each $x_i$ as a sum over a finite block of indices of the original [sequence](real-analysis.md#sequence), with these index blocks disjoint and successive. Given $x_i=m$, take two fresh groups of $m$ terms. In either group the $m+1$ [partial sums](real-analysis.md#partial-sum), including $0$, give two equal [congruence classes](number-theory.md#congruence-class) modulo $m$ by the [pigeonhole principle](algebra.md#pigeonhole-principle). Their difference is a nonempty consecutive sum divisible by $m$, and hence at least $m$. Add the two such sums to obtain $x_{i+1}\ge2m$ divisible by $m$. Its index block is the [union](set.md#set-union) of the two selected subblocks. Discard the rest of these groups and continue after them. Because the blocks are disjoint, every finite sum of the $x_i$ is a finite sum of distinct original terms. This proves both the [finite-sums set](#finite-sums-set) containment and the strictly increasing divisibility chain.

#### IP set

↑ **Parent:** [Finite-sums set](#finite-sums-set)

A subset $A$ of the [positive integers](number-theory.md#positive-integer) is an IP set if it contains a [finite-sums set](#finite-sums-set) generated by an infinite sequence of positive integers. Sums use distinct indices, although the generators themselves need not be distinct. An IP set is necessarily infinite, because its successive partial sums are unbounded. The [partition regularity of IP sets](#partition-regularity-of-ip-sets) is the relative form of the [Hindman theorem](#hindman-theorem) needed when applying that theorem inside an already specified IP set.

##### Alternating dyadic intervals contain disjoint IP sets

↑ **Parent:** [IP set](#ip-set)

Let $E$ be the union of integer intervals $[2^{2j},2^{2j+1})$ for $j\geq0$. Every nonempty sum of distinct $4^j$ has largest summand $4^J$ and lies in $[4^J,2\cdot4^J)$, since the sum of all smaller summands is $(4^J-1)/3$. Thus $\operatorname{FS}(4^j)\subseteq E$. Doubling gives $\operatorname{FS}(2\cdot4^j)\subseteq E^c$. Both sides are [IP sets](#ip-set). Each can be adjoined to the [IP-star filter](#ip-star-filter) while preserving the [finite intersection property](topology.md#finite-intersection-property), yielding two distinct [IP ultrafilters](set-theory.md#ultrafilter-with-finite-sums-members).

##### IP-star set

↑ **Parent:** [IP set](#ip-set)

An IP-star set meets every [IP set](#ip-set). Equivalently, its complement is not an [IP set](#ip-set): a disjoint IP set is precisely an IP subset of the complement. This is a condition on all infinite [finite-sums sets](#finite-sums-set), not merely on a single generating sequence.

###### IP-star filter

↑ **Parent:** [IP-star set](#ip-star-set)

The [IP-star sets](#ip-star-set) form a proper [filter on a set](set-theory.md#filter-set-theory) over the [positive integers](number-theory.md#positive-integer). Indeed, sets that are not [IP sets](#ip-set) are closed under taking subsets. They are also closed under finite unions, because the [partition regularity of IP sets](#partition-regularity-of-ip-sets) would otherwise put an IP set in one of the union's constituent sets. Taking complements gives upward closure and closure under finite intersections for the [IP-star sets](#ip-star-set). The full set belongs to this filter and the empty set does not.

##### Partition regularity of IP sets

↑ **Parent:** [IP set](#ip-set)

Every [finite coloring](#finite-coloring) of an [IP set](#ip-set) has a color class that is an [IP set](#ip-set). Here is a reduction to the ordinary [Hindman theorem](#hindman-theorem). Given $\operatorname{FS}(x_i)$ in the original set, color an integer $n>0$ by the color of $\sum_{i\in\operatorname{supp}_2(n)}x_i$, where the support consists of positions of its nonzero digits in the [binary expansion](arithmetic.md#binary-expansion). The [Hindman theorem](#hindman-theorem) produces $w_i>0$ with [monochromatic](#monochromatic-set) $\operatorname{FS}(w_i)$. Replace the $w_i$ by consecutive, disjoint finite block sums $v_j$ with separated binary supports: after a block has been chosen, take $K$ above all previously used positions; two of $2^K+1$ partial sums of a fresh tail agree modulo $2^K$, so their positive difference supplies the next block sum divisible by $2^K$. Now binary addition of distinct $v_j$ has no carries. Therefore $y_j=\sum_{i\in\operatorname{supp}_2(v_j)}x_i$ generates a [monochromatic](#monochromatic-set) [finite-sums set](#finite-sums-set) in the original IP set.

<h3 id="milliken-taylor-theorem">Milliken–Taylor theorem</h3>

↑ **Parent:** [Hindman theorem](#hindman-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Milliken–Taylor_theorem)

The Milliken–Taylor theorem gives monochromatic systems of separated block sums with a fixed compressed coefficient vector, such as $(1,2,3)$. Systems associated with two nonproportional compressed coefficient vectors need not have the same color: in particular, there is a finite coloring for which a [finite-sums set](#finite-sums-set) and the $(1,2,3)$ Milliken–Taylor system cannot be monochromatic together.

## Monochromatic sums-and-products obstruction

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

There is a [finite coloring](#finite-coloring) of the [positive integers](number-theory.md#positive-integer) for which no infinite set has all pairwise sums and pairwise products in one color. Refining this coloring by the parity of the [2-adic valuation](number-theory.md#2-adic-valuation) also prevents a constant infinite sequence from evading the obstruction.

## Euclidean Ramsey set

↑ **Parent:** [Ramsey theory](ramsey-theory.md)

A finite set $X\subseteq\mathbb R^d$ is Euclidean Ramsey when, for every number of colors, some finite-dimensional [Euclidean space](functional-analysis.md#euclidean-norm) has the property that every coloring of it contains a monochromatic [isometric copy](riemannian-geometry.md#isometry) of $X$.

### Spherical point set

↑ **Parent:** [Euclidean Ramsey set](#euclidean-ramsey-set)

A finite point set is spherical when it lies on a [sphere](geometry-and-topology.md#sphere). Every [Euclidean Ramsey set](#euclidean-ramsey-set) is spherical. Whether every finite spherical point set is Euclidean Ramsey is open.

### Product theorem for Euclidean Ramsey sets

↑ **Parent:** [Euclidean Ramsey set](#euclidean-ramsey-set)

If finite point sets $X$ and $Y$ are Euclidean Ramsey, then their orthogonal [Cartesian product](set-theory.md#cartesian-product) $X\times Y$ is Euclidean Ramsey. The proof first chooses a finite Ramsey witness for $X$, colors a witness for $Y$ by the complete color pattern it induces on the first witness, and then applies the two Ramsey properties in succession.

### Three-term unit arithmetic progression is not Euclidean Ramsey

↑ **Parent:** [Euclidean Ramsey set](#euclidean-ramsey-set)

The collinear set $\{0,1,2\}$ is not a [Euclidean Ramsey set](#euclidean-ramsey-set). In every dimension, coloring $x$ by $\lfloor2\|x\|^2\rfloor$ modulo ten prevents a monochromatic congruent copy; the [parallelogram law](linear-algebra.md#parallelogram-law) would force the corresponding three integer parts to have a second difference strictly between two and six, which cannot be divisible by ten.

### Triangle is a Euclidean Ramsey set

↑ **Parent:** [Euclidean Ramsey set](#euclidean-ramsey-set)

Every nondegenerate [triangle](geometry-and-topology.md#triangle) is a [Euclidean Ramsey set](#euclidean-ramsey-set).

### Line segment is a Euclidean Ramsey set

↑ **Parent:** [Euclidean Ramsey set](#euclidean-ramsey-set)

Every [line segment](mathematical-optimization.md#line-segment) is a [Euclidean Ramsey set](#euclidean-ramsey-set).

### Regular polygon is a Euclidean Ramsey set

↑ **Parent:** [Euclidean Ramsey set](#euclidean-ramsey-set)

Every [regular polygon](geometry-and-topology.md#regular-polygon) is a [Euclidean Ramsey set](#euclidean-ramsey-set). Its cyclic rotation acts transitively on the vertices, so this is a special case of the [Kriz theorem for cyclic transitive point sets](#kriz-theorem-for-cyclic-transitive-point-sets).

### Approximately Euclidean Ramsey set

↑ **Parent:** [Euclidean Ramsey set](#euclidean-ramsey-set)

A finite Euclidean set $X$ is approximately Ramsey if, for every number of colors and every $\varepsilon>0$, some finite set has a monochromatic subset whose corresponding pairwise distances differ from those of $X$ by less than $\varepsilon$.

### Edge Ramsey set

↑ **Parent:** [Euclidean Ramsey set](#euclidean-ramsey-set)

A finite Euclidean configuration is edge Ramsey when every finite edge coloring of a suitable finite Euclidean set contains a monochromatic isometric copy. The edge Ramsey configurations are exactly the equidistant sets, equivalently the vertex sets of regular simplices.

### Cyclic transitive point set

↑ **Parent:** [Euclidean Ramsey set](#euclidean-ramsey-set)

A finite point set is cyclic transitive when a cyclic group of [isometries](riemannian-geometry.md#isometry) acts transitively on it.

#### Kriz theorem for cyclic transitive point sets

↑ **Parent:** [Cyclic transitive point set](#cyclic-transitive-point-set)

Every finite [cyclic transitive point set](#cyclic-transitive-point-set) is a [Euclidean Ramsey set](#euclidean-ramsey-set). In particular every [regular polygon](geometry-and-topology.md#regular-polygon) is Euclidean Ramsey.

##### A-invariant coloring of a Cartesian power

↑ **Parent:** [Kriz theorem for cyclic transitive point sets](#kriz-theorem-for-cyclic-transitive-point-sets)

For $A\subseteq X$, a coloring of $X^n$ is $A$-invariant when changing any coordinates from one member of $A$ to another does not change the color. A product argument upgrades the existence of a copy of $X$ on which $A$ is monochromatic to an $A$-invariant copy of every finite Cartesian power $X^n$.

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
