# Ordinal

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal)

An ordinal is a transitive set well-ordered by membership and represents the order type of a well-order.

**Table of contents**

- [Hardy hierarchy](#hardy-hierarchy)
- [Finite ordinal](#finite-ordinal)
- [Bounded successor characterization of finite ordinals](#bounded-successor-characterization-of-finite-ordinals)
- [Club set](#club-set)
  - [Club of closure points for countable set-valued functions](#club-of-closure-points-for-countable-set-valued-functions)
  - [Diagonal intersection](#diagonal-intersection)
  - [Club sequence](#club-sequence)
    - [Square principle](#square-principle)
    - [Minimal walk along a club sequence](#minimal-walk-along-a-club-sequence)
      - [Minimal-walk tree](#minimal-walk-tree)
      - [Trace coherence lemma for minimal walks](#trace-coherence-lemma-for-minimal-walks)
      - [First-divergence lemma for minimal walks](#first-divergence-lemma-for-minimal-walks)
  - [Stationary set](#stationary-set)
    - [Stationary partition at a successor cardinal](#stationary-partition-at-a-successor-cardinal)
    - [Non-reflecting subset](#non-reflecting-subset)
      - [Nonreflection of fixed order-type fibers](#nonreflection-of-fixed-order-type-fibers)
    - [Stationarity in a limit ordinal](#stationarity-in-a-limit-ordinal)
    - [Stationary partition by cofinal-sequence fibers](#stationary-partition-by-cofinal-sequence-fibers)
    - [Ulam matrix on omega-one](#ulam-matrix-on-omega-one)
      - [Disjoint stationary subsets of omega-one](#disjoint-stationary-subsets-of-omega-one)
    - [Diamond principle](#diamond-principle)
      - [CCC forcing cannot create diamond](#ccc-forcing-cannot-create-diamond)
      - [Stationary diamond principle](#stationary-diamond-principle)
        - [Stationary diamond at a regular cardinal](#stationary-diamond-at-a-regular-cardinal)
          - [Countable-family diamond principle](#countable-family-diamond-principle)
            - [Countable-family diamond equivalence](#countable-family-diamond-equivalence)
        - [Antichain sealing by diamond](#antichain-sealing-by-diamond)
    - [Club principle](#club-principle)
      - [Stationary-indexed club principle](#stationary-indexed-club-principle)
    - [Regressive function](#regressive-function)
      - [Fodor lemma](#fodor-lemma)
        - [Filtration form of Fodor lemma](#filtration-form-of-fodor-lemma)
    - [Stationarity of ordinals of prescribed cofinality](#stationarity-of-ordinals-of-prescribed-cofinality)
  - [Club filter](#club-filter)
    - [Stationary nonclosed member of the club filter](#stationary-nonclosed-member-of-the-club-filter)
    - [Club filter completeness](#club-filter-completeness)
  - [Closed unbounded class of ordinals](#closed-unbounded-class-of-ordinals)
- [Successor ordinal](#successor-ordinal)
- [Countable ordinal](#countable-ordinal)
- [Order type](#order-type)
  - [Mostowski collapse theorem](#mostowski-collapse-theorem)
    - [Mostowski collapse](#mostowski-collapse)
    - [Transitive collapse fixes transitive subsets](#transitive-collapse-fixes-transitive-subsets)
- [Limit ordinal](#limit-ordinal)
- [Normal function on an ordinal](#normal-function-on-an-ordinal)
  - [Fixed point of a normal ordinal function](#fixed-point-of-a-normal-ordinal-function)
- [Transfinite recursion](#transfinite-recursion)
  - [Natural-number recursion theorem](#natural-number-recursion-theorem)
- [Transfinite induction](#transfinite-induction)
- [Ordinal addition](#ordinal-addition)
  - [Associativity of ordinal addition](#associativity-of-ordinal-addition)
  - [Commuting ordinal addition](#commuting-ordinal-addition)
- [Ordinal multiplication](#ordinal-multiplication)
  - [Ordinal division algorithm](#ordinal-division-algorithm)
  - [Commuting squares of ordinals](#commuting-squares-of-ordinals)
  - [Distributive law for ordinal multiplication](#distributive-law-for-ordinal-multiplication)
- [Ordinal exponentiation](#ordinal-exponentiation)
  - [Epsilon zero](#epsilon-zero)
- [Derived-set iteration of a well-order](#derived-set-iteration-of-a-well-order)
  - [Derived sets of an ordinal](#derived-sets-of-an-ordinal)
- [Ordinal interval](#ordinal-interval)
- [First uncountable ordinal](#first-uncountable-ordinal)
  - [First uncountable ordinal is regular](#first-uncountable-ordinal-is-regular)
  - [Tail of the first uncountable ordinal](#tail-of-the-first-uncountable-ordinal)
- [Second uncountable ordinal](#second-uncountable-ordinal)
- [Cantor normal form](#cantor-normal-form)
  - [Generalized Cantor normal form](#generalized-cantor-normal-form)
  - [Commensurable ordinals](#commensurable-ordinals)
  - [Computable Cantor normal form notation](#computable-cantor-normal-form-notation)
    - [Slow well-ordering below epsilon zero](#slow-well-ordering-below-epsilon-zero)
  - [Leading term of an ordinal](#leading-term-of-an-ordinal)
    - [Greatest power of omega below an ordinal](#greatest-power-of-omega-below-an-ordinal)
    - [Leading exponent of an ordinal product](#leading-exponent-of-an-ordinal-product)
- [Additively indecomposable ordinal](#additively-indecomposable-ordinal)
  - [Additively closed ordinal](#additively-closed-ordinal)
  - [Division by an additively indecomposable ordinal](#division-by-an-additively-indecomposable-ordinal)
  - [Multiplicatively closed ordinal](#multiplicatively-closed-ordinal)
    - [Multiplicative closure criterion for a power of omega](#multiplicative-closure-criterion-for-a-power-of-omega)
- [Ordinal arithmetic](#ordinal-arithmetic)
  - [Fundamental sequence of a limit ordinal](#fundamental-sequence-of-a-limit-ordinal)
  - [Fast-growing hierarchy](#fast-growing-hierarchy)
    - [Eventual dominance in a fast-growing hierarchy](#eventual-dominance-in-a-fast-growing-hierarchy)
  - [Hessenberg natural sum](#hessenberg-natural-sum)
    - [Shuffle bound for ordinal partitions](#shuffle-bound-for-ordinal-partitions)
      - [Ordinal partition bound](#ordinal-partition-bound)

## Hardy hierarchy

↑ **Parent:** [Ordinal](ordinal.md)

## Finite ordinal

↑ **Parent:** [Ordinal](ordinal.md)

A finite [ordinal](ordinal.md) is the order type of a finite [well-order](set.md#well-order); in the von Neumann representation it is one of $0,1,2,\ldots$. They are exactly the [ordinals](ordinal.md) $x$ such that $x$ and each member of $x$ are either zero or [successor ordinals](#successor-ordinal). If an [ordinal](ordinal.md) is infinite, it either is the nonzero limit $\omega$ or contains $\omega$ as a member, so it fails this test. Thus the [finite ordinals](#finite-ordinal) give the usual representation of the [natural numbers](arithmetic.md#natural-number).

## Bounded successor characterization of finite ordinals

↑ **Parent:** [Ordinal](ordinal.md)

A [Von Neumann ordinal](ordinal.md) $x$ is finite exactly when $x$ and every member of $x$ are either zero or [successor ordinals](#successor-ordinal). Every [finite ordinal](#finite-ordinal) has that property. Conversely, an infinite [ordinal](ordinal.md) is either $\omega$, which is a nonzero limit, or is greater than $\omega$ and contains that nonzero [limit ordinal](#limit-ordinal). The test can be expressed by a bounded [first-order formula](mathematical-logic.md#first-order-formula): ordinality uses transitivity and membership comparability, and a nonempty [ordinal](ordinal.md) is a successor exactly when it has a greatest member. This defines the class of [natural numbers](arithmetic.md#natural-number) without quantifying over arbitrary infinite [inductive sets](set-theory.md#inductive-set).

## Club set

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Club_set)

For a [limit ordinal](#limit-ordinal) $\kappa$, a [subset](set.md#subset) $C\subseteq\kappa$ is club if it is unbounded and contains each limit below $\kappa$ of an increasing sequence from $C$. At an uncountable [regular cardinal](cardinal-number.md#regular-cardinal) $\kappa$, intersections of fewer than $\kappa$ club [sets](set.md) are club: above a starting point cycle through the sets and take suprema, using regularity to stay below $\kappa$; closure puts the resulting limit in all of them. Club [sets](set.md) provide the reflecting ranks in [worldly cardinals below an inaccessible cardinal](cardinal-number.md#worldly-cardinals-below-an-inaccessible-cardinal).

### Club of closure points for countable set-valued functions

↑ **Parent:** [Club set](#club-set)

For a regular uncountable [cardinal](cardinal-number.md) $\lambda$ and $B:\lambda\to[\lambda]^\omega$, the [limit ordinals](#limit-ordinal) closed under all earlier values of $B$ form a [club set](#club-set). Countably iterate bounds for $\bigcup_{\alpha<\gamma}B(\alpha)$ to obtain unboundedly many closure points. Regularity keeps each bound and the countable supremum below $\lambda$. Limits of closure points remain closure points.

### Diagonal intersection

↑ **Parent:** [Club set](#club-set)

For $\langle C_\alpha:\alpha<\delta\rangle$, its diagonal intersection consists of $\beta<\delta$ belonging to every $C_\alpha$ with $\alpha<\beta$. For club sets on a regular uncountable cardinal, this is a club.

### Club sequence

↑ **Parent:** [Club set](#club-set)

A sequence $\langle C_\delta\rangle$ in which $C_\delta$ is closed and unbounded in $\delta$. At a successor ordinal its predecessor is a club singleton. Such sequences define [minimal walks along a club sequence](#minimal-walk-along-a-club-sequence).

#### Square principle

↑ **Parent:** [Club sequence](#club-sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square_principle)

For an infinite [cardinal](cardinal-number.md) $\kappa$, the square principle supplies [club sets](#club-set) $C_\zeta\subseteq\zeta$ at limit $\zeta<\kappa^+$, with [order type](#order-type) at most $\kappa$, coherent at limit points: $C_\gamma=C_\zeta\cap\gamma$ whenever $\gamma$ is a limit point of $C_\zeta$. The bound precludes a single [club set](#club-set) threading the entire sequence. For regular uncountable $\kappa$, coherence together with the weaker-looking size clause $\operatorname{cf}(\zeta)<\kappa\Rightarrow|C_\zeta|<\kappa$ implies the order-type bound. At $\kappa=\omega$, that clause alone is vacuous and cannot replace the bound.

#### Minimal walk along a club sequence

↑ **Parent:** [Club sequence](#club-sequence)

To walk from $\beta$ to $\alpha<\beta$, start at $\beta$ and repeatedly move from $\delta$ to $\min(C_\delta\setminus\alpha)$ until reaching $\alpha$. The strict decrease in [ordinals](ordinal.md) makes the walk finite. Its trace records the successive $C_\delta\cap\alpha$.

##### Minimal-walk tree

↑ **Parent:** [Minimal walk along a club sequence](#minimal-walk-along-a-club-sequence)

The tree of restrictions $\rho_\beta\upharpoonright\alpha$, ordered by extension. For a [club sequence](#club-sequence) on $\omega_2$ with club order types at most $\omega_1$, the [Continuum hypothesis](cardinal-number.md#continuum-hypothesis) bounds each level by $\aleph_1$. Trace injectivity and [Fodor lemma](#fodor-lemma) exclude a [cofinal branch](set.md#cofinal-branch).

##### Trace coherence lemma for minimal walks

↑ **Parent:** [Minimal walk along a club sequence](#minimal-walk-along-a-club-sequence)

If $\rho_\beta(\alpha)=\rho_\gamma(\alpha)$, then the trace functions agree below $\alpha$. Each shorter trace is reconstructed by locating the first recorded club initial segment that meets $[\xi,\alpha)$ and continuing the walk from its least such point.

##### First-divergence lemma for minimal walks

↑ **Parent:** [Minimal walk along a club sequence](#minimal-walk-along-a-club-sequence)

The walks to $\xi<\alpha$ share a unique maximal initial chain of nodes. At the next step the walk to $\xi$ moves into $[\xi,\alpha)$; the walk to $\alpha$ stays at or above $\alpha$ or has just ended.

### Stationary set

↑ **Parent:** [Club set](#club-set)

A subset of a regular uncountable [cardinal number](cardinal-number.md) $\kappa$ is stationary if it meets every [club set](#club-set) in $\kappa$. Intersecting a stationary set with a [club set](#club-set) preserves stationarity. Every member of the [club filter](#club-filter) is stationary. At a regular infinite $\theta<\kappa$, the [stationarity of ordinals of prescribed cofinality](#stationarity-of-ordinals-of-prescribed-cofinality) supplies important examples.

#### Stationary partition at a successor cardinal

↑ **Parent:** [Stationary set](#stationary-set)

Every stationary subset of a successor cardinal $\lambda^+$ can be partitioned into $\lambda^+$ disjoint stationary subsets. For each $\beta\in[\lambda,\lambda^+)$ choose a bijection $e_\beta:\lambda\to\beta$. For each $\xi<\lambda^+$, the function $\beta\mapsto e_\beta^{-1}(\xi)$ is regressive on the stationary tail with $\beta>\xi$. The [Fodor lemma](#fodor-lemma) gives a stationary fiber with one value $i_\xi<\lambda$. Some value occurs for $\lambda^+$ many indices, whose fibers are pairwise disjoint. Assign any leftover part of $S$ to one fiber.

#### Non-reflecting subset

↑ **Parent:** [Stationary set](#stationary-set)

A [subset](set.md#subset) $X\subseteq\lambda$ is non-reflecting in the indicated sense if it is not stationary below any $\delta<\lambda$ of uncountable [cofinality](cardinal-number.md#cofinality). The [subset](set.md#subset) itself need not be stationary. Nonreflection is inherited by [subsets](set.md#subset). With this definition every [subset](set.md#subset) of $\omega_1$ is non-reflecting, since all smaller [ordinals](ordinal.md) have countable [cofinality](cardinal-number.md#cofinality).

##### Nonreflection of fixed order-type fibers

↑ **Parent:** [Non-reflecting subset](#non-reflecting-subset)

For a coherent [club set](#club-set) sequence, the limit points of $C_\delta$ form a [club set](#club-set) whenever $\operatorname{cf}(\delta)>\omega$. Along these points, $\operatorname{otp}(C_\gamma)=\operatorname{otp}(C_\delta\cap\gamma)$ strictly increases, so a fixed fiber $E_\xi$ meets this a [club set](#club-set) at most once and cannot reflect at $\delta$. Under the [square principle](#square-principle) order-type bound, the fibers with $\xi\le\kappa$ partition all [limit ordinals](#limit-ordinal) below $\kappa^+$ into $\kappa$ non-reflecting pieces.

#### Stationarity in a limit ordinal

↑ **Parent:** [Stationary set](#stationary-set)

For any nonzero [limit ordinal](#limit-ordinal) $\delta$, a [club set](#club-set) is an unbounded [subset](set.md#subset) closed under limit points below $\delta$. A [subset](set.md#subset) is stationary if it meets every such [club set](#club-set). Statements concerning the completeness of the [club filter](#club-filter) or [Fodor lemma](#fodor-lemma) require regular uncountable height; they should not be transferred to arbitrary singular or countable [limit ordinals](#limit-ordinal) without checking their hypotheses.

#### Stationary partition by cofinal-sequence fibers

↑ **Parent:** [Stationary set](#stationary-set)

For an uncountable [regular cardinal](cardinal-number.md#regular-cardinal) $\kappa$, choose cofinal sequences $c_\alpha:\omega\to\alpha$ for the [stationary set](#stationary-set) of [ordinals](ordinal.md) of [cofinality](cardinal-number.md#cofinality) $\omega$. Above any bound, some fixed coordinate exceeds the bound on a stationary [subset](set.md#subset); [Fodor lemma](#fodor-lemma) makes that coordinate constant on a stationary [subset](set.md#subset). Thus the stationary constant fibers, over all coordinates, have unboundedly many values. Regularity makes one coordinate have $\kappa$ such values. Its fibers are disjoint [stationary sets](#stationary-set); adding all leftover [ordinals](ordinal.md) to one piece partitions $\kappa$.

#### Ulam matrix on omega-one

↑ **Parent:** [Stationary set](#stationary-set)

A family $(A_{\alpha,n})_{\alpha<\omega_1,n<\omega}$ whose row at $\alpha$ partitions $(\alpha,\omega_1)$ and whose fixed-column cells are pairwise disjoint. Choose [injections](algebra.md#injective-function) $e_\beta:\beta\to\omega$ and put $A_{\alpha,n}=\{\beta>\alpha:e_\beta(\alpha)=n\}$. This gives a matrix used to split [stationary sets](#stationary-set) into many stationary pieces.

##### Disjoint stationary subsets of omega-one

↑ **Parent:** [Ulam matrix on omega-one](#ulam-matrix-on-omega-one)

There are $\aleph_1$ pairwise disjoint stationary subsets of the nonzero countable limit ordinals. In a [Ulam matrix on omega-one](#ulam-matrix-on-omega-one), each row partitions a stationary tail into countably many cells, so some cell is stationary. One column contains stationary cells in uncountably many rows, and the column cells are disjoint. Unions indexed by different subsets of $\omega_1$ then differ on a stationary set.

#### Diamond principle

↑ **Parent:** [Stationary set](#stationary-set)

A sequence $D_\alpha\subseteq\alpha$ guesses every $X\subseteq\omega_1$ stationarily often: $\{\alpha:D_\alpha=X\cap\alpha\}$ is stationary.

##### CCC forcing cannot create diamond

↑ **Parent:** [Diamond principle](#diamond-principle)

For each index, collect the ground [subsets](set.md#subset) which some condition forces to be the corresponding diamond guess. Distinct forced values have incompatible witnessing conditions, so the [countable chain condition for forcing](forcing.md#countable-chain-condition-for-forcing) makes this a countable family. Every ground [subset](set.md#subset) is guessed by these families on a ground stationary set, by testing each ground [club set](#club-set). The [countable-family diamond equivalence](#countable-family-diamond-equivalence) then yields diamond in the ground model. A generic guess need not itself be a ground [subset](set.md#subset); only values forced equal to one are collected.

##### Stationary diamond principle

↑ **Parent:** [Diamond principle](#diamond-principle)

For a stationary $S\subseteq\omega_1$, a sequence $D_\alpha\subseteq\alpha$ indexed by $S$ guesses every $X\subseteq\omega_1$ on a stationary subset of $S$.

###### Stationary diamond at a regular cardinal

↑ **Parent:** [Stationary diamond principle](#stationary-diamond-principle)

A sequence $D_\alpha\subseteq\alpha$, indexed by a stationary [subset](set.md#subset) $S$ of a regular uncountable [cardinal](cardinal-number.md) $\lambda$, guesses every $X\subseteq\lambda$ stationarily often: $\{\alpha\in S:D_\alpha=X\cap\alpha\}$ is stationary. This extends the usual [stationary diamond principle](#stationary-diamond-principle) at $\omega_1$.

###### Countable-family diamond principle

↑ **Parent:** [Stationary diamond at a regular cardinal](#stationary-diamond-at-a-regular-cardinal)

At each $\alpha\in S$, a countable family $E_\alpha\subseteq\mathcal P(\alpha)$ is supplied. Every $X\subseteq\lambda$ has $X\cap\alpha\in E_\alpha$ on a stationary [subset](set.md#subset) of $S$. The [countable-family diamond equivalence](#countable-family-diamond-equivalence) shows that this apparently weaker prediction is equivalent to a single diamond guess at each index.

###### Countable-family diamond equivalence

↑ **Parent:** [Countable-family diamond principle](#countable-family-diamond-principle)

Enumerate each countable guessing family and use a [bijection](function.md#bijection) $\pi:\lambda\times\omega\to\lambda$ with a [club set](#club-set) of prefix-closure points. The $n$th candidate sequence decodes the $n$th component of the $n$th family entry. If all candidates fail, choose counterexample sets $X_n$ and [club sets](#club-set) witnessing failure, then code the $X_n$ together using $\pi$. A correct family guess on the common closure [club set](#club-set) and all failure [club sets](#club-set) decodes to one of the forbidden correct guesses. The singleton-family implication supplies the reverse direction.

###### Antichain sealing by diamond

↑ **Parent:** [Stationary diamond principle](#stationary-diamond-principle)

At a correctly guessing limit stage of a normal tree construction, make every new level node extend a member of the guessed maximal [tree antichain](set.md#tree-antichain). It follows that the antichain has no later member. This produces a [Suslin tree](set.md#suslin-tree) from the [stationary diamond principle](#stationary-diamond-principle).

#### Club principle

↑ **Parent:** [Stationary set](#stationary-set)

There are cofinal sequences $A_\delta\subseteq\delta$ of order type $\omega$ for the countable limit ordinals, such that every uncountable $X\subseteq\omega_1$ contains some $A_\delta$.

##### Stationary-indexed club principle

↑ **Parent:** [Club principle](#club-principle)

For a stationary $S\subseteq\omega_1$, there are cofinal ladders $A_\delta\subset\delta$ of order type $\omega$, indexed by [limit ordinals](#limit-ordinal) in $S$, such that every uncountable $X\subseteq\omega_1$ contains one of these ladders. This predicts a contained ladder, whereas [stationary diamond principle](#stationary-diamond-principle) predicts a whole initial segment.

#### Regressive function

↑ **Parent:** [Stationary set](#stationary-set)

A function on a set of ordinals with $f(\alpha)<\alpha$ at every nonzero point of its domain. On a stationary subset of a regular uncountable cardinal, [Fodor lemma](#fodor-lemma) makes it constant on a stationary subset.

##### Fodor lemma

↑ **Parent:** [Regressive function](#regressive-function)

A [regressive function](#regressive-function) on a stationary subset of a regular uncountable cardinal is constant on a stationary subset.

###### Filtration form of Fodor lemma

↑ **Parent:** [Fodor lemma](#fodor-lemma)

If $S\subseteq\kappa$ is stationary and $f(\alpha)\in A_\alpha$ for a [kappa-filtration](set-theory.md#kappa-filtration), then $f$ is constant on a stationary [subset](set.md#subset). Restrict to limit indices and use continuity to find a smaller stage containing each value. [Fodor lemma](#fodor-lemma) fixes that stage on a stationary [subset](set.md#subset). Its size is less than $\kappa$, so [club filter completeness](#club-filter-completeness) makes one value fiber stationary.

#### Stationarity of ordinals of prescribed cofinality

↑ **Parent:** [Stationary set](#stationary-set)

For a regular infinite $\theta<\kappa$, with $\kappa$ a regular uncountable [cardinal number](cardinal-number.md), $S_\theta^\kappa=\{\delta<\kappa:\operatorname{cf}(\delta)=\theta\}$ is stationary. Build a strictly increasing continuous $\theta$-sequence in any [club set](#club-set), and take its supremum. Closure places it in that club and the [cofinality of an increasing ordinal supremum](cardinal-number.md#cofinality-of-an-increasing-ordinal-supremum) gives [cofinality](cardinal-number.md#cofinality) $\theta$. In particular the two disjoint sets $S_\omega^{\omega_2}$ and $S_{\omega_1}^{\omega_2}$ show that the [club filter](#club-filter) on $\omega_2$ is not an [ultrafilter](set-theory.md#ultrafilter).

### Club filter

↑ **Parent:** [Club set](#club-set)

On a regular uncountable [cardinal number](cardinal-number.md) $\kappa$, the club filter consists of all subsets containing a [club set](#club-set). It is a [kappa-complete filter](set-theory.md#kappa-complete-filter) by [club filter completeness](#club-filter-completeness). Its members are [stationary sets](#stationary-set), although a [stationary set](#stationary-set) need not be a filter member, and a filter member need not itself be closed.

#### Stationary nonclosed member of the club filter

↑ **Parent:** [Club filter](#club-filter)

For any regular uncountable [cardinal number](cardinal-number.md) $\kappa$, the set $\kappa\setminus\{\omega\}$ contains the final-segment [club set](#club-set) $[\omega+1,\kappa)$, so belongs to the [club filter](#club-filter) and is a [stationary set](#stationary-set). It is not closed, since its finite ordinals have supremum $\omega$, which is missing.

#### Club filter completeness

↑ **Parent:** [Club filter](#club-filter)

The [club filter](#club-filter) on a regular uncountable [cardinal number](cardinal-number.md) $\kappa$ is $\kappa$-complete. Intersections of fewer than $\kappa$ [club sets](#club-set) are closed. For unboundedness, repeatedly step past a point of each club and take a countable supremum; regularity keeps all suprema below $\kappa$, and closure puts the final supremum in every club.

### Closed unbounded class of ordinals

↑ **Parent:** [Club set](#club-set)

An unbounded [class in set theory](set-theory.md#class-set-theory) of [ordinals](ordinal.md) is closed if every nonempty set-sized increasing sequence of its members has its supremum in the class. This is the proper-class analogue of a [club set](#club-set). The [reflection theorem for definable hierarchies](set-theory.md#reflection-theorem-for-definable-hierarchies) gives such a class for every finite collection of [first-order formulas](mathematical-logic.md#first-order-formula).

## Successor ordinal

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Successor_ordinal)

The successor of an ordinal $\alpha$ is $\alpha+1=\alpha\cup\{\alpha\}$.

## Countable ordinal

↑ **Parent:** [Ordinal](ordinal.md)

A countable ordinal has a [countable set](cardinal-number.md#countable-set) as its underlying set.

These are the [ordinals](ordinal.md) strictly below the [first uncountable ordinal](#first-uncountable-ordinal).

## Order type

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order_type)

The order type of a well-order is the unique ordinal isomorphic to it.

### Mostowski collapse theorem

↑ **Parent:** [Order type](#order-type)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mostowski_collapse_theorem)

Every well-founded extensional relation is uniquely isomorphic to membership on a transitive set.

#### Mostowski collapse

↑ **Parent:** [Mostowski collapse theorem](#mostowski-collapse-theorem)

The recursively defined [isomorphism](algebra.md#isomorphism) from a [well-founded](set-theory.md#well-founded-relation) extensional set-like relation to membership on a [transitive set](set-theory.md#transitive-set) or class. The [Mostowski collapse theorem](#mostowski-collapse-theorem) asserts its existence and uniqueness; the class form requires each predecessor extension to be a set.

#### Transitive collapse fixes transitive subsets

↑ **Parent:** [Mostowski collapse theorem](#mostowski-collapse-theorem)

If $X$ has a well-founded extensional inherited membership relation and $T\subseteq X$ is a [transitive set](set-theory.md#transitive-set), its [Mostowski collapse theorem](#mostowski-collapse-theorem) map $\pi$ fixes every member of $T$. The recursion $\pi(x)=\{\pi(y):y\in x\cap X\}$ and [well-founded relation](set-theory.md#well-founded-relation) induction give this pointwise. If also $T\in X$, then $\pi(T)=T$.

## Limit ordinal

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Limit_ordinal)

A nonzero ordinal is a limit ordinal when it is not a successor ordinal. Equivalently, it is the supremum of all smaller ordinals.

## Normal function on an ordinal

↑ **Parent:** [Ordinal](ordinal.md)

A function $f:\lambda\to\lambda$ on an ordinal is normal when it is strictly increasing and continuous at limit ordinals: $f(\delta)=\sup_{\alpha<\delta}f(\alpha)$ for every limit $\delta<\lambda$.

### Fixed point of a normal ordinal function

↑ **Parent:** [Normal function on an ordinal](#normal-function-on-an-ordinal)

For a strictly increasing ordinal class function continuous at limits, start with $\alpha_0=0$ and iterate $\alpha_{n+1}=f(\alpha_n)$. If the sequence stabilizes, its stable value is a [fixed point](function.md#fixed-point). Otherwise its supremum $\alpha$ is a limit and continuity gives $f(\alpha)=\sup_n f(\alpha_n)=\sup_n\alpha_{n+1}=\alpha$. Starting the iteration above any prescribed ordinal gives arbitrarily large fixed points.

## Transfinite recursion

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transfinite_recursion)

Transfinite recursion defines a value at each ordinal from the function of all earlier values.

### Natural-number recursion theorem

↑ **Parent:** [Transfinite recursion](#transfinite-recursion)

Given an initial value $a$ and a rule $G$, there is a unique function $F$ on $\omega$ satisfying $F(0)=a$ and $F(n+1)=G(F(n))$.

## Transfinite induction

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transfinite_induction)

If a property of an ordinal follows whenever it holds for every smaller ordinal, then it holds for every ordinal.

## Ordinal addition

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal_addition)

Ordinal addition is ordered concatenation and is associative but generally not commutative.

### Associativity of ordinal addition

↑ **Parent:** [Ordinal addition](#ordinal-addition)

For all ordinals $\alpha,\beta,\gamma$,

$$
(\alpha+\beta)+\gamma=\alpha+(\beta+\gamma).
$$

This follows by [transfinite induction](#transfinite-induction) on $\gamma$ from the recursive definition of [ordinal addition](#ordinal-addition).

### Commuting ordinal addition

↑ **Parent:** [Ordinal addition](#ordinal-addition)

Nonzero ordinals commute under addition precisely when they are positive finite right multiples of a common ordinal. This follows by comparing their [Cantor normal forms](#cantor-normal-form) at the first exponent where they differ.

## Ordinal multiplication

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal_multiplication)

Ordinal multiplication is defined recursively by

$$
\alpha0=0,
\qquad
\alpha(\beta+1)=\alpha\beta+\alpha,
\qquad
\alpha\lambda=\sup_{\xi<\lambda}\alpha\xi
$$

for nonzero [limit ordinal](#limit-ordinal) $\lambda$. It is associative and left-distributive over [ordinal addition](#ordinal-addition), but generally neither commutative nor right-distributive.

### Ordinal division algorithm

↑ **Parent:** [Ordinal multiplication](#ordinal-multiplication)

For [ordinals](ordinal.md) $\alpha$ and $\delta>0$, there are unique ordinals $q,r$ with the displayed relation. The function $q\mapsto\delta q$ is strictly increasing, continuous at limit ordinals and unbounded. Its first value above $\alpha$ occurs at a successor, giving the largest $q$ with $\delta q\le\alpha$. The ordered tail of $\alpha$ after that initial segment gives $r$, and maximality gives $r<\delta$.

### Commuting squares of ordinals

↑ **Parent:** [Ordinal multiplication](#ordinal-multiplication)

Two [ordinals](ordinal.md) commute under [ordinal multiplication](#ordinal-multiplication) if and only if their squares commute. One implication follows from [associativity](algebraic-operation.md#associative-property). For the converse, squaring is strictly increasing: $A<B$ implies $A^2\leq BA<B^2$. If $\alpha\beta<\beta\alpha$, monotonicity gives

$$
\alpha^2\beta^2\leq(\alpha\beta)^2<(\beta\alpha)^2\leq\beta^2\alpha^2,
$$

a contradiction to commuting squares. Swap the factors to exclude the reverse inequality; zero factors cause no exception.

### Distributive law for ordinal multiplication

↑ **Parent:** [Ordinal multiplication](#ordinal-multiplication)

[Ordinal multiplication](#ordinal-multiplication) is distributive in its right argument:

$$
\alpha(\beta+\gamma)=\alpha\beta+\alpha\gamma.
$$

Indeed a sequence of copies of $\alpha$ indexed by the concatenation of $\beta$ and $\gamma$ is the concatenation of the two sequences of copies. The other distributive law fails: $(1+1)\omega=\omega$, while $\omega+\omega>\omega$.

## Ordinal exponentiation

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal_exponentiation)

Ordinal exponentiation is defined recursively by

$$
\alpha^0=1,\qquad
\alpha^{\beta+1}=\alpha^\beta\alpha,\qquad
\alpha^\lambda=\sup_{\xi<\lambda}\alpha^\xi
$$

for nonzero limit $\lambda$. Transfinite induction gives

$$
\alpha^{\beta+\gamma}=\alpha^\beta\alpha^\gamma.
$$

### Epsilon zero

↑ **Parent:** [Ordinal exponentiation](#ordinal-exponentiation)

The [ordinal](ordinal.md) $\varepsilon_0$ is the least fixed point of $\alpha\mapsto\omega^\alpha$. It is the supremum of $1,\omega,\omega^\omega,\omega^{\omega^\omega},\ldots$, and is countable.

## Derived-set iteration of a well-order

↑ **Parent:** [Ordinal](ordinal.md)

For a well-ordered set $X$, let $X'$ contain the points whose strict initial segments are nonempty and have no greatest element, and iterate this operation transfinitely, taking intersections at limit stages. Every nonempty derivative loses at least its least element. If no derivative became empty, choosing one point from each successive difference would inject the ordinal supplied by [Hartogs theorem](set-theory.md#hartogs-theorem) for $X$ into $X$, a contradiction.

### Derived sets of an ordinal

↑ **Parent:** [Derived-set iteration of a well-order](#derived-set-iteration-of-a-well-order)

For an ordinal $\xi$,

$$
\xi'=\{\omega\beta<\xi:\beta>0\},
\qquad
\xi''=\{\omega^2\beta<\xi:\beta>0\}.
$$

Thus the derivative index of $\omega$ is one and that of $\omega^2$ is two.

## Ordinal interval

↑ **Parent:** [Ordinal](ordinal.md)

For $\alpha<\beta$, the ordinal interval $\beta\setminus\alpha$ is the ordered tail from $\alpha$ inclusive to $\beta$ exclusive.

## First uncountable ordinal

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/First_uncountable_ordinal)

The first uncountable ordinal $\omega_1$ is the set of all countable ordinals.

### First uncountable ordinal is regular

↑ **Parent:** [First uncountable ordinal](#first-uncountable-ordinal)

The [first uncountable ordinal](#first-uncountable-ordinal) has [cofinality](cardinal-number.md#cofinality) $\omega_1$. Indeed, the supremum of any [countable set](cardinal-number.md#countable-set) of countable ordinals is still a [countable ordinal](#countable-ordinal), so no countable sequence is cofinal in $\omega_1$.

### Tail of the first uncountable ordinal

↑ **Parent:** [First uncountable ordinal](#first-uncountable-ordinal)

Deleting any countable initial segment from $\omega_1$ leaves a well-order of type $\omega_1$.

## Second uncountable ordinal

↑ **Parent:** [Ordinal](ordinal.md)

The second uncountable ordinal $\omega_2$ is the least ordinal whose [cardinal number](cardinal-number.md) is strictly larger than that of the [first uncountable ordinal](#first-uncountable-ordinal) $\omega_1$. Equivalently, it is the initial ordinal of the successor cardinal $\aleph_2$.

## Cantor normal form

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cantor_normal_form)

Every nonzero ordinal has a unique finite expression $\omega^{\delta_1}n_1+\cdots+\omega^{\delta_r}n_r$ with decreasing exponents and positive finite coefficients.

### Generalized Cantor normal form

↑ **Parent:** [Cantor normal form](#cantor-normal-form)

For every [ordinal](ordinal.md) base $\rho>1$, a nonzero ordinal has a unique finite [ordinal addition](#ordinal-addition) expansion with strictly decreasing exponents $\beta_i$ and coefficients $0<\xi_i<\rho$. Choose the largest power at most the remaining ordinal and apply the [ordinal division algorithm](#ordinal-division-algorithm). The next remainder has smaller leading exponent, so [well-foundedness](set-theory.md#well-founded-relation) forces termination. Each lower tail is smaller than its preceding power; uniqueness of division consequently fixes the exponent, coefficient and tail successively. For $\rho=\omega$ this is [Cantor normal form](#cantor-normal-form).

### Commensurable ordinals

↑ **Parent:** [Cantor normal form](#cantor-normal-form)

Two [ordinals](ordinal.md) are commensurable when neither is absorbed by adding the other on its left. For positive ordinals, this is equivalent to equality of their leading [Cantor normal form](#cantor-normal-form) exponent. If leading exponents differ, the lower-leading ordinal is absorbed by the higher power of $\omega$. If they agree, either sum adds the two positive leading coefficients and therefore exceeds both original ordinals. Zero is commensurable with no ordinal.

### Computable Cantor normal form notation

↑ **Parent:** [Cantor normal form](#cantor-normal-form)

Finite canonical terms built from zero, [ordinal](ordinal.md) sums and powers of omega describe exactly the [ordinals](ordinal.md) below [epsilon zero](#epsilon-zero). Syntactic validity and comparison are decidable by recursion through the exponent subterms. Enumerating valid term codes transfers their order to a [computable well-order](set.md#decidable-well-order) on all [natural numbers](arithmetic.md#natural-number).

#### Slow well-ordering below epsilon zero

↑ **Parent:** [Computable Cantor normal form notation](#computable-cantor-normal-form-notation)

Use the unary [Cantor normal form](#cantor-normal-form) tree norm, counting one root and recursively counting all repeated exponent subterms. There are only finitely many notations of bounded norm. This finite principle bounds all descending sequences whose norms grow at most linearly with the position. [Friedman's finite form of Kruskal's theorem](set.md#friedman-s-finite-form-of-kruskal-s-theorem) implies it through the [natural-sum ordinal rank of a finite rooted tree](tree-graph-theory.md#natural-sum-ordinal-rank-of-a-finite-rooted-tree). The Friedman–Smith miniaturization theorem turns this controlled termination principle for standard epsilon-zero notations into the [formal consistency statement](mathematical-logic.md#formal-consistency-statement) for [Peano arithmetic](mathematical-logic.md#peano-arithmetic); the technical ordinal-analysis result is needed in addition to the tree coding. Section 2.2 of [https://formal.hknu.ac.kr/Publi/kruskalJKMS.pdf](https://formal.hknu.ac.kr/Publi/kruskalJKMS.pdf) records the general miniaturization and soundness theorem.

### Leading term of an ordinal

↑ **Parent:** [Cantor normal form](#cantor-normal-form)

The leading term $\omega^\delta n$ is the highest-exponent term in Cantor normal form; the remaining tail is strictly below $\omega^\delta$.

#### Greatest power of omega below an ordinal

↑ **Parent:** [Leading term of an ordinal](#leading-term-of-an-ordinal)

Every nonzero ordinal $\alpha$ has a greatest exponent $\beta$ such that $\omega^\beta\leq\alpha$. It is the leading exponent in the [Cantor normal form](#cantor-normal-form) of $\alpha$, and

$$
\alpha=\omega^\beta n+\gamma
$$

for a positive finite integer $n$ and $\gamma<\omega^\beta$.

#### Leading exponent of an ordinal product

↑ **Parent:** [Leading term of an ordinal](#leading-term-of-an-ordinal)

Let nonzero ordinals $\xi,\eta$ have leading exponents $\rho,\sigma$. If $\eta$ is finite, then $\xi\eta$ has leading exponent $\rho$. If $\eta$ is infinite, so that $\sigma>0$, then $\xi\eta$ has leading exponent $\rho+\sigma$. This follows by multiplying the leading terms in [Cantor normal form](#cantor-normal-form) and using continuity of [ordinal multiplication](#ordinal-multiplication) at limit ordinals.

## Additively indecomposable ordinal

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Additively_indecomposable_ordinal)

The additively indecomposable ordinals are exactly the powers $\omega^\delta$.

### Additively closed ordinal

↑ **Parent:** [Additively indecomposable ordinal](#additively-indecomposable-ordinal)

A nonzero ordinal $\delta$ is additively closed when $\beta+\gamma<\delta$ for all $\beta,\gamma<\delta$. These are exactly the ordinals $\omega^\alpha$: sufficiency follows from [Cantor normal form](#cantor-normal-form), while necessity follows by splitting any leading coefficient or nonzero tail below $\delta$ into two smaller summands.

### Division by an additively indecomposable ordinal

↑ **Parent:** [Additively indecomposable ordinal](#additively-indecomposable-ordinal)

For every ordinal $\gamma$ and $\lambda=\omega^\alpha$, there are unique ordinals $\beta,\delta$ such that

$$
\gamma=\lambda\beta+\delta,
\qquad \delta<\lambda.
$$

Choose the greatest initial multiple $\lambda\beta\leq\gamma$; if its remainder were at least $\lambda$, the next multiple would still fit. Uniqueness follows because every remainder below $\lambda$ lies before $\lambda(\beta+1)$.

### Multiplicatively closed ordinal

↑ **Parent:** [Additively indecomposable ordinal](#additively-indecomposable-ordinal)

An ordinal $\delta>2$ is multiplicatively closed when $\beta\gamma<\delta$ for all $\beta,\gamma<\delta$. These are exactly

$$
\delta=\omega^{\omega^\alpha}.
$$

#### Multiplicative closure criterion for a power of omega

↑ **Parent:** [Multiplicatively closed ordinal](#multiplicatively-closed-ordinal)

For nonzero $\lambda$, the ordinal $\omega^\lambda$ is [multiplicatively closed](#multiplicatively-closed-ordinal) exactly when $\lambda$ is [additively closed](#additively-closed-ordinal). One direction follows from

$$
\omega^\rho\omega^\sigma=\omega^{\rho+\sigma}.
$$

For the other, the [leading exponent of an ordinal product](#leading-exponent-of-an-ordinal-product) shows that products of ordinals below $\omega^\lambda$ still have leading exponent below $\lambda$.

## Ordinal arithmetic

↑ **Parent:** [Ordinal](ordinal.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal_arithmetic)

Ordinal arithmetic defines addition, multiplication and exponentiation of [ordinals](ordinal.md) through order types or [transfinite recursion](#transfinite-recursion). The usual operations need not be commutative. Natural sum and natural product instead combine [Cantor normal forms](#cantor-normal-form) and are commutative; the [Hessenberg natural sum](#hessenberg-natural-sum) is the natural addition operation.

### Fundamental sequence of a limit ordinal

↑ **Parent:** [Ordinal arithmetic](#ordinal-arithmetic)

For a countable limit [ordinal](ordinal.md), a fundamental sequence is an increasing cofinal sequence of smaller ordinals. Effective choices allow a [fast-growing hierarchy](#fast-growing-hierarchy) to turn limit recursion into recursion at a finite input. Below [epsilon zero](#epsilon-zero), write the final term as $\gamma+\omega^\beta$. For successor $\beta=\delta+1$, take $\gamma+\omega^\delta(n+1)$; for nonzero limit $\beta$, take $\gamma+\omega^{\beta[n]}$. Earlier terms in the [Cantor normal form](#cantor-normal-form) remain fixed.

### Fast-growing hierarchy

↑ **Parent:** [Ordinal arithmetic](#ordinal-arithmetic)

A fast-growing hierarchy indexes number-theoretic [functions](function.md) by an effective system of [ordinal](ordinal.md) notations. Successor stages iterate the preceding function, while limit stages diagonalize along a chosen [fundamental sequence of a limit ordinal](#fundamental-sequence-of-a-limit-ordinal). These choices are part of the definition. With the standard [Cantor normal form](#cantor-normal-form) sequences below [epsilon zero](#epsilon-zero), each fixed $F_\alpha$ for $\alpha<\varepsilon_0$ is provably total in [Peano arithmetic](mathematical-logic.md#peano-arithmetic), but the uniform endpoint $F_{\varepsilon_0}$ is not. Every function provably total in [Peano arithmetic](mathematical-logic.md#peano-arithmetic) is eventually bounded by some lower level. These classification results are proved in [https://epub.ub.uni-muenchen.de/3843/1/3843.pdf](https://epub.ub.uni-muenchen.de/3843/1/3843.pdf) .

#### Eventual dominance in a fast-growing hierarchy

↑ **Parent:** [Fast-growing hierarchy](#fast-growing-hierarchy)

For the standard [fundamental sequences of limit ordinals](#fundamental-sequence-of-a-limit-ordinal) below [epsilon zero](#epsilon-zero), the index order corresponds to eventual, rather than necessarily pointwise, growth. For example, under $\omega[n]=n+1$ and successor iteration $n+1$ times, $F_\omega(1)=F_2(1)=7$ whereas $F_3(1)=2047$. Limit stages are diagonal choices, so a larger index can give a smaller value at small arguments.

### Hessenberg natural sum

↑ **Parent:** [Ordinal arithmetic](#ordinal-arithmetic)

The Hessenberg natural sum aligns equal exponents in two Cantor normal forms and adds their finite coefficients; unlike ordinal addition it is commutative.

It is the commutative natural addition operation in [ordinal arithmetic](#ordinal-arithmetic).

#### Shuffle bound for ordinal partitions

↑ **Parent:** [Hessenberg natural sum](#hessenberg-natural-sum)

If a well-order is the union of suborders of types $\xi$ and $\eta$, its type is at most $\xi\mathbin\#\eta$.

##### Ordinal partition bound

↑ **Parent:** [Shuffle bound for ordinal partitions](#shuffle-bound-for-ordinal-partitions)

If an ordinal is partitioned into two copies of type $\beta$, its type is below $\beta+\beta+\beta$; two copies do not always give a strict bound.

## ↑ Ancestors (5)

1. [Set theory](set-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (172)

- [Absoluteness of cardinalhood in limit ranks](set-theory.md#absoluteness-of-cardinalhood-in-limit-ranks)
- [Arithmetical comprehension theory](mathematical-logic.md#arithmetical-comprehension-theory)
- [Bounded successor characterization of finite ordinals](#bounded-successor-characterization-of-finite-ordinals)
- [Cardinal collapse](forcing.md#cardinal-collapse)
- [Cardinality](cardinal-number.md#cardinality)
- [Category of ordinals in reverse order](category.md#category-of-ordinals-in-reverse-order)
- [Closed elementary-submodel construction of an end-homogeneous sequence](set-theory.md#closed-elementary-submodel-construction-of-an-end-homogeneous-sequence)
- [Closed forcing adds no short ground-valued sequences](forcing.md#closed-forcing-adds-no-short-ground-valued-sequences)
- [Closed unbounded class of ordinals](#closed-unbounded-class-of-ordinals)
- [Coding level of the constructible hierarchy](definable-power-set.md#coding-level-of-the-constructible-hierarchy)
- [Cofinality-preserving forcing](forcing.md#cofinality-preserving-forcing)
- [Commensurable ordinals](#commensurable-ordinals)
- [Commuting squares of ordinals](#commuting-squares-of-ordinals)
- [Computable Cantor normal form notation](#computable-cantor-normal-form-notation)
- [Constructible-level absoluteness over ZF](definable-power-set.md#constructible-level-absoluteness-over-zf)
- [Countable ordinal](#countable-ordinal)
- [Definable continuous hierarchy](set-theory.md#definable-continuous-hierarchy)
- [Epsilon zero](#epsilon-zero)
- [Eventual domination on a regular cardinal](set-theory.md#eventual-domination-on-a-regular-cardinal)
- [Fast-growing hierarchy](#fast-growing-hierarchy)
- [Finite Lévy collapse to omega-one](forcing.md#finite-levy-collapse-to-omega-one)
- [Finite ordinal](#finite-ordinal)
- [Forcing name rank](forcing.md#forcing-name-rank)
- [Full second-order replacement rank obstruction](set-theory.md#full-second-order-replacement-rank-obstruction)
- [Fundamental sequence of a limit ordinal](#fundamental-sequence-of-a-limit-ordinal)
- [Generalized Cantor normal form](#generalized-cantor-normal-form)
- [Generic coordinate reals for finite-function forcing](forcing.md#generic-coordinate-reals-for-finite-function-forcing)
- [Gentzen ordinal reduction for arithmetic](mathematical-logic.md#gentzen-ordinal-reduction-for-arithmetic)
- [Goodstein's theorem](integer.md#goodstein-s-theorem)
- [Hartogs number](set-theory.md#hartogs-number)
- [Inner model](set-theory.md#inner-model)
- [Inner models with all reals preserve omega-one](definable-power-set.md#inner-models-with-all-reals-preserve-omega-one)
- [Lévy reflection theorem](set-theory.md#levy-reflection-theorem)
- [Minimal walk along a club sequence](#minimal-walk-along-a-club-sequence)
- [Non-reflecting subset](#non-reflecting-subset)
- [Order isomorphism](set.md#order-isomorphism)
- [Ordinal arithmetic](#ordinal-arithmetic)
- [Ordinal division algorithm](#ordinal-division-algorithm)
- [Ordinal rank of a Goodstein term](integer.md#ordinal-rank-of-a-goodstein-term)
- [Paris model](mathematical-logic.md#paris-model)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-18.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-18.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-21.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#7/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-24.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#16f/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#16f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#16f/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#16f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-27.md#11/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-27.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-27.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-27.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2.md#16h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#16h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-11.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#11/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#11/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3.md#16g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-26.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-26.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-26.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1.md#16g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#16g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1.md#16g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#16g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-25.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#16g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#16g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-20.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-20.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-20.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4.md#16h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-83.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#1/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#1/ii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#2/iv/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#3/ii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#3/ii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#4/ii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#4/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#5/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#5/iv/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#5/iv/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/ii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/ii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/iii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-19.md#6/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#1/i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/iii/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/iii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#2/iii/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#5/iv/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-19.md#6/iv/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-21.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#13i/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#13i/b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3.md#13i/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#13i/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#3/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-24.md#2/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-24.md#2/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-24.md#4/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-24.md#4/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-24.md#4/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-25.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-120.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-121.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-121.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-121.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-121.md#4/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-121.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#14h/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#14h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#14h/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#14h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#1/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#2/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#4/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-121.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-121.md#2/ii/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#16i/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#16i/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#16i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-121.md#1/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-121.md#1/iv/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-121.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-116.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#16h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#16h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-116.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-128.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-128.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-128.md#2/b/solution)
- [Proof outline of Zorn's lemma](set-theory.md#proof-outline-of-zorn-s-lemma)
- [Scott formula](mathematical-logic.md#scott-formula)
- [Small-limit preservation is insufficient for the large elements-colimit criterion](functor.md#small-limit-preservation-is-insufficient-for-the-large-elements-colimit-criterion)
- [Stationary partition by cofinal-sequence fibers](#stationary-partition-by-cofinal-sequence-fibers)
- [Winning-position attractor in an infinite game](descriptive-set-theory.md#winning-position-attractor-in-an-infinite-game)
