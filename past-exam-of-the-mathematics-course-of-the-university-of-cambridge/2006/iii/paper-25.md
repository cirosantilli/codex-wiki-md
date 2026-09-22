# Paper 25

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper25.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper25.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)
- [7](#7)
  - [Solution](#7/solution)
- [8](#8)
  - [Solution](#8/solution)
- [9](#9)
  - [Solution](#9/solution)
- [10](#10)
  - [Solution](#10/solution)
- [11](#11)
  - [i](#11/i)
    - [Solution](#11/i/solution)
  - [ii](#11/ii)
    - [Solution](#11/ii/solution)
  - [iii](#11/iii)
    - [Solution](#11/iii/solution)

## 1

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [partial computable function](../../../foundations-of-mathematics.md#computable-function) is the [function](../../../function.md) computed by a finite program, with an undefined value when its computation never terminates. A [total computable function](../../../foundations-of-mathematics.md#total-computable-function) terminates on every input. Fix an effective enumeration $(\varphi_e)_{e\in\omega}$ of the [partial computable functions](../../../foundations-of-mathematics.md#computable-function), with a [universal partial computable function](../../../foundations-of-mathematics.md#universal-partial-computable-function) $U(e,x)=\varphi_e(x)$. Composition, [primitive recursion](../../../foundations-of-mathematics.md#primitive-recursion) and [unbounded minimization](../../../foundations-of-mathematics.md#mu-operator) give a machine-independent description of this class. [Unbounded minimization](../../../foundations-of-mathematics.md#mu-operator) is allowed to diverge. The [S-m-n theorem](../../../foundations-of-mathematics.md#smn-theorem) permits parameters in a program to be specialized effectively: an algorithm described uniformly in $e$ has an index obtained computably from $e$.

The [halting set](../../../foundations-of-mathematics.md#halting-set) $K=\{e:\varphi_e(e)\text{ halts}\}$ is [computably enumerable](../../../foundations-of-mathematics.md#recursively-enumerable-set): simulate all computations in parallel and enumerate each index whose diagonal computation terminates. It is not a [computable set](../../../foundations-of-mathematics.md#computable-set). Otherwise the program which terminates exactly when the proposed decision procedure says its own diagonal computation does not terminate gives a contradiction. There is also no effective enumeration consisting exactly of all [total computable functions](../../../foundations-of-mathematics.md#total-computable-function): from such an enumeration $(f_n)$ the [total computable function](../../../foundations-of-mathematics.md#total-computable-function) $g(n)=f_n(n)+1$ differs from every listed [function](../../../function.md). Thus the effective enumeration of partial programs cannot be replaced by a decidable catalogue of total ones.

For the [Rice theorem](../../../foundations-of-mathematics.md#rice-s-theorem), let $C$ be a nontrivial property of [partial computable functions](../../../foundations-of-mathematics.md#computable-function), depending on the computed [function](../../../function.md) rather than the program text. First suppose the nowhere-defined [function](../../../function.md) is not in $C$, and choose a program computing some $g\in C$. Uniformly in $e$, define a program which, on input $x$, first waits for $\varphi_e(e)$ to terminate and then runs the computation of $g(x)$. The [S-m-n theorem](../../../foundations-of-mathematics.md#smn-theorem) gives a computable index map $e\mapsto p(e)$, and

$$
\varphi_{p(e)}=\begin{cases}g,&e\in K,\\\text{nowhere-defined function},&e\notin K.\end{cases}
$$

Consequently a decision procedure for membership in $C$ would decide the [halting set](../../../foundations-of-mathematics.md#halting-set). If the nowhere-defined [function](../../../function.md) belongs to $C$, apply the same argument to its complement. **Every nontrivial extensional property of [partial computable functions](../../../foundations-of-mathematics.md#computable-function) has an undecidable index [set](../../../set.md).** Syntactic properties of program descriptions are outside this assertion, and the theorem concerns unrestricted program indices, not merely an assumed list of terminating programs.

Here is an explicit [Jockusch triple coloring computing the halting set](../../../foundations-of-mathematics.md#jockusch-triple-coloring-computing-the-halting-set). Choose computable increasing finite stages $K_s$ with [union](../../../set.md#set-union) $K$. For $x<y<z$, put

$$
c(\{x,y,z\})=\begin{cases}0,&K_y\cap x=K_z\cap x,\\1,&K_y\cap x\ne K_z\cap x.\end{cases}
$$

This is a [computable colouring](../../../ramsey-theory.md#computable-colouring). An infinite [monochromatic](../../../ramsey-theory.md#monochromatic-set) [set](../../../set.md) cannot have color $1$: fix its first element $x$ and choose two later elements beyond the stage at which $K_s\cap x$ stabilizes. Their triple has color $0$.

Suppose $H$ is infinite and homogeneous of color $0$. To decide whether $n\in K$ using $H$, find $x\in H$ with $x>n$, and then $y\in H$ with $y>x$. For every $z\in H$ above $y$, homogeneity gives $K_y\cap x=K_z\cap x$. Such $z$ are unbounded, so $K_y\cap x=K\cap x$. Testing $n\in K_y$ therefore decides $n\in K$. Hence every [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) computes the [halting set](../../../foundations-of-mathematics.md#halting-set), and **there is no infinite recursive [monochromatic set](../../../ramsey-theory.md#monochromatic-set).** The [infinity](../../../mathematics.md#infinity) qualification is essential: finite [homogeneous sets](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) are recursive.

## 2

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Work in a ground [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of [set theory](../../../set-theory.md) satisfying [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory), and let $\pi$ be a definable [bijection](../../../function.md#bijection) of its universe, whose inverse is also definable. Write $\psi=\pi^{-1}$ and replace membership by

$$
x\mathrel E y\quad\Longleftrightarrow\quad x\in\pi(y).
$$

In this [Rieger-Bernays permutation model](../../../set-theory.md#rieger-bernays-permutation-model), an object having prescribed extension $b$ is represented by $\psi(b)$. The [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) in the ground model guarantees that images of [sets](../../../set.md) under $\pi$ and $\psi$ are [sets](../../../set.md). The [axiom of extensionality](../../../set-theory.md#axiom-of-extensionality) follows from injectivity of $\pi$; the new [empty set](../../../set.md#empty-set) is $\psi(\varnothing)$, and the new pair of $x,y$ is $\psi(\{x,y\})$.

For the [Axiom of union](../../../set-theory.md#axiom-of-union) and [Axiom of power set](../../../set-theory.md#axiom-of-power-set), representatives are respectively

$$
\psi\left(\bigcup_{y\in\pi(x)}\pi(y)\right),\qquad
\psi\left(\{\psi(s):s\subseteq\pi(x)\}\right).
$$

Indeed, $z$ is an $E$-subset of $x$ exactly when $\pi(z)\subseteq\pi(x)$. Translate every [first-order formula](../../../mathematical-logic.md#first-order-formula) by replacing membership with membership in $\pi(y)$. Ground [separation](../../../set-theory.md#axiom-schema-of-specification) then forms each desired subextension of $\pi(x)$, and ground [replacement](../../../set-theory.md#axiom-schema-of-replacement) forms each functional image; applying $\psi$ supplies its representative. To verify the [axiom of infinity](../../../set-theory.md#axiom-of-infinity), define by ground recursion

$$
a_0=\psi(\varnothing),\qquad a_{n+1}=\psi(\pi(a_n)\cup\{a_n\}).
$$

Then $\psi(\{a_n:n<\omega\})$ is an $E$-inductive [set](../../../set.md). Thus every [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axiom except possibly the [Axiom of foundation](../../../set-theory.md#axiom-of-regularity) survives.

Interchange two distinct objects $a$ and $\{a\}$, fixing everything else. Then $\pi(a)=\{a\}$, so $a$ is a [Quine atom](../../../set-theory.md#quine-atom): internally $a=\{a\}$. The nonempty [set](../../../set.md) $a$ has no member disjoint from itself, violating the [Axiom of foundation](../../../set-theory.md#axiom-of-regularity). The original membership model satisfies that axiom. **[Foundation](../../../set-theory.md#axiom-of-regularity) is therefore relatively independent of the other [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axioms.**

A full [Rieger-Bernays permutation model](../../../set-theory.md#rieger-bernays-permutation-model) of a choice model still satisfies the [axiom of choice](../../../set-theory.md#axiom-of-choice): choose an old member of each nonempty extension $\pi(y)$ and encode the resulting choice graph with the new ordered-pair operations. To obtain failure of choice, an additional restriction by symmetries is necessary.

Start instead with [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) and use the definable permutation interchanging every $a_n=\omega+n$ with $\{a_n\}$. These transpositions are disjoint and produce an [infinite set](../../../set.md#infinite-set) $A$ of [Quine atoms](../../../set-theory.md#quine-atom). Inside the resulting membership model build the cumulative universe over $A$, closing at successive stages under [sets](../../../set.md) of previously constructed objects, represented by $\psi(X)$. Atomic objects are kept as the designated base objects; $\psi(\{a\})=a$ for $a\in A$. Every permutation of $A$ extends recursively to an automorphism of this universe, with the atomic self-loops fixed by the recursive convention.

An object has [finite support](../../../group-theory.md#finite-support-in-a-permutation-action) if every permutation fixing some finite $S\subseteq A$ pointwise fixes it. Retain the objects which have [finite support](../../../group-theory.md#finite-support-in-a-permutation-action) and whose members recursively also have [finite support](../../../group-theory.md#finite-support-in-a-permutation-action), interpreting the atomic self-loops as the base case. This is the [hereditarily finite-supported Quine-atom model](../../../set-theory.md#hereditarily-finite-supported-quine-atom-model). It is transitive for the new membership relation. [Extensionality](../../../set-theory.md#axiom-of-extensionality) is inherited. Pairs and [unions](../../../set.md#set-union) have supports contained in the [union](../../../set.md#set-union) of the finitely many relevant supports. For a supported [set](../../../set.md) $x$, the collection of all retained [subsets](../../../set.md#subset) of $x$ is a ground [set](../../../set.md), by the full model's [power set](../../../set.md#power-set) axiom, and is fixed by every permutation fixing a support of $x$. Its members are retained, so this collection supplies the internal [power set](../../../set.md#power-set). A [first-order formula](../../../mathematical-logic.md#first-order-formula) with retained parameters is invariant under their common stabilizer. Consequently its definable [subset](../../../set.md#subset) of $x$, and the range of a functional relation on $x$, have that same [finite support](../../../group-theory.md#finite-support-in-a-permutation-action); ground [separation](../../../set-theory.md#axiom-schema-of-specification) and [replacement](../../../set-theory.md#axiom-schema-of-replacement) first ensure that they are [sets](../../../set.md). The pure natural-number hierarchy supplies [infinity](../../../mathematics.md#infinity). These arguments verify all of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) except [Axiom of foundation](../../../set-theory.md#axiom-of-regularity), which fails at the [Quine atoms](../../../set-theory.md#quine-atom).

The family $[A]^2$ of all two-element [subsets](../../../set.md#subset) is retained and has empty support. If it had a retained choice [function](../../../function.md) $f$, choose two distinct [Quine atoms](../../../set-theory.md#quine-atom) $a,b$ outside a [finite support](../../../group-theory.md#finite-support-in-a-permutation-action) of $f$. The transposition of $a,b$ fixes $f$ and fixes the unordered pair $\{a,b\}$, but moves either possible value $f(\{a,b\})$. This is impossible. Thus **[ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) without [Foundation](../../../set-theory.md#axiom-of-regularity) has both choice models and models in which Choice fails**, relative to the usual consistency assumption. The construction also explains why twisting membership alone was insufficient.

## 3

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use [rooted-tree homeomorphic embedding](../../../combinatorics.md#homeomorphic-embedding-of-a-rooted-tree): edges may be stretched into downward paths, different child branches stay disjoint, and the source root may map to any target vertex. Write $S\preceq T$ for this relation. More generally allow labels in a [well-quasi-ordering](../../../set.md#well-quasi-ordering) $Q$ and require every source label to be at most its image label. We prove this labelled version, which includes the unlabelled case by taking one label.

First, every infinite [sequence](../../../real-analysis.md#sequence) in a [well-quasi-ordering](../../../set.md#well-quasi-ordering) has an infinite nondecreasing subsequence. In every [infinite set](../../../set.md#infinite-set) of indices there is an index with infinitely many later successors above its value. Otherwise repeatedly discard the finitely many successors of each chosen index, obtaining a [bad sequence](../../../set.md#bad-sequence). Applying this observation successively within the infinite successor [set](../../../set.md) produces the required [subsequence](../../../real-analysis.md#subsequence).

We also need the [Higman lemma](../../../set.md#higman-s-lemma), and prove it here. If finite [words](../../../foundations-of-mathematics.md#string) over $Q$ admitted a [bad sequence](../../../set.md#bad-sequence), choose one $w_0,w_1,\ldots$ with each [word](../../../foundations-of-mathematics.md#string) of least possible length among choices permitting a bad continuation of its fixed prefix. No [word](../../../foundations-of-mathematics.md#string) is empty. Write $w_i=v_i a_i$, and extract indices $n_0<n_1<\cdots$ with $a_{n_0}\le a_{n_1}\le\cdots$. The [sequence](../../../real-analysis.md#sequence)

$$
w_0,\ldots,w_{n_0-1},v_{n_0},v_{n_1},\ldots
$$

is bad: an earlier $w_i$ embedding into some $v_{n_j}$ would embed into $w_{n_j}$, while $v_{n_i}\preceq v_{n_j}$ together with $a_{n_i}\le a_{n_j}$ would give $w_{n_i}\preceq w_{n_j}$. This contradicts the minimal length of $w_{n_0}$, since $v_{n_0}$ is shorter. Hence finite [words](../../../foundations-of-mathematics.md#string) are [well-quasi-ordered](../../../set.md#well-quasi-ordering) under [subsequence](../../../real-analysis.md#subsequence) embedding with increased labels.

Now suppose labelled [rooted trees](../../../combinatorics.md#rooted-tree) admitted a [bad sequence](../../../set.md#bad-sequence) $T_0,T_1,\ldots$, chosen minimally by number of vertices at each successive position. Let $B$ consist of all immediate child subtrees of all the $T_i$, with the inherited labels. We claim $B$ is a [well-quasi-ordering](../../../set.md#well-quasi-ordering). Otherwise take a bad [sequence](../../../real-analysis.md#sequence) of members of $B$. Only finitely many distinct [rooted trees](../../../combinatorics.md#rooted-tree) occur among the children of any finite initial list of $T_i$, so, by discarding terms and selecting a [subsequence](../../../real-analysis.md#subsequence), we may arrange its members $S_0,S_1,\ldots$ to come from strictly increasing parent indices $n_0<n_1<\cdots$. Then

$$
T_0,\ldots,T_{n_0-1},S_0,S_1,\ldots
$$

is bad. A prefix [rooted tree](../../../combinatorics.md#rooted-tree) embedding into $S_j$ would embed into its parent $T_{n_j}$; embeddings between the $S_j$ are excluded by their choice. But $S_0$ has fewer vertices than $T_{n_0}$, contradicting minimality. This proves the claim.

List the child subtrees of each $T_i$ in any order. By the [Higman lemma](../../../set.md#higman-s-lemma) these child lists are [well-quasi-ordered](../../../set.md#well-quasi-ordering). Extract an infinite [subsequence](../../../real-analysis.md#subsequence) with nondecreasing root labels, and then compare two child lists on that [subsequence](../../../real-analysis.md#subsequence). Their [subsequence](../../../real-analysis.md#subsequence) embedding gives distinct target child branches into which the source child subtrees embed. Map the source root to the target root and join each embedded child root to it by the corresponding downward path. The paths are disjoint except at the root, and labels increase. Thus $T_i\preceq T_j$ for some $i<j$, contradicting badness. This proves [Kruskal's tree theorem](../../../set.md#kruskal-s-tree-theorem) and its labelled version. If root preservation is required, mark the root with a special label incomparable with all ordinary labels; the same proof then forces root to map to root.

For [Friedman's finite form of Kruskal's theorem](../../../set.md#friedman-s-finite-form-of-kruskal-s-theorem), fix $k\in\omega$ and suppose there are arbitrarily long bad lists satisfying $|T_i|\le k+i$ for $i=1,2,\ldots$. Make a [finite bad-sequence tree](../../../set.md#finite-bad-sequence-tree) whose nodes are these lists, using one representative of each finite rooted-[rooted tree](../../../combinatorics.md#rooted-tree) isomorphism type. At each position only finitely many choices satisfy the size bound, so the [rooted tree](../../../combinatorics.md#rooted-tree) is finitely branching. An infinite path exists: at every stage choose a child having extensions of arbitrarily large length, which must exist because there are finitely many children. The path is an infinite bad [sequence](../../../real-analysis.md#sequence), contradicting [Kruskal's tree theorem](../../../set.md#kruskal-s-tree-theorem). Therefore

$$
\boxed{\forall k\in\omega\ \exists N\ \forall (T_i)_{1\le i\le N}\quad
\bigl[(\forall i\ |T_i|\le k+i)\Rightarrow(\exists i<j\ T_i\preceq T_j)\bigr].}
$$

The identical argument works with finitely many labels and any fixed finite size bound at each position.

## 4

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [axiom of determinacy](../../../descriptive-set-theory.md#axiom-of-determinacy), abbreviated AD, asserts that every length-$\omega$ [infinite game of perfect information](../../../descriptive-set-theory.md#infinite-game-of-perfect-information) in which the two players alternately choose [natural numbers](../../../arithmetic.md#natural-number) is determined. For a payoff [set](../../../set.md) $A\subseteq\omega^\omega$, player I wins exactly when the completed play belongs to $A$. A [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) specifies the next move at every finite position where its player is to move; determination means that one player has a [winning strategy](../../../descriptive-set-theory.md#winning-strategy-in-an-infinite-game).

Finite games are determined by backward induction, choosing the least move leading to a guaranteed win when several are available. In [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) one can also prove [open determinacy](../../../descriptive-set-theory.md#open-determinacy), hence determinacy for closed payoffs. Here is the full open-payoff argument. Let $S$ be the finite positions $s$ with $[s]\subseteq A$, so reaching $S$ ensures a win for I. Starting with $W_0=S$, repeatedly add an I-position with some child already in $W$, and a II-position with every child already in $W$; take [unions](../../../set.md#set-union) at limit stages. This increasing process stabilizes because the [set](../../../set.md) of finite positions is a [set](../../../set.md): continuing strict enlargement through its Hartogs number would choose distinct new positions, contradicting that bound. Assign to each admitted position its least entry stage.

At an I-position in the final $W$, choose the least child of smaller entry stage. At a II-position in $W\setminus S$, every child has smaller entry stage. A play following this I-strategy cannot remain outside $S$ forever, since that would give an infinite strictly descending [sequence](../../../real-analysis.md#sequence) of [ordinals](../../../set-theory.md#ordinal). It reaches $S$ and wins. Outside $W$, every child of an I-position remains outside $W$, and a II-position has at least one child outside $W$. Player II chooses the least such child. The play never reaches $S$, so it cannot belong to the [open set](../../../topology.md#open-set) $A$. The initial position is either inside or outside $W$, proving determination. For a closed payoff apply the same argument to the open complementary payoff for the other player, with the appropriate player assigned to each level. None of these [strategies](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) needs a choice principle because moves are [natural numbers](../../../arithmetic.md#natural-number) and least available moves are definable.

To refute simultaneous AD and the [axiom of choice](../../../set-theory.md#axiom-of-choice), assume choice and [well-order](../../../set.md#well-order) all [strategies](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) of either player in length $\mathfrak c=2^{\aleph_0}$. There are exactly $\mathfrak c$ [strategies](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) for each player, and any fixed [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) has exactly $\mathfrak c$ compatible plays, since the opponent's successive moves are arbitrary. At stage $\alpha<\mathfrak c$, choose two fresh plays: $x_\alpha$ compatible with I's $\alpha$th [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game), and $y_\alpha$ compatible with II's $\alpha$th [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game). Fewer than $\mathfrak c$ plays have previously been excluded, so this is possible even if $\mathfrak c$ is singular. Put $A=\{y_\alpha:\alpha<\mathfrak c\}$. No $x_\alpha$ ever enters $A$. I's $\alpha$th [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) loses on $x_\alpha$, and II's $\alpha$th [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) loses on $y_\alpha$. Thus this game has no [winning strategy](../../../descriptive-set-theory.md#winning-strategy-in-an-infinite-game) for either player, and

$$
\boxed{\mathsf{AD}\ \Longrightarrow\ \neg\mathsf{AC}.}
$$

## 5

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

All assertions of independence below are relative consistency assertions. We construct structures satisfying the other [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axioms but falsifying the indicated axiom; an ordinary model of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) supplies the positive side. The convenient ground theory is [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), which has the same consistency strength as [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) by the [constructible universe theorem](../../../definable-power-set.md#constructible-universe-theorem).

For the [Axiom of union](../../../set-theory.md#axiom-of-union), put $\lambda=\beth_\omega$ and use the [hereditarily locally small membership model](../../../set-theory.md#hereditarily-locally-small-membership-model)

$$
B_\lambda=\{x:\forall y\in\operatorname{TC}(\{x\})\ (|y|<\lambda)\}.
$$

It is a [transitive class](../../../set-theory.md#transitive-class). The condition requires each individual [set](../../../set.md) in the membership ancestry to have size below $\lambda$; it does not require its entire [transitive closure](../../../set-theory.md#transitive-closure) to have size below $\lambda$. [Extensionality](../../../set-theory.md#axiom-of-extensionality) and [foundation](../../../set-theory.md#axiom-of-regularity) are inherited. Pairs and [subsets](../../../set.md#subset) of members remain in the class, giving [pairing](../../../set-theory.md#axiom-of-pairing) and [separation](../../../set-theory.md#axiom-schema-of-specification), and $\omega$ witnesses [infinity](../../../mathematics.md#infinity). For $x\in B_\lambda$, the actual $\mathcal P(x)$ also belongs to $B_\lambda$: if $|x|=\mu<\lambda$, then $2^\mu<\lambda$ by the strong-limit property, while every [subset](../../../set.md#subset) of $x$ and every member further below it remains locally small. This verifies the full [power set](../../../set.md#power-set) axiom. If an internally definable functional relation has domain $x\in B_\lambda$, ground [replacement](../../../set-theory.md#axiom-schema-of-replacement), applied to the relativized [first-order formula](../../../mathematical-logic.md#first-order-formula), gives its range $r$. Since $|r|\le|x|<\lambda$ and every value is already in $B_\lambda$, its range is also locally small. Thus every [replacement](../../../set-theory.md#axiom-schema-of-replacement) instance holds.

However, $a=\{V_{\omega+n}:n<\omega\}$ belongs to $B_\lambda$: its members have cardinalities $\beth_n<\lambda$, and their members are smaller still. Its actual [union](../../../set.md#set-union) is $V_{\omega+\omega}$, of [cardinality](../../../set-theory.md#cardinality) $\beth_\omega=\lambda$, which is not in $B_\lambda$. Transitivity makes any internal [union](../../../set.md#set-union) witness equal to this actual [union](../../../set.md#set-union). Hence **[Union](../../../set.md#set-union) fails while all the other [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axioms hold.**

For the [Axiom of power set](../../../set-theory.md#axiom-of-power-set), use the [hereditarily countable sets](../../../set-theory.md#hereditarily-countable-set) $H_{\omega_1}$ in the ground choice universe. This is transitive and contains $\omega$. Pairs, [subsets](../../../set.md#subset) and [unions](../../../set.md#set-union) have [countable](../../../set-theory.md#countable-set) [transitive closure](../../../set-theory.md#transitive-closure). For [replacement](../../../set-theory.md#axiom-schema-of-replacement), a functional image of a [countable](../../../set-theory.md#countable-set) domain is [countable](../../../set-theory.md#countable-set), and the [union](../../../set.md#set-union) of countably many [countable](../../../set-theory.md#countable-set) transitive closures is [countable](../../../set-theory.md#countable-set); hence that image is again hereditarily [countable](../../../set-theory.md#countable-set). These observations, with inherited [extensionality](../../../set-theory.md#axiom-of-extensionality) and [foundation](../../../set-theory.md#axiom-of-regularity), verify all the remaining axioms. Every real, viewed as a [subset](../../../set.md#subset) of $\omega$, belongs to $H_{\omega_1}$. A power-set witness for $\omega$ would therefore contain every such real, but a hereditarily [countable](../../../set-theory.md#countable-set) [set](../../../set.md) has only countably many members, whereas $\mathcal P(\omega)$ is [uncountable](../../../set-theory.md#uncountable-set) by [Cantor's theorem](../../../set.md#cantor-s-theorem). **[Power set](../../../set.md#power-set) fails.**

For the [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement), use $V_{\omega+\omega}$ with actual membership. This limit-rank structure contains $\omega$ and is closed under pairs, [unions](../../../set.md#set-union) and [power sets](../../../set.md#power-set): every relevant finite increase in rank stays below $\omega+\omega$. A separated [subset](../../../set.md#subset) has rank no higher than that of the original [set](../../../set.md). [Extensionality](../../../set-theory.md#axiom-of-extensionality) and [foundation](../../../set-theory.md#axiom-of-regularity) are inherited. The internally definable [function](../../../function.md)

$$
f:\omega\longrightarrow V_{\omega+\omega},\qquad f(n)=V_{\omega+n},
$$

is obtained by $n$ successive power-set operations starting with the parameter $V_\omega$. Each finite iteration, including its finite history, belongs to the structure. Its range has rank $\omega+\omega$ and is not an element of $V_{\omega+\omega}$. Thus the [replacement](../../../set-theory.md#axiom-schema-of-replacement) instance for this [first-order formula](../../../mathematical-logic.md#first-order-formula) fails, although every other [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axiom holds.

For the [axiom of extensionality](../../../set-theory.md#axiom-of-extensionality), take the well-founded cumulative [set](../../../set.md) universe over two distinct [urelements](../../../set-theory.md#urelement), and forget the predicate distinguishing [urelements](../../../set-theory.md#urelement) from [sets](../../../set.md). Each [urelement](../../../set-theory.md#urelement) has no members, just as the ordinary [empty set](../../../set.md#empty-set) has no members, so [extensionality](../../../set-theory.md#axiom-of-extensionality) fails. Every other axiom survives in this pure membership language. [Pairing](../../../set-theory.md#axiom-of-pairing), [union](../../../set.md#set-union), [separation](../../../set-theory.md#axiom-schema-of-specification) and [replacement](../../../set-theory.md#axiom-schema-of-replacement) are witnessed by the corresponding ordinary [sets](../../../set.md) of [urelements](../../../set-theory.md#urelement) and [sets](../../../set.md); [foundation](../../../set-theory.md#axiom-of-regularity) follows from their well-founded ranks, and the pure $\omega$ supplies [infinity](../../../mathematics.md#infinity). Here [foundation](../../../set-theory.md#axiom-of-regularity) is written with “has a member” as its nonemptiness antecedent, and disjointness means having no common member. Formulations using inequality to one designated empty object are not equivalent after removing [extensionality](../../../set-theory.md#axiom-of-extensionality). There is also one necessary adjustment to [power set](../../../set.md#power-set): an [urelement](../../../set-theory.md#urelement) is vacuously a [subset](../../../set.md#subset) of every object because it has no members. Thus the power-set witness for $x$ is the ordinary [set](../../../set.md) of all usual [subsets](../../../set.md#subset) of its extension, together with both [urelements](../../../set-theory.md#urelement). This is still a [set](../../../set.md), and contains exactly the objects satisfying the unrestricted [subset](../../../set.md#subset) [first-order formula](../../../mathematical-logic.md#first-order-formula). Consequently **the countermodel falsifies [Extensionality](../../../set-theory.md#axiom-of-extensionality) alone**, without silently weakening [Power set](../../../set.md#power-set) to [sets](../../../set.md) only.

Finally, the [hereditarily finite sets](../../../set-theory.md#hereditarily-finite-set) $V_\omega$ satisfy [extensionality](../../../set-theory.md#axiom-of-extensionality), [foundation](../../../set-theory.md#axiom-of-regularity), [pairing](../../../set-theory.md#axiom-of-pairing), [union](../../../set.md#set-union), [power set](../../../set.md#power-set) and [separation](../../../set-theory.md#axiom-schema-of-specification). Every functional image of a finite domain is a [finite set](../../../set.md#finite-set) of hereditarily finite objects, hence also belongs to $V_\omega$, giving all [replacement](../../../set-theory.md#axiom-schema-of-replacement) instances. No [finite set](../../../set.md#finite-set) contains $\varnothing$ and is closed under successor: it would then contain every finite von Neumann [ordinal](../../../set-theory.md#ordinal). **[Infinity](../../../mathematics.md#infinity) fails while the remaining axioms hold.**

## 6

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Let $M$ be an externally [countable](../../../set-theory.md#countable-set) model of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), and let $\kappa=(\omega_1)^M$. In $M$ form the forcing order

$$
\mathbb P=\{p:p\text{ is a finite partial function }\omega\longrightarrow\kappa\},\qquad q\le p\iff q\supseteq p.
$$

This is the [finite-function collapse to countable size](../../../forcing.md#finite-function-collapse-to-countable-size). For every $n\in\omega^M$ and $\alpha\in\kappa^M$, the internal [sets](../../../set.md)

$$
D_n=\{p:n\in\operatorname{dom}(p)\},\qquad E_\alpha=\{p:\alpha\in\operatorname{ran}(p)\}
$$

are dense: extend a finite [function](../../../function.md) by assigning a missing input, and use a fresh input to put any required value in its range.

Externally enumerate all the dense [subsets](../../../set.md#subset) of $\mathbb P$ which $M$ recognizes as dense. There are only countably many, because $M$ is [countable](../../../set-theory.md#countable-set). Recursively choose $p_{i+1}\le p_i$ in the $i$th such dense [set](../../../set.md) and let $G$ be the upward closure of this descending chain. This produces a [generic filter](../../../forcing.md#generic-filter) over $M$. By the [forcing theorem](../../../forcing.md#forcing-theorem), its [generic extension](../../../forcing.md#generic-extension) $M[G]$ satisfies [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). The canonical [forcing name](../../../forcing.md#forcing-name) $\dot g=\bigcup\dot G$ is forced to be a [function](../../../function.md) with domain $\omega$ and range $\kappa$: the dense [sets](../../../set.md) $D_n$ and $E_\alpha$ ensure exactly these assertions. Therefore

$$
\boxed{M[G]\models\text{“the old }\omega_1\text{ is countable.”}}
$$

Its new first [uncountable](../../../set-theory.md#uncountable-set) [ordinal](../../../set-theory.md#ordinal) is accordingly different from $\kappa$.

For a transitive $M$, ordinary evaluation of names gives the familiar literal extension. The question only assumes a [countable](../../../set-theory.md#countable-set) model, so one must also cover externally ill-founded models. In that case use the quotient of the internally defined [forcing names](../../../forcing.md#forcing-name) by forced equality modulo $G$, with membership defined by forced membership. The internal forcing identities and the forcing theorem hold in $M$ and give a well-defined [first-order structure](../../../mathematical-logic.md#first-order-structure) satisfying every standard [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) axiom. Check names embed the original membership structure, so identify their images with $M$. Its domain is a quotient of a [subset](../../../set.md#subset) of the [countable](../../../set-theory.md#countable-set) domain of $M$, hence is externally [countable](../../../set-theory.md#countable-set). Thus **the required extension exists even without assuming transitivity.** It is a membership extension, not an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension): the assertion that the parameter $\kappa$ is [uncountable](../../../set-theory.md#uncountable-set) changes truth value.

## 7

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

For nonempty [first-order structures](../../../mathematical-logic.md#first-order-structure) $(M_i)_{i\in I}$ in a common language and an [ultrafilter](../../../set-theory.md#ultrafilter) $D$ on $I$, identify product [functions](../../../function.md) by

$$
f\sim_D g\quad\Longleftrightarrow\quad\{i:f(i)=g(i)\}\in D.
$$

The [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) $\prod_i M_i/D$ has these equivalence classes as elements. [Functions](../../../function.md) are interpreted coordinatewise, and a relation holds of classes exactly when its coordinatewise truth [set](../../../set.md) belongs to $D$. Closure under finite [intersections](../../../set.md#set-intersection) makes these interpretations independent of representatives.

The [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) asserts

$$
\prod_i M_i/D\models\varphi([f_1],\ldots,[f_n])
\quad\Longleftrightarrow\quad
\{i:M_i\models\varphi(f_1(i),\ldots,f_n(i))\}\in D.
$$

Prove it by induction on [first-order formulas](../../../mathematical-logic.md#first-order-formula). Atomic [first-order formulas](../../../mathematical-logic.md#first-order-formula) hold by the definitions and induction on terms. Conjunction uses [intersections](../../../set.md#set-intersection), and negation uses the fact that an [ultrafilter](../../../set-theory.md#ultrafilter) contains exactly one of a [set](../../../set.md) and its complement. For an existential [first-order formula](../../../mathematical-logic.md#first-order-formula), a product witness gives a coordinate witness on a $D$-large [set](../../../set.md). Conversely, on the $D$-large [set](../../../set.md) where a coordinate witness exists, choose one in each factor, and choose arbitrary values elsewhere. Its class is a product witness by the induction hypothesis. This is the only witness-selection step; the surrounding argument is made in a choice metatheory. The special case with all factors equal is an [ultrapower](../../../foundations-of-mathematics.md#ultrapower), and constant [functions](../../../function.md) give an [elementary embedding](../../../set-theory.md#elementary-embedding).

Here is a direct [compactness theorem](../../../mathematical-logic.md#compactness-theorem) proof. Suppose every finite [subset](../../../set.md#subset) of a theory $T$ has a model. Index factors by the finite [subsets](../../../set.md#subset) $i\subseteq T$, choosing $M_i\models i$. For finite $F\subseteq T$, the cone $C_F=\{i:F\subseteq i\}$ is nonempty, and $C_F\cap C_H=C_{F\cup H}$. Extend the generated proper filter to an [ultrafilter](../../../set-theory.md#ultrafilter) $D$. For every sentence $\sigma\in T$, its truth [set](../../../set.md) contains $C_{\{\sigma\}}$, so the [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) gives $\prod_iM_i/D\models T$. **Finite satisfiability therefore implies satisfiability**, directly from the [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) construction rather than from a syntactic completeness argument.

For [saturated models](../../../foundations-of-mathematics.md#saturated-model), a structure is $\kappa$-saturated if every [complete type](../../../foundations-of-mathematics.md#complete-type) over fewer than $\kappa$ parameters is realized. A useful concrete case is [countable saturation of a nonprincipal ultraproduct over omega](../../../foundations-of-mathematics.md#countable-saturation-of-a-nonprincipal-ultraproduct-over-omega). In a [countable](../../../set-theory.md#countable-set) language, enumerate any finitely satisfiable type over countably many parameters as $\varphi_1(x),\varphi_2(x),\ldots$, and represent its parameters by product [functions](../../../function.md). By the [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem), the [set](../../../set.md) $A_n$ of coordinates where the first $n$ [first-order formulas](../../../mathematical-logic.md#first-order-formula) have a simultaneous witness belongs to the [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) $D$. Put

$$
B_n=\{i:i\ge n\}\cap\bigcap_{j\le n}A_j.
$$

These are decreasing $D$-large [sets](../../../set.md). At coordinate $i$, let $h(i)$ be the largest $n\le i$ with $i\in B_n$, or zero if none exists, and choose a witness for the first $h(i)$ [first-order formulas](../../../mathematical-logic.md#first-order-formula). For fixed $n$, every coordinate in $B_n$ has $h(i)\ge n$, so the resulting product [function](../../../function.md) satisfies $\varphi_n$ on a $D$-large [set](../../../set.md). Its class realizes the whole type. Thus such an [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) is $\aleph_1$-saturated.

There is also an existence construction at every prescribed degree $\kappa$. Given an infinite model $M$, choose a [regular cardinal](../../../set-theory.md#regular-cardinal) $\lambda\ge\kappa$ and construct an elementary chain $(M_\alpha)_{\alpha\le\lambda}$. At a successor stage, add a new constant for a realization of every type over every [subset](../../../set.md#subset) of $M_\alpha$ of size below $\kappa$, together with the [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure) of $M_\alpha$. Every finite part is satisfiable: only finitely many types and finitely many [first-order formulas](../../../mathematical-logic.md#first-order-formula) from each are involved, and each finite type fragment has a witness in $M_\alpha$. Compactness therefore supplies a simultaneous [elementary extension](../../../foundations-of-mathematics.md#elementary-extension). At limits take [unions](../../../set.md#set-union). To justify elementarity of a [union](../../../set.md#set-union), any existential [first-order formula](../../../mathematical-logic.md#first-order-formula) with parameters in an earlier stage has a witness in that stage whenever it has one at a later stage, by elementarity; this is the [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test).

Any fewer-than-$\kappa$ parameters of $M_\lambda$ occur together in some $M_\alpha$, by regularity of $\lambda$. A type over them which is finitely satisfiable in $M_\lambda$ is finitely satisfiable in $M_\alpha$, again by elementarity, and was realized in $M_{\alpha+1}$. Hence **every infinite structure has a $\kappa$-saturated [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) for any prescribed cardinal $\kappa$.** No bound on the size of this extension is asserted; full saturation at the model's own [cardinality](../../../set-theory.md#cardinality) has additional cardinal-arithmetic issues.

## 8

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

For the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem), start with an infinite structure $M$ and a [total order](../../../set.md#total-order) $I$. Choose a [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) $M^*$, and adjoin constants $c_i$ for $i\in I$. Require the [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure) of $M^*$, distinctness of these new constants, and the [order-indiscernible sequence](../../../foundations-of-mathematics.md#order-indiscernible-sequence) schema: any two increasing tuples of the $c_i$ of the same length satisfy the same [first-order formulas](../../../mathematical-logic.md#first-order-formula) in the expanded language. Every finite fragment mentions finitely many new constants and finitely many [first-order formulas](../../../mathematical-logic.md#first-order-formula). Enumerate a countably infinite subset of $M$. For each of the finitely many [first-order formulas](../../../mathematical-logic.md#first-order-formula), color its increasing tuples by its truth value in $M^*$, including whatever fixed parameters occur in the fragment. Successive applications of the infinite [Ramsey theorem](../../../graph-theory.md#ramsey-theorem) leave an infinite [subset](../../../set.md#subset) homogeneous for all these colorings. Assign the finitely many new constants to distinct elements of this [subset](../../../set.md#subset) in their index order. Their finite indiscernibility requirements and the [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure) are then simultaneously satisfied.

The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) supplies an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) $N^*$ containing the required distinct indiscernibles. Their [Skolem hull](../../../mathematical-logic.md#skolem-hull) is an [elementary substructure](../../../mathematical-logic.md#elementary-substructure): an existential [first-order formula](../../../mathematical-logic.md#first-order-formula) true of its elements has its chosen Skolem-function witness in the hull, so the [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test) applies. Any [order automorphism](../../../set.md#order-automorphism) $\sigma$ of $I$ acts on this hull by

$$
t(c_{i_1},\ldots,c_{i_n})\longmapsto t(c_{\sigma(i_1)},\ldots,c_{\sigma(i_n)}).
$$

Indiscernibility makes this well defined, since every equality of two term representations is preserved. The same argument preserves every [first-order formula](../../../mathematical-logic.md#first-order-formula); the inverse is given by $\sigma^{-1}$. Thus it is an automorphism, uniquely determined in the language of the chosen [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) by its values on the generators. This proves both the indiscernible-model and automorphism forms of the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem). Uniqueness is not claimed for automorphisms of the reduct which need not preserve the chosen [Skolem functions](../../../mathematical-logic.md#skolem-function).

For [simple typed set theory with atoms](../../../set-theory.md#simple-typed-set-theory-with-atoms), write $S_i$ for the [set](../../../set.md) predicate at sort $i$. Members have sort one lower; [urelements](../../../set-theory.md#urelement) have no typed members, [extensionality](../../../set-theory.md#axiom-of-extensionality) applies to [sets](../../../set.md), and every well-typed [first-order formula](../../../mathematical-logic.md#first-order-formula) defines a [set](../../../set.md) at the next sort. [Typical ambiguity](../../../set-theory.md#typical-ambiguity) adds $\phi\leftrightarrow\phi^+$ for each closed sentence, where $+$ raises every sort by one. We prove finite satisfiability using [Ramsey theorem](../../../graph-theory.md#ramsey-theorem), rather than assuming that adjacent sorts have the same [cardinality](../../../set-theory.md#cardinality).

Let $X_n=V_{\omega+2n}$. If $n<m$, then $\mathcal P(X_n)\subseteq X_m$. For increasing integers $h_0<h_1<h_2<\cdots$, interpret sort $i$ by $D_i=X_{h_{i+1}}$, interpret $S_i$ by the objects of $\mathcal P(X_{h_i})$, and interpret adjacent-sort membership by actual membership restricted to these designated [sets](../../../set.md). All other objects of a sort are typed [urelements](../../../set-theory.md#urelement). Every [subset](../../../set.md#subset) of $D_i$ is a designated [set](../../../set.md) in $D_{i+1}$, so comprehension holds for every [first-order formula](../../../mathematical-logic.md#first-order-formula), including [first-order formulas](../../../mathematical-logic.md#first-order-formula) with quantifiers and parameters at other sorts. Two designated [sets](../../../set.md) with the same members are equal, while the other objects have no typed members. Thus this is a full model of the typed axioms for every increasing [sequence](../../../real-analysis.md#sequence) of levels. The extra preceding level $h_0$ gives a consistent interpretation of the bottom [set](../../../set.md) predicate as well.

Take finitely many ambiguity sentences and let $r$ bound their highest sort before raising. Color increasing $(r+2)$-tuples $(h_0,\ldots,h_{r+1})$ by the vector of truth values of these sentences in the corresponding finite sorted structure. There are finitely many colors. The infinite [Ramsey theorem](../../../graph-theory.md#ramsey-theorem) supplies an [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) of indices. Choose the level [sequence](../../../real-analysis.md#sequence) from it. The sentence $\phi$ is evaluated in the window $(h_0,\ldots,h_{r+1})$, while $\phi^+$ is evaluated in the next window $(h_1,\ldots,h_{r+2})$; homogeneity makes their truth values equal. Sentences using fewer sorts simply ignore the unused final levels. Thus every finite family of ambiguity axioms has a model satisfying all the typed axioms. Apply many-sorted first-order [compactness theorem](../../../mathematical-logic.md#compactness-theorem) to obtain

$$
\boxed{\operatorname{Con}(\mathrm{TSTU}+\mathrm{Typical\ Ambiguity}).}
$$

This is a relative consistency construction in the ordinary set-theoretic metatheory. Allowing urelements is essential here: skipping ranks leaves objects outside the represented [power sets](../../../set.md#power-set), and those objects must be permitted as [urelements](../../../set-theory.md#urelement).

## 9

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="9/solution">Solution</h3>

↑ **Parent:** [9](#9)

An [uncountable](../../../set-theory.md#uncountable-set) cardinal $\kappa$ is a [measurable cardinal](../../../set-theory.md#measurable-cardinal) if there is a nonprincipal $\kappa$-complete [ultrafilter](../../../set-theory.md#ultrafilter) $U$ on $\kappa$: [intersections](../../../set.md#set-intersection) of fewer than $\kappa$ members of $U$ remain in $U$. Such an [ultrafilter](../../../set-theory.md#ultrafilter) is uniform. No [singleton](../../../set.md#singleton-mathematics) belongs to it, and intersecting the complements of fewer than $\kappa$ [singletons](../../../set.md#singleton-mathematics) shows that no [set](../../../set.md) of [cardinality](../../../set-theory.md#cardinality) below $\kappa$ belongs to it.

Form the [ultrapower](../../../foundations-of-mathematics.md#ultrapower) of the universe by $U$, with classes $[f]$ of [functions](../../../function.md) $f:\kappa\to V$, and $[f]\in_U[g]$ exactly when $\{\xi:f(\xi)\in g(\xi)\}\in U$. The [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) proves that the map taking $x$ to the constant [function](../../../function.md) with value $x$ is elementary. The [ultrapower](../../../foundations-of-mathematics.md#ultrapower) relation is well-founded: from an infinite descending [sequence](../../../real-analysis.md#sequence) $[f_0]\ni_U[f_1]\ni_U\cdots$, [countable](../../../set-theory.md#countable-set) completeness gives a coordinate satisfying all the membership relations, producing an actual infinite descending membership [sequence](../../../real-analysis.md#sequence) and contradicting [foundation](../../../set-theory.md#axiom-of-regularity). It is also set-like. Predecessors of $[g]$ can be represented by [functions](../../../function.md) whose value at $\xi$ lies in $g(\xi)\cup\{\varnothing\}$; these [functions](../../../function.md) form a [set](../../../set.md). The [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem) therefore gives a [transitive class](../../../set-theory.md#transitive-class) $N$ and an [elementary embedding](../../../set-theory.md#elementary-embedding)

$$
j:V\longrightarrow N.
$$

The usual class-ultrapower notation is understood via set-sized representatives and this set-like collapse.

For $\alpha<\kappa$, any [function](../../../function.md) into $\alpha$ is constant on a $U$-large [set](../../../set.md): if none of its fewer-than-$\kappa$ fibers belonged to $U$, intersect their complements to get the [empty set](../../../set.md#empty-set) in $U$. Consequently every member of the [ultrapower](../../../foundations-of-mathematics.md#ultrapower) [ordinal](../../../set-theory.md#ordinal) represented by the constant $\alpha$ is represented by a constant [ordinal](../../../set-theory.md#ordinal) below $\alpha$. Induction on $\alpha$ now gives $j(\alpha)=\alpha$.

On the other hand the identity [function](../../../function.md) $d(\xi)=\xi$ represents an [ordinal](../../../set-theory.md#ordinal) below $j(\kappa)$. For every $\alpha<\kappa$, the tail $\{\xi:\xi>\alpha\}$ belongs to $U$, so the collapsed [ordinal](../../../set-theory.md#ordinal) $[d]$ is above $j(\alpha)=\alpha$. Hence

$$
\boxed{\operatorname{crit}(j)=\kappa,\qquad j(\kappa)>\kappa.}
$$

This proves nonidentity explicitly. The collapsed identity class is at least $\kappa$; it need not equal $\kappa$ unless an additional normality convention is imposed on $U$.

Conversely, an [elementary embedding](../../../set-theory.md#elementary-embedding) $j:V\to N$ into a [transitive class](../../../set-theory.md#transitive-class) with critical point $\kappa$ yields

$$
U=\{X\subseteq\kappa:\kappa\in j(X)\}.
$$

For the converse use the usual amenability assumption on the class embedding, so this collection is a [set](../../../set.md). Since $j(\kappa)>\kappa$, exactly one of $j(X)$ and $j(\kappa\setminus X)$ contains $\kappa$, proving the [ultrafilter](../../../set-theory.md#ultrafilter) condition. [Singletons](../../../set.md#singleton-mathematics) are excluded because $j(\alpha)=\alpha<\kappa$. If $\lambda<\kappa$ and $X_i\in U$ for $i<\lambda$, then $j$ fixes $\lambda$ and every index below it, giving $j(\bigcap_{i<\lambda}X_i)=\bigcap_{i<\lambda}j(X_i)$; the [intersection](../../../set.md#set-intersection) still contains $\kappa$. Thus $U$ is $\kappa$-complete and $\kappa$ is measurable.

In particular the first moved [ordinal](../../../set-theory.md#ordinal) is a [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal). If $\operatorname{cf}(\kappa)<\kappa$, partition $\kappa$ into fewer than $\kappa$ bounded intervals. Each is too small to lie in $U$, contradicting completeness. Thus $\kappa$ is regular. If $2^\lambda\ge\kappa$ for some $\lambda<\kappa$, choose distinct [subsets](../../../set.md#subset) $A_\xi\subseteq\lambda$ for $\xi<\kappa$. For each $\eta<\lambda$, choose the $U$-large side of the question $\eta\in A_\xi$. Intersect these fewer-than-$\kappa$ large sides. The [intersection](../../../set.md#set-intersection) belongs to $U$, but all its indices have identical $A_\xi$, so it contains at most one index, contradicting nonprincipality. Therefore $2^\lambda<\kappa$ for every $\lambda<\kappa$, as required.

## 10

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="10/solution">Solution</h3>

↑ **Parent:** [10](#10)

For an infinite cardinal $\rho$ put $\beth_0(\rho)=\rho$ and $\beth_{n+1}(\rho)=2^{\beth_n(\rho)}$. The [Erdős-Rado theorem for finite arities](../../../set-theory.md#erdos-rado-theorem-for-finite-arities) is

$$
\boxed{\beth_n(\rho)^+\longrightarrow(\rho^+)^{n+1}_\rho\qquad(n<\omega).}
$$

The [partition relation](../../../set-theory.md#partition-relation) requires a homogeneous [subset](../../../set.md#subset) of order type $\rho^+$ for every coloring of $(n+1)$-element [subsets](../../../set.md#subset) by at most $\rho$ colors. In particular it gives [uncountable](../../../set-theory.md#uncountable-set) [homogeneous sets](../../../ramsey-theory.md#homogeneous-set-for-a-colouring). The case $n=0$ is the infinite pigeonhole principle: a [union](../../../set.md#set-union) of $\rho$ [sets](../../../set.md) each of size at most $\rho$ cannot have size $\rho^+$.

We give the induction step by a [closed elementary-submodel construction of an end-homogeneous sequence](../../../set-theory.md#closed-elementary-submodel-construction-of-an-end-homogeneous-sequence). Let $\mu$ be infinite, $\theta=(2^\mu)^+$, and $c:[\theta]^{r+1}\to\rho$ with $\rho\le\mu$. Choose a sufficiently large regular $\chi$ and an elementary submodel $M\prec H_\chi$ with $c,\theta\in M$, all [ordinals](../../../set-theory.md#ordinal) below $\mu^+$ in $M$, $|M|=2^\mu$, and closure under externally given [sequences](../../../real-analysis.md#sequence) of length at most $\mu$. To construct it, take $\mu^+$ successive elementary Skolem-hull closures, at each step including all such [sequences](../../../real-analysis.md#sequence) from the preceding stage. [Cardinality](../../../set-theory.md#cardinality) stays $2^\mu$ because $(2^\mu)^\mu=2^\mu$. In the final [union](../../../set.md#set-union) every [sequence](../../../real-analysis.md#sequence) of length at most $\mu$ has all its entries in some earlier stage, by regularity of $\mu^+$, and so was included at the next stage.

Put $\beta=\sup(M\cap\theta)$. Regularity of $\theta$ gives $\beta<\theta$, and $\beta\notin M$ since otherwise its successor would contradict the definition of the supremum. Recursively, for $\alpha<\mu^+$ choose $x_\alpha\in M\cap\theta$ above all earlier $x_\xi$ and satisfying

$$
c(\{x_{\xi_1},\ldots,x_{\xi_r},x_\alpha\})
=c(\{x_{\xi_1},\ldots,x_{\xi_r},\beta\})\qquad(\xi_1<\cdots<\xi_r<\alpha).
$$

There are at most $\mu$ constraints. Their parameters and their colors belong to $M$, and closure puts their complete code in $M$. The point $\beta$ witnesses their simultaneous satisfiability in $H_\chi$; elementarity supplies a witness in $M$. This gives an increasing end-homogeneous [sequence](../../../real-analysis.md#sequence) of length $\mu^+$: on it, the color of an $(r+1)$-tuple depends only on the first $r$ entries.

For the induction from arity $n$ to $n+1$, take $\mu=\beth_{n-1}(\rho)$ and $r=n$. Color the $n$-tuples of the resulting [sequence](../../../real-analysis.md#sequence) by their common color with a later point, equivalently by their color with $\beta$. Its index order has type $\mu^+=\beth_{n-1}(\rho)^+$, so the induction hypothesis supplies a homogeneous index [set](../../../set.md) of type $\rho^+$. The original $(n+1)$-tuples on those indices have that same color. This completes the proof without substituting the theorem's name for its induction.

A useful [ordinal partition-bound function](../../../set-theory.md#ordinal-partition-bound-function) is

$$
f(\alpha)=\min\{\gamma\ge\alpha:\ \gamma\longrightarrow(\alpha)^2_\nu\text{ for every nonzero cardinal }\nu<\alpha\}.
$$

It is total: choose an infinite cardinal $\rho\ge|\alpha|$ with $\rho^+>\alpha$; the pairs case supplies $(2^\rho)^+$ with the required homogeneous order type for all these color numbers. It is nondecreasing and satisfies $f(\alpha)\ge\alpha$. Start iterating $f$ and take a supremum $\kappa$ at a limit stage. If the increasing iterates do not attain that supremum, then for every $\alpha<\kappa$ some iterate $a_\xi$ satisfies $\alpha\le a_\xi<\kappa$, and

$$
f(\alpha)\le f(a_\xi)=a_{\xi+1}<\kappa.
$$

If the iterates have already stabilized, their supremum is a fixed point directly. Thus the relevant nontrivial case is an [uncountable](../../../set-theory.md#uncountable-set) cardinal $\kappa$ closed below itself under $f$.

Such closure implies that $\kappa$ is a strong limit. Suppose $\lambda<\kappa$ is infinite and $\kappa\le2^\lambda$. Take distinct binary strings of length $\lambda$, indexed in order by $\kappa$, and color a pair by its first differing coordinate. No three strings are homogeneous: three bits cannot be pairwise different at the same coordinate. Closure would give $f(\lambda+1)<\kappa$, and its restriction would have a homogeneous [subset](../../../set.md#subset) of order type $\lambda+1$ in $\lambda$ colors, a contradiction. Hence $2^\lambda<\kappa$; finite exponents are harmless for an [uncountable](../../../set-theory.md#uncountable-set) $\kappa$.

Use the usual [tree property](../../../set.md#tree-property): every [set-theoretic tree](../../../set.md#set-theoretic-tree) of height $\kappa$ with nonempty levels of [cardinality](../../../set-theory.md#cardinality) below $\kappa$ has a cofinal branch. For an [uncountable](../../../set-theory.md#uncountable-set) cardinal satisfying this all-[set-theoretic trees](../../../set.md#set-theoretic-tree) convention, $\kappa$ must be regular. If it were singular with [cofinality](../../../set-theory.md#cofinality) $\tau<\kappa$, attach to one root $\tau$ chains whose lengths increase cofinally to $\kappa$. Every level has at most $\tau$ nodes, the height is $\kappa$, and no branch is cofinal. This contradiction proves regularity. Combined with the preceding closure argument it proves that the cardinal under discussion is strongly inaccessible.

For any $c:[\kappa]^2\to\nu$, $0<\nu<\kappa$, make a separated [set-theoretic tree](../../../set.md#set-theoretic-tree) of [functions](../../../function.md). Its level $\alpha$ consists of the [functions](../../../function.md) $t:\alpha\to\nu$ realized as $t(\xi)=c(\{\xi,\beta\})$ for some $\beta\ge\alpha$, with $\beta<\kappa$. Order these [functions](../../../function.md) by restriction. Levels are nonempty and have size at most $\nu^{|\alpha|}<\kappa$, using the strong-limit property. The [tree property](../../../set.md#tree-property) gives a branch $b:\kappa\to\nu$. Recursively select $x_\eta$ for $\eta<\kappa$, larger than all earlier selections, whose coloring [function](../../../function.md) agrees with $b$ through a level above those earlier selections; regularity allows that level to remain below $\kappa$, and its node has a realizing point. Then $c(\{x_\xi,x_\eta\})=b(x_\xi)$ for $\xi<\eta$. One of the fewer-than-$\kappa$ colors occurs on $\kappa$ selected points, by regularity. These points are homogeneous, proving $\kappa\to(\kappa)^2_\nu$ for every $\nu<\kappa$. Consequently

$$
\boxed{\kappa\text{ closed below itself under }f\ +\ \mathrm{TP}(\kappa)\quad\Longrightarrow\quad f(\kappa)=\kappa.}
$$

A strictly increasing [countable](../../../set-theory.md#countable-set) iteration has a supremum of [countable](../../../set-theory.md#countable-set) [cofinality](../../../set-theory.md#cofinality), so it cannot meet this regular [set-theoretic tree](../../../set.md#set-theoretic-tree)-property condition; no continuity of $f$ has been assumed.

The final printed assertion needs its convention specified. The usual [tree property](../../../set.md#tree-property) alone does not imply strong inaccessibility; it can consistently hold at [successor cardinals](../../../set-theory.md#successor-cardinal). In the argument just given, strong inaccessibility follows from [function](../../../function.md) closure together with that [set-theoretic tree](../../../set.md#set-theoretic-tree) property. There is also a stronger [branching form of the tree property](../../../set.md#branching-form-of-the-tree-property) for which the assertion holds literally: require a cofinal branch in every separated rooted height-$\kappa$ [set-theoretic tree](../../../set.md#set-theoretic-tree) whose nodes each have fewer than $\kappa$ immediate successors, without restricting level sizes. The singular-chain example proves regularity under this convention too. If $2^\lambda\ge\kappa$ for $\lambda<\kappa$, take the full binary [set-theoretic tree](../../../set.md#set-theoretic-tree) through level $\lambda$, choose $\kappa$ distinct nodes on that level, and attach to its $\xi$th chosen node a chain of length $\xi$, for $\xi<\kappa$. It has height $\kappa$ and at most two successors per node, but every branch has length below $\kappa$. Thus this branching property implies the strong-limit condition and hence strong inaccessibility. At a [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) it agrees, for separated [set-theoretic trees](../../../set.md#set-theoretic-tree), with the usual level-size convention: regularity bounds the [union](../../../set.md#set-union) of fewer than $\kappa$ successor [sets](../../../set.md), and strong-limit arithmetic bounds the possible predecessor [sequences](../../../real-analysis.md#sequence) at limit levels.

## 11

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="11/i">i</h3>

↑ **Parent:** [11](#11)

<h4 id="11/i/solution">Solution</h4>

↑ **Parent:** [I](#11/i)

We prove the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem) by [ultraproducts](../../../foundations-of-mathematics.md#ultraproduct), with no application of [Ramsey theorem](../../../graph-theory.md#ramsey-theorem). Expand the infinite structure $M$ by [Skolem functions](../../../mathematical-logic.md#skolem-function), choose distinct elements $a_0,a_1,\ldots$, and choose a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) $D$ on $\omega$. Let $I$ be the desired total index order and put $J=\omega^I$.

For every finite ordered [subset](../../../set.md#subset) $F=\{i_1<\cdots<i_n\}$, define an [ultrafilter](../../../set-theory.md#ultrafilter) $D_F$ on $\omega^F$ by the ordered [Fubini product of ultrafilters](../../../set-theory.md#fubini-product-of-ultrafilters): a [set](../../../set.md) $B$ belongs to $D_F$ exactly when

$$
(Dm_1)(Dm_2)\cdots(Dm_n)\quad (m_1,\ldots,m_n)\in B.
$$

Here $(Dm)\psi(m)$ means $\{m:\psi(m)\}\in D$, with the quantifiers nested in the displayed order. The resulting collection is an [ultrafilter](../../../set-theory.md#ultrafilter), by induction using the [ultrafilter](../../../set-theory.md#ultrafilter) laws for negation and conjunction. For $F\subseteq H$, the inverse image of $B\subseteq\omega^F$ under coordinate projection belongs to $D_H$ exactly when $B\in D_F$: quantifiers on unused coordinates leave a truth value unchanged.

Consequently there is a well-defined [ultrafilter](../../../set-theory.md#ultrafilter) on the [Boolean algebra](../../../mathematical-logic.md#boolean-algebra) of finite-coordinate cylinders in $J$, declaring a cylinder large by this test. Coherence proves finite [intersection](../../../set.md#set-intersection) closure and ensures that the empty cylinder is not large. Extend its generated filter to an [ultrafilter](../../../set-theory.md#ultrafilter) $U$ on all [subsets](../../../set.md#subset) of $J$. Form the [ultrapower](../../../foundations-of-mathematics.md#ultrapower) $N=(M^*)^J/U$, and for $i\in I$ let $b_i$ be the class of $s\mapsto a_{s(i)}$.

If $i\ne j$, the coordinate equality test belongs to no corresponding two-coordinate product [ultrafilter](../../../set-theory.md#ultrafilter): for every value of the outer coordinate, the inner equality [set](../../../set.md) is a [singleton](../../../set.md#singleton-mathematics), excluded by nonprincipality. Hence the $b_i$ are distinct. For any [first-order formula](../../../mathematical-logic.md#first-order-formula) $\varphi(x_1,\ldots,x_n)$ and any $i_1<\cdots<i_n$, the [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem) gives

$$
N\models\varphi(b_{i_1},\ldots,b_{i_n})
\quad\Longleftrightarrow\quad
(Dm_1)\cdots(Dm_n)\ M^*\models\varphi(a_{m_1},\ldots,a_{m_n}).
$$

The right side is independent of the actual increasing index tuple, so the $b_i$ form an [order-indiscernible sequence](../../../foundations-of-mathematics.md#order-indiscernible-sequence). Constant [functions](../../../function.md) embed $M^*$ elementarily into $N$. Take the [Skolem hull](../../../mathematical-logic.md#skolem-hull) of the generators. The [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test) gives an [elementary substructure](../../../mathematical-logic.md#elementary-substructure), and transporting terms along an index-order automorphism gives a well-defined automorphism of the hull, with inverse obtained by transporting along the inverse index automorphism. Equality of term representations is preserved by indiscernibility. **This is the indiscernible and automorphism conclusion of Ehrenfeucht–Mostowski, obtained entirely from [ultrafilters](../../../set-theory.md#ultrafilter) and Łoś's theorem.** The ordered Fubini products need not be symmetric; order indiscernibility is exactly what their coherence supplies.

<h3 id="11/ii">ii</h3>

↑ **Parent:** [11](#11)

<h4 id="11/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11/ii)

Use the [bounded successor characterization of finite ordinals](../../../set-theory.md#bounded-successor-characterization-of-finite-ordinals). Let $\operatorname{Ord}(x)$ assert that $x$ is transitive, each of its members is transitive, and any two members are equal or comparable by membership. This is a bounded [first-order formula](../../../mathematical-logic.md#first-order-formula); [foundation](../../../set-theory.md#axiom-of-regularity) makes its linear membership order well-founded, so it is precisely the [Von Neumann ordinal](../../../set-theory.md#ordinal) predicate. Define

$$
\operatorname{Succ}_0(x)\quad\Longleftrightarrow\quad
x=\varnothing\ \lor\ (\exists y\in x)(\forall z\in x)(z=y\ \lor\ z\in y),
$$

and put

$$
\boxed{\operatorname{Nat}(x)\quad\Longleftrightarrow\quad
\operatorname{Ord}(x)\ \land\ \operatorname{Succ}_0(x)\ \land\
(\forall y\in x)\operatorname{Succ}_0(y).}
$$

For an [ordinal](../../../set-theory.md#ordinal), having a greatest member $y$ says exactly $x=y\cup\{y\}$. The displayed definition makes no reference to an infinite [inductive set](../../../set-theory.md#inductive-set) or to $\omega$; all quantifiers are bounded within the candidate and its members. Occurrences of $x=\varnothing$ can also be expressed as $(\forall u\in x)\,u\ne u$, so no unbounded quantifier is hidden in empty-set notation.

Every usual [natural number](../../../arithmetic.md#natural-number) satisfies this predicate, by induction: it is a [finite ordinal](../../../set-theory.md#finite-ordinal), and every nonzero initial segment is a successor. Conversely, suppose an [ordinal](../../../set-theory.md#ordinal) $x$ is not a usual [natural number](../../../arithmetic.md#natural-number). [Ordinal](../../../set-theory.md#ordinal) comparability gives $x\ge\omega$. If $x=\omega$, it has no greatest member, contradicting $\operatorname{Succ}_0(x)$. If $x>\omega$, then $\omega\in x$ has no greatest member, contradicting the corresponding bounded requirement on members of $x$. Hence $\operatorname{Nat}(x)$ holds exactly for the usual [natural numbers](../../../arithmetic.md#natural-number). The [axiom of infinity](../../../set-theory.md#axiom-of-infinity) and [separation](../../../set-theory.md#axiom-schema-of-specification) therefore collect this class as the usual [set](../../../set.md) $\omega$. This is a bounded definition of membership in the natural-number class; it does not claim that the [infinite set](../../../set.md#infinite-set) $\omega$ itself can be produced without the [infinity](../../../mathematics.md#infinity) axiom.

<h3 id="11/iii">iii</h3>

↑ **Parent:** [11](#11)

<h4 id="11/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#11/iii)

An [inner model](../../../set-theory.md#inner-model) of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) is a [transitive class](../../../set-theory.md#transitive-class) $N$ containing all [ordinals](../../../set-theory.md#ordinal) and satisfying [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) with the inherited membership relation. The “all [ordinals](../../../set-theory.md#ordinal)” requirement is important: an arbitrary transitive [set](../../../set.md) model or a rank segment is not an inner model in this sense.

Every such inner model contains the ambient [constructible universe](../../../definable-power-set.md#constructible-universe) $L$. Here is the reason. Inductively $L_\alpha^N=L_\alpha$. The zero stage is the same [empty set](../../../set.md#empty-set). If the stages at $\alpha$ agree, satisfaction for the common [set](../../../set.md) structure $(L_\alpha,\in)$ is absolute: atomic [first-order formulas](../../../mathematical-logic.md#first-order-formula) agree, Boolean operations agree, and quantified variables range over the identical [set](../../../set.md). The codes of finite [first-order formulas](../../../mathematical-logic.md#first-order-formula) are also the same because a [transitive model](../../../set-theory.md#transitive-model) of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) has the actual [natural numbers](../../../arithmetic.md#natural-number). Consequently definability with parameters from $L_\alpha$ produces exactly the same [subsets](../../../set.md#subset) in both models, so their successor constructible stages agree. At a [limit ordinal](../../../set-theory.md#limit-ordinal) both constructions take the [union](../../../set.md#set-union) of the same earlier stages. This proves agreement at every stage and hence $L\subseteq N$.

The [constructible universe theorem](../../../definable-power-set.md#constructible-universe-theorem) provides models of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) satisfying $V=L$ and the [axiom of choice](../../../set-theory.md#axiom-of-choice), whenever [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) is consistent. In such a universe any inner model $N$ of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) satisfies

$$
L=V\subseteq N\subseteq V,
$$

so $N=V$ and it also satisfies choice. Therefore

$$
\boxed{\text{No uniform inner-model construction from arbitrary ZF models can establish }\neg\mathsf{AC}.}
$$

Passing to $L$ proves the consistency of choice, but the same downward method cannot prove its negation from an arbitrary starting model: it has no possible output when the starting universe is constructible. This is the precise obstruction intended in an inner-model independence argument. It is not a claim that every inner model of every choice universe satisfies choice; symmetric submodels of suitable forcing extensions can fail choice, and that method first changes the ambient universe.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
