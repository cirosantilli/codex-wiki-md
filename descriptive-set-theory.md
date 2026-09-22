# Descriptive set theory

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Descriptive_set_theory)

Descriptive set theory studies definable subsets of spaces such as the [Baire space of sequences](#baire-space-of-sequences), with particular emphasis on hierarchies of complexity, regularity properties and [infinite games](#infinite-game-of-perfect-information).

**Table of contents**

- [Baire space of sequences](#baire-space-of-sequences)
- [Infinite game of perfect information](#infinite-game-of-perfect-information)
  - [Covering of an infinite game](#covering-of-an-infinite-game)
    - [Depth-stabilizing inverse limit of game coverings](#depth-stabilizing-inverse-limit-of-game-coverings)
    - [Unravelling of a game payoff](#unravelling-of-a-game-payoff)
      - [Announcement-and-challenge covering of a closed payoff](#announcement-and-challenge-covering-of-a-closed-payoff)
  - [Buchi game](#buchi-game)
  - [Strategy in an infinite game](#strategy-in-an-infinite-game)
    - [Winning strategy in an infinite game](#winning-strategy-in-an-infinite-game)
  - [Determined infinite game](#determined-infinite-game)
    - [Borel determinacy theorem](#borel-determinacy-theorem)
    - [Choice diagonalization of an undetermined game](#choice-diagonalization-of-an-undetermined-game)
    - [Open determinacy](#open-determinacy)
      - [Clopen determinacy with terminal losses](#clopen-determinacy-with-terminal-losses)
      - [Winning-position attractor in an infinite game](#winning-position-attractor-in-an-infinite-game)
    - [Axiom of determinacy](#axiom-of-determinacy)
      - [Projective determinacy](#projective-determinacy)
  - [Quasistrategy](#quasistrategy)
    - [Quasidetermined infinite game](#quasidetermined-infinite-game)
      - [Choice characterization of quasideterminacy](#choice-characterization-of-quasideterminacy)
- [Uniformization of a binary relation](#uniformization-of-a-binary-relation)
  - [Uniformization from determinacy](#uniformization-from-determinacy)
- [Pointclass](#pointclass)
  - [Analytic set](#analytic-set)
    - [Coanalytic set](#coanalytic-set)
  - [Projective hierarchy](#projective-hierarchy)
    - [Projective set](#projective-set)
- [Perfect set property](#perfect-set-property)
- [Suslin representation](#suslin-representation)
  - [X-Suslin set](#x-suslin-set)
    - [Kappa-Suslin set](#kappa-suslin-set)
      - [Every set of reals is continuum-Suslin](#every-set-of-reals-is-continuum-suslin)
      - [Successor-Suslin decomposition](#successor-suslin-decomposition)
      - [Aleph-one-Suslin decomposition into analytic sets](#aleph-one-suslin-decomposition-into-analytic-sets)
- [Set of well-order codes](#set-of-well-order-codes)
  - [Boundedness theorem for well-order codes](#boundedness-theorem-for-well-order-codes)
  - [Solovay rank-comparison game](#solovay-rank-comparison-game)
  - [Causal rank-raising map on well-order codes](#causal-rank-raising-map-on-well-order-codes)
- [Projectively well-ordered inner model](#projectively-well-ordered-inner-model)
  - [First uncountable ordinal of an inner model](#first-uncountable-ordinal-of-an-inner-model)
  - [Projective determinacy collapses the inner-model omega-one](#projective-determinacy-collapses-the-inner-model-omega-one)
- [Friedman–Moschovakis coding lemma](#friedman-moschovakis-coding-lemma)
  - [Friedman–Moschovakis coding game](#friedman-moschovakis-coding-game)

## Baire space of sequences

↑ **Parent:** [Descriptive set theory](descriptive-set-theory.md)

The set-theoretic Baire space is $\omega^\omega$, the set of all infinite [sequences](real-analysis.md#sequence) of [natural numbers](arithmetic.md#natural-number), with the product topology obtained from discrete $\omega$.

## Infinite game of perfect information

↑ **Parent:** [Descriptive set theory](descriptive-set-theory.md)

For $A\subseteq M^\omega$, the game $G(A)$ has two players alternately choose elements of the move set $M$, producing $x\in M^\omega$. Player I wins exactly when $x\in A$. Both players see the whole finite position before making each move.

### Covering of an infinite game

↑ **Parent:** [Infinite game of perfect information](#infinite-game-of-perfect-information)

A covering consists of a new game tree, a length-preserving prefix map to the original tree, and maps taking strategies of each player to strategies of that same player. Every play following a projected strategy lifts to a play following the original strategy, with identical projection or a premature terminal loss for that strategy's player. Terminal outcomes inherited from the original tree are respected. The strategy maps are local in depth. These conditions transfer every winning strategy, for any payoff pulled back by the prefix map. A $k$-covering leaves all positions, outcomes and strategy choices through depth $k$ unchanged.

#### Depth-stabilizing inverse limit of game coverings

↑ **Parent:** [Covering of an infinite game](#covering-of-an-infinite-game)

In a sequence of [game coverings](#covering-of-an-infinite-game) whose unchanged initial depths tend to infinity, each finite game-tree level eventually stabilizes. These stable levels form a limit game. Compositions of prefix projections and depth-local strategy maps give limit projections and strategy maps. Lift a compatible play coherently through successive coverings. If no premature loss occurs, stabilization of its finite prefixes supplies a compatible limit play. If a premature loss occurs, subsequent lift lengths cannot increase and eventually stabilize, supplying a losing terminal limit play. This proves the lifting condition for the limit covering. It makes countably many pulled-back payoffs [clopen](topology.md#clopen-set) simultaneously in the covering proof of [Borel determinacy theorem](#borel-determinacy-theorem).

#### Unravelling of a game payoff

↑ **Parent:** [Covering of an infinite game](#covering-of-an-infinite-game)

A [covering of an infinite game](#covering-of-an-infinite-game) unravels a payoff when its inverse image is a clopen subset of the new infinite-play space. A closed payoff can be unravelled by letting Player I announce a subset of the first exit positions, and letting Player II accept that announcement or challenge one announced position. Accepted plays stop at exit positions, while challenged plays are forced through the challenged exit. Strategy-transfer maps make this more than an ordinary continuous representation of the payoff. Depth-stabilizing inverse limits of coverings handle countable unions in a transfinite induction.

##### Announcement-and-challenge covering of a closed payoff

↑ **Parent:** [Unravelling of a game payoff](#unravelling-of-a-game-payoff)

After a fixed even-depth prefix, Player I announces a move and a set $X$ of first exit positions from a [closed set](topology.md#closed-set) of infinite plays. Player II accepts, or challenges an exit $r\in X$. Acceptance follows the old game until the first exit, where I wins exactly when that exit belongs to $X$. A challenge forces play through $r$ and then resumes the old game. Infinite accepted plays remain in the closed payoff; infinite challenged plays are outside it. Thus the pulled-back payoff is [clopen](topology.md#clopen-set). For an I-strategy, transfer by initially accepting and switching to the challenged simulation at an exit in $X$. For an II-strategy, announce the set of exits that this strategy never challenges under any announcement; it must accept this set. An exit outside it permits a challenged simulation, while an exit inside it is a premature loss for II. These maps prove the [game covering](#covering-of-an-infinite-game) lifting condition, rather than merely continuity of the projection.

### Buchi game

↑ **Parent:** [Infinite game of perfect information](#infinite-game-of-perfect-information)

In a turn-based game on a set of positions, Player I wins if the play visits a specified set $F$ infinitely often. Such games are determined even on infinite arenas. With $\operatorname{Pre}(X)$ meaning positions where I can force the next position into $X$, the winning region is the greatest fixed point of $X\mapsto\mu Y((F\cap\operatorname{Pre}(X))\cup\operatorname{Pre}(Y))$. Inner ordinal ranks force the next visit; outer removal ranks give Player II only finitely many visits outside the winning region.

### Strategy in an infinite game

↑ **Parent:** [Infinite game of perfect information](#infinite-game-of-perfect-information)

A strategy assigns one legal move to every finite position at which its player is to move. A play follows the strategy when every move of that player is the assigned move.

#### Winning strategy in an infinite game

↑ **Parent:** [Strategy in an infinite game](#strategy-in-an-infinite-game)

A strategy is winning when every play that follows it is won by its player.

### Determined infinite game

↑ **Parent:** [Infinite game of perfect information](#infinite-game-of-perfect-information)

An [infinite game of perfect information](#infinite-game-of-perfect-information) is determined when one of its two players has a [winning strategy in an infinite game](#winning-strategy-in-an-infinite-game).

#### Borel determinacy theorem

↑ **Parent:** [Determined infinite game](#determined-infinite-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Borel_determinacy_theorem)

Every [infinite game of perfect information](#infinite-game-of-perfect-information) on a set-sized move alphabet with a Borel payoff in its discrete product topology has a [winning strategy in an infinite game](#winning-strategy-in-an-infinite-game) for one player. A proof strengthens the induction hypothesis to existence of arbitrary-depth-preserving [game coverings](#covering-of-an-infinite-game) unravelling the payoff. The closed-set announcement construction starts the induction. For countable unions, successive coverings stabilize each finite level and their inverse limit makes every constituent payoff clopen; their union is open and can be unravelled once more.

#### Choice diagonalization of an undetermined game

↑ **Parent:** [Determined infinite game](#determined-infinite-game)

With the [axiom of choice](set-theory.md#axiom-of-choice), enumerate both players' binary-move [strategies in an infinite game](#strategy-in-an-infinite-game) in length $\mathfrak c$. Each strategy admits $\mathfrak c$ compatible plays. At stage $\alpha$, reserve a fresh play following I's strategy as a loss for I, and a fresh play following II's strategy as a win for I. Avoid all previously reserved plays, which number less than $\mathfrak c$. The collection of the second reservations is a payoff set against which neither player has a [winning strategy in an infinite game](#winning-strategy-in-an-infinite-game). This uses no regularity assumption on $\mathfrak c$.

#### Open determinacy

↑ **Parent:** [Determined infinite game](#determined-infinite-game)

An [infinite game of perfect information](#infinite-game-of-perfect-information) with an [open set](topology.md#open-set) of winning plays for I in the [product topology](geometry-and-topology.md#product-topology) on a discrete move set has a [winning strategy in an infinite game](#winning-strategy-in-an-infinite-game) for one player. Construct a [winning-position attractor in an infinite game](#winning-position-attractor-in-an-infinite-game) by [transfinite recursion](set-theory.md#transfinite-recursion); ranks give I a terminating descent strategy inside it, and its complement gives II a strategy avoiding every winning prefix. The move set need not be countable, in the usual set theory with [axiom of choice](set-theory.md#axiom-of-choice).

##### Clopen determinacy with terminal losses

↑ **Parent:** [Open determinacy](#open-determinacy)

Allow terminal positions of an [infinite game of perfect information](#infinite-game-of-perfect-information) to carry a losing-player label. A [clopen set](topology.md#clopen-set) of infinite winning plays still gives a [determined infinite game](#determined-infinite-game). At a position where all infinite continuations have one winner, the other player can win only by forcing a terminal loss for that winner. The usual [winning-position attractor in an infinite game](#winning-position-attractor-in-an-infinite-game) decides this reachability game. The tree of remaining undecided positions is [well-founded](set-theory.md#well-founded-relation): every infinite branch would eventually have its clopen payoff decided by a prefix. Assign the already decided winners upwards by [well-founded recursion](set-theory.md#well-founded-recursion). Terminal labels are essential; a terminal node created by a covering need not be lost by the player whose turn would have come next.

##### Winning-position attractor in an infinite game

↑ **Parent:** [Open determinacy](#open-determinacy)

Start with positions whose entire extension [cylinder set](geometry-and-topology.md#cylinder-set) lies in the winning [open set](topology.md#open-set). At each successor stage add I-positions with some successor already present and II-positions with every successor already present; take unions at limit [ordinals](set-theory.md#ordinal). The stable set is the least [fixed point](function.md#fixed-point) of this [order-preserving](set.md#order-preserving-function) operation. The first entry [ordinal](set-theory.md#ordinal) supplies a strictly decreasing rank until the winning prefix is reached.

#### Axiom of determinacy

↑ **Parent:** [Determined infinite game](#determined-infinite-game)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_determinacy)

The axiom of determinacy states that every game $G(A)$ with $A\subseteq\omega^\omega$ is determined. Its version for a move set $M$ is denoted $\mathsf{AD}_M$.

##### Projective determinacy

↑ **Parent:** [Axiom of determinacy](#axiom-of-determinacy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_determinacy)

Projective determinacy states that every [infinite game of perfect information](#infinite-game-of-perfect-information) whose payoff is a [projective set](#projective-set) is determined.

### Quasistrategy

↑ **Parent:** [Infinite game of perfect information](#infinite-game-of-perfect-information)

A quasistrategy assigns a nonempty set of allowed moves to every position at which its player moves. It is winning when every play consistent with those allowed moves is won by that player.

#### Quasidetermined infinite game

↑ **Parent:** [Quasistrategy](#quasistrategy)

An [infinite game of perfect information](#infinite-game-of-perfect-information) is quasidetermined when one of the players has a winning [quasistrategy](#quasistrategy). Choosing one allowed move at every relevant position refines a winning quasistrategy to a [winning strategy in an infinite game](#winning-strategy-in-an-infinite-game) whenever the required restricted choice principle holds.

##### Choice characterization of quasideterminacy

↑ **Parent:** [Quasidetermined infinite game](#quasidetermined-infinite-game)

For every move set $M$, the statement that every quasidetermined subset of $M^\omega$ is determined is equivalent in ZF to $\mathsf{AC}_{M^{<\omega}}(M)$. The forward direction encodes an arbitrary family of nonempty subsets of $M$ into a quasidetermined game; the reverse direction chooses one move from each value of a winning quasistrategy.

## Uniformization of a binary relation

↑ **Parent:** [Descriptive set theory](descriptive-set-theory.md)

For $A\subseteq X\times Y$, a uniformization is a [function](function.md) $f$ on the projection of $A$ to $X$ such that $(x,f(x))\in A$ for every $x$ in that projection. It chooses one witness from every nonempty vertical section of $A$.

### Uniformization from determinacy

↑ **Parent:** [Uniformization of a binary relation](#uniformization-of-a-binary-relation)

Under $\mathsf{AD}_{X}$, every relation $A\subseteq X\times X$ has a uniformization. Let the first moves of Players I and II be $x$ and $y$, and let II win when $x$ is outside the projection of $A$ or $(x,y)\in A$. Player I cannot have a winning strategy, so the first response of a winning strategy for II uniformizes $A$.

## Pointclass

↑ **Parent:** [Descriptive set theory](descriptive-set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pointclass)

A pointclass is a collection of subsets of topological spaces, usually specified by a common definability or closure condition.

### Analytic set

↑ **Parent:** [Pointclass](#pointclass)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Analytic_set)

An analytic subset of a Polish space is a continuous image of a [Borel set](measure-theory.md#borel-set), equivalently a projection of a closed subset of its product with the [Baire space of sequences](#baire-space-of-sequences).

#### Coanalytic set

↑ **Parent:** [Analytic set](#analytic-set)

A coanalytic set is the complement of an [analytic set](#analytic-set).

### Projective hierarchy

↑ **Parent:** [Pointclass](#pointclass)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_hierarchy)

The projective hierarchy starts with the [Borel sets](measure-theory.md#borel-set) and repeatedly applies projection and complementation. Its members are the projective sets.

#### Projective set

↑ **Parent:** [Projective hierarchy](#projective-hierarchy)

A projective set belongs to some finite level of the [projective hierarchy](#projective-hierarchy).

## Perfect set property

↑ **Parent:** [Descriptive set theory](descriptive-set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_set_property)

A subset of a Polish space has the perfect set property when it is countable or contains a nonempty perfect subset. Every uncountable [analytic set](#analytic-set) contains a perfect subset and consequently has cardinality $2^{\aleph_0}$.

## Suslin representation

↑ **Parent:** [Descriptive set theory](descriptive-set-theory.md)

Let $T\subseteq(X\times\omega)^{<\omega}$ be a [tree](combinatorics.md#tree-graph-theory). Its projection is

$$
p[T]=\{x\in\omega^\omega:\exists y\in X^\omega\ ((y,x)\in[T])\}.
$$

The tree $T$ is a Suslin representation of $p[T]$.

### X-Suslin set

↑ **Parent:** [Suslin representation](#suslin-representation)

A set $A\subseteq\omega^\omega$ is $X$-Suslin when $A=p[T]$ for a [tree](combinatorics.md#tree-graph-theory) $T\subseteq(X\times\omega)^{<\omega}$.

#### Kappa-Suslin set

↑ **Parent:** [X-Suslin set](#x-suslin-set)

A $\kappa$-Suslin set is an $X$-Suslin set with $X=\kappa$. If $X$ injects into $Y$, relabelling a [Suslin representation](#suslin-representation) shows that every $X$-Suslin set is $Y$-Suslin.

##### Every set of reals is continuum-Suslin

↑ **Parent:** [Kappa-Suslin set](#kappa-suslin-set)

Every $A\subseteq\omega^\omega$ is $2^{\aleph_0}$-Suslin. Give each $a\in A$ its own label and use the tree of finite pairs $(a\mathbin{\upharpoonright}n,a\mathbin{\upharpoonright}n)$, then relabel the first coordinate by an injection into a set of size $2^{\aleph_0}$.

##### Successor-Suslin decomposition

↑ **Parent:** [Kappa-Suslin set](#kappa-suslin-set)

For an infinite [cardinal number](set-theory.md#cardinal-number) $\kappa$, every $\kappa^+$-Suslin set is a union of $\kappa^+$ many $\kappa$-Suslin sets. A countable sequence of ordinals below the [successor cardinal](set-theory.md#successor-cardinal) $\kappa^+$ is bounded there, so restrict the representing tree successively to labels below each $\alpha<\kappa^+$.

##### Aleph-one-Suslin decomposition into analytic sets

↑ **Parent:** [Kappa-Suslin set](#kappa-suslin-set)

Every $\aleph_1$-Suslin set is a union of $\aleph_1$ [analytic sets](#analytic-set). Every countable sequence of countable ordinals is bounded below $\omega_1$, and after restricting all labels below one countable ordinal the first-coordinate space can be recoded by $\omega$.

## Set of well-order codes

↑ **Parent:** [Descriptive set theory](descriptive-set-theory.md)

The set $\mathrm{WF}\subseteq\omega^\omega$ consists of the reals coding [well-orders](set.md#well-order) of $\omega$. For $x\in\mathrm{WF}$, the norm $\lVert x\rVert$ is the [order type](set-theory.md#order-type) of the well-order coded by $x$.

### Boundedness theorem for well-order codes

↑ **Parent:** [Set of well-order codes](#set-of-well-order-codes)

Every [analytic set](#analytic-set) contained in $\mathrm{WF}$ has bounded rank: if $A\subseteq\mathrm{WF}$ is analytic, then

$$
\sup\{\lVert x\rVert:x\in A\}<\omega_1.
$$

In particular, the well-order codes produced continuously from all counterplays against one strategy have bounded ranks whenever they are all well-founded.

### Solovay rank-comparison game

↑ **Parent:** [Set of well-order codes](#set-of-well-order-codes)

In the Solovay rank-comparison game, Players I and II produce $x,y\in\omega^\omega$; ill-founded codes lose before ranks are compared, and among well-order codes the prescribed inequality between $\lVert x\rVert$ and $\lVert y\rVert$ decides the winner. No strategy for Player I can uniformly produce a well-order code at least as long as every code produced by Player II.

### Causal rank-raising map on well-order codes

↑ **Parent:** [Set of well-order codes](#set-of-well-order-codes)

There is a coordinatewise causal map $S:\omega^\omega\to\omega^\omega$ that recodes a relation after adjoining a new least element. If $x\in\mathrm{WF}$, then $S(x)\in\mathrm{WF}$ and $\lVert S(x)\rVert=\lVert x\rVert+1$; the tagged coding also ensures $S(x)\ne x$ when $x\notin\mathrm{WF}$. Because the first $n+1$ output coordinates depend only on the first $n+1$ input coordinates, Player II can produce $S(x)$ online.

## Projectively well-ordered inner model

↑ **Parent:** [Descriptive set theory](descriptive-set-theory.md)

An [inner model](set-theory.md#inner-model) $M$ is projectively well-ordered when there is a [projective](#projective-set) relation that well-orders the real numbers belonging to $M$.

### First uncountable ordinal of an inner model

↑ **Parent:** [Projectively well-ordered inner model](#projectively-well-ordered-inner-model)

For an [inner model](set-theory.md#inner-model) $M$, the ordinal $\omega_1^M$ is the least ordinal that $M$ regards as uncountable. Equivalently, it is the supremum of the order types of the [well-order codes](definable-power-set.md#well-order-code) belonging to $M$. It can be countable in the ambient universe.

### Projective determinacy collapses the inner-model omega-one

↑ **Parent:** [Projectively well-ordered inner model](#projectively-well-ordered-inner-model)

If $M$ is projectively well-ordered and [projective determinacy](#projective-determinacy) holds, then $\omega_1^M$ is countable in the ambient universe. Otherwise, selecting with the projective well-order the least $M$-code for each countable ordinal produces an uncountable projective set of unique well-order codes. It has no perfect subset by the [boundedness theorem for well-order codes](#boundedness-theorem-for-well-order-codes), contradicting the [perfect set property](#perfect-set-property) implied by projective determinacy.

<h2 id="friedman-moschovakis-coding-lemma">Friedman–Moschovakis coding lemma</h2>

↑ **Parent:** [Descriptive set theory](descriptive-set-theory.md)

Assume the [axiom of determinacy](#axiom-of-determinacy). If $\lambda$ is a surjective image of the [Baire space of sequences](#baire-space-of-sequences) and, for every $\xi<\lambda$, the power set $\mathcal P(\xi)$ is a surjective image of that space, then $\mathcal P(\lambda)$ is also a surjective image of it.

<h3 id="friedman-moschovakis-coding-game">Friedman–Moschovakis coding game</h3>

↑ **Parent:** [Friedman–Moschovakis coding lemma](#friedman-moschovakis-coding-lemma)

For $A\subseteq\lambda$, the Friedman–Moschovakis coding game asks the players to present coherent local codes for initial segments $A\cap\xi$ while challenging each other at larger ordinals. The diagonal and boundedness argument rules out a winning strategy for Player I; a winning strategy for Player II determines at most one set $A$. Coding strategies by reals therefore gives a surjection from the [Baire space of sequences](#baire-space-of-sequences) onto $\mathcal P(\lambda)$.

## ↑ Ancestors (5)

1. [Set theory](set-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
