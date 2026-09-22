# Forcing

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Forcing_(mathematics))

Forcing extends a model of set theory by adjoining a filter generic for a partially ordered set of finite or otherwise controlled approximations.

**Table of contents**

- [Forcing antichain](#forcing-antichain)
- [Cardinal collapse](#cardinal-collapse)
- [Cofinality-preserving forcing](#cofinality-preserving-forcing)
- [Martin's axiom](#martin-s-axiom)
- [Countable forcing](#countable-forcing)
  - [One-Cohen-real preservation of GCH](#one-cohen-real-preservation-of-gch)
  - [Countable forcing preserves Suslin trees](#countable-forcing-preserves-suslin-trees)
  - [Ground-model uncountable subset lemma for countable forcing](#ground-model-uncountable-subset-lemma-for-countable-forcing)
- [Separative forcing order](#separative-forcing-order)
- [Forcing atom](#forcing-atom)
  - [A forcing atom determines a ground-model generic filter](#a-forcing-atom-determines-a-ground-model-generic-filter)
  - [Atomless forcing order](#atomless-forcing-order)
    - [Generic filter for an atomless order is new](#generic-filter-for-an-atomless-order-is-new)
- [Product forcing](#product-forcing)
  - [Mutual genericity for product forcing](#mutual-genericity-for-product-forcing)
  - [Projection of a product-generic filter](#projection-of-a-product-generic-filter)
- [Infinite-reservoir stem forcing](#infinite-reservoir-stem-forcing)
- [Unbounded real over a model](#unbounded-real-over-a-model)
- [Cardinal-preserving forcing](#cardinal-preserving-forcing)
- [Forcing name](#forcing-name)
  - [Forcing name rank](#forcing-name-rank)
  - [Choice preservation by well-ordered names](#choice-preservation-by-well-ordered-names)
  - [Nice forcing name](#nice-forcing-name)
  - [Paired forcing name](#paired-forcing-name)
  - [Forcing name for the complement of a generic filter](#forcing-name-for-the-complement-of-a-generic-filter)
  - [Evaluation of a forcing name](#evaluation-of-a-forcing-name)
  - [Canonical forcing name](#canonical-forcing-name)
- [Finite-function collapse to countable size](#finite-function-collapse-to-countable-size)
  - [GCH preservation by a finite-function collapse](#gch-preservation-by-a-finite-function-collapse)
- [Standard notation for forcing](#standard-notation-for-forcing)
- [Jerusalem notation for forcing](#jerusalem-notation-for-forcing)
- [Compatible forcing conditions](#compatible-forcing-conditions)
  - [Incompatible forcing conditions](#incompatible-forcing-conditions)
- [Dense subset of a forcing order](#dense-subset-of-a-forcing-order)
  - [Dense above a forcing condition](#dense-above-a-forcing-condition)
  - [Dense below a forcing condition](#dense-below-a-forcing-condition)
    - [Dense-below generic meeting lemma](#dense-below-generic-meeting-lemma)
- [Generic filter](#generic-filter)
  - [Maximal-antichain criterion for genericity](#maximal-antichain-criterion-for-genericity)
  - [Rasiowa–Sikorski lemma](#rasiowa-sikorski-lemma)
  - [Generic extension](#generic-extension)
    - [Power-set failure in an increasing union of generic extensions](#power-set-failure-in-an-increasing-union-of-generic-extensions)
    - [Power set in a generic extension](#power-set-in-a-generic-extension)
    - [Forcing theorem](#forcing-theorem)
      - [Forcing decision pattern](#forcing-decision-pattern)
      - [Forcing preserves ordinals](#forcing-preserves-ordinals)
      - [Forcing truth lemma](#forcing-truth-lemma)
      - [Forcing definability lemma](#forcing-definability-lemma)
      - [Semantic forcing relation](#semantic-forcing-relation)
      - [Syntactic forcing relation](#syntactic-forcing-relation)
        - [Atomic membership truth lemma for forcing](#atomic-membership-truth-lemma-for-forcing)
        - [Existential clause of syntactic forcing](#existential-clause-of-syntactic-forcing)
      - [Separation in a generic extension](#separation-in-a-generic-extension)
- [Countable transitive model](#countable-transitive-model)
- [Cohen forcing](#cohen-forcing)
  - [Cohen forcing two-level continuum plateau](#cohen-forcing-two-level-continuum-plateau)
- [Eventually different forcing](#eventually-different-forcing)
- [Fn forcing](#fn-forcing)
  - [Countable chain condition for finite-function forcing](#countable-chain-condition-for-finite-function-forcing)
  - [Generic coordinate reals for finite-function forcing](#generic-coordinate-reals-for-finite-function-forcing)
- [Chain condition for forcing](#chain-condition-for-forcing)
  - [Ground-model club containment lemma](#ground-model-club-containment-lemma)
  - [Possible-values lemma for chain-condition forcing](#possible-values-lemma-for-chain-condition-forcing)
    - [Cardinal preservation by chain-condition forcing](#cardinal-preservation-by-chain-condition-forcing)
  - [Countable chain condition for forcing](#countable-chain-condition-for-forcing)
    - [Knaster forcing](#knaster-forcing)
      - [Knaster forcing preserves Suslin trees](#knaster-forcing-preserves-suslin-trees)
- [Closed forcing](#closed-forcing)
  - [Closed forcing adds no short ground-valued sequences](#closed-forcing-adds-no-short-ground-valued-sequences)
  - [Countably closed forcing](#countably-closed-forcing)
    - [Diamond-sequence forcing](#diamond-sequence-forcing)
    - [Countable-condition collapse](#countable-condition-collapse)
  - [Closed forcing adds no short ordinal sequences](#closed-forcing-adds-no-short-ordinal-sequences)
    - [Cardinal preservation by closed forcing](#cardinal-preservation-by-closed-forcing)
- [Antichain in a forcing order](#antichain-in-a-forcing-order)
- [Centered subset of a forcing order](#centered-subset-of-a-forcing-order)
  - [Sigma-centered forcing](#sigma-centered-forcing)
- [Hechler forcing](#hechler-forcing)
  - [Dominating real](#dominating-real)
- [Nice name for a real](#nice-name-for-a-real)
- [Finite-condition Lévy collapse](#finite-condition-levy-collapse)
  - [Finite Lévy collapse to omega-one](#finite-levy-collapse-to-omega-one)
  - [Maximal-antichain sizes in the finite Lévy collapse](#maximal-antichain-sizes-in-the-finite-levy-collapse)

## Forcing antichain

↑ **Parent:** [Forcing](forcing.md)

A [subset](set.md#subset) of a [forcing](forcing.md) order whose distinct members have no common stronger extension. A maximal [forcing antichain](#forcing-antichain) has a compatible member for every condition. For [forcing](forcing.md) by nodes of a [set-theoretic tree](set.md#set-theoretic-tree), ordered by extension, this coincides with a [tree antichain](set.md#tree-antichain).

## Cardinal collapse

↑ **Parent:** [Forcing](forcing.md)

A [forcing](forcing.md) collapses a ground-model [cardinal](set-theory.md#cardinal-number) $\kappa$ if it forces a [bijection](function.md#bijection) from a smaller [ordinal](set-theory.md#ordinal) onto the ground [ordinal](set-theory.md#ordinal) $\kappa$. The [ordinal](set-theory.md#ordinal) itself is preserved; its being an initial [ordinal](set-theory.md#ordinal) is lost.

## Cofinality-preserving forcing

↑ **Parent:** [Forcing](forcing.md)

A [forcing](forcing.md) is cofinality-preserving over a [transitive model](set-theory.md#transitive-model) $M$ if every [generic extension](#generic-extension) has the same [cofinality](set-theory.md#cofinality) for every ground [ordinal](set-theory.md#ordinal). The values are compared as [ordinals](set-theory.md#ordinal), which [forcing](forcing.md) preserves.

<h2 id="martin-s-axiom">Martin's axiom</h2>

↑ **Parent:** [Forcing](forcing.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Martin's_axiom)

For a [cardinal number](set-theory.md#cardinal-number) $\kappa$, $\mathrm{MA}_\kappa$ says that for every [forcing](forcing.md) with the [countable chain condition for forcing](#countable-chain-condition-for-forcing) and every family of at most $\kappa$ dense [subsets](set.md#subset), some [filter in an ordered set](set.md#filter-mathematics) meets them all. Full Martin axiom asserts this for all $\kappa<2^{\aleph_0}$. The strict upper bound is part of the definition.

## Countable forcing

↑ **Parent:** [Forcing](forcing.md)

A forcing order that is countable inside the ground model. It has the countable chain condition and preserves $\omega_1$. Internal countability is distinct from external countability of the entire model.

### One-Cohen-real preservation of GCH

↑ **Parent:** [Countable forcing](#countable-forcing)

Over a [Generalized continuum hypothesis](set-theory.md#generalized-continuum-hypothesis) ground model, adding one Cohen real preserves every infinite power $2^\lambda=\lambda^+$. For the countable [forcing](forcing.md), nice [subset](set.md#subset) [forcing names](#forcing-name) for $\lambda$ number at most $(2^{\aleph_0})^\lambda=2^\lambda$ in the ground model. Old [subsets](set.md#subset) give the matching lower bound and the [countable chain condition for forcing](#countable-chain-condition-for-forcing) preserves [cardinals](set-theory.md#cardinal-number). Starting from the [constructible universe](definable-power-set.md#constructible-universe), the new real is nonconstructible while the constructible levels remain unchanged.

### Countable forcing preserves Suslin trees

↑ **Parent:** [Countable forcing](#countable-forcing)

A ground-model [Suslin tree](set.md#suslin-tree) remains Suslin after countable forcing. A new uncountable chain or antichain would contain an uncountable ground-model subset by the [ground-model uncountable subset lemma for countable forcing](#ground-model-uncountable-subset-lemma-for-countable-forcing).

### Ground-model uncountable subset lemma for countable forcing

↑ **Parent:** [Countable forcing](#countable-forcing)

An uncountable set of ground-model elements in a [generic extension](#generic-extension) by countable forcing contains an uncountable ground-model subset. Partition membership witnesses according to the countably many forcing conditions.

## Separative forcing order

↑ **Parent:** [Forcing](forcing.md)

In [standard notation for forcing](#standard-notation-for-forcing), an order is separative if $p\not\leq q$ implies that some $r\leq p$ is incompatible with $q$. Separativity does not imply an [atomless forcing order](#atomless-forcing-order): the one-point order is separative and has a [forcing atom](#forcing-atom). Its only [generic filter](#generic-filter) is a ground-model set. Atomlessness is the hypothesis in [generic filter for an atomless order is new](#generic-filter-for-an-atomless-order-is-new).

## Forcing atom

↑ **Parent:** [Forcing](forcing.md)

A condition is an atom if every two stronger conditions are [compatible forcing conditions](#compatible-forcing-conditions). This is a compatibility definition, not necessarily minimality in an arbitrary [partial order](set.md#partially-ordered-set). An [atomless forcing order](#atomless-forcing-order) is one in which every condition has two incompatible strengthenings.

### A forcing atom determines a ground-model generic filter

↑ **Parent:** [Forcing atom](#forcing-atom)

For a [forcing atom](#forcing-atom) $p$ in a ground-model [forcing](forcing.md) order, $G_p$ is a ground-model [generic filter](#generic-filter). It contains $p$ and is upward closed. For $q,r\in G_p$, choose $q'\leq p,q$ and $r'\leq p,r$. The atom property gives $s\leq q',r'$, so $s\in G_p$ is a common strengthening of $q,r$. Thus $G_p$ is a [filter in an ordered set](set.md#filter-mathematics). Every [dense subset of a forcing order](#dense-subset-of-a-forcing-order) has some $d\leq p$, and $d\in G_p$. The defining compatibility predicate is bounded to the ground-model [set](set.md) of conditions, so [axiom schema of separation](set-theory.md#axiom-schema-of-specification) forms $G_p$ inside the ground model. For a nonminimal atom, this filter can strictly contain the [principal filter](set.md#principal-filter-in-an-ordered-set) above $p$.

### Atomless forcing order

↑ **Parent:** [Forcing atom](#forcing-atom)

An order is atomless if it has no [forcing atom](#forcing-atom), equivalently every condition has a pair of [incompatible forcing conditions](#incompatible-forcing-conditions) below it. For a fixed order belonging to a [transitive model](set-theory.md#transitive-model), this property is absolute because its quantifiers range over the unchanged [set](set.md) of conditions. Infinite-domain [Fn forcing](#fn-forcing) with at least two possible values is atomless: prescribe different values at one fresh coordinate.

#### Generic filter for an atomless order is new

↑ **Parent:** [Atomless forcing order](#atomless-forcing-order)

If a [generic filter](#generic-filter) $G$ for an [atomless forcing order](#atomless-forcing-order) belonged to its ground model, then the complement $\mathbb P\setminus G$ would be a dense ground-model [set](set.md). A condition outside $G$ is already there; a condition in $G$ has two incompatible strengthenings, at least one outside its directed filter. Genericity would then require meeting the complement, a contradiction.

## Product forcing

↑ **Parent:** [Forcing](forcing.md)

The conditions are pairs with coordinatewise extension: $(p,q)\leq(p',q')$ exactly when $p\leq p'$ and $q\leq q'$. The [projection of a product-generic filter](#projection-of-a-product-generic-filter) is a pair of factor filters whose [Cartesian product](set-theory.md#cartesian-product) is the original filter. Each is ground-model generic, and [mutual genericity for product forcing](#mutual-genericity-for-product-forcing) makes the second generic over the extension by the first.

### Mutual genericity for product forcing

↑ **Parent:** [Product forcing](#product-forcing)

If $H=G_0\times G_1$ is generic for [product forcing](#product-forcing) over $M$, then $G_1$ is generic over $M[G_0]$. For a name $\dot D$ for a dense [subset](set.md#subset) of the second factor, take $p_0\in G_0$ forcing density. Ground-model pairs with first coordinate incompatible with $p_0$, or with first coordinate below $p_0$ forcing the second into $\dot D$, form a dense product [set](set.md). The [existential clause of syntactic forcing](#existential-clause-of-syntactic-forcing) and the membership clause for a [canonical forcing name](#canonical-forcing-name) give the density witnesses. The product filter meets this [set](set.md), cannot use the incompatible case, and hence its second projection meets $\dot D^{G_0}$.

### Projection of a product-generic filter

↑ **Parent:** [Product forcing](#product-forcing)

For a [generic filter](#generic-filter) $H$ in [product forcing](#product-forcing), let $G_0,G_1$ be its coordinate projections. They are [filters in an ordered set](set.md#filter-mathematics). Given $p\in G_0$ and $q\in G_1$, choose separate pairs witnessing their membership and then a common strengthening in $H$. Upward closure puts $(p,q)$ in $H$, proving the displayed equality. Every ground-model dense factor [set](set.md) lifts to a dense product [set](set.md), proving genericity of each projection over the ground model.

## Infinite-reservoir stem forcing

↑ **Parent:** [Forcing](forcing.md)

A condition consists of a finite sequence and an infinite reservoir of allowed future values. A stronger condition extends the sequence, shrinks the reservoir, and takes all newly appended values from the old reservoir. Stem values may repeat. The union of the generic stems is an [unbounded real over a model](#unbounded-real-over-a-model): for every ground-model function $g$ and every threshold $K$, the conditions whose stem already has some $k\geq K$ with $g(k)<s(k)$ form a [dense subset of a forcing order](#dense-subset-of-a-forcing-order). An infinite subset of $\omega$ always supplies a sufficiently large value.

## Unbounded real over a model

↑ **Parent:** [Forcing](forcing.md)

A function $f\in\omega^\omega$ is unbounded over a model $M$ if for every $g\in M\cap\omega^\omega$, infinitely many $k$ satisfy $g(k)<f(k)$. Equivalently, no ground-model function eventually dominates it. This is weaker than being a [dominating real](#dominating-real) over $M$.

## Cardinal-preserving forcing

↑ **Parent:** [Forcing](forcing.md)

A forcing order preserves cardinals over a ground model if every ground-model [cardinal number](set-theory.md#cardinal-number) remains a cardinal in every [generic extension](#generic-extension). This assertion and any sufficient [chain condition for forcing](#chain-condition-for-forcing) are evaluated inside the ground model. External countability of a [countable transitive model](#countable-transitive-model) does not make all of its forcing orders internally ccc.

## Forcing name

↑ **Parent:** [Forcing](forcing.md)

A forcing name is a recursively built set of pairs $(\sigma,p)$, where $\sigma$ is a lower-rank forcing name and $p$ is a forcing condition. Ground-model names are interpreted using a [generic filter](#generic-filter) to form the [generic extension](#generic-extension).

### Forcing name rank

↑ **Parent:** [Forcing name](#forcing-name)

The [ordinal](set-theory.md#ordinal) assigned recursively by $\operatorname{nrk}(\tau)=\sup\{\operatorname{nrk}(\sigma)+1:(\sigma,p)\in\tau\}$. It measures dependency on subnames and justifies generic evaluation by recursion. The ordinary [rank of a set](set-theory.md#rank-of-a-set) also accounts for the coding of the [ordered pairs](set.md#ordered-pair) and the [forcing](forcing.md) conditions; it need not equal this dependency [rank of a set](set-theory.md#rank-of-a-set).

### Choice preservation by well-ordered names

↑ **Parent:** [Forcing name](#forcing-name)

If the ground model has [axiom of choice](set-theory.md#axiom-of-choice), [well-order](set.md#well-order) the [set](set.md) of subnames appearing in a [forcing name](#forcing-name) for an arbitrary extension [set](set.md). Evaluate those activated by the [generic filter](#generic-filter). Each element of the extension [set](set.md) has a least preimage index; ordering by these indices [well-orders](set.md#well-order) the [set](set.md). Only ground choice and the [ZF](set-theory.md#zermelo-fraenkel-set-theory) part of the [forcing theorem](#forcing-theorem) are needed.

### Nice forcing name

↑ **Parent:** [Forcing name](#forcing-name)

A name for a subset of a ground-model set, given coordinatewise by [antichains in a forcing order](#antichain-in-a-forcing-order). For countable-chain-condition forcing, each coordinate uses a countable antichain, which bounds the number of names for reals.

### Paired forcing name

↑ **Parent:** [Forcing name](#forcing-name)

For the condition-first [forcing name](#forcing-name) convention, pair every condition with each of two names $\tau,\tau'$. Under any nonempty [generic filter](#generic-filter), the [evaluation of a forcing name](#evaluation-of-a-forcing-name) is then $\{\tau_G,\tau'_G\}$, the unordered pair of the two values. Equal values give a singleton. With the name-first convention, reverse the two components of each syntactic pair.

### Forcing name for the complement of a generic filter

↑ **Parent:** [Forcing name](#forcing-name)

The [forcing name](#forcing-name) $\{(\check p,q):p,q\in\mathbb P,\ q\perp p\}$ evaluates to $\mathbb P\setminus G$. If $p\notin G$, genericity applied to $\{q:q\leq p\text{ or }q\perp p\}$ supplies an incompatible member of $G$. If $p\in G$, directedness prevents such a member.

### Evaluation of a forcing name

↑ **Parent:** [Forcing name](#forcing-name)

Interpret a [forcing name](#forcing-name) recursively by $\operatorname{val}(\tau,G)=\{\operatorname{val}(\sigma,G):\exists p\in G\ ((\sigma,p)\in\tau)\}$. The collection of interpreted ground-model names is the [generic extension](#generic-extension).

### Canonical forcing name

↑ **Parent:** [Forcing name](#forcing-name)

The canonical forcing name for a ground-model set $x$ is $\check x=\{(\check y,\mathbf1):y\in x\}$. Its [evaluation of a forcing name](#evaluation-of-a-forcing-name) under every [generic filter](#generic-filter) is $x$.

## Finite-function collapse to countable size

↑ **Parent:** [Forcing](forcing.md)

For an infinite ground-model [cardinal number](set-theory.md#cardinal-number) $\kappa$, use finite [partial functions](function.md#partial-function) from $\omega$ to $\kappa$, ordered by reverse inclusion. The union of a [generic filter](#generic-filter) is a surjection $\omega\to\kappa$. The order has size $\kappa$, hence the $\kappa^+$-chain condition, and preserves cardinals at least $\kappa^+$.

### GCH preservation by a finite-function collapse

↑ **Parent:** [Finite-function collapse to countable size](#finite-function-collapse-to-countable-size)

If the ground model satisfies the [Generalized continuum hypothesis](set-theory.md#generalized-continuum-hypothesis), a [finite-function collapse to countable size](#finite-function-collapse-to-countable-size) of $\kappa$ preserves it. The old $\kappa^+$ becomes the new $\aleph_1$, and there are at most $2^\kappa=\kappa^+$ names for subsets of $\omega$. For every old cardinal $\lambda\geq\kappa^+$ there are at most $2^{\lambda\cdot\kappa}=2^\lambda=\lambda^+$ names for subsets of $\lambda$. [Cardinal preservation by chain-condition forcing](#cardinal-preservation-by-chain-condition-forcing) and [Cantor theorem](set.md#cantor-s-theorem) turn these upper bounds into the required equalities.

## Standard notation for forcing

↑ **Parent:** [Forcing](forcing.md)

In standard forcing notation, $q\leq p$ says that $q$ is stronger than $p$: the smaller condition carries more information.

## Jerusalem notation for forcing

↑ **Parent:** [Forcing](forcing.md)

In Jerusalem notation, $p\leq q$ says that $q$ is stronger than $p$: the larger condition carries more information.

## Compatible forcing conditions

↑ **Parent:** [Forcing](forcing.md)

Two forcing conditions are compatible when they have a common stronger extension. In standard notation this means that some $r$ satisfies $r\leq p,q$; in [Jerusalem notation for forcing](#jerusalem-notation-for-forcing) it means that some $r$ satisfies $p,q\leq r$.

### Incompatible forcing conditions

↑ **Parent:** [Compatible forcing conditions](#compatible-forcing-conditions)

Two forcing conditions are incompatible when they have no common stronger extension.

## Dense subset of a forcing order

↑ **Parent:** [Forcing](forcing.md)

A subset $D$ of a [forcing](forcing.md) order $P$ is dense if every $p\in P$ has a stronger condition $q\leq p$ in $D$. This order-density condition is the one used by a [generic filter](#generic-filter); it is distinct from density in an arbitrarily specified topology.

### Dense above a forcing condition

↑ **Parent:** [Dense subset of a forcing order](#dense-subset-of-a-forcing-order)

For the convention that larger conditions are stronger, density above $p$ means every strengthening of $p$ has a further strengthening in $D$. It is the extension-cone density usually called [dense below a forcing condition](#dense-below-a-forcing-condition) when smaller conditions are stronger. The sign must be translated with the order convention, rather than copied unchanged.

### Dense below a forcing condition

↑ **Parent:** [Dense subset of a forcing order](#dense-subset-of-a-forcing-order)

A set $D\subseteq\mathbb P$ is dense below $p$ when every $q\leq p$ has an extension $r\leq q$ belonging to $D$.

#### Dense-below generic meeting lemma

↑ **Parent:** [Dense below a forcing condition](#dense-below-a-forcing-condition)

If $p\in G$ and a ground-model [set](set.md) $D$ is [dense below a forcing condition](#dense-below-a-forcing-condition) $p$, then the [generic filter](#generic-filter) $G$ meets $D$. Add all [incompatible forcing conditions](#incompatible-forcing-conditions) with $p$ to $D$. The enlarged [set](set.md) is globally dense: a condition compatible with $p$ first has a common strengthening, then a further strengthening in $D$. Genericity meets the enlargement, and directedness excludes its incompatible part.

## Generic filter

↑ **Parent:** [Forcing](forcing.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generic_filter)

A filter $G\subseteq\mathbb P$ is generic over a model $M$ when it meets every dense subset of $\mathbb P$ belonging to $M$.

### Maximal-antichain criterion for genericity

↑ **Parent:** [Generic filter](#generic-filter)

A filter is generic over its ground model exactly when it meets each ground-model maximal [forcing antichain](#forcing-antichain) in one point. Extensions of a maximal antichain form a dense set, while any ground dense set contains an antichain maximal in the whole [forcing](forcing.md). Directedness permits at most one antichain member in a filter.

<h3 id="rasiowa-sikorski-lemma">Rasiowa–Sikorski lemma</h3>

↑ **Parent:** [Generic filter](#generic-filter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rasiowa–Sikorski_lemma)

If $M$ is a [countable transitive model](#countable-transitive-model), $\mathbb P\in M$, and $p\in\mathbb P$, enumerate the dense subsets of $\mathbb P$ belonging to $M$ and recursively choose a decreasing sequence starting below $p$ that meets each one. Its upward closure is a [generic filter](#generic-filter) over $M$ containing $p$.

### Generic extension

↑ **Parent:** [Generic filter](#generic-filter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generic_extension)

If $G$ is a [generic filter](#generic-filter) over a [countable transitive model](#countable-transitive-model) $M$, the generic extension $M[G]$ consists of the interpretations by $G$ of all forcing names in $M$.

#### Power-set failure in an increasing union of generic extensions

↑ **Parent:** [Generic extension](#generic-extension)

Let $M_{n+1}=M_n[G_n]$ for a fixed [atomless forcing order](#atomless-forcing-order) $\mathbb P$, and $N=\bigcup_{n<\omega}M_n$. If a [set](set.md) $A\in N$ were its internal [power set](set.md#power-set) of $\mathbb P$, choose $n$ with $A\in M_n$. The next [generic filter](#generic-filter) $G_n$ belongs to $N$, so $G_n\in A$; transitivity of $M_n$ implies $G_n\in M_n$, contradicting [generic filter for an atomless order is new](#generic-filter-for-an-atomless-order-is-new). The chain is increasing but need not be an elementary chain.

#### Power set in a generic extension

↑ **Parent:** [Generic extension](#generic-extension)

For a [forcing name](#forcing-name) $\tau$, let $U$ consist of pairs $(\rho,p)$ where $(\rho,r)\in\tau$ for some $r\geq p$. Every ground-model [subset](set.md#subset) $\nu$ of $U$ is a name whose value is contained in $\tau^G$. Every subset $\sigma^G\subseteq\tau^G$ has an equivalent such name: retain those $(\rho,p)\in U$ with $p\Vdash\rho\in\sigma$. The [atomic membership truth lemma for forcing](#atomic-membership-truth-lemma-for-forcing) proves equality of values. Collect all these names from the ground-model [power set](set.md#power-set) $\mathcal P^M(U)$ into a single outer name, pairing each with every condition. Its value is the full internal [power set](set.md#power-set), without presupposing that power set in the extension.

#### Forcing theorem

↑ **Parent:** [Generic extension](#generic-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Forcing_theorem)

The forcing theorem identifies truth in a [generic extension](#generic-extension) with the forcing relation: a formula is true in $M[G]$ exactly when some condition in $G$ forces it.

##### Forcing decision pattern

↑ **Parent:** [Forcing theorem](#forcing-theorem)

For a name with finitely many possible values, record which value each condition forces, using an extra marker for undecided conditions. Equal patterns mean that any condition deciding one entry decides all entries with that pattern identically.

##### Forcing preserves ordinals

↑ **Parent:** [Forcing theorem](#forcing-theorem)

A generic extension of a transitive model has exactly the same ordinals as its ground model. Rank induction on names bounds every value; transitivity and agreement on membership make ordinalhood absolute.

##### Forcing truth lemma

↑ **Parent:** [Forcing theorem](#forcing-theorem)

A formula holds in a [generic extension](#generic-extension) exactly when some condition in the [generic filter](#generic-filter) forces it for names of its parameters.

##### Forcing definability lemma

↑ **Parent:** [Forcing theorem](#forcing-theorem)

For each formula, its forcing relation on names and conditions is uniformly first-order definable inside the ground model. This permits ground-model separation and replacement using forcing predicates.

##### Semantic forcing relation

↑ **Parent:** [Forcing theorem](#forcing-theorem)

For a [countable transitive model](#countable-transitive-model) $M$, semantic forcing declares $p\Vdash\varphi$ when every [generic filter](#generic-filter) $G$ over $M$ containing $p$ gives $M[G]\models\varphi$.

##### Syntactic forcing relation

↑ **Parent:** [Forcing theorem](#forcing-theorem)

The syntactic forcing relation is defined recursively inside the ground model from the ranks of forcing names and the logical complexity of $\varphi$. The [forcing theorem](#forcing-theorem) proves that it agrees with the [semantic forcing relation](#semantic-forcing-relation).

###### Atomic membership truth lemma for forcing

↑ **Parent:** [Syntactic forcing relation](#syntactic-forcing-relation)

For [forcing names](#forcing-name) $\sigma,\tau$ and a [generic filter](#generic-filter) $G$, $\sigma^G\in\tau^G$ exactly when some $p\in G$ syntactically forces $\sigma\in\tau$. Assuming the equality truth lemma, interpreted membership supplies an active pair $(\rho,r)\in\tau$ and a condition in $G$ forcing $\sigma=\rho$; a common strengthening forces membership. Conversely the defining equality witnesses occur [dense below a forcing condition](#dense-below-a-forcing-condition) forcing membership. The [dense-below generic meeting lemma](#dense-below-generic-meeting-lemma) supplies one in $G$, and the equality truth lemma recovers interpreted membership.

###### Existential clause of syntactic forcing

↑ **Parent:** [Syntactic forcing relation](#syntactic-forcing-relation)

For the usual recursive [syntactic forcing relation](#syntactic-forcing-relation), $p\Vdash^*\exists x\,\varphi(x)$ means that conditions $q\leq p$ forcing $\varphi(\sigma)$ for some [forcing name](#forcing-name) $\sigma$ are [dense below a forcing condition](#dense-below-a-forcing-condition) $p$. This density clause proves the existential step of the [forcing theorem](#forcing-theorem) from the truth lemma for each named instance. A [generic filter](#generic-filter) containing $p$ meets that dense set after it is augmented by conditions incompatible with $p$.

##### Separation in a generic extension

↑ **Parent:** [Forcing theorem](#forcing-theorem)

Let $\dot x,\dot a_1,\ldots,\dot a_n$ be forcing names and let $\varphi$ be a formula. The name

$$
\dot y=\{(\tau,r):\exists q\,((\tau,q)\in\dot x\land r\leq q\land r\Vdash^*\varphi(\tau,\dot a_1,\ldots,\dot a_n))\}
$$

belongs to the ground model by [axiom schema of separation](set-theory.md#axiom-schema-of-specification). The [forcing theorem](#forcing-theorem) shows that its value in a generic extension is exactly

$$
\dot y^G=\{z\in\dot x^G:M[G]\models\varphi(z,\dot a_1^G,\ldots,\dot a_n^G)\}.
$$

Consequently every [generic extension](#generic-extension) satisfies the separation schema.

## Countable transitive model

↑ **Parent:** [Forcing](forcing.md)

A countable transitive model is a countable set $M$ such that membership on $M$ is the actual membership relation, $M$ is transitive, and $(M,\in)$ satisfies the specified axioms of set theory.

A countable transitive model is in particular a [standard model (set theory)](set-theory.md#standard-model-set-theory) with both countability and transitivity.

## Cohen forcing

↑ **Parent:** [Forcing](forcing.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cohen_forcing)

Cohen forcing consists of finite partial approximations to a new subset or function, ordered by reverse inclusion. Meeting the ground-model dense sets makes the union a total generic object.

### Cohen forcing two-level continuum plateau

↑ **Parent:** [Cohen forcing](#cohen-forcing)

Over a model of [Generalized continuum hypothesis](set-theory.md#generalized-continuum-hypothesis), add $\aleph_3$ Cohen reals with finite binary [partial functions](function.md#partial-function). The [Delta-system lemma](set-theory.md#delta-system-lemma) proves the [countable chain condition for forcing](#countable-chain-condition-for-forcing). The generic reals give the continuum lower bound $\aleph_3$, while nice [forcing names](#forcing-name) for [subsets](set.md#subset) of $\omega_1$ number at most $(\aleph_3)^{\aleph_1}=\aleph_3$ in the ground model. [Cardinal](set-theory.md#cardinal-number) preservation then gives $2^{\aleph_0}=2^{\aleph_1}=\aleph_3$.

## Eventually different forcing

↑ **Parent:** [Forcing](forcing.md)

An eventually different condition is a finite sequence together with finitely many ground-model functions that all newly appended coordinates must avoid. The generic union eventually differs from every ground-model function.

## Fn forcing

↑ **Parent:** [Forcing](forcing.md)

The order $\operatorname{Fn}(X,Y,\kappa)$ consists of partial functions $p:X\rightharpoonup Y$ with $|\operatorname{dom}p|<\kappa$, ordered by reverse inclusion so that larger functions are stronger conditions.

### Countable chain condition for finite-function forcing

↑ **Parent:** [Fn forcing](#fn-forcing)

The order $\operatorname{Fn}(X,Y,\omega)$ has the [countable chain condition for forcing](#countable-chain-condition-for-forcing) whenever $Y$ is countable. For an uncountable family of conditions, apply the [Delta-system lemma](set-theory.md#delta-system-lemma) to the finite domains. On their common finite root there are only countably many assignments, so thin to an uncountable family agreeing on that root. Any two conditions now have a compatible union. For binary [Cohen forcing](#cohen-forcing), there are only finitely many root assignments.

### Generic coordinate reals for finite-function forcing

↑ **Parent:** [Fn forcing](#fn-forcing)

For [Fn forcing](#fn-forcing) on $\kappa\times\omega$ with values in $2$, the [generic filter](#generic-filter) union is total by the dense coordinate-domain requirements. For each pair of distinct rows, the [set](set.md) of conditions giving them opposite bits at some column is dense: choose a column untouched in both finite rows. Thus the rows are distinct [subsets](set.md#subset) of $\omega$ and provide an [injective function](algebra.md#injective-function) from the ground-model [ordinal](set-theory.md#ordinal) $\kappa$ into the extension's [power set](set.md#power-set) of $\omega$. This construction alone does not prove preservation of its ground-model [cardinal number](set-theory.md#cardinal-number) status.

## Chain condition for forcing

↑ **Parent:** [Forcing](forcing.md)

A forcing order has the $\kappa$-chain condition when every antichain has cardinality below $\kappa$. It preserves cardinals and cofinalities at least $\kappa$.

### Ground-model club containment lemma

↑ **Parent:** [Chain condition for forcing](#chain-condition-for-forcing)

If forcing has the $\kappa$-chain condition for a regular uncountable $\kappa$, every forced club subset of $\kappa$ contains a ground-model club below the forcing condition. Bound the possible witnesses above each ordinal using antichains, then take closure points of the bound function.

### Possible-values lemma for chain-condition forcing

↑ **Parent:** [Chain condition for forcing](#chain-condition-for-forcing)

Suppose $\mathbb P$ has the $\kappa$-chain condition and $\dot f$ is forced to be a function from an ordinal $\mu$ to an ordinal $\lambda$. For each $\xi<\mu$, a maximal [antichain in a forcing order](#antichain-in-a-forcing-order) deciding $\dot f(\xi)$ has size below $\kappa$. Hence the ground model has a set $B_\xi\subseteq\lambda$ of size below $\kappa$ containing every possible value of $\dot f(\xi)$.

#### Cardinal preservation by chain-condition forcing

↑ **Parent:** [Possible-values lemma for chain-condition forcing](#possible-values-lemma-for-chain-condition-forcing)

If $\kappa$ is a [regular cardinal](set-theory.md#regular-cardinal) and $\mathbb P$ has the $\kappa$-chain condition, then forcing with $\mathbb P$ preserves every [cardinal number](set-theory.md#cardinal-number) and [cofinality](set-theory.md#cofinality) at least $\kappa$. Indeed, a proposed surjection $f:\mu\to\lambda$ with $\mu<\lambda$ has its range contained in $\bigcup_{\xi<\mu}B_\xi$ from the [possible-values lemma for chain-condition forcing](#possible-values-lemma-for-chain-condition-forcing). The regularity of $\kappa$ and [infinite cardinal arithmetic](set-theory.md#infinite-cardinal-arithmetic) make this union have cardinality below the ground-model cardinal $\lambda$, a contradiction.

### Countable chain condition for forcing

↑ **Parent:** [Chain condition for forcing](#chain-condition-for-forcing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Countable_chain_condition_for_forcing)

A forcing order has the countable chain condition when every [antichain in a forcing order](#antichain-in-a-forcing-order) is [countable](set-theory.md#countable-set). Such forcing preserves cardinals and cofinalities at least $\aleph_1$.

#### Knaster forcing

↑ **Parent:** [Countable chain condition for forcing](#countable-chain-condition-for-forcing)

Every uncountable [subset](set.md#subset) of a Knaster [forcing](forcing.md) has an uncountable pairwise compatible [subset](set.md#subset). The property implies the [countable chain condition for forcing](#countable-chain-condition-for-forcing). Finite [Cohen forcing](#cohen-forcing) has this property by the [delta-system lemma](set-theory.md#delta-system-lemma) and agreement on the finite root. A Knaster [forcing](forcing.md) times any [CCC](#countable-chain-condition-for-forcing) [forcing](forcing.md) is [CCC](#countable-chain-condition-for-forcing)

##### Knaster forcing preserves Suslin trees

↑ **Parent:** [Knaster forcing](#knaster-forcing)

If $T$ is a normal splitting [Suslin tree](set.md#suslin-tree) and $P$ is Knaster, then $P\times T$ is [CCC](#countable-chain-condition-for-forcing), so $P$ forces that the ground tree is still [CCC](#countable-chain-condition-for-forcing) Countable levels and splitting persist. A new [cofinal branch](set.md#cofinal-branch) would give an uncountable antichain by splitting, so none is added. This permits adding many Cohen reals while retaining a Suslin tree, and distinguishes Knaster preservation from an unjustified preservation claim for every [CCC](#countable-chain-condition-for-forcing) [forcing](forcing.md).

## Closed forcing

↑ **Parent:** [Forcing](forcing.md)

A forcing order is $\kappa$-closed when every decreasing sequence of conditions of length below $\kappa$ has a lower bound. Countably closed forcing adds no new countable sequences of ground-model elements and in particular adds no new real numbers.

### Closed forcing adds no short ground-valued sequences

↑ **Parent:** [Closed forcing](#closed-forcing)

If a [forcing](forcing.md) is $\kappa$-closed in the ground model, then it adds no [functions](function.md) from a ground [ordinal](set-theory.md#ordinal) $\alpha<\kappa$ into a ground [set](set.md) $B$. Recursively decide each value inside the ground model and take common stronger bounds at limit stages and after the final step. Conditions deciding a whole ground [function](function.md) are dense below any condition asserting this type of [function](function.md). The [dense-below generic meeting lemma](#dense-below-generic-meeting-lemma) ensures the [generic filter](#generic-filter) meets that [dense subset of a forcing order](#dense-subset-of-a-forcing-order). One arbitrary bound need not be in the [filter in an ordered set](set.md#filter-mathematics).

### Countably closed forcing

↑ **Parent:** [Closed forcing](#closed-forcing)

Every descending countable sequence of conditions has a common stronger condition. This is $\omega_1$-closed forcing and adds no countable ordinal sequences.

#### Diamond-sequence forcing

↑ **Parent:** [Countably closed forcing](#countably-closed-forcing)

Conditions are countable successor-length sequences $\langle A_\xi\subseteq\xi\rangle$, ordered by end extension. A countable fusion construction decides a named subset below a fresh limit index and writes that trace at the index inside any named club. The generic sequence satisfies the [diamond principle](set-theory.md#diamond-principle).

#### Countable-condition collapse

↑ **Parent:** [Countably closed forcing](#countably-closed-forcing)

Countable partial functions from $\omega_1$ to a nonempty ground-model set $A$, ordered by extension, add a surjection $\omega_1\to A$. Countable closure preserves $\omega_1$ and adds no reals.

### Closed forcing adds no short ordinal sequences

↑ **Parent:** [Closed forcing](#closed-forcing)

If a ground-model order is $\lambda$-closed, it adds no ordinal-valued functions with domain $\mu<\lambda$. Recursively decide each name value inside the ground model, using closure at intermediate limit stages and once more at the end. Below each starting condition, conditions deciding the entire function are dense. A [generic filter](#generic-filter) meets them by the [dense-below generic meeting lemma](#dense-below-generic-meeting-lemma). The recursion must be internal to the ground model, since its closure property only covers its own sequences.

#### Cardinal preservation by closed forcing

↑ **Parent:** [Closed forcing adds no short ordinal sequences](#closed-forcing-adds-no-short-ordinal-sequences)

A $\lambda$-[closed forcing](#closed-forcing) order preserves a ground-model [cardinal number](set-theory.md#cardinal-number) $\lambda$, even when it is singular. A proposed surjection from an ordinal below $\lambda$ to $\lambda$ would be an old function because [closed forcing adds no short ordinal sequences](#closed-forcing-adds-no-short-ordinal-sequences), contradicting old cardinalhood. This concerns $\lambda$ and smaller cardinals; closure alone does not supply preservation of all larger cardinals.

## Antichain in a forcing order

↑ **Parent:** [Forcing](forcing.md)

An antichain in a forcing order is a set of pairwise [incompatible forcing conditions](#incompatible-forcing-conditions).

## Centered subset of a forcing order

↑ **Parent:** [Forcing](forcing.md)

A subset of a forcing order is centered when every finite collection of its conditions has a common stronger extension.

### Sigma-centered forcing

↑ **Parent:** [Centered subset of a forcing order](#centered-subset-of-a-forcing-order)

A forcing order is sigma-centered when it is the union of countably many [centered subsets](#centered-subset-of-a-forcing-order). Every sigma-centered forcing has the [countable chain condition for forcing](#countable-chain-condition-for-forcing).

## Hechler forcing

↑ **Parent:** [Forcing](forcing.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hechler_forcing)

A Hechler condition is a pair $(s,f)$ consisting of a finite sequence $s\in\omega^{<\omega}$ and a function $f\in\omega^\omega$. An extension lengthens the stem, increases the side function, and places every new stem value above the old side function. The generic union is a [dominating real](#dominating-real).

### Dominating real

↑ **Parent:** [Hechler forcing](#hechler-forcing)

A function $d\in\omega^\omega$ dominates $h\in\omega^\omega$ when $d(n)>h(n)$ for all but finitely many $n$. A dominating real over a ground model dominates every such function belonging to that model.

## Nice name for a real

↑ **Parent:** [Forcing](forcing.md)

For a forcing order with the [countable chain condition for forcing](#countable-chain-condition-for-forcing), a real can be represented by a nice name determined by a countable [antichain in a forcing order](#antichain-in-a-forcing-order) for each natural-number coordinate. This bounds the number of reals in the extension in terms of the size of the forcing order.

<h2 id="finite-condition-levy-collapse">Finite-condition Lévy collapse</h2>

↑ **Parent:** [Forcing](forcing.md)

The finite-condition Lévy collapse $\operatorname{Lv}(\kappa)$ consists of finite [partial functions](function.md#partial-function) $p$ with $\operatorname{dom}p\subseteq\kappa\times\omega$ and $p(\alpha,n)<\alpha$, ordered by reverse inclusion. The generic union gives a surjection $\omega\to\alpha$ for every infinite $\alpha<\kappa$. If $\kappa$ is regular and uncountable, the [Delta-system lemma at a regular uncountable cardinal](set-theory.md#delta-system-lemma-at-a-regular-uncountable-cardinal) proves the $\kappa$-chain condition, so the extension makes $\kappa=\aleph_1$.

<h3 id="finite-levy-collapse-to-omega-one">Finite Lévy collapse to omega-one</h3>

↑ **Parent:** [Finite-condition Lévy collapse](#finite-condition-levy-collapse)

With $\kappa$ an uncountable [regular cardinal](set-theory.md#regular-cardinal), finite [partial functions](function.md#partial-function) on $\kappa\times\omega$ assigning a value below the first coordinate collapse every ground [ordinal](set-theory.md#ordinal) below $\kappa$ to countable size. The [Delta-system lemma](set-theory.md#delta-system-lemma) gives the $\kappa$ [chain in a partial order](set.md#chain-in-a-partial-order) condition; the [possible-values lemma for chain-condition forcing](#possible-values-lemma-for-chain-condition-forcing) then preserves the regularity of $\kappa$. Therefore $\kappa$ becomes the extension $\omega_1$. Strong inaccessibility is enough but is not needed for this identification.

<h3 id="maximal-antichain-sizes-in-the-finite-levy-collapse">Maximal-antichain sizes in the finite Lévy collapse</h3>

↑ **Parent:** [Finite-condition Lévy collapse](#finite-condition-levy-collapse)

For a regular uncountable $\kappa$, the finite-condition collapse has the $\kappa$ [chain in a partial order](set.md#chain-in-a-partial-order) condition, by a regular-cardinal [Delta-system lemma](set-theory.md#delta-system-lemma) and thinning to identical assignments on the finite root. Thus every maximal [forcing antichain](#forcing-antichain) has ground-model size less than $\kappa$. There is no fixed size: for any nonzero [cardinal](set-theory.md#cardinal-number) $\mu<\kappa$, assigning all values below $\mu$ at the one coordinate $(\mu,0)$ is a maximal [forcing antichain](#forcing-antichain) of size $\mu$.

## ↑ Ancestors (5)

1. [Set theory](set-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (38)

- [A forcing atom determines a ground-model generic filter](#a-forcing-atom-determines-a-ground-model-generic-filter)
- [Cardinal collapse](#cardinal-collapse)
- [Closed forcing adds no short ground-valued sequences](#closed-forcing-adds-no-short-ground-valued-sequences)
- [Cofinality-preserving forcing](#cofinality-preserving-forcing)
- [Dense subset of a forcing order](#dense-subset-of-a-forcing-order)
- [Forcing antichain](#forcing-antichain)
- [Forcing name rank](#forcing-name-rank)
- [Knaster forcing](#knaster-forcing)
- [Knaster forcing preserves Suslin trees](#knaster-forcing-preserves-suslin-trees)
- [Martin's axiom](#martin-s-axiom)
- [Maximal-antichain criterion for genericity](#maximal-antichain-criterion-for-genericity)
- [One-Cohen-real preservation of GCH](#one-cohen-real-preservation-of-gch)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#5/solution)
- [Paper 19](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#4/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#4/ii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#4/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#5/ii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/ii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/iii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#1/ii/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#3/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#3/iv/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/iv/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-121.md#3/iv/a/solution)
- [Suslin-tree obstruction to Martin's axiom](set.md#suslin-tree-obstruction-to-martin-s-axiom)
