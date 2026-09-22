# Set

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Set_(mathematics))

A set is a collection of distinct objects regarded as its elements.

**Table of contents**

- [Partition of a set](#partition-of-a-set)
  - [Colouring of a set](#colouring-of-a-set)
- [Coinfinite set](#coinfinite-set)
- [Dedekind-finite set](#dedekind-finite-set)
  - [Finite repetition-free sequences preserve Dedekind-finiteness](#finite-repetition-free-sequences-preserve-dedekind-finiteness)
  - [Infinite Dedekind-finite set](#infinite-dedekind-finite-set)
- [Set difference](#set-difference)
- [Complement of a set](#complement-of-a-set)
- [Pointed set](#pointed-set)
- [Multiset](#multiset)
- [Nondecreasing family of sets](#nondecreasing-family-of-sets)
- [Power set](#power-set)
  - [Cantor's theorem](#cantor-s-theorem)
- [Finite set](#finite-set)
- [Infinite set](#infinite-set)
- [Empty set](#empty-set)
- [Singleton (mathematics)](#singleton-mathematics)
- [Distinct elements](#distinct-elements)
- [Generating set](#generating-set)
- [Subset](#subset)
- [Set union](#set-union)
  - [Countable union](#countable-union)
- [Set intersection](#set-intersection)
  - [Countable intersection](#countable-intersection)
- [Symmetric difference](#symmetric-difference)
  - [Finite symmetric difference](#finite-symmetric-difference)
- [Pair](#pair)
  - [Ordered pair](#ordered-pair)
    - [Kuratowski ordered pair](#kuratowski-ordered-pair)
  - [Unordered pair](#unordered-pair)
- [Preorder](#preorder)
  - [Hoare domination preorder](#hoare-domination-preorder)
    - [Finite-subset lifting of a well-quasi-order](#finite-subset-lifting-of-a-well-quasi-order)
  - [Well-quasi-ordering](#well-quasi-ordering)
    - [Perfect subsequence lemma](#perfect-subsequence-lemma)
    - [Finite product closure of well-quasi-orderings](#finite-product-closure-of-well-quasi-orderings)
    - [Better-quasi-ordering](#better-quasi-ordering)
      - [Power-set closure of better-quasi-orderings](#power-set-closure-of-better-quasi-orderings)
      - [Continuous array in better-quasi-order theory](#continuous-array-in-better-quasi-order-theory)
      - [Barrier in better-quasi-order theory](#barrier-in-better-quasi-order-theory)
        - [Nash-Williams barrier partition theorem](#nash-williams-barrier-partition-theorem)
    - [Rado order](#rado-order)
      - [Bad barrier array for the Rado order](#bad-barrier-array-for-the-rado-order)
    - [Higman's lemma](#higman-s-lemma)
    - [Bad sequence](#bad-sequence)
      - [Minimal bad sequence](#minimal-bad-sequence)
    - [Finite bad-sequence tree](#finite-bad-sequence-tree)
    - [Kruskal's tree theorem](#kruskal-s-tree-theorem)
      - [Labelled version of Kruskal's tree theorem](#labelled-version-of-kruskal-s-tree-theorem)
      - [Friedman's finite form of Kruskal's theorem](#friedman-s-finite-form-of-kruskal-s-theorem)
- [Partially ordered set](#partially-ordered-set)
  - [Upper and lower sets](#upper-and-lower-sets)
  - [Greatest element and least element](#greatest-element-and-least-element)
    - [Greatest element](#greatest-element)
  - [Maximal and minimal elements](#maximal-and-minimal-elements)
    - [Maximal element of a partially ordered set](#maximal-element-of-a-partially-ordered-set)
    - [Minimal element of a partially ordered set](#minimal-element-of-a-partially-ordered-set)
  - [Upper and lower bounds](#upper-and-lower-bounds)
    - [Upper bound in a partially ordered set](#upper-bound-in-a-partially-ordered-set)
      - [Least upper bound in a partially ordered set](#least-upper-bound-in-a-partially-ordered-set)
  - [Increasing function on a partially ordered set](#increasing-function-on-a-partially-ordered-set)
  - [Szpilrajn extension theorem](#szpilrajn-extension-theorem)
  - [Dilworth's theorem](#dilworth-s-theorem)
  - [Lower bound in a partially ordered set](#lower-bound-in-a-partially-ordered-set)
    - [Greatest lower bound in a partially ordered set](#greatest-lower-bound-in-a-partially-ordered-set)
  - [Chain-complete partially ordered set](#chain-complete-partially-ordered-set)
  - [Complete partial order](#complete-partial-order)
    - [Directed-complete partial order](#directed-complete-partial-order)
      - [Scott continuous map](#scott-continuous-map)
      - [Pointed complete partial order](#pointed-complete-partial-order)
        - [Embedding-projection pair](#embedding-projection-pair)
          - [Inverse-limit solution of the reflexive domain equation](#inverse-limit-solution-of-the-reflexive-domain-equation)
        - [Function space of complete partial orders](#function-space-of-complete-partial-orders)
          - [Pointwise directed supremum](#pointwise-directed-supremum)
      - [Least fixed point from a directed family of maps](#least-fixed-point-from-a-directed-family-of-maps)
  - [Product order](#product-order)
    - [Maximal external point](#maximal-external-point)
      - [Expected number of coordinatewise maxima](#expected-number-of-coordinatewise-maxima)
  - [Strict partial order](#strict-partial-order)
    - [Reflexification of a strict partial order](#reflexification-of-a-strict-partial-order)
  - [Chain-poset nonembedding lemma](#chain-poset-nonembedding-lemma)
  - [Set-theoretic tree](#set-theoretic-tree)
    - [Branching form of the tree property](#branching-form-of-the-tree-property)
    - [Splitting tree](#splitting-tree)
    - [Tree with unique limits](#tree-with-unique-limits)
    - [Well-pruned set-theoretic tree](#well-pruned-set-theoretic-tree)
      - [Unbounded-extension kernel of a regular tree](#unbounded-extension-kernel-of-a-regular-tree)
    - [Kappa-tree](#kappa-tree)
      - [Tree property](#tree-property)
      - [Uniformly narrow regular-height tree branch theorem](#uniformly-narrow-regular-height-tree-branch-theorem)
    - [Kurepa tree](#kurepa-tree)
      - [Kurepa tree from an inaccessible binary tree](#kurepa-tree-from-an-inaccessible-binary-tree)
      - [Kurepa hypothesis](#kurepa-hypothesis)
      - [Kurepa-family hypothesis](#kurepa-family-hypothesis)
    - [Aronszajn tree](#aronszajn-tree)
      - [Coherent-injection Aronszajn tree](#coherent-injection-aronszajn-tree)
      - [Suslin tree](#suslin-tree)
        - [Suslin-tree obstruction to Martin's axiom](#suslin-tree-obstruction-to-martin-s-axiom)
      - [Special Aronszajn tree](#special-aronszajn-tree)
        - [Rationally labelled Aronszajn tree construction](#rationally-labelled-aronszajn-tree-construction)
          - [Bounded rational extension property](#bounded-rational-extension-property)
      - [Aleph-two Aronszajn tree](#aleph-two-aronszajn-tree)
    - [Normal set-theoretic tree](#normal-set-theoretic-tree)
    - [Cofinal branch](#cofinal-branch)
    - [Tree antichain](#tree-antichain)
  - [Chain in a partial order](#chain-in-a-partial-order)
  - [Differential poset](#differential-poset)
    - [Normal ordering identity for up and down operators](#normal-ordering-identity-for-up-and-down-operators)
  - [Filter (mathematics)](#filter-mathematics)
    - [Principal filter in an ordered set](#principal-filter-in-an-ordered-set)
  - [Linear extension](#linear-extension)
    - [Reduced adjacent-swap path between linear extensions](#reduced-adjacent-swap-path-between-linear-extensions)
  - [Order-preserving function](#order-preserving-function)
    - [Inflationary map](#inflationary-map)
    - [Strict order-preserving function](#strict-order-preserving-function)
  - [Order dimension](#order-dimension)
    - [Two-dimensional partially ordered set](#two-dimensional-partially-ordered-set)
      - [Finite-local characterization of two-dimensional partially ordered sets](#finite-local-characterization-of-two-dimensional-partially-ordered-sets)
  - [Chain in a partially ordered set](#chain-in-a-partially-ordered-set)
  - [Directed set](#directed-set)
- [Total order](#total-order)
  - [Minimum of a subset of a total order](#minimum-of-a-subset-of-a-total-order)
  - [Maximum of a subset of a total order](#maximum-of-a-subset-of-a-total-order)
  - [Totally ordered set](#totally-ordered-set)
  - [Dense order](#dense-order)
  - [Aleph-one-like linear order](#aleph-one-like-linear-order)
    - [Stationary encoding in an aleph-one-like dense order](#stationary-encoding-in-an-aleph-one-like-dense-order)
  - [Order topology](#order-topology)
    - [Lexicographic order topology on the real plane](#lexicographic-order-topology-on-the-real-plane)
  - [Countable chain condition for a linear order](#countable-chain-condition-for-a-linear-order)
  - [Order-dense subset](#order-dense-subset)
  - [Order completeness](#order-completeness)
    - [Dedekind completion](#dedekind-completion)
  - [Order isomorphism](#order-isomorphism)
  - [Order sum](#order-sum)
  - [Order automorphism](#order-automorphism)
    - [Rigid dense subset of the real line](#rigid-dense-subset-of-the-real-line)
    - [Extension of an order automorphism from a dense subset](#extension-of-an-order-automorphism-from-a-dense-subset)
  - [Strict total order](#strict-total-order)
  - [Well-order](#well-order)
    - [Decidable well-order](#decidable-well-order)
  - [Empty order](#empty-order)
  - [Initial segment](#initial-segment)

## Partition of a set

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partition_of_a_set)

A partition of a [set](set.md) $X$ is a family of pairwise disjoint nonempty [subsets](#subset) whose [union](#set-union) is $X$. Every [equivalence relation](set-theory.md#equivalence-relation) defines a partition into [equivalence classes](set-theory.md#equivalence-class), and conversely belonging to the same cell of a partition defines an [equivalence relation](set-theory.md#equivalence-relation). The nonempty [colour classes](ramsey-theory.md#colour-class) of a [finite colouring](ramsey-theory.md#finite-coloring) form a finite partition.

### Colouring of a set

↑ **Parent:** [Partition of a set](#partition-of-a-set)

A colouring assigns to each member of a [set](set.md) $X$ a colour in another set $C$. Its nonempty fibres form a [partition of a set](#partition-of-a-set). The colour set may be infinite; a [finite colouring](ramsey-theory.md#finite-coloring) is the special case with finitely many colours. A [homogeneous set for a colouring](ramsey-theory.md#homogeneous-set-for-a-colouring) of finite subsets has all its subsets of the specified size assigned one colour.

## Coinfinite set

↑ **Parent:** [Set](set.md)

A [subset](#subset) $A$ of a specified ambient [set](set.md) $X$ is coinfinite if its [complement of a set](#complement-of-a-set) $X\setminus A$ is infinite. In $\mathbb N$, the even numbers are both infinite and coinfinite, whereas a [cofinite set](set-theory.md#cofinite-set) is not coinfinite.

## Dedekind-finite set

↑ **Parent:** [Set](set.md)

A [set](set.md) $X$ is Dedekind-finite when no [injective function](algebra.md#injective-function) $\mathbb N\to X$ exists. In classical [Zermelo–Fraenkel set theory](set-theory.md#zermelo-fraenkel-set-theory) this is equivalent to $X$ not being in [bijection](function.md#bijection) with a proper subset: an injective non-surjective self-map generates distinct iterates from an element outside its image, and a countably infinite subset permits a shift fixing its complement. A [finite set](#finite-set) is Dedekind-finite. Without the [axiom of choice](set-theory.md#axiom-of-choice), some [infinite sets](#infinite-set) can also be Dedekind-finite.

### Finite repetition-free sequences preserve Dedekind-finiteness

↑ **Parent:** [Dedekind-finite set](#dedekind-finite-set)

If $X$ is a [Dedekind-finite set](#dedekind-finite-set), its [set](set.md) of [finite repetition-free sequences](real-analysis.md#finite-repetition-free-sequence) is also Dedekind-finite. An injective [sequence](real-analysis.md#sequence) of distinct finite lists would, by [countable union of explicitly ordered finite lists without choice](set-theory.md#countable-union-of-explicitly-ordered-finite-lists-without-choice), either produce an injection $\mathbb N\to X$ or use only finitely many entries. The latter possibility is impossible because a fixed finite pool supports only finitely many repetition-free lists. If $X$ is infinite, the one-entry lists also show that the resulting [set](set.md) is infinite.

### Infinite Dedekind-finite set

↑ **Parent:** [Dedekind-finite set](#dedekind-finite-set)

An [infinite Dedekind-finite set](#infinite-dedekind-finite-set) is an [infinite set](#infinite-set) with no [subset](#subset) that is a [countably infinite set](set-theory.md#countably-infinite-set). The name Dedekind [set](set.md) is sometimes used for this combination of properties. Under the [axiom of choice](set-theory.md#axiom-of-choice) no such [set](set.md) exists; results about these [sets](set.md) must avoid obtaining arbitrary enumerations of finite subsets by unstated choices.

## Set difference

↑ **Parent:** [Set](set.md)

The difference consists of the elements of $A$ not belonging to $B$. In [ZF](set-theory.md#zermelo-fraenkel-set-theory) it exists by [axiom schema of separation](set-theory.md#axiom-schema-of-specification). It gives complements relative to a fixed tuple domain in [finite relation closure for set-theoretic coding](definable-power-set.md#finite-relation-closure-for-set-theoretic-coding).

## Complement of a set

↑ **Parent:** [Set](set.md)

## Pointed set

↑ **Parent:** [Set](set.md)

A pointed set is a [set](set.md) $X$ with a distinguished element $x_0\in X$. A morphism of pointed sets is a [function](function.md) carrying the distinguished element to the distinguished element. The resulting [category of pointed sets](category.md#category-of-pointed-sets) has every singleton as a [zero object](category.md#zero-object).

## Multiset

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiset)

A multiset records a nonnegative integer multiplicity for each element of a [set](set.md). A finite multiset has finite support and finite total multiplicity. Its [cardinality](set-theory.md#cardinality) is the sum of its multiplicities; its disjoint union with another multiset adds multiplicities. The [hook lengths](representation-theory-of-the-symmetric-group.md#hook-length) of a [Young diagram](representation-theory-of-the-symmetric-group.md#young-diagram) form a multiset, since different cells can have equal lengths.

## Nondecreasing family of sets

↑ **Parent:** [Set](set.md)

A family of sets $(A_t)$ indexed by an [partially ordered set](#partially-ordered-set) is nondecreasing when

$$
s\leq t\quad\Longrightarrow\quad A_s\subseteq A_t.
$$

## Power set

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Power_set)

The power set $\mathcal P(X)$ is the set of all subsets of $X$.

<h3 id="cantor-s-theorem">Cantor's theorem</h3>

↑ **Parent:** [Power set](#power-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cantor's_theorem)

There is no surjection from a set $X$ onto its [power set](#power-set) $\mathcal P(X)$. Consequently $\mathcal P(X)$ has strictly greater cardinality than $X$.

## Finite set

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_set)

A finite set is a [set](set.md) with finitely many elements.

## Infinite set

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Infinite_set)

An infinite set is a [set](set.md) with infinitely many elements. Equivalently, assuming the [axiom of choice](set-theory.md#axiom-of-choice), it contains a [countably infinite set](set-theory.md#countably-infinite-set).

## Empty set

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Empty_set)

The empty set has no elements.

## Singleton (mathematics)

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singleton_(mathematics))

A singleton set has exactly one element.

## Distinct elements

↑ **Parent:** [Set](set.md)

Elements are distinct when they are unequal.

## Generating set

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generating_set)

A generating set is a subset from which every element of a structure can be obtained using the structure's operations.

## Subset

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subset)

A set $A$ is a subset of $B$ when every element of $A$ belongs to $B$.

## Set union

↑ **Parent:** [Set](set.md)

The union $\bigcup_{i\in I}A_i$ contains exactly the elements that belong to at least one set $A_i$.

### Countable union

↑ **Parent:** [Set union](#set-union)

The [union](#set-union) of a sequence of sets: an element belongs to it exactly when it belongs to at least one $A_n$.

## Set intersection

↑ **Parent:** [Set](set.md)

The intersection $\bigcap_{i\in I}A_i$ contains exactly the elements that belong to every set $A_i$.

### Countable intersection

↑ **Parent:** [Set intersection](#set-intersection)

The countable intersection of a [sequence](real-analysis.md#sequence) of [sets](set.md) contains exactly the elements belonging to every set. [De Morgan's laws](computer-science.md#de-morgan-s-laws) identify its [relative complement](#set-difference) with the union of their complements.

## Symmetric difference

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_difference)

The symmetric difference $A\mathbin\triangle B=(A\setminus B)\cup(B\setminus A)$ contains the elements belonging to exactly one of the two [sets](set.md).

### Finite symmetric difference

↑ **Parent:** [Symmetric difference](#symmetric-difference)

Two [sets](set.md) differ by finite symmetric difference when only finitely many points belong to exactly one of them. This is an [equivalence relation](set-theory.md#equivalence-relation), since $A\mathbin\triangle C\subseteq(A\mathbin\triangle B)\cup(B\mathbin\triangle C)$.

## Pair

↑ **Parent:** [Set](set.md)

A pair is a collection of two objects. An ordered pair records which object is first, whereas an unordered pair does not.

An [ordered pair](#ordered-pair) is a pair with distinguished first and second positions; an unordered pair does not record those positions.

### Ordered pair

↑ **Parent:** [Pair](#pair)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordered_pair)

#### Kuratowski ordered pair

↑ **Parent:** [Ordered pair](#ordered-pair)

This representation of an [ordered pair](#ordered-pair) by [sets](set.md) satisfies $\langle a,b\rangle=\langle c,d\rangle$ exactly when $a=c$ and $b=d$. Its intersection recovers $\{a\}$, and its union recovers $\{a,b\}$; if the latter is a singleton then $b=a$. Its [rank of a set](set-theory.md#rank-of-a-set) is $\max(\operatorname{rank}(a),\operatorname{rank}(b))+2$, which bounds the ranks of [function](function.md) graphs in [absoluteness of cardinalhood in limit ranks](set-theory.md#absoluteness-of-cardinalhood-in-limit-ranks).

### Unordered pair

↑ **Parent:** [Pair](#pair)

## Preorder

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Preorder)

A preorder is a set equipped with a reflexive and transitive relation; unlike a partial order, distinct elements may be mutually comparable in both directions.

### Hoare domination preorder

↑ **Parent:** [Preorder](#preorder)

For subsets of a [preorder](#preorder), Hoare domination means every source element has some greater or equal target element: $S\le_H T\iff\forall s\in S\;\exists t\in T\;(s\le t)$. It is reflexive and transitive. If the base is a [well-quasi-ordering](#well-quasi-ordering), its finite subsets are [well-quasi-ordered](#well-quasi-ordering) by this relation; arbitrary subsets need not be, as the [Rado order](#rado-order) shows.

#### Finite-subset lifting of a well-quasi-order

↑ **Parent:** [Hoare domination preorder](#hoare-domination-preorder)

Finite subsets of a [well-quasi-ordering](#well-quasi-ordering), compared by [Hoare domination preorder](#hoare-domination-preorder), form a [well-quasi-ordering](#well-quasi-ordering). Enumerate each finite subset as a [word](foundations-of-mathematics.md#string) and apply [Higman lemma](#higman-s-lemma): a subsequence embedding with increased letters supplies a domination witness for every source element. This does not assert the same result for the full [power set](#power-set).

### Well-quasi-ordering

↑ **Parent:** [Preorder](#preorder)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Well-quasi-ordering)

A [preorder](#preorder) is a [well-quasi-ordering](#well-quasi-ordering) if every infinite [sequence](real-analysis.md#sequence) has indices $i<j$ with $x_i\leq x_j$. An infinite [sequence](real-analysis.md#sequence) with no such pair is a bad [sequence](real-analysis.md#sequence). This formulation handles combinatorial embedding relations that need not be antisymmetric on syntactic codes.

#### Perfect subsequence lemma

↑ **Parent:** [Well-quasi-ordering](#well-quasi-ordering)

Every infinite [sequence](real-analysis.md#sequence) in a [well-quasi-ordering](#well-quasi-ordering) has an infinite [subsequence](real-analysis.md#subsequence) all of whose earlier terms precede its later terms. Some term must have infinitely many later terms above it: otherwise choose each new index outside the finitely many upper-cone index [sets](set.md) of the terms already chosen, producing a [bad sequence](#bad-sequence). Apply the same observation successively inside the infinite upper-cone [subsequence](real-analysis.md#subsequence). Each restriction preserves all earlier inequalities, proving the assertion.

#### Finite product closure of well-quasi-orderings

↑ **Parent:** [Well-quasi-ordering](#well-quasi-ordering)

A finite [Cartesian product](set-theory.md#cartesian-product) of [well-quasi-orderings](#well-quasi-ordering) is well-quasi-ordered in the componentwise order. Every infinite sequence in one well-quasi-order has an infinite nondecreasing subsequence: colour pairs by whether they are ordered, apply [Ramsey's theorem](ramsey-theory.md#ramsey-s-theorem), and exclude an all-bad subsequence. Restrict successively to such a subsequence in each coordinate. The same argument, or the infinite pigeonhole principle, proves closure under finite disjoint unions with no cross-component comparisons.

#### Better-quasi-ordering

↑ **Parent:** [Well-quasi-ordering](#well-quasi-ordering)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Better-quasi-ordering)

A quasi-order is better-quasi-ordered if every array into it from every [barrier in better-quasi-order theory](#barrier-in-better-quasi-order-theory) is good: some barrier members $s\triangleleft t$ satisfy $f(s)\le f(t)$. Singleton barriers recover the usual infinite-sequence condition for a [well-quasi-ordering](#well-quasi-ordering). The stronger condition is useful for infinitary closure operations for which well-quasi-ordering alone fails. Equivalently one may use continuous maps from infinite subsets of an infinite subset of the natural numbers, with the discrete topology on the range, and compare $X$ with $X\setminus\{\min X\}$.

##### Power-set closure of better-quasi-orderings

↑ **Parent:** [Better-quasi-ordering](#better-quasi-ordering)

If $Q$ is a [better-quasi-ordering](#better-quasi-ordering), its full [power set](#power-set) is better-quasi-ordered by the [Hoare domination preorder](#hoare-domination-preorder). A bad continuous array of subsets would allow a choice of $q_X\in A_X$ not below any member of $A_{X^-}$, where $X^-$ deletes the least element. Choose this witness as a fixed function of the two locally constant subsets. Then $X\mapsto q_X$ is a bad [continuous array in better-quasi-order theory](#continuous-array-in-better-quasi-order-theory) into $Q$, a contradiction. Empty source subsets cannot occur in a bad array because they precede every subset.

##### Continuous array in better-quasi-order theory

↑ **Parent:** [Better-quasi-ordering](#better-quasi-ordering)

A continuous array takes infinite subsets of an infinite $A\subseteq\omega$, in the [ordinary topology on infinite subsets](ramsey-theory.md#ordinary-topology-on-infinite-subsets), to a discrete [preorder](#preorder) $Q$. It is bad if $F(X)\not\leq F(X\setminus\{\min X\})$ for every infinite $X$. A [barrier in better-quasi-order theory](#barrier-in-better-quasi-order-theory) array induces such a continuous array by evaluating its unique barrier initial segment. The continuous-array and barrier formulations of [better-quasi-ordering](#better-quasi-ordering) are equivalent, using refinement of fronts to barriers in the reverse direction.

##### Barrier in better-quasi-order theory

↑ **Parent:** [Better-quasi-ordering](#better-quasi-ordering)

A barrier on an infinite $A\subseteq\mathbb N$ is a family of nonempty finite increasing sequences, viewed as finite subsets, no one contained properly in another, such that every infinite subset of $A$ has a member of the family as an initial segment. Write $s\triangleleft t$ if there is a finite increasing sequence $u$ of which $s$ is an initial segment and of which $t$ is an initial segment after its first term is deleted. This shift relation underlies the good-array definition of [better-quasi-ordering](#better-quasi-ordering).

###### Nash-Williams barrier partition theorem

↑ **Parent:** [Barrier in better-quasi-order theory](#barrier-in-better-quasi-order-theory)

Every finite coloring of a [barrier in better-quasi-order theory](#barrier-in-better-quasi-order-theory) has an infinite restriction on which all barrier members have the same color. It extends finite-dimensional [Ramsey's theorem](ramsey-theory.md#ramsey-s-theorem) from fixed-length subsets to variable-length initial segments. A proof proceeds by well-founded induction on the initial-segment tree and a fusion construction selecting successively nested infinite tails. It implies that every finite [set](set.md) with the equality order is a [better-quasi-ordering](#better-quasi-ordering). The barrier/front partition proof is given in Section 3.2 of [https://arxiv.org/pdf/1604.05866](https://arxiv.org/pdf/1604.05866) .

#### Rado order

↑ **Parent:** [Well-quasi-ordering](#well-quasi-ordering)

The Rado order has domain $R=\{(m,n)\in\mathbb N^2:m<n\}$ and $(m,n)\le_R(k,l)$ iff either $m=k$ and $n\le l$, or $n<k$. It is a [well-quasi-ordering](#well-quasi-ordering): either one row recurs infinitely in a [sequence](real-analysis.md#sequence), or the first coordinates are unbounded and yield a cross-row comparison. Its infinite rows form an infinite [antichain](extremal-set-theory.md#antichain) under [Hoare domination preorder](#hoare-domination-preorder), showing that arbitrary-subset lifting need not preserve [well-quasi-ordering](#well-quasi-ordering).

##### Bad barrier array for the Rado order

↑ **Parent:** [Rado order](#rado-order)

The [barrier in better-quasi-order theory](#barrier-in-better-quasi-order-theory) $[\omega]^2$ has shifts $\{m,n\}\triangleleft\{n,l\}$ for $m<n<l$. Map each pair to the corresponding element of the [Rado order](#rado-order). Neither clause of $(m,n)\le_R(n,l)$ holds: the first coordinates differ, and the second coordinate of the first pair equals, rather than precedes, the first coordinate of the second. Thus this array is bad, although the [Rado order](#rado-order) is a [well-quasi-ordering](#well-quasi-ordering). It separates [better-quasi-ordering](#better-quasi-ordering) from [well-quasi-ordering](#well-quasi-ordering).

<h4 id="higman-s-lemma">Higman's lemma</h4>

↑ **Parent:** [Well-quasi-ordering](#well-quasi-ordering)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Higman's_lemma)

If $Q$ is a [well-quasi-ordering](#well-quasi-ordering), its finite [words](foundations-of-mathematics.md#string) form a [well-quasi-ordering](#well-quasi-ordering) under subsequence embedding with coordinatewise increase of letters. A [minimal bad sequence](#minimal-bad-sequence) proof removes the last letter of selected [words](foundations-of-mathematics.md#string) whose last letters form a nondecreasing [subsequence](real-analysis.md#subsequence), then contradicts minimality. The result implies [finite-subset lifting of a well-quasi-order](#finite-subset-lifting-of-a-well-quasi-order) under [Hoare domination preorder](#hoare-domination-preorder).

#### Bad sequence

↑ **Parent:** [Well-quasi-ordering](#well-quasi-ordering)

A bad sequence in a [preorder](#preorder) is an infinite [sequence](real-analysis.md#sequence) with no indices $i<j$ satisfying $x_i\le x_j$. A [preorder](#preorder) is a [well-quasi-ordering](#well-quasi-ordering) precisely when no such sequence exists.

##### Minimal bad sequence

↑ **Parent:** [Bad sequence](#bad-sequence)

A minimal bad sequence chooses each successive object of least possible natural-number size among choices that admit an infinite bad continuation of the already fixed prefix. Replacing its next object by a strictly smaller one cannot leave a [bad sequence](#bad-sequence). This contradiction principle proves [Higman lemma](#higman-s-lemma) and the [labelled version of Kruskal's tree theorem](#labelled-version-of-kruskal-s-tree-theorem).

#### Finite bad-sequence tree

↑ **Parent:** [Well-quasi-ordering](#well-quasi-ordering)

Given a size bound with finitely many possible objects at each position, put finite bad [sequences](real-analysis.md#sequence) in a tree ordered by extension. The tree is finitely branching. Arbitrarily long bad [sequences](real-analysis.md#sequence) would give an infinite bad [sequence](real-analysis.md#sequence) by [König infinity lemma](combinatorics.md#konig-s-lemma). This compactness argument converts an infinite [well-quasi-ordering](#well-quasi-ordering) theorem into a uniform finite length bound.

<h4 id="kruskal-s-tree-theorem">Kruskal's tree theorem</h4>

↑ **Parent:** [Well-quasi-ordering](#well-quasi-ordering)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kruskal's_tree_theorem)

Finite [rooted trees](combinatorics.md#rooted-tree) are [well-quasi-ordered](#well-quasi-ordering) by [rooted-tree homeomorphic embedding](combinatorics.md#homeomorphic-embedding-of-a-rooted-tree). Consequently every infinite [sequence](real-analysis.md#sequence) contains an earlier tree embedding into a later one. Size-controlled finite forms follow by applying [König infinity lemma](combinatorics.md#konig-s-lemma) to the finitely branching tree of bad prefixes.

<h5 id="labelled-version-of-kruskal-s-tree-theorem">Labelled version of Kruskal's tree theorem</h5>

↑ **Parent:** [Kruskal's tree theorem](#kruskal-s-tree-theorem)

Finite [rooted trees](combinatorics.md#rooted-tree) labelled in a [well-quasi-ordering](#well-quasi-ordering) are a [well-quasi-ordering](#well-quasi-ordering) under [label-monotone tree embedding](combinatorics.md#label-monotone-tree-embedding). A [minimal bad sequence](#minimal-bad-sequence) argument makes the collection of proper rooted subtrees a [well-quasi-ordering](#well-quasi-ordering); [Higman lemma](#higman-s-lemma) then compares their child lists while the root labels are compared in the label order.

<h5 id="friedman-s-finite-form-of-kruskal-s-theorem">Friedman's finite form of Kruskal's theorem</h5>

↑ **Parent:** [Kruskal's tree theorem](#kruskal-s-tree-theorem)

For every natural parameter $k$, there is a finite length $N$ such that every [sequence](real-analysis.md#sequence) of $N$ finite [rooted trees](combinatorics.md#rooted-tree) satisfying $|T_i|\leq k+i$ has an earlier tree homeomorphically embedding into a later tree. It is a true finite-combinatorial principle unprovable in [Peano arithmetic](mathematical-logic.md#peano-arithmetic) and in [arithmetical transfinite recursion theory](mathematical-logic.md#arithmetical-transfinite-recursion-theory). Each fixed-parameter instance can still be verified by a sufficiently large finite search.

## Partially ordered set

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partially_ordered_set)

A partially ordered set, or poset, is a set equipped with a reflexive, antisymmetric and transitive binary relation.

### Upper and lower sets

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Upper_and_lower_sets)

In a [partially ordered set](#partially-ordered-set) $P$, an upper [set](set.md) $U$ satisfies $x\in U$ and $x\leq y\Rightarrow y\in U$; a lower [set](set.md) $L$ satisfies $x\in L$ and $y\leq x\Rightarrow y\in L$. The [complement of a set](#complement-of-a-set) exchanges the two conditions: if $x\notin U$ and $y\leq x$, then $y\in U$ would force $x\in U$, so $P\setminus U$ is lower. In a [Boolean lattice](extremal-set-theory.md#boolean-lattice) ordered by inclusion, these are the [up-set](extremal-set-theory.md#up-set) and [down-set](extremal-set-theory.md#down-set) conditions.

### Greatest element and least element

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Greatest_element_and_least_element)

A greatest element lies above every member of an ordered set, and a least element lies below every member. Antisymmetry makes either unique if it exists. A greatest element is maximal, but a maximal element need not be greatest.

#### Greatest element

↑ **Parent:** [Greatest element and least element](#greatest-element-and-least-element)

An element is greatest when every element of the ordered set is less than or equal to it.

### Maximal and minimal elements

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximal_and_minimal_elements)

A maximal element has no strictly greater element; a minimal element has no strictly smaller one. Either can be nonunique, unlike a greatest or least element. These notions are defined for arbitrary [partially ordered sets](#partially-ordered-set).

#### Maximal element of a partially ordered set

↑ **Parent:** [Maximal and minimal elements](#maximal-and-minimal-elements)

An element $m$ of a partially ordered set is maximal when $m\leq x$ implies $x=m$. A poset can have several maximal elements and need not have a greatest element.

#### Minimal element of a partially ordered set

↑ **Parent:** [Maximal and minimal elements](#maximal-and-minimal-elements)

An element $m$ of a partially ordered set is minimal when $x\leq m$ implies $x=m$.

### Upper and lower bounds

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Upper_and_lower_bounds)

An upper bound of a subset is an element above every member, and a [lower bound](#lower-bound-in-a-partially-ordered-set) is below every member. They need not lie in the subset or be unique. [Infimum and supremum](real-analysis.md#infimum-and-supremum) are the greatest lower and least upper bounds when those exist.

#### Upper bound in a partially ordered set

↑ **Parent:** [Upper and lower bounds](#upper-and-lower-bounds)

An upper bound of a subset $A$ of a [partially ordered set](#partially-ordered-set) is an element $u$ satisfying $a\leq u$ for every $a\in A$.

##### Least upper bound in a partially ordered set

↑ **Parent:** [Upper bound in a partially ordered set](#upper-bound-in-a-partially-ordered-set)

The least [upper bound in a partially ordered set](#upper-bound-in-a-partially-ordered-set) of a subset $A$, when it exists. It bounds every element of $A$ and is at most every other upper bound. For two elements it is written $x\vee y$; an empty join is a least element.

### Increasing function on a partially ordered set

↑ **Parent:** [Partially ordered set](#partially-ordered-set)

A real-valued function on a [partially ordered set](#partially-ordered-set) is increasing when it preserves its order. Indicators of [increasing events](probability-inequality.md#increasing-event) are examples. In spin or edge configuration spaces the order is coordinatewise, so increasing observables grow when a zero coordinate is replaced by one. [Positive association of random variables](probability-theory.md#positive-association-of-random-variables) concerns pairs of such observables, and [stochastic domination](probability-and-statistics.md#stochastic-domination-of-probability-measures) compares their expectations.

### Szpilrajn extension theorem

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Szpilrajn_extension_theorem)

Every [partial order](#partially-ordered-set) has a [total order](#total-order) extension. Apply [Zorn's lemma](set-theory.md#zorn-s-lemma) to extensions ordered by inclusion: the union of a chain is a [partial order](#partially-ordered-set). If a maximal extension leaves two elements incomparable, adjoining one comparison and taking its [transitive closure of a relation](set-theory.md#transitive-closure-relation) creates no cycle, contradicting maximality. Quotienting a [preorder](#preorder) by its [indifference relation](set-theory.md#indifference-relation) and lifting a [total order](#total-order) gives a complete weak-order extension preserving its strict part.

<h3 id="dilworth-s-theorem">Dilworth's theorem</h3>

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dilworth's_theorem)

Every finite [partially ordered set](#partially-ordered-set) can be partitioned into as many [chains in a partial order](#chain-in-a-partial-order) as its largest [antichain](extremal-set-theory.md#antichain). Reachability in an acyclic [directed graph](graph-theory.md#directed-graph) is a [partial order](#partially-ordered-set), so the theorem supplies chains which can be expanded into directed paths, possibly overlapping at intervening vertices.

### Lower bound in a partially ordered set

↑ **Parent:** [Partially ordered set](#partially-ordered-set)

A [lower bound](#lower-bound-in-a-partially-ordered-set) of a subset $S$ of a [partially ordered set](#partially-ordered-set) is an element $\ell$ no greater than every member of $S$. For minimization, a number below every feasible objective value is therefore a [lower bound](#lower-bound-in-a-partially-ordered-set) on the optimum; a relaxation often provides such a certificate.

// Target: mathematical-optimization.bigb

#### Greatest lower bound in a partially ordered set

↑ **Parent:** [Lower bound in a partially ordered set](#lower-bound-in-a-partially-ordered-set)

A [lower bound in a partially ordered set](#lower-bound-in-a-partially-ordered-set) which is greater than or equal to every other lower bound. For a pair it is written $a\wedge b$; an empty meet, when it exists, is the greatest element. In a [complete lattice](mathematical-logic.md#complete-lattice), every subset has a meet. In the [open-set frame](category-theory.md#open-set-frame), this is the interior of the intersection, with finite meets given by the intersections themselves.

### Chain-complete partially ordered set

↑ **Parent:** [Partially ordered set](#partially-ordered-set)

A chain-complete [partially ordered set](#partially-ordered-set) has a supremum for every chain, with the empty-chain condition requiring a least element if empty chains are included. This implies the weaker upper-bound hypothesis of [Zorn lemma](set-theory.md#zorn-s-lemma), which requires only that each chain have some upper bound, not necessarily a least one. Some treatments use “chain-complete” for that weaker condition, so the convention should be specified. In the inclusion order on [lattice ideals](mathematical-logic.md#lattice-ideal) avoiding a specified element, the union of a nonempty chain is an ideal and is its supremum. This union observation is the step needed to apply Zorn in prime-ideal separation arguments.

### Complete partial order

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_partial_order)

A family of order-completeness notions used in semantics: in particular, a [directed-complete partial order](#directed-complete-partial-order) has every directed [join](#least-upper-bound-in-a-partially-ordered-set), while a pointed one additionally has a least element. The precise completeness condition should be specified, since this terminology is not synonymous with [complete lattice](mathematical-logic.md#complete-lattice).

#### Directed-complete partial order

↑ **Parent:** [Complete partial order](#complete-partial-order)

A [partially ordered set](#partially-ordered-set) is directed-complete if every [directed set](#directed-set) in it has a [least upper bound](#least-upper-bound-in-a-partially-ordered-set). A [complete lattice](mathematical-logic.md#complete-lattice) is directed-complete. Conversely, directed completeness together with all finite [joins](#least-upper-bound-in-a-partially-ordered-set), including the empty join, gives arbitrary [joins](#least-upper-bound-in-a-partially-ordered-set): take the [directed set](#directed-set) of joins of finite subsets.

##### Scott continuous map

↑ **Parent:** [Directed-complete partial order](#directed-complete-partial-order)

A monotone map preserving suprema of nonempty [directed sets](#directed-set). Between pointed domains it need not send bottom to bottom. The pointwise directed supremum of a directed family of such maps is again Scott continuous: interchange the two directed suprema in $\sup_f\sup_{x\in A}f(x)$.

##### Pointed complete partial order

↑ **Parent:** [Directed-complete partial order](#directed-complete-partial-order)

A [directed-complete partial order](#directed-complete-partial-order) with a least element. Here directed suprema concern nonempty directed sets. Morphisms are [Scott continuous maps](#scott-continuous-map) and need not preserve the least element. Requiring strictness would change the category and its cartesian-closure argument.

###### Embedding-projection pair

↑ **Parent:** [Pointed complete partial order](#pointed-complete-partial-order)

For [Scott continuous maps](#scott-continuous-map) $e:D\to E$, $p:E\to D$, these two identities say that $D$ is embedded in $E$ and that projection followed by embedding approximates from below. Such pairs lift to endomorphism spaces by $f\mapsto efp$ and $g\mapsto pge$. Their composite on the smaller space is the identity, and the other composite is $g\mapsto(ep)g(ep)\leq g$.

###### Inverse-limit solution of the reflexive domain equation

↑ **Parent:** [Embedding-projection pair](#embedding-projection-pair)

For $D_{n+1}=[D_n\to D_n]$ with recursively lifted [embedding-projection pairs](#embedding-projection-pair), form coherent sequences $x_n=p_nx_{n+1}$, ordered componentwise. Stage projections $P_n$ and embeddings $E_n$ satisfy $P_nE_n=\operatorname{id}$, $E_nP_n\uparrow\operatorname{id}$. A coherent family $f_n\in[D_n\to D_n]$ induces $f=\sup_nE_nf_nP_n$; conversely $f_n=P_nfE_n$. These constructions are inverse. Removing the initial coordinate of the coherent sequence identifies this function-space limit with the original domain limit.

###### Function space of complete partial orders

↑ **Parent:** [Pointed complete partial order](#pointed-complete-partial-order)

The [Scott continuous maps](#scott-continuous-map) from $D$ to $E$, ordered pointwise. A nonempty directed family has pointwise supremum, and the constant-bottom function is least. Joint evaluation is Scott continuous: for a directed family of pairs $(f_i,x_i)$, directedness makes diagonal values cofinal among all $f_i(x_j)$. Evaluation and [currying](category.md#currying) make the category of pointed complete partial orders and non-strict Scott continuous maps a [Cartesian closed category](category.md#cartesian-closed-category).

###### Pointwise directed supremum

↑ **Parent:** [Function space of complete partial orders](#function-space-of-complete-partial-orders)

For a [directed set](#directed-set) of [Scott continuous maps](#scott-continuous-map) $f_i:D\to E$, its [least upper bound](#least-upper-bound-in-a-partially-ordered-set) is $f(x)=\sup_i f_i(x)$. The two directed suprema over $i$ and over inputs commute, proving that $f$ remains Scott continuous. Thus the [function space of complete partial orders](#function-space-of-complete-partial-orders) is a [complete partial order](#complete-partial-order).

##### Least fixed point from a directed family of maps

↑ **Parent:** [Directed-complete partial order](#directed-complete-partial-order)

Let $f$ be [order-preserving](#order-preserving-function) and [inflationary](#inflationary-map) on a [directed-complete partial order](#directed-complete-partial-order). Define $x\mathrel R y$ when every set containing $x$ and closed under $f$ and directed [joins](#least-upper-bound-in-a-partially-ordered-set) contains $y$. This is a [partial order](#partially-ordered-set) refining $\le$. The [order-preserving](#order-preserving-function) maps $h$ satisfying $x\mathrel R h(x)$ form a composition-closed family $H$. The values $H x$ are [directed](#directed-set), since $h(k(x))$ bounds $h(x)$ and $k(x)$. Their [least upper bound](#least-upper-bound-in-a-partially-ordered-set) $h_0(x)$ lies in every such closed set containing $x$, so $h_0\in H$. Then $f\circ h_0\in H$ gives $f(h_0(x))\le h_0(x)$, while inflationarity gives the reverse inequality. If $p=f(p)$ and $x\le p$, the lower set $\{y:y\le p\}$ is closed, proving $h_0(x)\le p$. Thus $h_0(x)$ is the least [fixed point](function.md#fixed-point) of $f$ above $x$.

### Product order

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Product_order)

The product order on a Cartesian product of [partially ordered sets](#partially-ordered-set) compares every coordinate separately. Points that improve one coordinate and worsen another are incomparable. It is generally a [partial order](#partially-ordered-set), not a [total order](#total-order).

#### Maximal external point

↑ **Parent:** [Product order](#product-order)

A maximal external point of a finite set has no other point strictly larger in every coordinate. This weak nondominance differs from a [maximal element](#maximal-element-of-a-partially-ordered-set) in the [product order](#product-order) when coordinate ties exist: for example $(1,0)$ passes the weak test against $(1,1)$ but is not maximal in the product order. In an independent continuous-coordinate random sample, ties have probability zero, so the two notions coincide almost surely.

##### Expected number of coordinatewise maxima

↑ **Parent:** [Maximal external point](#maximal-external-point)

For $n$ independent uniform points in a rectangle, condition on one point with normalized coordinates $(x,y)$. It is a [maximal external point](#maximal-external-point) if all others avoid the upper-right rectangle of area $(1-x)(1-y)$, giving conditional probability $[1-(1-x)(1-y)]^{n-1}$. Integrating gives $H_n/n$, where $H_n$ is a [harmonic number](analytic-number-theory.md#harmonic-number). [Linearity of expectation](probability-theory.md#linearity-of-expectation) over the $n$ [indicator random variables](probability-theory.md#indicator-random-variable) gives $\mathbb E K_n=H_n$. The same answer holds for independent continuous coordinate distributions, by transforming each coordinate with its distribution function.

### Strict partial order

↑ **Parent:** [Partially ordered set](#partially-ordered-set)

A [strict partial order](#strict-partial-order) is an irreflexive transitive relation. In a classical set, it corresponds to a [partial order](#partially-ordered-set) through reflexification, but recovering the strict relation from the weak one requires inequality. In an arbitrary [topos](category-theory.md#elementary-topos), this reverse operation need not be geometric or define an inverse interpretation.

#### Reflexification of a strict partial order

↑ **Parent:** [Strict partial order](#strict-partial-order)

Reflexification turns a [strict partial order](#strict-partial-order) into a [partial order](#partially-ordered-set). Reflexivity is immediate, transitivity follows by the four disjunction cases, and antisymmetry follows because two opposed strict comparisons imply a forbidden self-comparison. The construction uses only [coherent logic](mathematical-logic.md#coherent-logic), so is preserved by [inverse image functors of geometric morphisms](category-theory.md#inverse-image-functor-of-a-geometric-morphism).

### Chain-poset nonembedding lemma

↑ **Parent:** [Partially ordered set](#partially-ordered-set)

If $\operatorname{Ch}(P)$ is the inclusion-ordered collection of every [chain in a partial order](#chain-in-a-partial-order), including the empty chain, it has no [order-preserving](#order-preserving-function) injection into $P$. Supposing $j$ exists, recursively set $p_\alpha=j(\{p_\beta:\beta<\alpha\})$ for $\alpha<h(P)$. By induction the earlier values form a chain; its proper initial chains are distinct, so monotonicity and injectivity make $p_\alpha$ strictly greater than every earlier value. This would inject the [Hartogs ordinal](set-theory.md#hartogs-number) into $P$.

### Set-theoretic tree

↑ **Parent:** [Partially ordered set](#partially-ordered-set)

A [partial order](#partially-ordered-set) in which the strict predecessors of each node form a [well-order](#well-order). The height of a node is the [order type](set-theory.md#order-type) of its predecessors; nodes of a common height form a level. This order-theoretic meaning is distinct from a graph-theoretic [tree](combinatorics.md#tree-graph-theory).

#### Branching form of the tree property

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

For an [uncountable](set-theory.md#uncountable-set) cardinal $\kappa$, this convention requires a cofinal branch in every separated rooted tree of height $\kappa$ with fewer than $\kappa$ immediate successors per node, without bounding level sizes. It is stronger than the usual [tree property](#tree-property) away from inaccessible cardinals. If $\operatorname{cf}(\kappa)<\kappa$, attach chains of cofinally increasing lengths below $\kappa$ above fewer than $\kappa$ children of one root; this contradicts the property. If $2^\lambda\geq\kappa$ for $\lambda<\kappa$, take a binary tree through level $\lambda$, choose $\kappa$ distinct nodes there, and attach to the $\xi$th a chain of length $\xi$. It has height $\kappa$, binary branching, and no cofinal branch. Hence the property implies that $\kappa$ is a [strongly inaccessible cardinal](set-theory.md#strongly-inaccessible-cardinal). At such a cardinal a separated tree with small immediate branching has small levels, so this convention agrees with the usual [tree property](#tree-property). It is not the different notion called the strong tree property in modern [set](set.md) theory.

#### Splitting tree

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

A tree is splitting if every node has two incompatible extensions. This property is additional to height and level-size bounds in a [kappa-tree](#kappa-tree). A [cofinal branch](#cofinal-branch) through a splitting tree of regular uncountable height produces an equally large antichain by taking off-branch extensions and proceeding beyond their divergence heights. Thus a splitting $\omega_1$-tree with countable antichains has no uncountable chains; the nonsplitting chain $\omega_1$ itself is a counterexample to omitting splitting.

#### Tree with unique limits

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

At a limit level, two nodes with the same predecessor at every smaller level must be equal. This is a uniqueness condition; it need not provide an upper node for every [cofinal branch](#cofinal-branch) through the lower levels.

#### Well-pruned set-theoretic tree

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

Every node has an extension at every higher level below the height of the [set-theoretic tree](#set-theoretic-tree). Equivalently, its extension heights are unbounded in the [set-theoretic tree](#set-theoretic-tree) height. Having no terminal nodes alone is weaker.

##### Unbounded-extension kernel of a regular tree

↑ **Parent:** [Well-pruned set-theoretic tree](#well-pruned-set-theoretic-tree)

For a [kappa-tree](#kappa-tree), retain nodes whose extension heights are unbounded in $\kappa$. The retained nodes are predecessor-closed. Each level remains nonempty: otherwise regularity would bound the union of fewer than $\kappa$ bounded extension [sets](set.md). The same argument above a retained node ensures retained extensions at every later level. Singular height invalidates this proof and the unrestricted conclusion.

#### Kappa-tree

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

For a regular uncountable [cardinal number](set-theory.md#cardinal-number) $\kappa$, a [set-theoretic tree](#set-theoretic-tree) of height $\kappa$ with nonempty levels of [cardinality](set-theory.md#cardinality) less than $\kappa$. The regular-height convention is important for the [unbounded-extension kernel of a regular tree](#unbounded-extension-kernel-of-a-regular-tree).

##### Tree property

↑ **Parent:** [Kappa-tree](#kappa-tree)

For an infinite cardinal $\kappa$, the tree property says that every tree of height $\kappa$ with nonempty levels of cardinality less than $\kappa$ has a cofinal branch. In the all-trees-of-size-$\kappa$ convention it also forces regularity: disjoint chains of lengths cofinal in a singular $\kappa$ form a counterexample. It does not, by itself, imply strong inaccessibility. A strong limit cardinal with the tree property satisfies the self-partition relation by applying it to the end-homogeneous coloring tree. At a strongly inaccessible cardinal this is the usual weak-compactness characterization.

##### Uniformly narrow regular-height tree branch theorem

↑ **Parent:** [Kappa-tree](#kappa-tree)

For infinite [regular cardinals](set-theory.md#regular-cardinal) $\kappa<\lambda$, a $\lambda$-tree whose levels all have size less than $\kappa$ has a [cofinal branch](#cofinal-branch). At levels of [cofinality](set-theory.md#cofinality) $\kappa$, bound all heights distinguishing distinct predecessor chains. The [Fodor lemma](set-theory.md#fodor-lemma) makes this bound constant on a stationary set; one predecessor at that height occurs stationarily often. The resulting predecessor chains agree below their common heights and unite into a branch through every level. Distinct limit-level nodes with identical predecessor chains do not affect this argument.

#### Kurepa tree

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

A [set-theoretic tree](#set-theoretic-tree) of height $\omega_1$ with countable levels and at least $\aleph_2$ distinct [cofinal branches](#cofinal-branch).

##### Kurepa tree from an inaccessible binary tree

↑ **Parent:** [Kurepa tree](#kurepa-tree)

Let $\kappa$ be [strongly inaccessible cardinal](set-theory.md#strongly-inaccessible-cardinal) in the ground model and perform the [finite Lévy collapse to omega-one](forcing.md#finite-levy-collapse-to-omega-one). The ground full binary [set-theoretic tree](#set-theoretic-tree) of height $\kappa$ has all levels of size less than $\kappa$, so these levels become countable. Its at least $(\kappa^+)^M$ ground branches remain distinct. The [chain in a partial order](#chain-in-a-partial-order) condition preserves $(\kappa^+)^M$, which is the extension $\aleph_2$. The unchanged ground [set-theoretic tree](#set-theoretic-tree) therefore witnesses the [Kurepa hypothesis](#kurepa-hypothesis).

##### Kurepa hypothesis

↑ **Parent:** [Kurepa tree](#kurepa-tree)

There exists an $\omega_1$-tree with countable levels and at least $\aleph_2$ distinct [cofinal branches](#cofinal-branch).

##### Kurepa-family hypothesis

↑ **Parent:** [Kurepa tree](#kurepa-tree)

There is $\mathcal F\subseteq\mathcal P(\omega_1)$ of size $\aleph_2$ such that $\{X\cap\alpha:X\in\mathcal F\}$ is countable for every $\alpha<\omega_1$. Its initial-segment tree, pruned and leveled to be normal, is a [Kurepa tree](#kurepa-tree).

#### Aronszajn tree

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

A [set-theoretic tree](#set-theoretic-tree) of height $\omega_1$ with countable levels and no [cofinal branch](#cofinal-branch). More generally, a $\kappa$-Aronszajn tree has height a regular uncountable $\kappa$, levels of size less than $\kappa$, and no [cofinal branch](#cofinal-branch).

##### Coherent-injection Aronszajn tree

↑ **Parent:** [Aronszajn tree](#aronszajn-tree)

Given [coherent coinfinite injections into omega](algebra.md#coherent-coinfinite-injections-into-omega), use all restrictions $e_\alpha\upharpoonright\beta$, where $\beta\le\alpha<\omega_1$, ordered by proper extension. Every level is countable because its nodes differ finitely from a fixed [function](function.md) on a countable domain. An uncountable [chain in a partial order](#chain-in-a-partial-order) would have unbounded domain heights, and its union would inject $\omega_1$ into $\omega$, which is impossible.

##### Suslin tree

↑ **Parent:** [Aronszajn tree](#aronszajn-tree)

An [Aronszajn tree](#aronszajn-tree) with no uncountable [tree antichain](#tree-antichain). A normal splitting [Suslin tree](#suslin-tree) yields a [Suslin line](foundations-of-mathematics.md#suslin-line) by a lexicographic ordering followed by [Dedekind completion](#dedekind-completion).

<h6 id="suslin-tree-obstruction-to-martin-s-axiom">Suslin-tree obstruction to Martin's axiom</h6>

↑ **Parent:** [Suslin tree](#suslin-tree)

A [well-pruned set-theoretic tree](#well-pruned-set-theoretic-tree) that is an [Aronszajn tree](#aronszajn-tree) and a [Suslin tree](#suslin-tree) gives a [forcing](forcing.md) with the [countable chain condition for forcing](forcing.md#countable-chain-condition-for-forcing): stronger nodes extend weaker ones. The $\omega_1$ [dense subsets of a forcing order](forcing.md#dense-subset-of-a-forcing-order) of nodes at or above each level cannot all be met by a [filter in an ordered set](#filter-mathematics), since that would produce a [cofinal branch](#cofinal-branch). Thus $\mathrm{MA}_{\aleph_1}$ fails. When the continuum exceeds $\aleph_1$, full [Martin axiom](forcing.md#martin-s-axiom) includes this instance.

##### Special Aronszajn tree

↑ **Parent:** [Aronszajn tree](#aronszajn-tree)

An [Aronszajn tree](#aronszajn-tree) that is a union of countably many [tree antichains](#tree-antichain). Equivalently, it admits a map into a countable set that is injective on each chain.

###### Rationally labelled Aronszajn tree construction

↑ **Parent:** [Special Aronszajn tree](#special-aronszajn-tree)

Construct countable levels of bounded increasing rational sequences, maintaining the [bounded rational extension property](#bounded-rational-extension-property). At successor stages append every allowed rational. At a countable limit, handle each earlier-node/rational-cap pair by a cofinal sequence of extensions with values approaching a rational strictly below the cap. Its union has that rational supremum. Countably many requirements give a countable new level. Strictly increasing labels exclude uncountable chains, and label fibers are [tree antichains](#tree-antichain), so the result is a [special Aronszajn tree](#special-aronszajn-tree).

###### Bounded rational extension property

↑ **Parent:** [Rationally labelled Aronszajn tree construction](#rationally-labelled-aronszajn-tree-construction)

For every earlier node and rational cap above its label, an extension at each later level remains below the cap. In the [rationally labelled Aronszajn tree construction](#rationally-labelled-aronszajn-tree-construction) this reserves space for limit-stage unions. Choosing an intermediate rational and forcing successive values toward it ensures a rational supremum and strictly increasing labels even at limit levels.

##### Aleph-two Aronszajn tree

↑ **Parent:** [Aronszajn tree](#aronszajn-tree)

A [set-theoretic tree](#set-theoretic-tree) of height $\omega_2$, levels of size at most $\aleph_1$, and no [cofinal branch](#cofinal-branch). The [Continuum hypothesis](set-theory.md#continuum-hypothesis) supplies one through the [minimal-walk tree](set-theory.md#minimal-walk-tree).

#### Normal set-theoretic tree

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

A [set-theoretic tree](#set-theoretic-tree) with one root, extensions of every node at every higher level, at least two immediate successors for every node, and distinct limit-level nodes distinguished by their predecessor chains. If splitting occurs only at later levels, a continuous cofinal selection of levels can enforce immediate splitting.

#### Cofinal branch

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

A maximal chain with nodes at unbounded heights in a [set-theoretic tree](#set-theoretic-tree). Taking predecessor closure gives one node at each level below the tree height.

#### Tree antichain

↑ **Parent:** [Set-theoretic tree](#set-theoretic-tree)

A set of pairwise incomparable nodes in a [set-theoretic tree](#set-theoretic-tree). A maximal [tree antichain](#tree-antichain) has a comparable member for every node of the tree.

### Chain in a partial order

↑ **Parent:** [Partially ordered set](#partially-ordered-set)

A subset of a [partially ordered set](#partially-ordered-set) on which the inherited order is total. The upper-bound hypothesis in [Zorn lemma](set-theory.md#zorn-s-lemma) concerns all such subsets, not just countable increasing sequences.

### Differential poset

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_poset)

A differential poset is a locally finite graded [partially ordered set](#partially-ordered-set) with a unique minimum, finite ranks, and up and down cover operators satisfying $DU-UD=rI$ for a fixed positive integer $r$. The [Young lattice](representation-theory-of-the-symmetric-group.md#young-s-lattice) has $r=1$: distinct equal-rank diagrams have equally many common upper and lower covers, and each diagram has one more upper cover than lower cover.

#### Normal ordering identity for up and down operators

↑ **Parent:** [Differential poset](#differential-poset)

If $DU-UD=I$, commuting every $D$ past every $U$ gives $(D+U)^\ell=\sum_{i+j+2m=\ell}\ell!U^iD^j/(2^m i!j!m!)$. The recurrence follows from $DU^i=U^iD+iU^{i-1}$. Applied to the empty diagram in the [Young lattice](representation-theory-of-the-symmetric-group.md#young-s-lattice), it counts [oscillating tableaux](representation-theory-of-the-symmetric-group.md#oscillating-path-in-the-young-lattice).

### Filter (mathematics)

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Filter_(mathematics))

A filter is a nonempty upward-closed [subset](#subset) $G$ of a [partial order](#partially-ordered-set) such that every two members have a common lower bound in $G$. With [standard notation for forcing](forcing.md#standard-notation-for-forcing), lower means stronger, so these are exactly the directed filters used to define a [generic filter](forcing.md#generic-filter). The [projection of a product-generic filter](forcing.md#projection-of-a-product-generic-filter) uses these properties before genericity of its factor filters is proved.

#### Principal filter in an ordered set

↑ **Parent:** [Filter (mathematics)](#filter-mathematics)

The principal [filter in an ordered set](#filter-mathematics) generated by $p$ contains exactly the elements above $p$. It is upward closed, and $p$ is a common lower bound in the filter for any two of its members. With [standard notation for forcing](forcing.md#standard-notation-for-forcing), these are the conditions weaker than $p$. The principal filter need not be a [generic filter](forcing.md#generic-filter): a dense [set](set.md) can require a strict strengthening. The compatible-condition filter in [a forcing atom determines a ground-model generic filter](forcing.md#a-forcing-atom-determines-a-ground-model-generic-filter) includes strengthenings as well as weakenings and can therefore be strictly larger.

### Linear extension

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_extension)

A linear extension is a total ordering of the elements of a [partially ordered set](#partially-ordered-set) that preserves all its comparisons. For a finite set it can be recorded as a list. If two adjacent elements in that list are incomparable, their interchange is again a linear extension.

#### Reduced adjacent-swap path between linear extensions

↑ **Parent:** [Linear extension](#linear-extension)

Two linear extensions of a finite [partially ordered set](#partially-ordered-set) can be joined using as many admissible adjacent swaps as the inversion count of their relative permutation. Label the current list by the desired positions in the target. An adjacent descent consists of incomparable elements, since comparable elements have the same order in both lists. Swap that descent; its inversion count decreases by one. Iteration sorts the list and gives a path of minimal [Coxeter length](semisimple-lie-algebra.md#coxeter-length).

### Order-preserving function

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order-preserving_function)

An order-preserving function $f:P\to Q$ between [partially ordered sets](#partially-ordered-set) satisfies $x\leq y\Rightarrow f(x)\leq f(y)$.

#### Inflationary map

↑ **Parent:** [Order-preserving function](#order-preserving-function)

An inflationary map on a [partially ordered set](#partially-ordered-set) satisfies $x\le f(x)$ for every $x$. This condition is distinct from being [order-preserving](#order-preserving-function).

#### Strict order-preserving function

↑ **Parent:** [Order-preserving function](#order-preserving-function)

A [strict order-preserving function](#strict-order-preserving-function) preserves strict comparisons. Between [strict partial orders](#strict-partial-order) it may identify incomparable elements. Between [strict total orders](#strict-total-order) it is necessarily injective, and in a finite chain it is exactly an increasing injection. It need not reflect comparisons between incomparable elements of general partial orders.

### Order dimension

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order_dimension)

The order dimension of a [partially ordered set](#partially-ordered-set) $(X,<)$ is the least cardinality of a family of [total orders](#total-order) on $X$ whose intersection is $<$. Such a family is called a realizer of the partial order.

#### Two-dimensional partially ordered set

↑ **Parent:** [Order dimension](#order-dimension)

A partially ordered set is two-dimensional when there are two total orders $<_1$ and $<_2$ on its ground set such that

$$
x<y\quad\Longleftrightarrow\quad x<_1y\text{ and }x<_2y.
$$

##### Finite-local characterization of two-dimensional partially ordered sets

↑ **Parent:** [Two-dimensional partially ordered set](#two-dimensional-partially-ordered-set)

A partially ordered set is two-dimensional if every one of its finite induced suborders is two-dimensional. Encode two candidate total orders by propositional variables; every finite collection of the order, extension, and intersection clauses concerns a finite induced suborder, so the [propositional compactness theorem](mathematical-logic.md#propositional-compactness-theorem) supplies two global realizing orders.

### Chain in a partially ordered set

↑ **Parent:** [Partially ordered set](#partially-ordered-set)

A chain in a [partially ordered set](#partially-ordered-set) is a subset in which every two elements are comparable.

The order induced on this subset is a [total order](#total-order).

### Directed set

↑ **Parent:** [Partially ordered set](#partially-ordered-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Directed_set)

A directed set is a nonempty [preorder](#preorder) in which every finite subset has an upper bound. It provides an index set in which any finite collection of stages has a common later stage.

## Total order

↑ **Parent:** [Set](set.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Total_order)

A total order is a reflexive, antisymmetric, transitive relation in which every two elements are comparable.

### Minimum of a subset of a total order

↑ **Parent:** [Total order](#total-order)

A minimum of $A$ is a member of $A$ less than or equal to every member of $A$. It equals the [infimum](real-analysis.md#infimum) when that lower bound is attained. A nonempty finite subset of a [totally ordered set](#totally-ordered-set) has a minimum; a nonempty open real interval does not.

### Maximum of a subset of a total order

↑ **Parent:** [Total order](#total-order)

A maximum of a subset $S$ of a [total order](#total-order) is an element $m\in S$ with $s\leq m$ for every $s\in S$. If it exists it is unique. Every nonempty finite subset has a maximum, by repeated pairwise comparison. Unlike a supremum, a maximum must belong to the subset. The completion time of jobs processed on finitely many parallel machines is the maximum of the machine completion times.

### Totally ordered set

↑ **Parent:** [Total order](#total-order)

A [totally ordered set](#totally-ordered-set) is a set equipped with a [total order](#total-order). Internally in a [topos](category-theory.md#elementary-topos), weak totality does not imply decidable equality. The empty ordered set is allowed unless an inhabitation axiom is explicitly imposed.

### Dense order

↑ **Parent:** [Total order](#total-order)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dense_order)

A [total order](#total-order) is dense when between every two distinct ordered points lies a third. Endpoints are allowed; “without endpoints” is an additional condition. A dense order with two points $a<b$ cannot be a [well-order](#well-order), since $\{x:a<x\}$ is nonempty and has no least member. Its first-order axioms are the total-order axioms plus $\forall x,y\,(x<y\Rightarrow\exists z\,(x<z<y))$. Countability and uncountability are not first-order axiomatizable restrictions, by the upward and downward witness constructions of the [Löwenheim-Skolem theorem](mathematical-logic.md#lowenheim-skolem-theorem).

### Aleph-one-like linear order

↑ **Parent:** [Total order](#total-order)

An [aleph-one-like linear order](#aleph-one-like-linear-order) has size $\aleph_1$ and every point has only countably many predecessors. Consequently every proper initial segment is countable, since it is bounded by any point outside it. This differs from requiring every nonempty interval to be uncountable.

#### Stationary encoding in an aleph-one-like dense order

↑ **Parent:** [Aleph-one-like linear order](#aleph-one-like-linear-order)

For a subset $S$ of the nonzero countable limit ordinals, let $B_\alpha=1+\mathbb Q$ when $\alpha\in S$ and $B_\alpha=\mathbb Q$ otherwise. The [order sum](#order-sum) is an [aleph-one-like linear order](#aleph-one-like-linear-order) whose nonempty proper initial segments are $\mathbb Q$ or $\mathbb Q+1$. At the limit cut before block $\delta$, the complementary final segment has a least point exactly when $\delta\in S$. [Club agreement of countable filtrations](set-theory.md#club-agreement-of-countable-filtrations) makes this condition invariant modulo a nonstationary difference. [Disjoint stationary subsets of omega-one](set-theory.md#disjoint-stationary-subsets-of-omega-one) consequently supply $2^{\aleph_1}$ nonisomorphic orders.

### Order topology

↑ **Parent:** [Total order](#total-order)

The topology generated by open intervals and open initial and final rays in a [total order](#total-order). For a dense order without endpoints, a subset is dense in this topology exactly when it meets every nonempty open interval.

#### Lexicographic order topology on the real plane

↑ **Parent:** [Order topology](#order-topology)

Give $\mathbb R^2$ the [lexicographic order](extremal-set-theory.md#lexicographic-order) and the [order topology](#order-topology). Every point $(a,b)$ has an interval neighbourhood between $(a,b-\varepsilon)$ and $(a,b+\varepsilon)$, lying entirely in the vertical line $\{a\}\times\mathbb R$. These intervals give each such line its usual real [topology](topology.md), and every line is open. Thus this space is a disjoint union of uncountably many open copies of the real line and is not a [second-countable space](topology.md#second-countable-space): any [basis of a topology](topology.md#basis-of-a-topology) must supply a different member inside each of these disjoint nonempty open sets.

### Countable chain condition for a linear order

↑ **Parent:** [Total order](#total-order)

Every pairwise disjoint collection of nonempty open intervals is countable. This is one of the defining properties of a [Suslin line](foundations-of-mathematics.md#suslin-line).

### Order-dense subset

↑ **Parent:** [Total order](#total-order)

A subset of a [total order](#total-order) meeting every nonempty open interval between two distinct points. A countable [order-dense subset](#order-dense-subset) witnesses separability in the [order topology](#order-topology) of a dense order.

### Order completeness

↑ **Parent:** [Total order](#total-order)

Every nonempty bounded-above subset of a [total order](#total-order) has a least upper bound. In the real line this is the [supremum](real-analysis.md#supremum) property used to extend maps defined on an [order-dense subset](#order-dense-subset).

#### Dedekind completion

↑ **Parent:** [Order completeness](#order-completeness)

The completion of a [total order](#total-order) by its nonprincipal proper cuts, supplying least upper bounds. For a dense order it contains the original order densely, and preserves the interval countable chain condition and separability or nonseparability.

### Order isomorphism

↑ **Parent:** [Total order](#total-order)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order_isomorphism)

An [order isomorphism](#order-isomorphism) is a [bijection](function.md#bijection) preserving and reflecting the order relation. It transfers [well-foundedness](set-theory.md#well-founded-relation) and [order type](set-theory.md#order-type) between a coded order and its [ordinal](set-theory.md#ordinal) interpretation.

### Order sum

↑ **Parent:** [Total order](#total-order)

The order sum $A+B$ is the disjoint union of two [total orders](#total-order), preserving each order and placing every element of $A$ before every element of $B$. For example $\mathbb N+\mathbb Z$ has a least element but also has elements with infinitely many predecessors.

### Order automorphism

↑ **Parent:** [Total order](#total-order)

An [order automorphism](#order-automorphism) of a [total order](#total-order) $(I,<)$ is a [bijection](function.md#bijection) $\pi:I\to I$ such that $i<j$ if and only if $\pi(i)<\pi(j)$. Composition and inverses are again [order automorphisms](#order-automorphism). Transporting the indices of an [order-indiscernible sequence](foundations-of-mathematics.md#order-indiscernible-sequence) by such a map preserves every [first-order formula](mathematical-logic.md#first-order-formula) on increasing finite tuples.

#### Rigid dense subset of the real line

↑ **Parent:** [Order automorphism](#order-automorphism)

An [order-dense subset](#order-dense-subset) with no nonidentity [order automorphism](#order-automorphism). A transfinite diagonal construction marks an included point and an excluded image for every nonidentity real-line [order automorphism](#order-automorphism), yielding such a subset of size $2^{\aleph_0}$.

#### Extension of an order automorphism from a dense subset

↑ **Parent:** [Order automorphism](#order-automorphism)

An [order automorphism](#order-automorphism) of an [order-dense subset](#order-dense-subset) $D$ of the real line extends uniquely by $\widetilde\varphi(x)=\sup\{\varphi(d):d\in D,d<x\}$. [Order completeness](#order-completeness) supplies the extension, and the lower cuts in $D$ give uniqueness.

### Strict total order

↑ **Parent:** [Total order](#total-order)

A strict total order is an irreflexive and transitive relation $<$ for which exactly one of $x<y$ and $y<x$ holds whenever $x\ne y$. It corresponds to a total order through $x\leq y$ if and only if $x<y$ or $x=y$.

### Well-order

↑ **Parent:** [Total order](#total-order)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Well-order)

A well-order is a [total order](#total-order) in which every nonempty subset has a least element.

#### Decidable well-order

↑ **Parent:** [Well-order](#well-order)

A [decidable well-order](#decidable-well-order) on the [natural numbers](arithmetic.md#natural-number) is a [well-order](#well-order) whose comparison relation is computable. Comparing two codes is an effective finite task; the proof that the relation has no infinite descending chain is a separate mathematical assertion. [Computable Cantor normal form notation](set-theory.md#computable-cantor-normal-form-notation) gives such an order of type [epsilon zero](set-theory.md#epsilon-zero).

### Empty order

↑ **Parent:** [Total order](#total-order)

The empty order is the unique total order on the [empty set](#empty-set).

### Initial segment

↑ **Parent:** [Total order](#total-order)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Initial_segment)

An initial segment contains every element below each of its elements.

## ↑ Ancestors (5)

1. [Set theory](set-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (388)

- [A forcing atom determines a ground-model generic filter](forcing.md#a-forcing-atom-determines-a-ground-model-generic-filter)
- [Absoluteness of cardinalhood in limit ranks](set-theory.md#absoluteness-of-cardinalhood-in-limit-ranks)
- [Algebraic structure](algebra.md#algebraic-structure)
- [Atomless forcing order](forcing.md#atomless-forcing-order)
- [Automatic continuity onto a semisimple Banach algebra](banach-algebra.md#automatic-continuity-onto-a-semisimple-banach-algebra)
- [Axiom of constructibility](definable-power-set.md#axiom-of-constructibility)
- [Axiom of countable choice](set-theory.md#axiom-of-countable-choice)
- [Axiom of extensionality](set-theory.md#axiom-of-extensionality)
- [Axiom of global choice](set-theory.md#axiom-of-global-choice)
- [Axiom of pairing](set-theory.md#axiom-of-pairing)
- [Basic Fraenkel permutation model](set-theory.md#basic-fraenkel-permutation-model)
- [Binary operation](algebra.md#binary-operation)
- [Borel null set](measure-theory.md#borel-null-set)
- [Bounded subfunctor solution set for precomposition](category.md#bounded-subfunctor-solution-set-for-precomposition)
- [Bounding-to-almost-disjointness inequality](set-theory.md#bounding-to-almost-disjointness-inequality)
- [Branching form of the tree property](#branching-form-of-the-tree-property)
- [Cardinality](set-theory.md#cardinality)
- [Category of partial functions](category.md#category-of-partial-functions)
- [Category of relations (sets)](category.md#category-of-relations-sets)
- [Category of sets](category.md#category-of-sets)
- [Choice preservation by well-ordered names](forcing.md#choice-preservation-by-well-ordered-names)
- [Closed forcing adds no short ground-valued sequences](forcing.md#closed-forcing-adds-no-short-ground-valued-sequences)
- [Club set](set-theory.md#club-set)
- [Cofinality of a continuous cardinal hierarchy](set-theory.md#cofinality-of-a-continuous-cardinal-hierarchy)
- [Cofinite set](set-theory.md#cofinite-set)
- [Coinfinite set](#coinfinite-set)
- [Colouring of a set](#colouring-of-a-set)
- [Concentration of discrete cubes at diameter scale](probability-theory.md#concentration-of-discrete-cubes-at-diameter-scale)
- [Connected component of a category](category.md#connected-component-of-a-category)
- [Constructible-level absoluteness over ZF](definable-power-set.md#constructible-level-absoluteness-over-zf)
- [Constructible-universe obstruction to a uniform inner-model proof of failure of choice](set-theory.md#constructible-universe-obstruction-to-a-uniform-inner-model-proof-of-failure-of-choice)
- [Countability from vanishing averages of distinct sequences](set-theory.md#countability-from-vanishing-averages-of-distinct-sequences)
- [Countable intersection](#countable-intersection)
- [Countable saturation of a nonprincipal ultraproduct over omega](foundations-of-mathematics.md#countable-saturation-of-a-nonprincipal-ultraproduct-over-omega)
- [Countable set](set-theory.md#countable-set)
- [Countable subadditivity of a measure](measure-theory.md#countable-subadditivity-of-a-measure)
- [Countable union of explicitly ordered finite lists without choice](set-theory.md#countable-union-of-explicitly-ordered-finite-lists-without-choice)
- [Counting lemma for octahedrally quasirandom three-uniform hypergraphs](hypergraph.md#counting-lemma-for-octahedrally-quasirandom-three-uniform-hypergraphs)
- [Cubic lattice](graph.md#cubic-lattice)
- [Dedekind-finite set](#dedekind-finite-set)
- [Definable continuous hierarchy](set-theory.md#definable-continuous-hierarchy)
- [Dense-below generic meeting lemma](forcing.md#dense-below-generic-meeting-lemma)
- [Discrete category](category.md#discrete-category)
- [Disjoint occurrence of increasing events](bond-percolation.md#disjoint-occurrence-of-increasing-events)
- [Egorov's theorem](real-analysis.md#egorov-s-theorem)
- [Empty product](arithmetic.md#empty-product)
- [Equivalence class](set-theory.md#equivalence-class)
- [Equivalence of partial functions modulo finite changes](set-theory.md#equivalence-of-partial-functions-modulo-finite-changes)
- [Extensional cumulative universe over Quine atoms](set-theory.md#extensional-cumulative-universe-over-quine-atoms)
- [Failure of concentration in fixed-dimensional grids](probability-theory.md#failure-of-concentration-in-fixed-dimensional-grids)
- [Fiber of a function](function.md#fiber-of-a-function)
- [Fichtenholz-Kantorovich independent family](set-theory.md#fichtenholz-kantorovich-independent-family)
- [Finite additivity of a set function](function.md#finite-additivity-of-a-set-function)
- [Finite-injury computable colouring of pairs](ramsey-theory.md#finite-injury-computable-colouring-of-pairs)
- [Finite intersection witness for cross-intersecting families](extremal-set-theory.md#finite-intersection-witness-for-cross-intersecting-families)
- [Finite modification of Bernoulli percolation](probability-theory.md#finite-modification-of-bernoulli-percolation)
- [Finite modification of the identity on the real line](function.md#finite-modification-of-the-identity-on-the-real-line)
- [Finite repetition-free sequence](real-analysis.md#finite-repetition-free-sequence)
- [Finite repetition-free sequences preserve Dedekind-finiteness](#finite-repetition-free-sequences-preserve-dedekind-finiteness)
- [Finite set](#finite-set)
- [Finite-stage equality in a filtered set colimit](category.md#finite-stage-equality-in-a-filtered-set-colimit)
- [Finite subsets do not define a topology on an infinite set](topology.md#finite-subsets-do-not-define-a-topology-on-an-infinite-set)
- [Finite symmetric difference](#finite-symmetric-difference)
- [Finite-symmetric-difference colouring of infinite subsets](set-theory.md#finite-symmetric-difference-colouring-of-infinite-subsets)
- [Finitely supported permutation](combinatorics.md#finitely-supported-permutation)
- [Function class](function.md#function-class)
- [Generic coordinate reals for finite-function forcing](forcing.md#generic-coordinate-reals-for-finite-function-forcing)
- [Generic filter for an atomless order is new](forcing.md#generic-filter-for-an-atomless-order-is-new)
- [Geometric locus](geometry-and-topology.md#geometric-locus)
- [Half-size cyclic Freiman model with a sharp difference-set bound](additive-combinatorics.md#half-size-cyclic-freiman-model-with-a-sharp-difference-set-bound)
- [Hartogs numbers under choice](set-theory.md#hartogs-numbers-under-choice)
- [Hausdorff measure](measure-theory.md#hausdorff-measure)
- [Hereditarily locally small membership model](set-theory.md#hereditarily-locally-small-membership-model)
- [Hitting set](extremal-set-theory.md#hitting-set)
- [Hom-set](category.md#hom-set)
- [Homogeneous set for a colouring](ramsey-theory.md#homogeneous-set-for-a-colouring)
- [Incidence matrix of a set system](extremal-set-theory.md#incidence-matrix-of-a-set-system)
- [Increasing chain of countable sets](set-theory.md#increasing-chain-of-countable-sets)
- [Increasing enumeration of an infinite subset of natural numbers](set-theory.md#increasing-enumeration-of-an-infinite-subset-of-natural-numbers)
- [Indiscrete category](category.md#indiscrete-category)
- [Inductive set](set-theory.md#inductive-set)
- [Infinite Dedekind-finite set](#infinite-dedekind-finite-set)
- [Infinite set](#infinite-set)
- [Inner models with all reals preserve omega-one](definable-power-set.md#inner-models-with-all-reals-preserve-omega-one)
- [Intersection of equivalence relations](set-theory.md#intersection-of-equivalence-relations)
- [Intersection polynomial](combinatorics.md#intersection-polynomial)
- [Intersection-preserving lexicographic UV-compression](extremal-set-theory.md#intersection-preserving-lexicographic-uv-compression)
- [Irregular pair of vertex sets](probabilistic-combinatorics.md#irregular-pair-of-vertex-sets)
- [Isomorphism of categories](category.md#isomorphism-of-categories)
- [Kappa-filtration](set-theory.md#kappa-filtration)
- [Kuratowski ordered pair](#kuratowski-ordered-pair)
- [Linear space (geometry)](combinatorics.md#linear-space-geometry)
- [Local lemma Ramsey lower bound](probabilistic-combinatorics.md#local-lemma-ramsey-lower-bound)
- [Matroid](combinatorics.md#matroid)
- [Meromorphic continuation](complex-analysis.md#meromorphic-continuation)
- [Metric](topological-analysis.md#metric)
- [Multipartite hypergraph](hypergraph.md#multipartite-hypergraph)
- [Multiset](#multiset)
- [Mutual genericity for product forcing](forcing.md#mutual-genericity-for-product-forcing)
- [Nash-Williams barrier partition theorem](#nash-williams-barrier-partition-theorem)
- [Oddtown theorem](extremal-set-theory.md#oddtown-theorem)
- [Partition of a set](#partition-of-a-set)
- [Partition topology](topology.md#partition-topology)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4.md#1e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4.md#1e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4.md#6e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4.md#8e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#7/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#7/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#1b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#1b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#5b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#8d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#9c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4.md#5f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4.md#6f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4.md#6f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-10.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#11/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#12/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-7.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-7.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-9.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4.md#2c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-4.md#5c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#7/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#7/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1.md#3d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4.md#5e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4.md#8e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5.md#11/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5.md#12/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#11/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#11/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#11/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-27.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-27.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4.md#5d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4.md#5d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-27.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-27.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-27.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-27.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-27.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-27.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-27.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-27.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-27.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4.md#7e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4.md#7e/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4.md#8e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-10.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-10.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-10.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-10.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4.md#5d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4.md#5d/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4.md#5d/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4.md#5d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4.md#8d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-25.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-25.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-25.md#7/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-83.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-83.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-18.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4.md#2e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4.md#7e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4.md#7e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4.md#8e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4.md#8e/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#1/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#1/ii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/iii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/iii/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#3/iv/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#3/iv/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/iv/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/iv/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-12.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#3/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4.md#2e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#2d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#2d/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#6d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#6d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#6d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4.md#6d/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#11h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#15h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#17i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#19h/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#22f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#22f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#22f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#22f/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#24i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#25i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#26j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#26j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#26j/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#8e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#11h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#14h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#17g/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#19f/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#22i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#25k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#8e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-109.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-109.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-119.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-119.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-119.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#2/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#3/ii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#3/iv/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#4/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#4/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-121.md#1/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-128.md#2/b/solution)
- [Perfect subsequence lemma](#perfect-subsequence-lemma)
- [Ping-pong lemma](geometric-group-theory.md#ping-pong-lemma)
- [Pointed set](#pointed-set)
- [Pointwise periodic self-map](function.md#pointwise-periodic-self-map)
- [Power of sets as a capital regular category](category.md#power-of-sets-as-a-capital-regular-category)
- [Power-set failure in an increasing union of generic extensions](forcing.md#power-set-failure-in-an-increasing-union-of-generic-extensions)
- [Principal filter in an ordered set](#principal-filter-in-an-ordered-set)
- [Private-witness diagonalization for incomparable enumerable sets](foundations-of-mathematics.md#private-witness-diagonalization-for-incomparable-enumerable-sets)
- [Product probability space](probability-theory.md#product-probability-space)
- [Projection of a product-generic filter](forcing.md#projection-of-a-product-generic-filter)
- [Quotient set](set-theory.md#quotient-set)
- [Ramsey family in the homogeneous-cone sense](ramsey-theory.md#ramsey-family-in-the-homogeneous-cone-sense)
- [Rank-indiscernible construction of an NFU model](set-theory.md#rank-indiscernible-construction-of-an-nfu-model)
- [Rank-shifting NFU model with explicit set predicate](set-theory.md#rank-shifting-nfu-model-with-explicit-set-predicate)
- [Reachability in a graph](graph.md#reachability-in-a-graph)
- [Recursively repetition-free labelled tree](combinatorics.md#recursively-repetition-free-labelled-tree)
- [Recursively repetition-free labelled trees preserve Dedekind-finiteness](combinatorics.md#recursively-repetition-free-labelled-trees-preserve-dedekind-finiteness)
- [Relative constructible universe](definable-power-set.md#relative-constructible-universe)
- [Restricted set comprehension](set-theory.md#restricted-set-comprehension)
- [Rigidity of a scalene triangle](riemannian-geometry.md#rigidity-of-a-scalene-triangle)
- [Rooted branch-set reduction](graph-theory.md#rooted-branch-set-reduction)
- [Rooted separation of a graph](graph-theory.md#rooted-separation-of-a-graph)
- [Rule of product](combinatorics.md#rule-of-product)
- [Russell's paradox](set-theory.md#russell-s-paradox)
- [Satisfaction for a set structure](mathematical-logic.md#satisfaction-for-a-set-structure)
- [Saturated elementary extension theorem](foundations-of-mathematics.md#saturated-elementary-extension-theorem)
- [Scalar estimate for Talagrand product induction](probability-inequality.md#scalar-estimate-for-talagrand-product-induction)
- [Semigroup](algebra.md#semigroup)
- [Separating set system](extremal-set-theory.md#separating-set-system)
- [Separation proof in the constructible universe](definable-power-set.md#separation-proof-in-the-constructible-universe)
- [Sierpiński set](measure-theory.md#sierpinski-set)
- [Simple graph](graph.md#simple-graph)
- [Solution-set condition](category.md#solution-set-condition)
- [Spectrum of a polynomial-generated Banach subalgebra](banach-algebra.md#spectrum-of-a-polynomial-generated-banach-subalgebra)
- [Symmetric difference](#symmetric-difference)
- [Symmetry enlargement under group translates](group-theory.md#symmetry-enlargement-under-group-translates)
- [Topology axiom](topology.md#topology-axiom)
- [Trifurcation boundary-counting lemma](bond-percolation.md#trifurcation-boundary-counting-lemma)
- [Ultrafilter characterization of compact Hausdorff spaces](set-theory.md#ultrafilter-characterization-of-compact-hausdorff-spaces)
- [Ultrafilter selection from a partition-rich family](set-theory.md#ultrafilter-selection-from-a-partition-rich-family)
- [Unbounded-extension kernel of a regular tree](#unbounded-extension-kernel-of-a-regular-tree)
- [Uncountability by interleaving prescribed binary coordinates](real-analysis.md#uncountability-by-interleaving-prescribed-binary-coordinates)
- [Uniform period criterion for pointwise periodic maps](function.md#uniform-period-criterion-for-pointwise-periodic-maps)
- [Union of equivalence relations](set-theory.md#union-of-equivalence-relations)
- [Upper and lower sets](#upper-and-lower-sets)
- [Urelement](set-theory.md#urelement)
- [Vertex set](graph.md#vertex-set)
- [Weakly initial set](category.md#weakly-initial-set)
- [Weakly terminal set](category.md#weakly-terminal-set)
- [Weighted inclusion-exclusion principle](combinatorics.md#weighted-inclusion-exclusion-principle)
- [Well-copowered category](category.md#well-copowered-category)
