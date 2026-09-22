# Paper 21

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper21.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper21.pdf)

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
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

We use [rooted-tree homeomorphic embedding](../../../combinatorics.md#homeomorphic-embedding-of-a-rooted-tree): an injective [vertex](../../../graph.md#vertex-graph-theory) map preserves ancestors and lowest common ancestors, while an [edge](../../../graph-theory.md#edge-of-a-graph) may map to a longer path. The root may map below the host root. Write $T\preceq U$ for this relation. The assertion of [Kruskal's tree theorem](../../../set.md#kruskal-s-tree-theorem) is that finite [rooted trees](../../../combinatorics.md#rooted-tree) form a [well-quasi-ordering](../../../set.md#well-quasi-ordering): every infinite [sequence](../../../real-analysis.md#sequence) has $i<j$ with $T_i\preceq T_j$.

We first supply the [word](../../../foundations-of-mathematics.md#string) lemma needed in the proof. In a [well-quasi-order](../../../set.md#well-quasi-ordering) $Q$, every [sequence](../../../real-analysis.md#sequence) has an infinite nondecreasing [subsequence](../../../real-analysis.md#subsequence). Indeed, if no term had infinitely many later terms above it, successive choices beyond the finite [sets](../../../set.md) of later dominators would give a [bad sequence](../../../set.md#bad-sequence). Some term therefore has infinitely many later dominators; repeat the argument inside that infinite [subsequence](../../../real-analysis.md#subsequence), which is still well-quasi-ordered, to build a chain.

Now order finite [words](../../../foundations-of-mathematics.md#string) over $Q$ by [subsequence](../../../real-analysis.md#subsequence) embedding with coordinatewise increase. Suppose a bad [word](../../../foundations-of-mathematics.md#string) [sequence](../../../real-analysis.md#sequence) exists and choose one $w_0,w_1,\ldots$ minimally: at each position use a [word](../../../foundations-of-mathematics.md#string) of least length allowing a bad continuation of the fixed prefix. No [word](../../../foundations-of-mathematics.md#string) is empty. Write $w_i=v_i a_i$, removing its last letter. Choose indices $i_0<i_1<\cdots$ with $a_{i_0}\le a_{i_1}\le\cdots$. The [sequence](../../../real-analysis.md#sequence)

$$
w_0,\ldots,w_{i_0-1},v_{i_0},v_{i_1},\ldots
$$

would also be bad. An old [word](../../../foundations-of-mathematics.md#string) embedding into $v_{i_j}$ embeds into $w_{i_j}$, contrary to the original badness; and $v_{i_j}\preceq v_{i_l}$ would extend, using the last-letter comparison, to $w_{i_j}\preceq w_{i_l}$. But $v_{i_0}$ is shorter than $w_{i_0}$, contradicting minimality. This proves [Higman lemma](../../../set.md#higman-s-lemma), including its empty-word case.

Suppose next that there is a [bad sequence](../../../set.md#bad-sequence) of finite [rooted trees](../../../combinatorics.md#rooted-tree), and choose a [minimal bad sequence](../../../set.md#minimal-bad-sequence) $T_0,T_1,\ldots$ by [vertex](../../../graph.md#vertex-graph-theory) count. Let $\mathcal S$ consist of all proper rooted subtrees hanging below [vertices](../../../graph.md#vertex-graph-theory) of the $T_i$. This collection is well-quasi-ordered. Otherwise choose a [bad sequence](../../../set.md#bad-sequence) $S_0,S_1,\ldots$ in $\mathcal S$. Its containing-tree indices can be selected strictly increasing, say $S_j$ is a proper subtree of $T_{i_j}$: a finite initial collection of containing [trees](../../../combinatorics.md#tree-graph-theory) has only finitely many proper subtrees, and a [bad sequence](../../../set.md#bad-sequence) cannot repeat an [isomorphism](../../../algebra.md#isomorphism) class. Then

$$
T_0,\ldots,T_{i_0-1},S_0,S_1,\ldots
$$

is bad. No earlier $T_l$ can embed into $S_j$, because $S_j\preceq T_{i_j}$ and this would contradict the original [sequence](../../../real-analysis.md#sequence). The new tail is bad by construction. Since $|S_0|<|T_{i_0}|$, this contradicts minimality.

List each [tree](../../../combinatorics.md#tree-graph-theory)'s immediate root subtrees in any chosen order. These are finite [words](../../../foundations-of-mathematics.md#string) in the [well-quasi-order](../../../set.md#well-quasi-ordering) $\mathcal S$, so the [word](../../../foundations-of-mathematics.md#string) lemma gives $i<j$ for which the child [word](../../../foundations-of-mathematics.md#string) of $T_i$ embeds into that of $T_j$. Send the root of $T_i$ to the root of $T_j$, and use the chosen embeddings inside the selected, distinct target branches. The connecting paths from the target root to the images of the source children have disjoint interiors; lowest common ancestors in different branches are preserved. This constructs $T_i\preceq T_j$, the final contradiction. Thus **finite [rooted trees](../../../combinatorics.md#rooted-tree) are well-quasi-ordered by homeomorphic embedding**. If labels lie in an arbitrary [well-quasi-order](../../../set.md#well-quasi-ordering), the same proof uses label-monotone embeddings; compare root labels and child [words](../../../foundations-of-mathematics.md#string) in their product [well-quasi-order](../../../set.md#well-quasi-ordering). The product property follows by taking a nondecreasing [subsequence](../../../real-analysis.md#subsequence) in the first coordinate and a good pair in the second.

For [Friedman's finite form of Kruskal's theorem](../../../set.md#friedman-s-finite-form-of-kruskal-s-theorem), fix $k$. Consider all finite bad prefixes $(T_1,\ldots,T_l)$ satisfying $|T_i|\le k+i$, up to rooted-tree [isomorphism](../../../algebra.md#isomorphism). They form a prefix [tree](../../../combinatorics.md#tree-graph-theory). At each node there are finitely many possible next [trees](../../../combinatorics.md#tree-graph-theory), because there are only finitely many rooted-tree [isomorphism](../../../algebra.md#isomorphism) types on at most $k+l+1$ [vertices](../../../graph.md#vertex-graph-theory). If prefixes of arbitrary length existed, the [König infinity lemma](../../../combinatorics.md#konig-s-lemma) would give an infinite branch, hence an infinite [bad sequence](../../../set.md#bad-sequence), contrary to what we proved. Its height is therefore bounded. Consequently

$$
\boxed{\forall k\ \exists N\ \forall(T_1,\ldots,T_N),\quad |T_i|\le k+i\ \Longrightarrow\ \exists i<j\ (T_i\preceq T_j).}
$$

The same finite-prefix argument works with a fixed finite label alphabet, and more generally with any prescribed size bound $b(i)$ having only finitely many possibilities at each position. These are finite existence statements; no numerical estimate on $N$ is needed for the conclusion.

## 2

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The independence statements are [relative consistency](../../../mathematical-logic.md#relative-consistency) statements. We construct models from an ambient model of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice); the construction is an interpretation and does not assume that the ambient model is transitive. [Foundation](../../../set-theory.md#axiom-of-regularity) is already true in the ordinary ambient membership structure, so its positive consistency direction is immediate.

For the negative direction, construct an [extensional cumulative universe over Quine atoms](../../../set-theory.md#extensional-cumulative-universe-over-quine-atoms). Let $A$ be a countably infinite [set](../../../set.md) of formal symbols $q_a$. Give each $q_a$ the extension $\{q_a\}$. For a [set](../../../set.md) $X$ of already constructed objects, let $S(X)$ be its unique representative: [set](../../../set.md) $S(\{q_a\})=q_a$, and otherwise use a fresh tagged code $(1,X)$. Atom codes have a different tag. Begin with $U_0=A$ and put

$$
U_{\alpha+1}=U_\alpha\cup\{S(X):X\subseteq U_\alpha\},\qquad U_\lambda=\bigcup_{\alpha<\lambda}U_\alpha.
$$

[Set](../../../set.md) $W=\bigcup_\alpha U_\alpha$. The interpreted membership relation $E$ gives $S(X)$ exactly the members $X$, and gives $q_a$ exactly the member $q_a$. This convention matters: creating a second representative for $\{q_a\}$ would violate [extensionality](../../../set-theory.md#axiom-of-extensionality). Every object is uniquely determined by its extension, so $E$ satisfies full [extensionality](../../../set-theory.md#axiom-of-extensionality). Every set-sized collection $X$ of objects has bounded construction rank, by ambient [replacement](../../../set-theory.md#axiom-schema-of-replacement), and hence has its representative $S(X)$ in $W$.

Here are the remaining axiom verifications. [Empty set](../../../set.md#empty-set) and [pairing](../../../set-theory.md#axiom-of-pairing) use $S(\varnothing)$ and $S(\{x,y\})$. If $E(y)=X$, its interpreted [union](../../../set.md#set-union) is $S(\bigcup_{x\in X}E(x))$. Its interpreted [power set](../../../set.md#power-set) is

$$
S\bigl(\{S(Y):Y\subseteq X\}\bigr),
$$

since every [subset](../../../set.md#subset) extension has a unique representative. The pure, atom-free finite hierarchy supplies a copy of $\omega$ and an inductive [set](../../../set.md). For [separation](../../../set-theory.md#axiom-schema-of-specification), translate an $E$-formula into the ambient language, with quantifiers restricted to the definable class $W$; ambient [separation](../../../set-theory.md#axiom-schema-of-specification) gives the appropriate [subset](../../../set.md#subset) of $X$, and $S$ represents it. For [replacement](../../../set-theory.md#axiom-schema-of-replacement), uniqueness in the interpreted functional relation gives an ambient definable functional image of the [set](../../../set.md) $X$. Ambient [replacement](../../../set-theory.md#axiom-schema-of-replacement) makes that image set-sized, and $S$ again represents it. These arguments also establish that all the operations used have bounded construction rank.

Ambient choice gives choice in $W$: choose a member from each nonempty extension in a set-sized family and represent the graph, using interpreted [ordered pairs](../../../set.md#ordered-pair). But $q_a E q_a$, and the nonempty [set](../../../set.md) with extension $\{q_a\}$ has no $E$-minimal member. Thus

$$
\boxed{\operatorname{Con}(\mathrm{ZFC})\Longrightarrow\operatorname{Con}(\mathrm{ZF}-\mathrm{Foundation}+\mathrm{AC}+\neg\mathrm{Foundation}).}
$$

Together with the ordinary model, this proves independence of [foundation](../../../set-theory.md#axiom-of-regularity) from the other [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axioms, even when choice is retained.

To extend the construction to failure of choice, let the full [permutation group](../../../finite-group-theory.md#permutation-group) of $A$ act on $W$ by

$$
\pi(q_a)=q_{\pi(a)},\qquad \pi(S(X))=S(\pi``X).
$$

The singleton convention is equivariant, so this is an [automorphism](../../../algebra.md#automorphism) of $(W,E)$. An object has [finite support](../../../group-theory.md#finite-support-in-a-permutation-action) if some finite $F\subseteq A$ has the property that every [permutation](../../../combinatorics.md#permutation) fixing $F$ pointwise fixes the object. Retain objects all of whose membership descendants have [finite support](../../../group-theory.md#finite-support-in-a-permutation-action), stopping the hereditary recursion at the atomic self-loops. This gives the [hereditarily finite-supported Quine-atom model](../../../set-theory.md#hereditarily-finite-supported-quine-atom-model) $\mathcal H$; each $q_a$ belongs to it, with support $\{q_a\}$.

[Extensionality](../../../set-theory.md#axiom-of-extensionality) persists because every retained object's members are retained. [Empty set](../../../set.md#empty-set), [pairing](../../../set-theory.md#axiom-of-pairing), [infinity](../../../mathematics.md#infinity) and [union](../../../set.md#set-union) preserve hereditary [finite support](../../../group-theory.md#finite-support-in-a-permutation-action). For [separation](../../../set-theory.md#axiom-schema-of-specification) on a retained [set](../../../set.md) $x$, the [union](../../../set.md#set-union) of finite supports for $x$ and the formula's parameters supports the separated extension: [permutations](../../../combinatorics.md#permutation) fixing those supports preserve satisfaction in $\mathcal H$. All its members are retained, so its representative is retained. For [replacement](../../../set-theory.md#axiom-schema-of-replacement), the same support fixes the functional range, because an [automorphism](../../../algebra.md#automorphism) must take the unique output at an input to the unique output at its transported input. Ambient [replacement](../../../set-theory.md#axiom-schema-of-replacement) bounds that range; all its members are in $\mathcal H$, so its representative belongs to $\mathcal H$. Finally, the collection of all retained [subset](../../../set.md#subset) representatives of $x$ is an ambient [set](../../../set.md), contained in the full interpreted [power set](../../../set.md#power-set) of $x$. A support of $x$ permutes this collection onto itself, and its members are retained. Its representative is therefore the internal [power set](../../../set.md#power-set) in $\mathcal H$. This verifies every [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axiom except [foundation](../../../set-theory.md#axiom-of-regularity); [foundation](../../../set-theory.md#axiom-of-regularity) still fails at each $q_a$.

The atom [set](../../../set.md) $A$ and the family $[A]^2$ of its two-element [subsets](../../../set.md#subset) have empty support and are retained. Suppose a [choice function](../../../set-theory.md#choice-function) $f$ on $[A]^2$ were retained, with [finite support](../../../group-theory.md#finite-support-in-a-permutation-action) $F$. Choose distinct $q_a,q_b$ outside $F$ and transpose them. The transposition fixes $f$ and fixes the unordered pair $\{q_a,q_b\}$, but moves whichever of its two members $f$ selects. Equivariance would require that selected member to be fixed, a contradiction. Hence

$$
\boxed{\operatorname{Con}(\mathrm{ZFC})\Longrightarrow\operatorname{Con}(\mathrm{ZF}-\mathrm{Foundation}+\neg\mathrm{AC}+\neg\mathrm{Foundation}).}
$$

The full universe $W$ gives the corresponding positive-choice model. Choice is therefore independent of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) without [foundation](../../../set-theory.md#axiom-of-regularity). Unlike a [permutation](../../../combinatorics.md#permutation) model with ordinary [urelements](../../../set-theory.md#urelement), this model retains full pure-set [extensionality](../../../set-theory.md#axiom-of-extensionality): the atomic objects are self-membered [sets](../../../set.md), not empty objects exempted from [extensionality](../../../set-theory.md#axiom-of-extensionality).

The constructible-universe interpretation gives $\operatorname{Con}(\mathrm{ZF})\Rightarrow\operatorname{Con}(\mathrm{ZFC})$. Thus the consistency assumptions in both displayed conclusions can equivalently be taken to be $\operatorname{Con}(\mathrm{ZF})$; no additional consistency strength is being used.

## 3

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An [inner model](../../../set-theory.md#inner-model) of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) is a [transitive class](../../../set-theory.md#transitive-class) $M$ containing every [ordinal](../../../set-theory.md#ordinal), with inherited membership, such that each [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axiom holds with all quantifiers restricted to $M$. Here transitivity means $x\in y\in M\Rightarrow x\in M$. For a proper class this is an axiom-by-axiom assertion, not an internal truth predicate for the whole class. An [inner model](../../../set-theory.md#inner-model) can have fewer [subsets](../../../set.md#subset) of a given [set](../../../set.md) than the surrounding universe; it need not have the same [cardinals](../../../set-theory.md#cardinal-number) or the same continuum function.

[Inner models](../../../set-theory.md#inner-model) prove [relative consistency](../../../mathematical-logic.md#relative-consistency). If a theory $T$ proves that a definable class $M$ satisfies every axiom of $S$, an inconsistency proof from $S$ could be relativized to $M$ and become an inconsistency proof from $T$. Thus **$\operatorname{Con}(T)\Rightarrow\operatorname{Con}(S)$**. This reasoning concerns formal interpretations and needs no assumption that a given model of $T$ is externally well-founded.

The central example is the [constructible universe](../../../definable-power-set.md#constructible-universe). Define

$$
L_0=\varnothing,\qquad L_{\alpha+1}=\operatorname{Def}(L_\alpha),\qquad L_\lambda=\bigcup_{\alpha<\lambda}L_\alpha,\qquad L=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha,
$$

where $\operatorname{Def}(X)$ contains exactly the [subsets](../../../set.md#subset) definable over $(X,\in)$ using parameters from $X$. [Satisfaction for a set structure](../../../mathematical-logic.md#satisfaction-for-a-set-structure) is definable, so this recursion is available in [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory). [Induction](../../../foundations-of-mathematics.md#mathematical-induction) shows that the levels are transitive and increasing: if $a\in L_\alpha$, the [subset](../../../set.md#subset) $\{x\in L_\alpha:x\in a\}$ is $a$, so $a\in L_{\alpha+1}$. The [ordinal](../../../set-theory.md#ordinal) part of $L_\alpha$ is $\alpha$, giving all [ordinals](../../../set-theory.md#ordinal) in $L$.

For completeness, the main axiom mechanisms explain why this example works. Finite [set](../../../set.md) operations on constructible parameters are definable at finitely many further stages. For a fixed finite family of formulas and parameters, close a [sequence](../../../real-analysis.md#sequence) of levels under their least constructible witness stages and take its [union](../../../set.md#set-union); [induction](../../../foundations-of-mathematics.md#mathematical-induction) on formulas gives a reflecting level. [Separation](../../../set-theory.md#axiom-schema-of-specification) of a constructible [set](../../../set.md) then occurs at the next definability stage. For [replacement](../../../set-theory.md#axiom-schema-of-replacement), ambient [replacement](../../../set-theory.md#axiom-schema-of-replacement) bounds the construction stages of the unique constructible outputs; a reflecting level above that bound makes the range definable. For the internal [power set](../../../set.md#power-set) of $a\in L$, use ambient [separation](../../../set-theory.md#axiom-schema-of-specification) to form $\mathcal P(a)\cap L$, bound the construction stages of its members, and at a sufficiently high level define the family of all [subsets](../../../set.md#subset) of $a$ in that level. Thus the internal [power set](../../../set.md#power-set) is constructible even though some ambient [subsets](../../../set.md#subset) may not be. [Foundation](../../../set-theory.md#axiom-of-regularity) is inherited by transitivity, and [infinity](../../../mathematics.md#infinity) comes from $L_\omega$ and its successor stages.

There is a canonical [well-order](../../../set.md#well-order) of $L$: order by first construction stage, then by the least definition code and finite parameter tuple, using the previously constructed [well-orders](../../../set.md#well-order) for parameters. Each [set](../../../set.md) in $L$ can be well-ordered by the restriction of this set-like class order; hence $L$ satisfies [AC](../../../set-theory.md#axiom-of-choice). Moreover the hierarchy computed inside $L$ is the same hierarchy, because definability over a fixed [set](../../../set.md) structure and limit unions are absolute. Thus $L$ satisfies $V=L$. The further [cardinal](../../../set-theory.md#cardinal-number) analysis of this hierarchy, encapsulated in the [constructible universe theorem](../../../definable-power-set.md#constructible-universe-theorem), gives [GCH](../../../set-theory.md#generalized-continuum-hypothesis). Consequently

$$
\boxed{\operatorname{Con}(\mathrm{ZF})\Longrightarrow\operatorname{Con}(\mathrm{ZFC}+V=L+\mathrm{GCH}).}
$$

This proves the [relative consistency](../../../mathematical-logic.md#relative-consistency) of choice, [CH](../../../set-theory.md#continuum-hypothesis) and [GCH](../../../set-theory.md#generalized-continuum-hypothesis); in particular none can be refuted by [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) if [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) is consistent. The assertions here are internal to $L$: they do not assert [CH](../../../set-theory.md#continuum-hypothesis) in the ambient universe.

[Inner models](../../../set-theory.md#inner-model) also isolate definable information. The [relative constructible universe](../../../definable-power-set.md#relative-constructible-universe) built with a [set](../../../set.md) parameter retains that parameter and all [ordinals](../../../set-theory.md#ordinal) while discarding unrelated [sets](../../../set.md). Such constructions help compare [relative consistency](../../../mathematical-logic.md#relative-consistency) strengths and identify which hypotheses survive passage to smaller universes; preservation of a large-cardinal property must be checked separately, not inferred merely from transitivity.

There is an important limitation, the [constructible-universe obstruction to a uniform inner-model proof of failure of choice](../../../set-theory.md#constructible-universe-obstruction-to-a-uniform-inner-model-proof-of-failure-of-choice). Every [inner model](../../../set-theory.md#inner-model) $M$ of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) contains the ambient $L$. Indeed $L_\alpha^M=L_\alpha$ by [induction](../../../foundations-of-mathematics.md#mathematical-induction): the same [set](../../../set.md) structure has the same definable [subsets](../../../set.md#subset) at a successor stage, and both hierarchies take the same [union](../../../set.md#set-union) at a limit. If the ambient universe satisfies $V=L$, this forces $M=V$. Thus [inner models](../../../set-theory.md#inner-model) cannot uniformly produce a model of $\neg\mathrm{AC}$ or $V\ne L$ from every [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) universe. To prove the opposite independence directions one needs an outer-model or other interpretation technique, such as [forcing](../../../forcing.md) or the non-well-founded symmetry construction in Question 2.

## 4

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For the effective counterexample, let $K$ be the [diagonal halting set](../../../foundations-of-mathematics.md#diagonal-halting-set) and let $K_s$ be the finite approximation obtained by running the first $s$ programs for $s$ steps. For $x<y<z$, define the [recursive triple colouring with no computable infinite homogeneous set](../../../foundations-of-mathematics.md#recursive-triple-colouring-with-no-computable-infinite-homogeneous-set) by

$$
c(\{x,y,z\})=\begin{cases}0,&K_y\cap\{0,\ldots,x\}=K_z\cap\{0,\ldots,x\},\\1,&\text{otherwise}.\end{cases}
$$

This is a total recursive two-coloring: only bounded computations are involved. An infinite [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) $H$ cannot have color one. Fix $x\in H$ and take $y,z\in H$ sufficiently large that every halting computation with index at most $x$ that ever halts has already halted by stage $y$; then the color is zero. If $H$ has color zero, it computes $K$: given $e$, find $x<y$ in $H$ with $x\ge e$ and inspect $K_y(e)$. Agreement with every later stage $z\in H$, and the unboundedness of $H$, give $K_y\cap\{0,\ldots,x\}=K\cap\{0,\ldots,x\}$. Hence this is the correct answer. The [set](../../../set.md) $K$ is not recursive: a purported halting decider would produce a program that halts exactly when the decider says it does not halt on its own index. Thus **there is no recursive infinite [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring)**. Here infinite is essential: every finite [subset](../../../set.md#subset) is recursive, and [sets](../../../set.md) with fewer than three elements are vacuously homogeneous.

A precise finite-arity [Erdős-Rado theorem for finite arities](../../../set-theory.md#erdos-rado-theorem-for-finite-arities) is

$$
\boxed{\beth_r(\lambda)^+\longrightarrow(\lambda^+)^{r+1}_\lambda\quad(r<\omega,\ \lambda\text{ an infinite cardinal}),}
$$

where $\beth_0(\lambda)=\lambda$ and $\beth_{r+1}(\lambda)=2^{\beth_r(\lambda)}$. We prove the [closed elementary-submodel construction of an end-homogeneous sequence](../../../set-theory.md#closed-elementary-submodel-construction-of-an-end-homogeneous-sequence) and then induct. We work with [AC](../../../set-theory.md#axiom-of-choice), as in the usual [cardinal](../../../set-theory.md#cardinal-number) partition calculus.

Put $\theta=(2^\mu)^+$, where $\mu$ is infinite, and let $c:[\theta]^{m+1}\to\lambda$ with $\lambda\le\mu$ and $m\ge1$. Choose a [regular cardinal](../../../set-theory.md#regular-cardinal) $\chi$ large enough that this coloring and its domain belong to $H_\chi$, the [sets](../../../set.md) of hereditary size below $\chi$. There is $M\prec H_\chi$ of size $2^\mu$ containing $c,\theta,\mu$, every [ordinal](../../../set-theory.md#ordinal) below $\mu^+$, and closed under externally given [sequences](../../../real-analysis.md#sequence) of length at most $\mu$. Here is the closure construction: start with a [Skolem hull](../../../mathematical-logic.md#skolem-hull) of the named parameters and the [ordinals](../../../set-theory.md#ordinal) below $\mu^+$; iterate hulls after adjoining all at-most-$\mu$-sequences of the preceding hull for $\mu^+$ stages. Every stage and the [union](../../../set.md#set-union) have size $2^\mu$, since $(2^\mu)^\mu=2^\mu$ and $\mu^+\le2^\mu$. The [elementary chain theorem](../../../foundations-of-mathematics.md#elementary-chain-theorem) gives elementarity. Any [sequence](../../../real-analysis.md#sequence) of at most $\mu$ members of the final [union](../../../set.md#set-union) lies in a bounded stage, because $\mu^+$ is regular, and is added at the next stage. This proves the required closure.

Let $\beta=\sup(M\cap\theta)$. Regularity of $\theta$ gives $\beta<\theta$, and $\beta\notin M$: otherwise $\beta+1$ would also belong to $M\cap\theta$. Recursively choose increasing $x_\alpha\in M\cap\theta$ for $\alpha<\mu^+$ so that, for every $m$-subset $u$ of the earlier points,

$$
c(u\cup\{x_\alpha\})=c(u\cup\{\beta\}).
$$

To justify the recursion, the earlier [sequence](../../../real-analysis.md#sequence) has length at most $\mu$, hence belongs to $M$. There are at most $\mu$ constraints. All their points and color values are in $M$, so their coded table belongs to $M$ by closure, even though $\beta$ itself is external to $M$. The supremum of the earlier points, plus one, also belongs to $M\cap\theta$ and is below $\beta$. Thus $\beta$ witnesses in $H_\chi$ that a point above that bound satisfying the table exists. Elementarity supplies such a point in $M$. This completes the recursion.

The [sequence](../../../real-analysis.md#sequence) is end-homogeneous: on any increasing $(m+1)$-tuple from it, the color depends only on its first $m$ entries. Define the induced $m$-tuple coloring by $g(u)=c(u\cup\{\beta\})$. For the [induction](../../../foundations-of-mathematics.md#mathematical-induction), the arity-one assertion $\lambda^+\to(\lambda^+)^1_\lambda$ is the infinite pigeonhole principle: a [union](../../../set.md#set-union) of $\lambda$ [sets](../../../set.md) each of size at most $\lambda$ has size at most $\lambda$. At step $r\ge1$, take $\mu=\beth_{r-1}(\lambda)$, so $\theta=\beth_r(\lambda)^+$. The constructed [sequence](../../../real-analysis.md#sequence) has size $\mu^+=\beth_{r-1}(\lambda)^+$. The [induction](../../../foundations-of-mathematics.md#mathematical-induction) hypothesis makes $g$ constant on a [subset](../../../set.md#subset) of size $\lambda^+$; end-homogeneity makes $c$ constant on its $(r+1)$-subsets. This proves the theorem. In particular $\lambda=\aleph_0$ gives an uncountable [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) for every finite-arity coloring with countably many colors, on a sufficiently large [cardinal](../../../set-theory.md#cardinal-number).

There is no unrestricted infinite-exponent analogue under [AC](../../../set-theory.md#axiom-of-choice). For any infinite [cardinal](../../../set-theory.md#cardinal-number) $\kappa$, choose one representative $R$ from each equivalence class of $[\kappa]^\omega$ modulo [finite symmetric difference](../../../set.md#finite-symmetric-difference). Color $X$ by the parity of $|X\mathbin\triangle R|$. Removing one element of $X$ leaves it in the same class and reverses the parity. Every infinite proposed [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) contains both a countably infinite $X$ and $X\setminus\{x\}$, so cannot be homogeneous. Thus the [finite-symmetric-difference colouring of infinite subsets](../../../set-theory.md#finite-symmetric-difference-colouring-of-infinite-subsets) proves

$$
\boxed{\kappa\not\longrightarrow(\omega)^\omega_2\quad\text{for every infinite }\kappa\text{, under AC}.}
$$

The contrast is between arbitrary colorings at countably infinite arity and the finite arities of the theorem; restrictions on the definability of an infinite-arity coloring can change the problem.

## 5

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [saturated model](../../../foundations-of-mathematics.md#saturated-model) condition in degree $\kappa$ means that a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) $M$ realizes every one-variable [complete type](../../../foundations-of-mathematics.md#complete-type) over a parameter [set](../../../set.md) $A\subseteq M$ of size less than $\kappa$. Equivalently every finitely satisfiable such [complete type](../../../foundations-of-mathematics.md#complete-type) is realized, since it can be extended to a [complete type](../../../foundations-of-mathematics.md#complete-type). Without a specified degree, saturated usually means $|M|$-saturated. [Countable](../../../set-theory.md#countable-set) saturation means $\aleph_1$-saturation, including [complete types](../../../foundations-of-mathematics.md#complete-type) over countably many parameters.

Here is a general [saturated elementary extension theorem](../../../foundations-of-mathematics.md#saturated-elementary-extension-theorem), with proof: for every infinite [regular cardinal](../../../set-theory.md#regular-cardinal) $\kappa$, every [first-order structure](../../../mathematical-logic.md#first-order-structure) $M$ has a $\kappa$-saturated [elementary extension](../../../foundations-of-mathematics.md#elementary-extension). At a stage $M_\alpha$, list all [complete types](../../../foundations-of-mathematics.md#complete-type) over its [subsets](../../../set.md#subset) of size less than $\kappa$. There is a [set](../../../set.md) of them, since their formulas lie in a set-sized language. Add a witness constant for each [complete type](../../../foundations-of-mathematics.md#complete-type) to the [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure) of $M_\alpha$, together with every formula in that [complete type](../../../foundations-of-mathematics.md#complete-type) evaluated at its witness constant. A finite part mentions finitely many [complete types](../../../foundations-of-mathematics.md#complete-type) and finitely many formulas from each; each finite conjunction is realizable in $M_\alpha$, and the witnesses for different [complete types](../../../foundations-of-mathematics.md#complete-type) are unconstrained relative to each other. Thus the finite part is satisfiable. The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) produces an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) $M_{\alpha+1}$ realizing all those [complete types](../../../foundations-of-mathematics.md#complete-type). At limits take elementary unions, justified by the [elementary chain theorem](../../../foundations-of-mathematics.md#elementary-chain-theorem).

Iterate for $\kappa$ stages and put $N=\bigcup_{\alpha<\kappa}M_\alpha$. If $A\subseteq N$ has size below $\kappa$, regularity bounds the stages at which its elements enter, so $A\subseteq M_\alpha$ for some $\alpha<\kappa$. A [complete type](../../../foundations-of-mathematics.md#complete-type) over $A$ consistent with $N$ is finitely satisfiable in $M_\alpha$: each finite conjunction is an existential formula with parameters from $M_\alpha$, and elementarity transfers its truth from $N$. The [complete type](../../../foundations-of-mathematics.md#complete-type) is therefore realized in $M_{\alpha+1}$. This proves

$$
\boxed{M\preccurlyeq N,\qquad N\text{ is }\kappa\text{-saturated}.}
$$

For a singular desired degree, apply the theorem at a larger [regular cardinal](../../../set-theory.md#regular-cardinal). If $M$ is infinite and an uncountable regular $\kappa$ satisfies $\kappa^{<\kappa}=\kappa$, with $|L|<\kappa$ and $|M|\le\kappa$, the construction can keep every stage of size $\kappa$. There are then at most $\kappa$ parameter [sets](../../../set.md) and [complete types](../../../foundations-of-mathematics.md#complete-type), and downward Löwenheim-Skolem gives that size after each extension; adding $\kappa$ distinct elements initially ensures final size exactly $\kappa$. The resulting model is saturated in the unqualified sense. The cardinal-arithmetic hypothesis belongs to this size refinement, not to the general existence theorem.

An explicit [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) version is useful too. In a [countable](../../../set-theory.md#countable-set) language let $U$ be a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) on $\omega$ and $N=\prod_{i<\omega}M_i/U$, where each factor is nonempty. Enumerate a [countable](../../../set-theory.md#countable-set) finitely satisfiable [complete type](../../../foundations-of-mathematics.md#complete-type), including its chosen parameter representatives, as $\varphi_1(x),\varphi_2(x),\ldots$. By the [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem), the [set](../../../set.md) $A_n$ of coordinates where the first $n$ formulas have a simultaneous witness belongs to $U$. Put

$$
B_n=\{i:i\ge n\}\cap\bigcap_{j\le n}A_j.
$$

These are decreasing members of $U$. At coordinate $i$, let $k(i)$ be the greatest $n\le i$ with $i\in B_n$, if there is one. Choose a witness to the first $k(i)$ formulas there, and an arbitrary element when there is none. For fixed $n$, every coordinate in $B_n$ has $k(i)\ge n$, so the chosen function satisfies $\varphi_n$ on a $U$-large [set](../../../set.md). Its [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) class realizes the whole [complete type](../../../foundations-of-mathematics.md#complete-type). A [countable](../../../set-theory.md#countable-set) language over a [countable](../../../set-theory.md#countable-set) parameter [set](../../../set.md) has only countably many formulas, so this proves [countable saturation of a nonprincipal ultraproduct over omega](../../../foundations-of-mathematics.md#countable-saturation-of-a-nonprincipal-ultraproduct-over-omega).

For [NFU](../../../set-theory.md#new-foundations-with-urelements), we give the [rank-indiscernible construction of an NFU model](../../../set-theory.md#rank-indiscernible-construction-of-an-nfu-model) explicitly. [NFU](../../../set-theory.md#new-foundations-with-urelements) has a unary predicate $S$ for [sets](../../../set.md), atoms have no members, [extensionality](../../../set-theory.md#axiom-of-extensionality) applies to [sets](../../../set.md), and comprehension applies to every [stratified formula](../../../set-theory.md#stratified-formula). A stratification assigns integer types to variables so that equality uses equal types and $x\in y$ requires $\operatorname{type}(y)=\operatorname{type}(x)+1$. A unary [set](../../../set.md) predicate adds no type difference.

Start with the actual [set](../../../set.md) structure $B=(V_{\omega+\omega},\in)$. This structure satisfies [extensionality](../../../set-theory.md#axiom-of-extensionality) and every pure-membership [separation](../../../set-theory.md#axiom-schema-of-specification) instance: the [subset](../../../set.md#subset) defined in a [set](../../../set.md) $a$ of rank below $\omega+\omega$ still has rank below $\omega+\omega$. We do not assert that $B$ satisfies [replacement](../../../set-theory.md#axiom-schema-of-replacement) or all of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). Expand it by [Skolem functions](../../../mathematical-logic.md#skolem-function). In it use the [sequence](../../../real-analysis.md#sequence) of rank objects $V_{\omega+n+6}$, $n<\omega$. For two such objects $d<e$ in [sequence](../../../real-analysis.md#sequence) order, we have

$$
d\subsetneq e,\qquad \forall x\,(x\subseteq d\Longrightarrow x\in e),
$$

with quantifiers in $B$. The second statement holds because every [subset](../../../set.md#subset) of $V_\alpha$ belongs to $V_{\alpha+1}$, and the later rank is at least $\alpha+1$.

Introduce constants $d_i$, $i\in\mathbb Z$, and require them to be order indiscernibles in the Skolem language, satisfying these two assertions whenever $i<j$. Also require $V_{\omega+5}\subseteq d_i$ for every $i$; this fixed rank object is first-order definable in $B$. Every finite part of these requirements together with $\operatorname{Th}(B^*)$ is satisfiable: color finite increasing tuples of the original rank [sequence](../../../real-analysis.md#sequence) by the truth values of the finitely many formulas mentioned, and use [Ramsey's theorem](../../../ramsey-theory.md#ramsey-s-theorem) to get a homogeneous [subsequence](../../../real-analysis.md#subsequence). The rank assertions hold for every increasing tuple there. The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) gives a model of the full theory. In its [Skolem hull](../../../mathematical-logic.md#skolem-hull) $N$ generated by the $d_i$, the integer shift extends to an [automorphism](../../../algebra.md#automorphism) $j$ with $j(d_i)=d_{i+1}$, by the term-transport proof of the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem). Thus $N$ still satisfies [extensionality](../../../set-theory.md#axiom-of-extensionality) and all pure-membership [separation](../../../set-theory.md#axiom-schema-of-specification) instances, and

$$
N\models\forall x\,(x\subseteq d_i\Longrightarrow x\in d_{i+1})
\quad(i\in\mathbb Z).
$$

This is a set-sized [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory); no satisfaction predicate for a proper-class universe is being assumed.

Externally let $D_i=\{x\in N:N\models x\in d_i\}$. The [automorphism](../../../algebra.md#automorphism) bijects $D_i$ onto $D_{i+1}$. Interpret a typed structure with sort $i$ equal to $D_i$. At sort $i+1$, declare $y$ a [set](../../../set.md) exactly when $N\models y\subseteq d_i$; otherwise it is an atom. Define adjacent-sort membership by

$$
x\in_i y\quad\Longleftrightarrow\quad N\models(y\subseteq d_i\ \land\ x\in y).
$$

The guard is necessary: a typed atom might have some ordinary $N$-members in $D_i$, and those must not become its typed members. Set-extensionality follows from [extensionality](../../../set-theory.md#axiom-of-extensionality) in $N$, because the ordinary members of a typed [set](../../../set.md) all lie in $D_i$. For any typed formula on sort $i$, its quantifiers can be restricted to the corresponding $d_l$, its [set](../../../set.md) predicates replaced by [subset](../../../set.md#subset) assertions, and its memberships replaced by the guarded relation. This is an ordinary pure-membership formula of $N$ with finitely many parameters. [Separation](../../../set-theory.md#axiom-schema-of-specification) gives its extension $X\subseteq d_i$, and the displayed closure assertion gives $X\in d_{i+1}$. It is therefore a typed [set](../../../set.md) witnessing comprehension. The [automorphism](../../../algebra.md#automorphism) shifts these sorted domains and preserves the [set](../../../set.md) flags and guarded memberships.

Collapse the types onto $D_0$. Define

$$
S(y)\quad\Longleftrightarrow\quad N\models j(y)\subseteq d_0,
\qquad x\mathrel E y\quad\Longleftrightarrow\quad S(y)\ \land\ N\models x\in j(y).
$$

Objects not satisfying $S$ have no $E$-members. If two [sets](../../../set.md) have the same $E$-members, their images under $j$ are [subsets](../../../set.md#subset) of $d_0$ with the same ordinary members, so are equal by [extensionality](../../../set-theory.md#axiom-of-extensionality) of $N$; injectivity of $j$ gives equality of the original objects.

To verify every stratified comprehension instance, assign a variable $v$ its stratification type $t(v)$ and translate its value $a\in D_0$ to $j^{t(v)}(a)\in D_{t(v)}$. Equality is preserved. An atomic $E(x,y)$ translates to the guarded adjacent-sort membership because $t(y)=t(x)+1$; the unary predicate $S(y)$ translates to $j^{t(y)}(y)\subseteq d_{t(y)-1}$. [Induction](../../../foundations-of-mathematics.md#mathematical-induction) on formulas, using the domain bijections for quantifiers, preserves truth. If the free variable $x$ has type $t$, typed comprehension produces its extension $X\subseteq d_t$, with $X\in d_{t+1}$. Put $b=j^{-(t+1)}(X)\in D_0$. Then $S(b)$ holds, and for every $a\in D_0$,

$$
a\mathrel E b\quad\Longleftrightarrow\quad N\models j^t(a)\in X
\quad\Longleftrightarrow\quad \varphi(a,\vec p).
$$

This is exactly the required [NFU](../../../set-theory.md#new-foundations-with-urelements) [set](../../../set.md). No formula containing the external [automorphism](../../../algebra.md#automorphism) $j$ has been used in a [separation](../../../set-theory.md#axiom-schema-of-specification) or comprehension scheme; $j$ only transports values after the pure formula is formed.

The construction also permits the usual [infinity](../../../mathematics.md#infinity) requirement. The ordinary $\omega$ and its successor graph $f$ are definable in $N$, hence fixed by $j$, and lie below $V_{\omega+5}$, so belong to all the required domains. Under $E$, the members of $\omega$ are still its ordinary $N$-members. The new Kuratowski pair satisfies

$$
\langle x,y\rangle_E=j^{-2}(\langle x,y\rangle_N).
$$

Since $j(f)=f$, membership of this pair in $f$ under $E$ is equivalent to $\langle x,y\rangle_N\in f$. Thus $f$ is an internal injection of $\omega$ into itself omitting zero, giving a Dedekind-infinite [set](../../../set.md).

We have built a model of [NFU](../../../set-theory.md#new-foundations-with-urelements), with [infinity](../../../mathematics.md#infinity) if it is included in the formulation, in ordinary [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) metatheory:

$$
\boxed{\text{ZFC proves the existence of a model of NFU.}}
$$

In particular $\operatorname{Con}(\mathrm{ZFC})\Rightarrow\operatorname{Con}(\mathrm{NFU})$. This proof does not assume $\operatorname{Con}(\mathrm{ZFC})$ as an additional internal axiom: its starting structure is the [set](../../../set.md) $V_{\omega+\omega}$, not a model of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice).

## 6

↑ **Parent:** [Paper 21](paper-21.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A useful form of the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem) says that, for an infinite [first-order structure](../../../mathematical-logic.md#first-order-structure) $M$ and any total order $I$, there is a model of $\operatorname{Th}(M)$ generated as a [Skolem hull](../../../mathematical-logic.md#skolem-hull) by distinct order indiscernibles $(a_i)_{i\in I}$. Every [order automorphism](../../../set.md#order-automorphism) of $I$ extends uniquely to an [automorphism](../../../algebra.md#automorphism) of the specified [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) of that hull. The model can be obtained inside an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) of a [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) of $M$; the generated hull itself need not contain $M$.

Choose a [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) $M^*$ by iteratively adjoining witness functions: for each existential formula in the current language choose a function returning a witness whenever one exists, with an arbitrary value otherwise. Repeat for countably many rounds. Every formula in the final language uses finitely many symbols, so has a witness function from a later round. Thus the expansion is Skolemized for its own formulas, as required for elementarity of its hull. Add constants $a_i$ for $i\in I$ to the complete theory of $M^*$, require them to be distinct, and impose the scheme

$$
\varphi(a_{i_1},\ldots,a_{i_n})\longleftrightarrow\varphi(a_{j_1},\ldots,a_{j_n})
\quad(i_1<\cdots<i_n,\ j_1<\cdots<j_n)
$$

for every formula in the Skolem language. If an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) of $M^*$ is desired, also add its [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure) with separate names for its elements.

Every finite part of this theory is satisfiable. Choose infinitely many distinct elements $b_0,b_1,\ldots$ of $M$. For each of the finitely many arities in that fragment, color increasing index tuples by the finite vector of truth values of the formulas occurring. Repeated applications of the infinite Ramsey theorem give an infinite [subset](../../../set.md#subset) on which all these vectors are constant. Interpret the finitely many $a_i$ in increasing-index order from that [subset](../../../set.md#subset). This satisfies the finite indiscernibility requirements and distinctness, while the [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure) is satisfied by the named original structure. The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) gives a structure $N^*$ satisfying the whole theory.

Let $H$ be the closure of the $a_i$ under the [Skolem functions](../../../mathematical-logic.md#skolem-function), including nullary ones. It is elementary in $N^*$: whenever an existential formula with parameters from $H$ is true in $N^*$, its Skolem witness lies in $H$. This is the [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test), whose proof is [induction](../../../foundations-of-mathematics.md#mathematical-induction) on formulas, using precisely this witness property for the existential step. Hence the reduct of $H$ is a model of $\operatorname{Th}(M)$.

For an [order automorphism](../../../set.md#order-automorphism) $\sigma:I\to I$, define

$$
\widehat\sigma\bigl(t(a_{i_1},\ldots,a_{i_n})\bigr)=t(a_{\sigma(i_1)},\ldots,a_{\sigma(i_n)}).
$$

This is well-defined. If two terms denote the same element, write their equality as a formula on the combined increasing tuple of their indices; indiscernibility preserves that formula after transport by $\sigma$. The same argument preserves every relation and function. Applying $\sigma^{-1}$ gives the inverse, so $\widehat\sigma$ is an [automorphism](../../../algebra.md#automorphism). Since all elements are terms in the generators, it is the unique [automorphism](../../../algebra.md#automorphism) of this [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) extending $a_i\mapsto a_{\sigma(i)}$. This proves the theorem.

One may require the indiscernibles to lie in any specified infinite [sequence](../../../real-analysis.md#sequence) of the starting structure, or to satisfy additional finite-tuple properties holding along that [sequence](../../../real-analysis.md#sequence): the same finite satisfiability proof chooses its homogeneous [subsequence](../../../real-analysis.md#subsequence) there. This strengthened form is what the rank-domain construction of [NFU](../../../set-theory.md#new-foundations-with-urelements) uses. **Uniqueness is asserted in the [Skolem expansion](../../../mathematical-logic.md#skolem-expansion), not for all [automorphisms](../../../algebra.md#automorphism) of its reduct.**

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

For $A\subseteq\omega^\omega$, let the players alternately choose natural numbers, producing $x\in\omega^\omega$; I wins exactly when $x\in A$. A [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) assigns a move to each finite position at which its player moves. It is winning if every compatible completed play is won by that player. A game is determined when one player has a [winning strategy](../../../descriptive-set-theory.md#winning-strategy-in-an-infinite-game). The [axiom of determinacy](../../../descriptive-set-theory.md#axiom-of-determinacy) is

$$
\boxed{\mathsf{AD}:\quad\text{every }A\subseteq\omega^\omega\text{ gives a determined game}.}
$$

We can prove determinacy for open and closed payoffs, including clopen payoffs; finite games are covered by backward [induction](../../../foundations-of-mathematics.md#mathematical-induction). Here is the full open-payoff argument. For an open $A$, let $W_0$ consist of finite positions whose entire cylinder of continuations is contained in $A$. Recursively put

$$
W_{\alpha+1}=W_\alpha\cup\{p:\text{I moves at }p\text{ and some }p^\frown n\in W_\alpha\}
\cup\{p:\text{II moves at }p\text{ and every }p^\frown n\in W_\alpha\},
$$

and take unions at limits. Since positions form a [set](../../../set.md), this process reaches a fixed point $W$. More explicitly, a strict increase at each stage would assign a distinct position to each stage beyond the Hartogs bound of the position [set](../../../set.md), which is impossible; for natural-number moves the least newly added position in a fixed enumeration makes that assignment explicit.

If the initial position belongs to $W$, I can win. At an I-position first added at a successor stage, choose the least move to a position of smaller first-entry rank. At an II-position first added at a successor stage, every successor already has smaller rank. A play following this [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) cannot have an infinite strictly descending [sequence](../../../real-analysis.md#sequence) of [ordinal](../../../set-theory.md#ordinal) ranks, so reaches $W_0$ in finitely many steps; all its further continuations lie in $A$. If the initial position is outside $W$, II keeps the play outside $W$: at an I-position no successor is in $W$, and at an II-position at least one successor is outside $W$, so II chooses the least such move. The play never reaches a winning prefix. Since $A$ is open, membership in $A$ would have been certified by some finite prefix, so the resulting play is outside $A$. Thus **every open game is determined**. Applying this argument to the open complement of a closed payoff, with the players' objectives interchanged, proves closed determinacy too. The argument needs no choice of moves beyond taking the least available natural number.

To refute [AD](../../../descriptive-set-theory.md#axiom-of-determinacy) under [AC](../../../set-theory.md#axiom-of-choice), first use binary moves. There are $\mathfrak c=2^{\aleph_0}$ [strategies](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) for each player, since its positions form a [countable](../../../set-theory.md#countable-set) [set](../../../set.md). Enumerate them as $(\sigma_\alpha)_{\alpha<\mathfrak c}$ and $(\tau_\alpha)_{\alpha<\mathfrak c}$. Each fixed [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) admits exactly $\mathfrak c$ compatible plays: the other player's arbitrary binary [sequence](../../../real-analysis.md#sequence) determines the completed play injectively. Recursively choose a play $u_\alpha$ following $\sigma_\alpha$ and a play $v_\alpha$ following $\tau_\alpha$, each different from all earlier reservations and from each other. This is possible because at stage $\alpha$ fewer than $\mathfrak c$ plays have been reserved. No regularity assumption on $\mathfrak c$ is used: every [ordinal](../../../set-theory.md#ordinal) $\alpha<\mathfrak c$ has cardinality below $\mathfrak c$, and doubling an infinite smaller [cardinal](../../../set-theory.md#cardinal-number) does not reach $\mathfrak c$.

[Set](../../../set.md) $B=\{v_\alpha:\alpha<\mathfrak c\}\subseteq2^\omega$. [Strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) $\sigma_\alpha$ loses on $u_\alpha\notin B$, while $\tau_\alpha$ loses on $v_\alpha\in B$. Thus this binary game is undetermined. Turn it into a natural-number game by declaring that the first player to play a number outside $\{0,1\}$ loses. Formally its I-payoff is

$$
A=B\cup\{x\in\omega^\omega:\text{the first }n\text{ with }x(n)>1\text{ is odd}\}.
$$

A [winning strategy](../../../descriptive-set-theory.md#winning-strategy-in-an-infinite-game) in this game could not prescribe an illegal move after a compatible legal history, since the opponent could thereby win. Its restriction to legal histories would therefore give a winning binary [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game), contradicting the construction. Hence the [choice diagonalization of an undetermined game](../../../descriptive-set-theory.md#choice-diagonalization-of-an-undetermined-game) proves

$$
\boxed{\mathsf{AC}\Longrightarrow\neg\mathsf{AD}.}
$$

This does not contradict open or closed determinacy: the diagonal payoff has no such regularity requirement.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
