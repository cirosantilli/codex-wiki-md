# Paper 19

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper19.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper19.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
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
  - [i](#7/i)
    - [Solution](#7/i/solution)
  - [ii](#7/ii)
    - [Solution](#7/ii/solution)
- [8](#8)
  - [Solution](#8/solution)

## 1

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [well-quasi-ordering](../../../set.md#well-quasi-ordering) is a [preorder](../../../set.md#preorder) $(Q,\le)$ such that every infinite [sequence](../../../real-analysis.md#sequence) $(x_n)$ has indices $i<j$ with $x_i\le x_j$. Reflexivity and transitivity are part of the definition; antisymmetry is unnecessary. An infinite [sequence](../../../real-analysis.md#sequence) without such a pair is a [bad sequence](../../../set.md#bad-sequence).

The [perfect subsequence lemma](../../../set.md#perfect-subsequence-lemma) strengthens this definition: **every infinite [sequence](../../../real-analysis.md#sequence) in a [well-quasi-order](../../../set.md#well-quasi-ordering) has an infinite nondecreasing [subsequence](../../../real-analysis.md#subsequence)**, meaning

$$
\boxed{i_0<i_1<\cdots,\qquad x_{i_r}\le x_{i_s}\quad(r<s).}
$$

Here is a proof that does not assume the lemma implicitly. There must be an index $i$ with infinitely many later indices $j$ satisfying $x_i\le x_j$. Otherwise each index would have only finitely many such successors. Starting with any index, choose the next one beyond the [union](../../../set.md#set-union) of those finite successor [sets](../../../set.md) for the previously chosen indices. This constructs a [bad sequence](../../../set.md#bad-sequence), contradicting the [well-quasi-ordering](../../../set.md#well-quasi-ordering) property.

Choose $i_0$ with infinitely many successors above it, and restrict to those successors. Apply the same argument to that infinite [subsequence](../../../real-analysis.md#subsequence), obtaining $i_1>i_0$ with infinitely many later successors above it within the restricted [sequence](../../../real-analysis.md#sequence). Continue. Every subsequent restriction lies inside all previous upper cones, so $x_{i_r}\le x_{i_s}$ for every $r<s$. This proves the lemma, including for a genuine [quasi-order](../../../set.md#preorder) with distinct equivalent elements. Both alternatives below use it.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For finite [rooted trees](../../../combinatorics.md#rooted-tree), use [rooted-tree homeomorphic embedding](../../../combinatorics.md#homeomorphic-embedding-of-a-rooted-tree): an [injective](../../../algebra.md#injective-function) vertex map preserves ancestors and [lowest common ancestors](../../../combinatorics.md#lowest-common-ancestor), so edges may become paths and distinct branches remain distinct. The root can map to a vertex below the host root. More generally label vertices in a [well-quasi-ordering](../../../set.md#well-quasi-ordering) $Q$ and require each source label to precede its image label. We prove this stronger [labelled version of Kruskal's tree theorem](../../../set.md#labelled-version-of-kruskal-s-tree-theorem), from which the unlabelled result follows by taking one label.

We first need the finite-word closure, and prove it rather than merely invoking [Higman lemma](../../../set.md#higman-s-lemma). If finite [words](../../../foundations-of-mathematics.md#string) over $Q$ were not a [well-quasi-ordering](../../../set.md#well-quasi-ordering) under order-preserving [subsequence](../../../real-analysis.md#subsequence) embedding with increased labels, choose a [minimal bad sequence](../../../set.md#minimal-bad-sequence) $w_0,w_1,\ldots$, minimizing the length of $w_n$ among [words](../../../foundations-of-mathematics.md#string) admitting a bad continuation of the already chosen prefix. No $w_n$ is empty. Write $w_n=v_na_n$ by removing its last letter. The [perfect subsequence lemma](../../../set.md#perfect-subsequence-lemma) gives $n_0<n_1<\cdots$ with $a_{n_r}\le a_{n_s}$ for $r<s$.

The [sequence](../../../real-analysis.md#sequence) $w_0,\ldots,w_{n_0-1},v_{n_0},v_{n_1},\ldots$ is still bad. An earlier $w_i$ embedding into a later $v_{n_r}$ would embed into $w_{n_r}$, contradicting the original [sequence](../../../real-analysis.md#sequence). An embedding of $v_{n_r}$ into $v_{n_s}$ extends by the last-letter comparison to an embedding of $w_{n_r}$ into $w_{n_s}$. Both possibilities are excluded. This contradicts minimality at position $n_0$, since $v_{n_0}$ is shorter. Thus the finite-word closure holds. The [perfect subsequence lemma](../../../set.md#perfect-subsequence-lemma) also proves finite product closure: first pass to a nondecreasing [subsequence](../../../real-analysis.md#subsequence) in one coordinate, then in the next, preserving all previous comparisons.

Suppose now that the labelled trees admit a [bad sequence](../../../set.md#bad-sequence) $T_0,T_1,\ldots$. Choose a [minimal bad sequence](../../../set.md#minimal-bad-sequence) by vertex number. Let $\mathcal U$ be all the proper descendant-rooted subtrees of these trees. We claim that $\mathcal U$ is a [well-quasi-ordering](../../../set.md#well-quasi-ordering). If it had a [bad sequence](../../../set.md#bad-sequence) of subtrees $U_r$, its parent indices can be made strictly increasing, say $U_r$ comes from $T_{n_r}$. Indeed each finite initial collection of parent trees has only finitely many subtrees, and a [bad sequence](../../../set.md#bad-sequence) cannot contain infinitely many terms from a finite collection. Passing to a [subsequence](../../../real-analysis.md#subsequence) therefore makes $n_0<n_1<\cdots$.

Then $T_0,\ldots,T_{n_0-1},U_0,U_1,\ldots$ is bad. A prefix tree embedding into $U_r$ would embed into its parent $T_{n_r}$, contrary to the original badness, and the tail is bad by construction. But $U_0$ has fewer vertices than $T_{n_0}$, contradicting minimality. This proves the claim.

Give the children of each root any fixed order. Its forest of child subtrees is a finite [word](../../../foundations-of-mathematics.md#string) in $\mathcal U$. The [word](../../../foundations-of-mathematics.md#string) theorem and finite product closure show that the pairs consisting of the root label and the child-subtree [word](../../../foundations-of-mathematics.md#string) are a [well-quasi-ordering](../../../set.md#well-quasi-ordering). Thus some $i<j$ have comparable root labels and an embedding of the child [word](../../../foundations-of-mathematics.md#string) of $T_i$ into that of $T_j$. Map the source root to the target root and use the obtained embeddings inside distinct target child subtrees. The paths from the target root into those distinct branches are disjoint except at the root, so this is a [label-monotone tree embedding](../../../combinatorics.md#label-monotone-tree-embedding). It contradicts badness. Hence

$$
\boxed{\text{finite rooted trees labelled in a WQO are a WQO under homeomorphic embedding.}}
$$

For [Friedman's finite form of Kruskal's theorem](../../../set.md#friedman-s-finite-form-of-kruskal-s-theorem), fix $k\in\mathbb N$. **There is $N(k)$ such that any $N(k)$ trees with $|T_i|\le k+i$ contain $i<j$ with $T_i\preceq T_j$.** Use indices starting at zero; shifting them only changes $k$. To prove this uniform finite bound, form the [finite bad-sequence tree](../../../set.md#finite-bad-sequence-tree) of finite bad prefixes obeying the size bounds. At position $i$ there are only finitely many rooted-tree [isomorphism](../../../algebra.md#isomorphism) types with at most $k+i$ vertices, so every node has finitely many successors.

If no bound existed, this tree would have nodes of arbitrarily large depth. A node with arbitrarily long extensions has a child with arbitrarily long extensions, since it has only finitely many children. Choosing such a child repeatedly produces an infinite branch, as in the [König infinity lemma](../../../combinatorics.md#konig-s-lemma). The branch is an infinite bad tree [sequence](../../../real-analysis.md#sequence), contradicting the theorem just proved. Therefore the required $N(k)$ exists. The same proof works with any fixed finite label alphabet and any specified size bound finite at each position.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The PDF's displayed inequality uses the relation it purports to define and therefore is not itself a complete definition. The absorption order consistent with that inequality and with the requested result is

$$
\boxed{x\preceq y\quad\Longleftrightarrow\quad x+y=x.}
$$

This is the reverse of the usual natural order of an [incline](../../../algebra.md#incline). We specify it explicitly: using instead $x+y=y$ would make the finite-generation conclusion false in general.

[Idempotence](../../../algebra.md#idempotence) gives $x+x=x$, proving reflexivity. If $x+y=x$ and $y+z=y$, then [associativity](../../../group.md#associative-property) gives

$$
x+z=(x+y)+z=x+(y+z)=x+y=x,
$$

so the relation is transitive. If also $y+x=y$, [commutativity](../../../algebra.md#commutativity) forces $x=y$. Thus it is even a [partial order](../../../set.md#partially-ordered-set). In this order $x+y\preceq x$ follows because $(x+y)+x=x+y$. Absorption says that multiplying a [monomial](../../../polynomial.md#monomial) by any additional factors moves it upward in $\preceq$.

Let $g_1,\ldots,g_r$ generate the [incline](../../../algebra.md#incline). Distributivity, [commutativity](../../../algebra.md#commutativity) and [idempotence](../../../algebra.md#idempotence) expand every element into a finite nonempty sum of [monomials](../../../polynomial.md#monomial) $g^a=g_1^{a_1}\cdots g_r^{a_r}$ with $a\in\mathbb N^r\setminus\{0\}$. A zero exponent means that factor is omitted; no multiplicative identity is assumed. If $a\le b$ componentwise, then $g^a+g^b=g^a$ by absorption, or by [idempotence](../../../algebra.md#idempotence) when $a=b$.

We prove the needed [reverse-inclusion well-quasi-ordering of monomial ideals](../../../commutative-algebra.md#reverse-inclusion-well-quasi-ordering-of-monomial-ideals) directly. Upward-closed [subsets](../../../set.md#subset) of $\mathbb N^r$ form a [well-quasi-ordering](../../../set.md#well-quasi-ordering) under reverse inclusion. For $r=1$ these are the tails, plus the [empty set](../../../set.md#empty-set), ordered like $\mathbb N\cup\{\infty\}$. For the induction, write an upset $U\subseteq\mathbb N^{r+1}$ as increasing slices $U_0\subseteq U_1\subseteq\cdots$ in $\mathbb N^r$. Their [union](../../../set.md#set-union) is an upset with a finite minimal basis by [Dickson lemma](../../../combinatorics.md#dickson-s-lemma). To see that finite-basis fact here, $\mathbb N^r$ is a [well-quasi-ordering](../../../set.md#well-quasi-ordering) by the finite product argument above, so its minimal elements cannot form an infinite [antichain](../../../extremal-set-theory.md#antichain); every element lies above a minimal one because its lower coordinate box is finite. All basis elements of the [union](../../../set.md#set-union) appear by some finite slice, so the slices eventually stabilize.

Encode $U$ by the finite [word](../../../foundations-of-mathematics.md#string) of slices before stabilization and its final slice. By the finite-word theorem proved in the other alternative, and finite product closure, these encodings are a [well-quasi-ordering](../../../set.md#well-quasi-ordering) with slice comparisons given by reverse inclusion. For two comparable encodings, let the earlier pre-stabilization slice $U_k$ match the later slice $V_{f(k)}$, where $f(k)\ge k$. Then

$$
U_k\supseteq V_{f(k)}\supseteq V_k.
$$

Beyond the earlier stabilization index, its final slice contains the later final slice and hence every later slice. Therefore $U\supseteq V$. This proves the induction, including empty slices and the empty upset.

For an [incline](../../../algebra.md#incline) element $x$, choose a finite exponent support $F_x$ of a sum representing it and put $\uparrow F_x=\{b:\exists a\in F_x\ (a\le b)\}$. Given an infinite [sequence](../../../real-analysis.md#sequence) of elements, the just-proved result supplies $i<j$ with $\uparrow F_{x_i}\supseteq\uparrow F_{x_j}$. Every [monomial](../../../polynomial.md#monomial) in the chosen sum for $x_j$ is therefore absorbed by a [monomial](../../../polynomial.md#monomial) in the sum for $x_i$. Adding these absorptions gives $x_i+x_j=x_i$, even if the [incline](../../../algebra.md#incline) has further identities between terms. Hence

$$
\boxed{\text{every finitely generated incline is well-quasi-ordered by }\preceq.}
$$

The order direction matters. On the positive integers take $x+y=\min(x,y)$ and multiplication to be ordinary addition of integers. This is an [incline](../../../algebra.md#incline) generated by $1$. Its usual natural order $x+y=y$ is the reverse of the ordinary numerical order, and the [sequence](../../../real-analysis.md#sequence) $1,2,3,\ldots$ is bad in that order. Its reverse absorption order is the ordinary numerical order, consistent with the theorem above.

## 2

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [large cardinal](../../../set-theory.md#large-cardinal) axiom says that there is an uncountable [cardinal](../../../set-theory.md#cardinal-number) with a strong closure, reflection, combinatorial or embedding property. Its interest is not merely the magnitude of the [cardinal](../../../set-theory.md#cardinal-number): it packages a universe-like portion of [set](../../../set.md) theory, or a coherent way of comparing the universe with a proper [inner model](../../../set-theory.md#inner-model). Such axioms form a hierarchy extending ordinary [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), compared through [relative consistency](../../../mathematical-logic.md#relative-consistency) implications. The consistency qualifications are essential; an existence axiom is not a theorem of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) simply because its consequences are attractive.

The basic example is a [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal): an uncountable [regular cardinal](../../../set-theory.md#regular-cardinal) $\kappa$ which is a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal), so

$$
\operatorname{cf}(\kappa)=\kappa,\qquad 2^\lambda<\kappa\quad(\lambda<\kappa).
$$

These conditions imply $|V_\alpha|<\kappa$ for every $\alpha<\kappa$. Prove this by induction along the [cumulative hierarchy](../../../set-theory.md#cumulative-hierarchy): the successor step uses the strong-limit property, and a limit step uses regularity to bound a [union](../../../set.md#set-union) of fewer than $\kappa$ smaller [sets](../../../set.md). Thus every member of $V_\kappa$ has [cardinality](../../../set-theory.md#cardinality) below $\kappa$.

Consequently **$V_\kappa$ is a [transitive model](../../../set-theory.md#transitive-model) of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice)**. Pairing, [union](../../../set.md#set-union), [power set](../../../set.md#power-set), [separation](../../../set-theory.md#axiom-schema-of-specification), [axiom of infinity](../../../set-theory.md#axiom-of-infinity) and [foundation](../../../set-theory.md#axiom-of-regularity) stay within the hierarchy. For [replacement](../../../set-theory.md#axiom-schema-of-replacement), a definable [function](../../../function.md) on $x\in V_\kappa$ has fewer than $\kappa$ values; regularity bounds their ranks below $\kappa$, putting the range in $V_\kappa$. Ambient [choice](../../../set-theory.md#axiom-of-choice) supplies a [choice function](../../../set-theory.md#choice-function) for a family in $V_\kappa$, and its graph also has bounded rank. This verifies the substantial closure axiom rather than only saying that the rank is large. It also shows why inaccessible existence cannot be proved in a consistent [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice): it would yield a [set](../../../set.md) [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) and hence its consistency, contrary to the [Gödel second incompleteness theorem](../../../mathematical-logic.md#godel-second-incompleteness-theorem).

An uncountable regular limit [cardinal](../../../set-theory.md#cardinal-number) is a [weakly inaccessible cardinal](../../../set-theory.md#weakly-inaccessible-cardinal); requiring the strong-limit inequality is stronger without additional hypotheses. Under [GCH](../../../set-theory.md#generalized-continuum-hypothesis), every smaller infinite [cardinal](../../../set-theory.md#cardinal-number) satisfies $2^\lambda=\lambda^+<\kappa$, so the two notions coincide. This distinction separates cardinal-arithmetic assumptions from the regularity requirement.

A [Mahlo cardinal](../../../set-theory.md#mahlo-cardinal) is an inaccessible $\kappa$ whose [inaccessible cardinals](../../../set-theory.md#strongly-inaccessible-cardinal) below it form a [stationary set](../../../set-theory.md#stationary-set). Thus every [club set](../../../set-theory.md#club-set) meets those inaccessibles, which strengthens mere unboundedness. There are inaccessible $\lambda<\delta<\kappa$; $V_\delta$ is a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) containing an inaccessible $\lambda$. Mahloness therefore supplies a consistency statement stronger than the bare existence of one inaccessible. Iterating the demand that smaller [cardinals](../../../set-theory.md#cardinal-number) have the same reflection property leads to further levels of the hierarchy.

A [weakly compact cardinal](../../../set-theory.md#weakly-compact-cardinal) is a logical and combinatorial strengthening of inaccessibility. One standard characterization is an inaccessible $\kappa$ with

$$
\kappa\longrightarrow(\kappa)^2_2:
$$

every two-colouring of pairs has a homogeneous [subset](../../../set.md#subset) of size $\kappa$. Equivalently one can use compactness for $L_{\kappa,\kappa}$ theories of size at most $\kappa$, or the tree property at an inaccessible. These viewpoints explain the terminology: a local collection of compatible requirements has a global realization, and tall narrow trees cannot avoid cofinal branches. They are characterization statements; the elementary closure and measure arguments below are separate proofs of the consequences used here.

A [measurable cardinal](../../../set-theory.md#measurable-cardinal) carries a nonprincipal [kappa-complete](../../../set-theory.md#kappa-complete-filter) [ultrafilter](../../../set-theory.md#ultrafilter) $U$ on $\kappa$. Every [set](../../../set.md) of size less than $\kappa$ is $U$-null, since it is a [union](../../../set.md#set-union) of fewer than $\kappa$ null singletons. Such a [cardinal](../../../set-theory.md#cardinal-number) is regular: a cofinal [sequence](../../../real-analysis.md#sequence) of length $\mu<\kappa$ would partition $\kappa$ into $\mu$ bounded, hence null, pieces; completeness would make their [union](../../../set.md#set-union) null, an impossibility.

It is also strong limit. If $\lambda<\kappa$ and there were distinct [sets](../../../set.md) $A_\alpha\subseteq\lambda$ for $\alpha<\kappa$, choose for each $\xi<\lambda$ the $U$-large side of the partition according to whether $\xi\in A_\alpha$. The [intersection](../../../set.md#set-intersection) of these fewer than $\kappa$ large sides belongs to $U$, but all its indices designate the same [subset](../../../set.md#subset) of $\lambda$, so it has at most one member. This contradicts nonprincipality. Hence $2^\lambda<\kappa$, proving that every [measurable cardinal](../../../set-theory.md#measurable-cardinal) is inaccessible.

The measure gives an [ultrapower embedding](../../../set-theory.md#ultrapower-embedding). Form equivalence classes of [functions](../../../function.md) $f:\kappa\to V$ under equality on a $U$-large [set](../../../set.md), with membership defined coordinatewise modulo $U$. Induction on [first-order formulas](../../../mathematical-logic.md#first-order-formula) proves elementarity: Boolean operations use the [ultrafilter](../../../set-theory.md#ultrafilter) laws, and the existential step chooses coordinate witnesses on a large [set](../../../set.md). Countable completeness makes the [ultrapower](../../../foundations-of-mathematics.md#ultrapower) [well-founded](../../../set-theory.md#well-founded-relation). An infinite descending membership chain would give countably many large coordinate conditions; their [intersection](../../../set.md#set-intersection) would produce an actual infinite membership descent in $V$. Collapse the [ultrapower](../../../foundations-of-mathematics.md#ultrapower) to a [transitive class](../../../set-theory.md#transitive-class) $M$, obtaining $j:V\to M$.

For $\alpha<\kappa$, every [function](../../../function.md) into $\alpha$ is constant on a large [set](../../../set.md) by completeness; induction shows $j(\alpha)=\alpha$. The class of the identity [function](../../../function.md) is larger than every such constant [ordinal](../../../set-theory.md#ordinal) and lies below $j(\kappa)$, so $j(\kappa)>\kappa$. Thus the [critical point of an elementary embedding](../../../set-theory.md#critical-point-of-an-elementary-embedding) is $\kappa$. The measure viewpoint has become a precise self-similarity principle for the universe.

A [supercompact cardinal](../../../set-theory.md#supercompact-cardinal) imposes arbitrarily strong closure on these embeddings: for every $\lambda\ge\kappa$ there is $j:V\to M$ with critical point $\kappa$, $j(\kappa)>\lambda$, and $M^\lambda\subseteq M$. It implies measurability by the derived [ultrafilter](../../../set-theory.md#ultrafilter)

$$
U=\{X\subseteq\kappa:\kappa\in j(X)\}.
$$

Elementarity makes this an [ultrafilter](../../../set-theory.md#ultrafilter); fixed [ordinals](../../../set-theory.md#ordinal) below $\kappa$ show that singletons are null. For $\mu<\kappa$, $j$ fixes the indexing length, so it carries an [intersection](../../../set.md#set-intersection) of $\mu$ [sets](../../../set.md) to the [intersection](../../../set.md#set-intersection) of their images. If all these images contain $\kappa$, so does their [intersection](../../../set.md#set-intersection), proving $\kappa$-completeness.

These examples illustrate three connected uses of [large cardinals](../../../set-theory.md#large-cardinal): obtaining [set](../../../set.md) [first-order models](../../../mathematical-logic.md#model-of-a-first-order-theory) and stronger consistency statements, extending finite or countable compactness and partition phenomena to uncountable domains, and constructing [elementary embeddings](../../../set-theory.md#elementary-embedding) with controlled closure. They also interact with [inner models](../../../set-theory.md#inner-model): an inaccessible remains inaccessible in the [constructible universe](../../../definable-power-set.md#constructible-universe), since it cannot acquire a new short cofinal [sequence](../../../real-analysis.md#sequence) there and there are fewer [subsets](../../../set.md#subset) of smaller [ordinals](../../../set-theory.md#ordinal). A [measurable cardinal](../../../set-theory.md#measurable-cardinal)'s measure need not belong to that [inner model](../../../set-theory.md#inner-model), so preservation of the stronger property is a different issue. [Large cardinal](../../../set-theory.md#large-cardinal) axioms are thus structured additional hypotheses, with carefully distinguishable consequences and relative-consistency claims, rather than a single claim that sufficiently big [cardinals](../../../set-theory.md#cardinal-number) exist.

## 3

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

All independence assertions here are [relative consistency](../../../mathematical-logic.md#relative-consistency) results. Begin with a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory); for the choice-preserving side use [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). The original [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) already gives the side where [foundation](../../../set-theory.md#axiom-of-regularity) holds. We construct the opposite side while checking the other axioms, then add a symmetry restriction to make [choice](../../../set-theory.md#axiom-of-choice) fail.

Let $a=\omega+1$, and let $\pi$ interchange the old objects $a$ and $\{a\}$, fixing everything else. They are distinct. On the same domain define the [Rieger-Bernays permutation model](../../../set-theory.md#rieger-bernays-permutation-model) by

$$
\boxed{x\mathrel E y\quad\Longleftrightarrow\quad x\in\pi(y).}
$$

Write $S(b)=\pi^{-1}(b)$; the $E$-members of $S(b)$ are exactly the old members of $b$. In particular $a\mathrel E a$, and $a$ has no other $E$-member. Thus $a$ is a [Quine atom](../../../set-theory.md#quine-atom), and the nonempty $E$-set $a$ has no member disjoint from itself. [Foundation](../../../set-theory.md#axiom-of-regularity) fails.

Here are the other axioms explicitly. Equal $E$-extensions imply $\pi(y)=\pi(z)$ by old [extensionality](../../../set-theory.md#axiom-of-extensionality), hence $y=z$. An $E$-pair of $x,z$ is $S(\{x,z\})$. An $E$-union of $y$ is

$$
S\left(\bigcup\{\pi(x):x\in\pi(y)\}\right).
$$

Its elements are precisely objects with an $E$-membership chain of length two into $y$. The $E$-power [set](../../../set.md) of $y$ is

$$
S\left(\{S(b):b\subseteq\pi(y)\}\right),
$$

since $x\subseteq_E y$ means $\pi(x)\subseteq\pi(y)$. These are old [sets](../../../set.md) by [power set](../../../set.md#power-set) and [replacement](../../../set-theory.md#axiom-schema-of-replacement).

Translate any [first-order formula](../../../mathematical-logic.md#first-order-formula) by replacing its membership symbol with $E$, a definable relation with parameter $a$. [Separation](../../../set-theory.md#axiom-schema-of-specification) on $y$ produces the representative of the old [set](../../../set.md) $\{x\in\pi(y):\varphi^E(x)\}$. For [replacement](../../../set-theory.md#axiom-schema-of-replacement), functionality in the new structure is exactly functionality of the translated [first-order formula](../../../mathematical-logic.md#first-order-formula) on the old [set](../../../set.md) $\pi(y)$; old [replacement](../../../set-theory.md#axiom-schema-of-replacement) gives its range, and $S$ represents that range as an $E$-set. Thus the full schemas, not merely their quantifier-free instances, survive. The old finite [ordinals](../../../set-theory.md#ordinal) and $\omega$ are fixed by $\pi$, so their empty-set and successor relations are unchanged; the old $\omega$ witnesses [axiom of infinity](../../../set-theory.md#axiom-of-infinity).

If the original [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) satisfies [AC](../../../set-theory.md#axiom-of-choice), the new one does too. For an $E$-family $y$ of nonempty $E$-sets, old [choice](../../../set-theory.md#axiom-of-choice) selects $c(x)\in\pi(x)$ for each $x\in\pi(y)$. The $E$-ordered-pair construction is definable, so old [replacement](../../../set-theory.md#axiom-schema-of-replacement) forms the graph of this selection in $E$-pair codes; applying $S$ makes it an $E$-function. It chooses an $E$-member from each member of the family. Therefore a full membership permutation alone does not refute [choice](../../../set-theory.md#axiom-of-choice). We have proved

$$
\boxed{\operatorname{Con}(\mathsf{ZF})\Rightarrow
\operatorname{Con}(\mathsf{ZF}-\mathsf{Foundation}+\neg\mathsf{Foundation}),}
$$

with [choice](../../../set-theory.md#axiom-of-choice) preserved if it was initially present. Together with the unchanged [well-founded](../../../set-theory.md#well-founded-relation) [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory), this proves [foundation](../../../set-theory.md#axiom-of-regularity)'s independence from the remaining axioms.

For the choice-failing extension, work in an ambient [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) and build the [extensional cumulative universe over Quine atoms](../../../set-theory.md#extensional-cumulative-universe-over-quine-atoms). Let $A$ be a countably infinite collection of distinct tagged objects. Give each $q\in A$ the membership extension $\{q\}$. Adjoin [sets](../../../set.md) in successive construction ranks, representing a set-sized collection $X$ by a unique new tagged object with extension $X$, except that the representative of $\{q\}$ is the already existing $q$. Denote this representative by $S(X)$ again. Thus $S(\{q\})=q$; adjoining a second, distinct ordinary singleton would incorrectly violate [extensionality](../../../set-theory.md#axiom-of-extensionality).

More formally take atom tags of kind zero, put $D_0=A$, and define

$$
D_{\alpha+1}=D_\alpha\cup\{(1,X):X\subseteq D_\alpha,
\ X\ne\{q\}\text{ for every }q\in A\},\qquad
D_\lambda=\bigcup_{\alpha<\lambda}D_\alpha.
$$

The extension of $(1,X)$ is $X$, and the extension of an atom $q$ is $\{q\}$. Tags of the two kinds are disjoint. Any set-sized collection of objects has bounded construction ranks and hence a representative at a later stage. This proves pairing, [union](../../../set.md#set-union), [power set](../../../set.md#power-set), [separation](../../../set-theory.md#axiom-schema-of-specification) and [replacement](../../../set-theory.md#axiom-schema-of-replacement) by representing their extensions, just as above. For [axiom of infinity](../../../set-theory.md#axiom-of-infinity), recursively construct the pure finite ordinals, collect these representatives in an ambient [set](../../../set.md) by [replacement](../../../set-theory.md#axiom-schema-of-replacement), and apply $S$ to that collection. The resulting inductive [set](../../../set.md) is fixed by every atom permutation. Every object has a unique extension, so full [extensionality](../../../set-theory.md#axiom-of-extensionality) holds, although [foundation](../../../set-theory.md#axiom-of-regularity) fails at the atoms.

Let $G$ be the full [symmetric group](../../../finite-group-theory.md#symmetric-group) of $A$. Extend $g\in G$ by $g(S(X))=S(g''X)$, recursively on the non-atomic construction ranks. This preserves membership, including the atomic self-loops. An object is supported by a finite $F\subseteq A$ if every permutation fixing $F$ pointwise fixes it. Retain the [hereditarily finite-supported Quine-atom model](../../../set-theory.md#hereditarily-finite-supported-quine-atom-model) $H$: every object reachable from a retained object by finitely many membership steps has [finite support](../../../group-theory.md#finite-support-in-a-permutation-action). In particular all members of a retained object are retained, every atom is supported by itself, and $S(A)$ is supported by the [empty set](../../../set.md#empty-set).

We verify the schemas in $H$, rather than assuming that an arbitrary invariant class is a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory). For [separation](../../../set-theory.md#axiom-schema-of-specification), a [subset](../../../set.md#subset) of a retained [set](../../../set.md) $x$ definable in $H$ from parameters $p_1,\ldots,p_m$ is fixed by permutations fixing the [union](../../../set.md#set-union) of their finite supports. Its members are already in $H$, so its representative belongs to $H$. For [replacement](../../../set-theory.md#axiom-schema-of-replacement), a definable functional image of $x$ is a [set](../../../set.md) in the ambient universe. Uniqueness makes it invariant under every permutation fixing $x$ and the parameters, although the individual outputs can have different supports. Those outputs are in $H$ by the relativized [first-order formula](../../../mathematical-logic.md#first-order-formula), so the range representative is hereditarily supported. This proves [replacement](../../../set-theory.md#axiom-schema-of-replacement) without falsely requiring one [finite support](../../../group-theory.md#finite-support-in-a-permutation-action) for every individual value.

The internal [power set](../../../set.md#power-set) is the representative of

$$
\{S(Y):Y\subseteq\operatorname{ext}(x),\ S(Y)\in H\}.
$$

It is an ambient [set](../../../set.md) and is fixed by the support of $x$, because a permutation carries retained [subsets](../../../set.md#subset) of $x$ to retained [subsets](../../../set.md#subset) of $x$. Every member is retained by its definition. This proves the internal power-set axiom. Finite [unions](../../../set.md#set-union) of supports handle pairing and [union](../../../set.md#set-union); the pure [natural numbers](../../../arithmetic.md#natural-number) have empty support; [extensionality](../../../set-theory.md#axiom-of-extensionality) is inherited because $H$ is membership-transitive. Hence $H$ satisfies all [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axioms except [foundation](../../../set-theory.md#axiom-of-regularity), which still fails.

In $H$ form the family of all two-element [subsets](../../../set.md#subset) of $A$, a family with empty support. Suppose it had a [choice function](../../../set-theory.md#choice-function) $f\in H$, with [finite support](../../../group-theory.md#finite-support-in-a-permutation-action) $F$. Choose distinct $q,r\in A\setminus F$. Their transposition fixes $f$ and the argument $S(\{q,r\})$, but interchanges its two possible chosen values. Equivariance gives a contradiction. Thus

$$
\boxed{H\models\mathsf{ZF}-\mathsf{Foundation}
+\neg\mathsf{Foundation}+\neg\mathsf{AC}.}
$$

The full construction over $A$, before restricting to $H$, has [choice](../../../set-theory.md#axiom-of-choice) by ambient [choice](../../../set-theory.md#axiom-of-choice) and the representability of [choice](../../../set-theory.md#axiom-of-choice) graphs. Alternatively an ordinary [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) gives the positive [choice](../../../set-theory.md#axiom-of-choice) side. This proves the independence of [AC](../../../set-theory.md#axiom-of-choice) from [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) minus [foundation](../../../set-theory.md#axiom-of-regularity). The required metatheoretic consistency can be expressed using Con([ZF](../../../set-theory.md#zermelo-fraenkel-set-theory)), since the [constructible universe](../../../definable-power-set.md#constructible-universe) of a [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) supplies [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), as explained in the next solution. No assumption of a [transitive model](../../../set-theory.md#transitive-model) follows from mere consistency or is needed for these interpreted [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) constructions.

## 4

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

An [inner model](../../../set-theory.md#inner-model) of a universe of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) is a [transitive class](../../../set-theory.md#transitive-class) $M$ containing every [ordinal](../../../set-theory.md#ordinal) and satisfying the required set-theoretic axioms with the inherited membership relation. Transitivity means that every member of a member of $M$ belongs to $M$. Requiring all [ordinals](../../../set-theory.md#ordinal) distinguishes an [inner model](../../../set-theory.md#inner-model) from a [transitive set](../../../set-theory.md#transitive-set) [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) such as $V_\kappa$: a [set](../../../set.md) [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) has bounded [ordinal](../../../set-theory.md#ordinal) height. One may specify an [inner model](../../../set-theory.md#inner-model) of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory), [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) or a stronger theory; [choice](../../../set-theory.md#axiom-of-choice) is not built into the term unless specified.

The fundamental example is the [constructible universe](../../../definable-power-set.md#constructible-universe). Form the [constructible hierarchy](../../../definable-power-set.md#constructible-hierarchy)

$$
L_0=\varnothing,\qquad L_{\alpha+1}=\operatorname{Def}(L_\alpha),\qquad
L_\lambda=\bigcup_{\alpha<\lambda}L_\alpha,
\qquad L=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha.
$$

Here [definable power set](../../../definable-power-set.md) means [subsets](../../../set.md#subset) definable over the [set](../../../set.md) structure $(L_\alpha,\in)$ by [first-order formulas](../../../mathematical-logic.md#first-order-formula) with finitely many parameters from that level. Each level is transitive, the levels increase, and $\operatorname{Ord}\cap L_\alpha=\alpha$, by induction. Thus $L$ is transitive and contains all [ordinals](../../../set-theory.md#ordinal).

The construction supplies a definable [well-order](../../../set.md#well-order): order objects first by their earliest construction stage, then by a least [first-order formula](../../../mathematical-logic.md#first-order-formula) code and a finite tuple of parameters in the already constructed level's [well-order](../../../set.md#well-order). Recursively extend the earlier [well-order](../../../set.md#well-order) at each successor stage and unite compatible orders at limits. [First-order formula](../../../mathematical-logic.md#first-order-formula) codes and finite tuples of well-ordered parameters are well-orderable. This yields a canonical global ordering definable within $L$; its restrictions to [sets](../../../set.md) will give [choice](../../../set-theory.md#axiom-of-choice) once the [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) axioms are checked.

For that check, a useful reflection argument is explicit. Given finitely many [first-order formulas](../../../mathematical-logic.md#first-order-formula) and a starting level, pass to a higher level containing witnesses for their existential subformulas on all parameter tuples from the current level, choosing least witnesses in the canonical order. There are set-many tuples, so ambient [replacement](../../../set-theory.md#axiom-schema-of-replacement) bounds their witness stages. Repeat for $\omega$ steps and take the [union](../../../set.md#set-union) level $L_\theta$. Every relevant witness with parameters in that level appears at a later step. Induction on [first-order formulas](../../../mathematical-logic.md#first-order-formula), with this witness property for the existential case, proves that $L_\theta$ reflects the chosen finite list of [first-order formulas](../../../mathematical-logic.md#first-order-formula) of $L$.

[Separation](../../../set-theory.md#axiom-schema-of-specification) on a constructible [set](../../../set.md) is then definability over a sufficiently large reflecting level, so its [subset](../../../set.md#subset) appears at the next level. For [replacement](../../../set-theory.md#axiom-schema-of-replacement), reflect the [first-order formula](../../../mathematical-logic.md#first-order-formula) specifying a functional image and its required existence statements. All inputs belong to a level containing the domain as a [set](../../../set.md); all their unique outputs then lie in one reflecting level. The image is definable there and hence is constructible. For [power set](../../../set.md#power-set), the ambient [set](../../../set.md) of constructible [subsets](../../../set.md#subset) of $x$ has bounded construction stages by [replacement](../../../set-theory.md#axiom-schema-of-replacement) in the ambient universe. At a level containing them all, this internal collection is definable by the bounded condition $y\subseteq x$, and therefore is itself in $L$. Pairing, [union](../../../set.md#set-union) and [axiom of infinity](../../../set-theory.md#axiom-of-infinity) follow directly from definability over sufficiently large levels, while [extensionality](../../../set-theory.md#axiom-of-extensionality) and [foundation](../../../set-theory.md#axiom-of-regularity) follow from transitivity. Thus $L\models\mathsf{ZF}$, and its canonical ordering gives $L\models\mathsf{AC}$.

This proves the important relative-consistency application

$$
\boxed{\operatorname{Con}(\mathsf{ZF})\Rightarrow\operatorname{Con}(\mathsf{ZFC}).}
$$

One does not conclude that [choice](../../../set-theory.md#axiom-of-choice) is true in the original universe. Instead the [inner model](../../../set-theory.md#inner-model) supplies a possibly smaller universe in which [choice](../../../set-theory.md#axiom-of-choice) holds.

Constructibility also supplies [GCH](../../../set-theory.md#generalized-continuum-hypothesis). Here is the cardinal-counting argument, making clear the role of the [condensation lemma for the constructible universe](../../../definable-power-set.md#condensation-lemma-for-the-constructible-universe). Work inside $L$. If $x\subseteq\kappa$ is constructible, take a large limit $L_\theta$ containing $x$ and an elementary hull of $\kappa\cup\{\kappa,x\}$ of size $\kappa$. Its transitive collapse is $L_\beta$ by condensation. The collapse fixes every [ordinal](../../../set-theory.md#ordinal) below $\kappa$, and hence fixes $x$ and $\kappa$. Since the hull has size $\kappa$, $\beta<\kappa^+$. Therefore every constructible [subset](../../../set.md#subset) of $\kappa$ appears below $L_{\kappa^+}$.

The condensation fact expresses the rigidity of this definability construction: [first-order formula](../../../mathematical-logic.md#first-order-formula) codes, finite parameter tuples and satisfaction in set-sized lower levels are preserved by the collapse. Inducting over the hull's [ordinal](../../../set-theory.md#ordinal) indices identifies each collapsed lower level with the corresponding $L$-level; elementarity supplies every definable [subset](../../../set.md#subset) coded by parameters in that collapsed lower level. Taking [unions](../../../set.md#set-union) identifies the entire collapsed hull with a level $L_\beta$.

Induction on construction stages gives $|L_\gamma|\le |\gamma|+\aleph_0$: each successor has only countably many [first-order formula](../../../mathematical-logic.md#first-order-formula) schemes with finite parameter tuples, and limits take [unions](../../../set.md#set-union). Hence $|L_{\kappa^+}|=\kappa^+$ for infinite $\kappa$. The preceding containment gives $2^\kappa\le\kappa^+$ in $L$, and Cantor's theorem gives the reverse inequality. Consequently

$$
\boxed{L\models\mathsf{ZFC}+\mathsf{GCH},\qquad
\operatorname{Con}(\mathsf{ZF})\Rightarrow
\operatorname{Con}(\mathsf{ZFC}+\mathsf{GCH}).}
$$

All these [cardinal](../../../set-theory.md#cardinal-number) computations are internal to $L$; they need not equal the ambient [cardinal](../../../set-theory.md#cardinal-number) computations.

[Inner models](../../../set-theory.md#inner-model) are also useful for analyzing stronger axioms. If $\kappa$ is inaccessible in $V$, it remains an uncountable [regular cardinal](../../../set-theory.md#regular-cardinal) in $L$, because a shorter cofinal [sequence](../../../real-analysis.md#sequence) in $L$ would already be one in $V$. For each [ordinal](../../../set-theory.md#ordinal) $\lambda<\kappa$, its constructible [subsets](../../../set.md#subset) are fewer than $\kappa$ even in the internal [cardinal](../../../set-theory.md#cardinal-number) comparison: in $V$, $\mathcal P(\lambda)$ has size below $\kappa$, so its constructible part cannot have an $L$-well-order of length at least $\kappa$. Thus it remains strong limit. Accordingly $L$ supplies relative-consistency information compatible with inaccessibles and [GCH](../../../set-theory.md#generalized-continuum-hypothesis). Stronger embedding or measure properties require extra analysis, since the witnessing objects may disappear upon passing to an [inner model](../../../set-theory.md#inner-model).

There is a useful limitation: **no uniform inner-model construction can refute [choice](../../../set-theory.md#axiom-of-choice) from every starting [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) universe**. Every [inner model](../../../set-theory.md#inner-model) $M$ of [ZF](../../../set-theory.md#zermelo-fraenkel-set-theory) contains the ambient $L$. Indeed, induction gives $L_\alpha^M=L_\alpha$: the same set-sized level has the same satisfaction relation for definitions, and limit stages take the same [unions](../../../set.md#set-union). If the starting universe already satisfies $V=L$, any [inner model](../../../set-theory.md#inner-model) containing all [ordinals](../../../set-theory.md#ordinal) must therefore be the whole universe, where [choice](../../../set-theory.md#axiom-of-choice) holds. To obtain a choice-failing [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) uniformly one needs a different method, such as the symmetry restriction in the preceding solution. Inner-model arguments establish consistency and preservation through carefully controlled smaller universes; they do not freely manufacture arbitrary desired axiom failures.

## 5

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Here a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [set](../../../set.md) must mean an infinite [homogeneous set for a colouring](../../../ramsey-theory.md#homogeneous-set-for-a-colouring): every singleton is a finite [monochromatic](../../../ramsey-theory.md#monochromatic-set) [set](../../../set.md). The requested phenomenon holds for every finite $n\ge2$. For $n=1$ it is impossible, since the colour classes of a finite [computable colouring](../../../ramsey-theory.md#computable-colouring) are computable and at least one is infinite. We treat this necessary qualification explicitly.

We construct a [finite-injury computable colouring of pairs](../../../ramsey-theory.md#finite-injury-computable-colouring-of-pairs) with no infinite computably enumerable [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring), which is stronger than the requested absence of a recursive one. Enumerate the [computably enumerable sets](../../../foundations-of-mathematics.md#recursively-enumerable-set) as $W_0,W_1,\ldots$, with computable finite approximations $W_{e,s}$. Requirement $e$ seeks distinct markers $a_e,b_e\in W_e$. At stage $s$, consider indices $e\le s$ not currently assigned markers. Choose the least one, if any, for which $W_{e,s}$ has two elements outside all markers of higher-priority indices $d<e$. Assign two such elements as its markers, using a fixed least-element rule, and cancel all markers at lower-priority indices. Do nothing if no such index exists. The active markers are therefore pairwise distinct at every stage.

For $x<y$, simulate this finite construction through stage $y$ and define

$$
c(\{x,y\})=
\begin{cases}
1,&x\text{ is an active second marker }b_e\text{ at stage }y,\\
0,&\text{otherwise}.
\end{cases}
$$

In particular every active first marker has colour zero against larger points. This is a total computable [function](../../../function.md): no question about eventual enumeration or eventual stabilization is used in computing a given pair.

Induction on $e$ proves [finite injury](../../../foundations-of-mathematics.md#finite-injury). Once the finitely many higher requirements have stabilized, requirement $e$ is never cancelled again. If it has markers they stay fixed. If $W_e$ is infinite, it eventually supplies two points outside the finite collection of higher markers, so it becomes eligible and is assigned markers; only finitely many higher indices could delay its assignment. Thus an infinite $W_e$ eventually has permanent distinct markers $a_e,b_e$. Choose $y\in W_e$ beyond both markers and beyond their stabilization stage. Then

$$
c(\{a_e,y\})=0,\qquad c(\{b_e,y\})=1.
$$

So $W_e$ is not homogeneous. Every infinite [recursive set](../../../foundations-of-mathematics.md#computable-set) is computably enumerable, proving the desired obstruction. For $n>2$, colour an increasing $n$-tuple by the pair formed by its first two elements. Every pair from an infinite homogeneous candidate can be completed by $n-2$ larger members of that candidate, so it would give an infinite pair-homogeneous [set](../../../set.md), already ruled out.

The uncountable positive theorem is the [Erdős-Rado theorem for finite arities](../../../set-theory.md#erdos-rado-theorem-for-finite-arities). For every infinite [cardinal](../../../set-theory.md#cardinal-number) $\kappa$ and finite $r\ge0$, define $\beth_0(\kappa)=\kappa$ and $\beth_{r+1}(\kappa)=2^{\beth_r(\kappa)}$. Then

$$
\boxed{\beth_r(\kappa)^+\longrightarrow(\kappa^+)^{r+1}_\kappa.}
$$

The [partition relation](../../../set-theory.md#partition-relation) means that every colouring of $(r+1)$-element [subsets](../../../set.md#subset) of the left-hand [cardinal](../../../set-theory.md#cardinal-number) by at most $\kappa$ colours has a homogeneous [subset](../../../set.md#subset) of size $\kappa^+$. In particular, taking $\kappa=\aleph_0$ gives an uncountable [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) for every finite arity, once the domain is sufficiently large.

We prove the end-homogeneity lemma needed for induction. Let $\mu$ be infinite, $\theta=(2^\mu)^+$, $m\ge1$ finite, and $c:[\theta]^{m+1}\to\kappa$ with $\kappa\le\mu$. In a sufficiently large $H_\chi$ choose an [elementary substructure](../../../mathematical-logic.md#elementary-substructure) $M$ of size $2^\mu$ containing $c,\theta$ and all [ordinals](../../../set-theory.md#ordinal) below $\mu^+$, and closed under externally given [sequences](../../../real-analysis.md#sequence) of length at most $\mu$. Here $H_\chi$ consists of [sets](../../../set.md) whose transitive closures have size below $\chi$.

To justify that closure, begin with a hull containing the indicated parameters and [ordinals](../../../set-theory.md#ordinal). At each successor stage add every [sequence](../../../real-analysis.md#sequence) of length at most $\mu$ from the preceding stage, then take a [Skolem hull](../../../mathematical-logic.md#skolem-hull). There are at most $(2^\mu)^\mu=2^\mu$ such [sequences](../../../real-analysis.md#sequence). Iterate for $\mu^+$ stages and take elementary [unions](../../../set.md#set-union) at limits. The [union](../../../set.md#set-union) still has size $2^\mu$, and every [sequence](../../../real-analysis.md#sequence) of at most $\mu$ of its elements is contained in one earlier stage by regularity of $\mu^+$, so appears at the next. This proves the claimed closed [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) rather than assuming its existence.

Let $\beta=\sup(M\cap\theta)<\theta$. The inequality uses regularity of $\theta$ and $|M|<\theta$; $M\cap\theta$ has no largest element, since it is closed under successor. Recursively choose increasing $x_\alpha\in M\cap\theta$ for $\alpha<\mu^+$, imposing, for every $m$-tuple $t$ of earlier points,

$$
c(t\cup\{x_\alpha\})=c(t\cup\{\beta\}).
$$

At any stage there are at most $\mu$ earlier points and constraints. Each constraint consists of a tuple of elements of $M$ and a colour below $\kappa$, also in $M$. The entire constraint code therefore belongs to $M$ by closure. The bound above the previous points belongs to $M$ as well. Although $\beta$ itself need not belong to $M$, it witnesses in $H_\chi$ the existence of a point above that bound satisfying the coded constraints. Elementarity supplies such a point inside $M$. This proves the recursion.

On the resulting [sequence](../../../real-analysis.md#sequence) $X$ of length $\mu^+$, the colour of an $(m+1)$-tuple depends only on its first $m$ entries: its last entry has the same colour contribution as $\beta$. This is the required [closed elementary-submodel construction of an end-homogeneous sequence](../../../set-theory.md#closed-elementary-submodel-construction-of-an-end-homogeneous-sequence).

Now prove the theorem by induction on $r$. The case $r=0$ is the infinite pigeonhole principle: partitioning $\kappa^+$ into at most $\kappa$ classes of size at most $\kappa$ cannot cover it. For $r\ge1$, [set](../../../set.md) $\mu=\beth_{r-1}(\kappa)$ and apply the lemma to the colouring on $(2^\mu)^+=\beth_r(\kappa)^+$. Define a colouring of $r$-tuples from its end-homogeneous [sequence](../../../real-analysis.md#sequence) of length $\mu^+$ by their colour when completed with $\beta$. The induction hypothesis supplies a [subset](../../../set.md#subset) of size $\kappa^+$ on which this derived colouring is constant. Every original $(r+1)$-tuple from that [subset](../../../set.md#subset) has the derived colour of its first $r$ entries, and is therefore [monochromatic](../../../ramsey-theory.md#monochromatic-set). This completes the proof.

The unrestricted infinite-exponent situation is very different under [AC](../../../set-theory.md#axiom-of-choice). On $[\lambda]^\omega$, choose one representative $R$ of each equivalence class modulo [finite symmetric difference](../../../set.md#finite-symmetric-difference), and colour $A$ by

$$
c(A)=|A\mathbin\triangle R|\pmod2.
$$

If $A$ is infinite and $a\in A$, deleting $a$ remains in the same equivalence class and flips the colour. Every infinite candidate [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) contains such an $A$ and $A\setminus\{a\}$ as [subsets](../../../set.md#subset), so

$$
\boxed{\lambda\nrightarrow(\omega)^\omega_2\quad\text{for every infinite cardinal }\lambda.}
$$

More generally the same argument works for [subsets](../../../set.md#subset) of any fixed infinite [cardinality](../../../set-theory.md#cardinality): deleting one element preserves that [cardinality](../../../set-theory.md#cardinality), so there is no unrestricted analogue with a [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) large enough to contain such [subsets](../../../set.md#subset). For the order-type-$\omega$ convention, choose $A$ in increasing order type $\omega$ and delete its first element; both [sets](../../../set.md) still have that order type. Thus the distinction from the finite-arity theorem is genuine, not merely a notational ambiguity. This argument uses [choice](../../../set-theory.md#axiom-of-choice) of representatives and is not a claim about every definability-restricted infinite-arity colouring.

## 6

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [complete type](../../../foundations-of-mathematics.md#complete-type) over $A\subseteq M$ is a maximal consistent [set](../../../set.md) of [first-order formulas](../../../mathematical-logic.md#first-order-formula) in a fixed finite tuple of variables with parameters from $A$, consistent with the theory of that parameter expansion. A [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) $M$ is a [saturated model](../../../foundations-of-mathematics.md#saturated-model) of degree $\kappa$ if every such type with $|A|<\kappa$ is realized in $M$. It suffices to require this for one-variable types and realize a finite tuple successively. Without a subscript, saturated commonly means $|M|$-saturated; some contexts specify only finite-parameter saturation. We state the degree explicitly.

The [saturated elementary extension theorem](../../../foundations-of-mathematics.md#saturated-elementary-extension-theorem) says that **every [first-order structure](../../../mathematical-logic.md#first-order-structure) has a $\kappa$-saturated [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) for any specified infinite $\kappa$**. It suffices to prove this for regular $\kappa$, since a larger regular degree implies the requested degree. At a single stage $M$, list all complete one-variable types over all [subsets](../../../set.md#subset) of $M$ of size below $\kappa$. This collection is a [set](../../../set.md). Adjoin a witness constant for each type to the [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure) of $M$ and require that constant to satisfy its type. Every finite [subset](../../../set.md#subset) is satisfiable in $M$: each type's finite conjunction has a witness there, and the finitely many new constants have no cross-constraints. The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) gives an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) realizing all these types simultaneously.

Repeat this step along an elementary chain $(M_\alpha)_{\alpha<\kappa}$, taking [unions](../../../set.md#set-union) at limit stages, and let $N$ be its [union](../../../set.md#set-union). The [elementary chain theorem](../../../foundations-of-mathematics.md#elementary-chain-theorem) follows here by induction on [first-order formulas](../../../mathematical-logic.md#first-order-formula): an existential statement true in the [union](../../../set.md#set-union) has a witness in a later stage; elementarity brings an existential witness back to the earlier stage containing its parameters. Thus each stage is elementary in $N$.

If $A\subseteq N$ has size below regular $\kappa$, all its elements lie in a single $M_\alpha$, by taking the [supremum](../../../real-analysis.md#supremum) of their fewer-than-$\kappa$ stage indices. Any [complete type](../../../foundations-of-mathematics.md#complete-type) over $A$ consistent with $N$ is already consistent over $M_\alpha$, since these structures have the same parameter theory. It was therefore realized in $M_{\alpha+1}$. This proves $\kappa$-saturation of $N$.

A corresponding theorem about full saturation is available with a stated cardinal-size hypothesis: if $\lambda$ is uncountable regular, $|\mathcal L|<\lambda$, and $\lambda^{<\lambda}=\lambda$, then every infinite [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of size at most $\lambda$ has an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) of size $\lambda$ which is $\lambda$-saturated. First adjoin $\lambda$ pairwise distinct constants to the [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure); every finite fragment is satisfiable because the original [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) is infinite. A [Skolem hull](../../../mathematical-logic.md#skolem-hull) of their realizations and the original domain has size $\lambda$. There are at most $\lambda$ small parameter [sets](../../../set.md) and at most $2^{|\mathcal L|+|A|+\aleph_0}\le\lambda$ types over each of them. Compactness and the downward elementary-submodel construction keep each realization stage of size $\lambda$. Taking a [Skolem hull](../../../mathematical-logic.md#skolem-hull) of the preceding stage and the chosen witnesses closes under at most $\lambda$ finite terms and proves this size bound and elementarity. The same length-$\lambda$ chain is consequently a fully [saturated model](../../../foundations-of-mathematics.md#saturated-model) of size $\lambda$. The [cardinal](../../../set-theory.md#cardinal-number) hypothesis is not silently asserted to hold for every [cardinal](../../../set-theory.md#cardinal-number).

We now prove consistency of [NFU](../../../set-theory.md#new-foundations-with-urelements) by the permitted alternative method of indiscernibles and a domain-shifting [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure). This can start from an explicit [set](../../../set.md) structure available in [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), so we need not assume that there is a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of all [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). Let

$$
H=V_{\omega+\omega},\qquad F(n)=V_{\omega+n}\quad(n\in\omega),
$$

and give $F$ the value $\varnothing$ off the [natural numbers](../../../arithmetic.md#natural-number). Regard $(H,\in,F,\omega)$ as a [first-order structure](../../../mathematical-logic.md#first-order-structure), with a named object $\omega$. The graph of $F$ is an external [set](../../../set.md) in the metatheory; it need not be a member of $H$. This structure is extensional and satisfies every [separation](../../../set-theory.md#axiom-schema-of-specification) instance in the pure membership language: any [subset](../../../set.md#subset) of $x\in H$ has rank below $\omega+\omega$ and belongs to $H$. It also satisfies, for natural $m<n$,

$$
\forall X\ (X\subseteq F(m)\Rightarrow X\in F(n)),
$$

since a [subset](../../../set.md#subset) of $V_{\omega+m}$ has rank at most $\omega+m$ and hence belongs to $V_{\omega+n}$.

Apply the indiscernible construction proved in question 7(i) to a [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) of this [set](../../../set.md) structure, requiring $(c_i)_{i\in\mathbb Z}$ to be increasing members of its named natural-number object. For every finite fragment use an increasing [sequence](../../../real-analysis.md#sequence) of ordinary [natural numbers](../../../arithmetic.md#natural-number) in the initial structure in the Ramsey argument. The resulting generated elementary hull $M$ has an external [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) $j$ with $j(c_i)=c_{i+1}$, preserving $F$ and the named $\omega$. Put $D_i=F^M(c_i)$ and $D=D_0$. Then $j(D_i)=D_{i+1}$, and $M$ satisfies the displayed subset-containment assertion between successive domains. No claim that $M$ satisfies [replacement](../../../set-theory.md#axiom-schema-of-replacement) is required.

All membership and [subset](../../../set.md#subset) statements about these objects are interpreted inside $M$. The hull is necessarily externally nonstandard: the natural-number objects $\ldots,c_{-2},c_{-1},c_0$ give an external descending chain. The external [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) is not an object that must be definable within that [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory).

On the external domain $D$ define

$$
\boxed{S(y)\iff M\models j(y)\subseteq D,\qquad
x\mathrel E y\iff S(y)\ \text{and}\ M\models x\in j(y).}
$$

This is the [rank-shifting NFU model with explicit set predicate](../../../set-theory.md#rank-shifting-nfu-model-with-explicit-set-predicate). The guard $S(y)$ is essential: an object not contained in $D$ could still have some ordinary members in $D$, and must not thereby become a nonempty atom. The objects failing $S$ have no $E$-members. If two objects satisfying $S$ have the same $E$-members, their images under $j$ are [subsets](../../../set.md#subset) of $D$ with the same members, so [extensionality](../../../set-theory.md#axiom-of-extensionality) in $M$ and injectivity of $j$ make the original objects equal. Thus set-extensionality and the atom condition hold.

It remains to prove every comprehension instance. Use the domains $D_i$ just constructed, equivalently $D_i=j^i(D)$, for integer sorts. The map $j$ is a [bijection](../../../function.md#bijection) from the objects of $D_i$ to the objects of $D_{i+1}$, and every [subset](../../../set.md#subset) of $D_i$ that exists in $M$ is an element of $D_{i+1}$. In sort $i$ define the [set](../../../set.md) predicate by $y\subseteq D_{i-1}$; from sort $i$ to $i+1$ define membership by ordinary membership guarded by $y\subseteq D_i$.

For a [stratified formula](../../../set-theory.md#stratified-formula), assign integer types to its variables with equal types for equality and adjacent types for membership. Shift all types uniformly if necessary so the finitely many used types are nonnegative. Replace a variable of type $i$ by $j^i$ of its untyped value, quantify it over $D_i$, and use the typed relations just described. Applying $j^i$ to the untyped definition shows that each atomic [first-order formula](../../../mathematical-logic.md#first-order-formula) has the same truth value under this translation; induction on connectives and quantifiers proves the same for the whole [first-order formula](../../../mathematical-logic.md#first-order-formula). Importantly the translated [first-order formula](../../../mathematical-logic.md#first-order-formula) is an ordinary [first-order formula](../../../mathematical-logic.md#first-order-formula) of $M$ with finitely many domain and transformed-parameter constants, not a [first-order formula](../../../mathematical-logic.md#first-order-formula) containing the external [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) as a predicate.

If the comprehension variable has type $i$, [separation](../../../set-theory.md#axiom-schema-of-specification) in $M$ produces its extension $X\subseteq D_i$. The subset-containment assertion gives $X\in D_{i+1}$. Put $y=j^{-(i+1)}(X)\in D$. Then $j(y)=j^{-i}(X)\subseteq D$, hence $S(y)$, and for every $x\in D$,

$$
x\mathrel E y\quad\Longleftrightarrow\quad j^i(x)\in X
\quad\Longleftrightarrow\quad\varphi(x).
$$

This verifies stratified comprehension with arbitrary parameters. The empty extension gives a distinguished [empty set](../../../set.md#empty-set); the always-true [first-order formula](../../../mathematical-logic.md#first-order-formula) gives a universal [set](../../../set.md). The unstratified Russell predicate is not an allowed comprehension instance. Thus

$$
\boxed{\mathsf{ZFC}\vdash\operatorname{Con}(\mathsf{NFU}).}
$$

Starting from the actual [set](../../../set.md) structure $H$ and applying compactness constructs a [set](../../../set.md) [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory), so this is a consistency proof in [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), not merely an assumption of Con([ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice)). It proves the requested consistency with an explicit interpretation; it does not depend on treating the much stronger full [extensionality](../../../set-theory.md#axiom-of-extensionality) of NF as already consistent. The external $j$ is a tool of the construction, not an extra symbol permitted in [NFU](../../../set-theory.md#new-foundations-with-urelements)'s comprehension scheme.

## 7

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="7/i">i</h3>

↑ **Parent:** [7](#7)

<h4 id="7/i/solution">Solution</h4>

↑ **Parent:** [I](#7/i)

One useful form of the [Ehrenfeucht-Mostowski theorem](../../../foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem) is this: for an infinite [first-order structure](../../../mathematical-logic.md#first-order-structure) $A$ and any total order $I$, there is a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of $\operatorname{Th}(A)$ generated in a chosen [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) by an [order-indiscernible sequence](../../../foundations-of-mathematics.md#order-indiscernible-sequence) $(c_i)_{i\in I}$ of distinct elements. Every [order automorphism](../../../set.md#order-automorphism) of $I$ induces an [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) of this expanded hull. One can additionally obtain an [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) containing $A$ by including its [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure). Uniqueness of the induced [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) is asserted in the [Skolem expansion](../../../mathematical-logic.md#skolem-expansion), not among arbitrary [structure automorphisms](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) of the reduct.

Choose a [Skolem expansion](../../../mathematical-logic.md#skolem-expansion) $A^*$: for every existential [first-order formula](../../../mathematical-logic.md#first-order-formula) choose a witness [function](../../../function.md), satisfying $\exists y\,\varphi(y,\bar x)\Rightarrow\varphi(f_\varphi(\bar x),\bar x)$. Iterate the expansion if necessary so witnesses are available for [first-order formulas](../../../mathematical-logic.md#first-order-formula) in the resulting language. Add constants $c_i$ and require $c_i\ne c_j$ for distinct indices. For every [first-order formula](../../../mathematical-logic.md#first-order-formula) $\varphi(x_1,\ldots,x_m)$ of the expanded language and every two increasing index tuples, add

$$
\varphi(c_{i_1},\ldots,c_{i_m})\longleftrightarrow
\varphi(c_{j_1},\ldots,c_{j_m}).
$$

Together with $\operatorname{Th}(A^*)$, this is the indiscernibility theory.

Every finite fragment is satisfiable. It mentions only finitely many [first-order formulas](../../../mathematical-logic.md#first-order-formula) and index constants. Choose a countably infinite [sequence](../../../real-analysis.md#sequence) of distinct elements of $A^*$. For each relevant arity, colour increasing tuples from that [sequence](../../../real-analysis.md#sequence) by the finite truth vector of all [first-order formulas](../../../mathematical-logic.md#first-order-formula) of that arity in the fragment. Successive applications of the infinite [Ramsey theorem for r-sets](../../../ramsey-theory.md#ramsey-s-theorem) leave an infinite [subset](../../../set.md#subset) homogeneous for each of these finitely many finite colourings. Interpret the finitely many index constants by distinct elements of that [subset](../../../set.md#subset) in increasing enumeration order. All the required truth-value equivalences then hold, and the original structure satisfies the finite part of its own theory.

If an actual [elementary extension](../../../foundations-of-mathematics.md#elementary-extension) of $A$ is desired, include constants for its elements and the [elementary diagram](../../../foundations-of-mathematics.md#elementary-diagram-of-a-structure) of $A^*$. A finite fragment still contains only finitely many parameter instances; include those truth vectors in the same colourings. Thus finite satisfiability is unchanged. The [compactness theorem](../../../mathematical-logic.md#compactness-theorem) now supplies a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) with the entire indiscernible [sequence](../../../real-analysis.md#sequence), and in the diagram version an elementary copy of $A$.

Take the [Skolem hull](../../../mathematical-logic.md#skolem-hull) of the generators, including the diagram constants when present. The witness [functions](../../../function.md) show directly that the hull is elementary: whenever an existential [first-order formula](../../../mathematical-logic.md#first-order-formula) with hull parameters is true in the ambient [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory), its Skolem witness belongs to the hull. Induction on [first-order formulas](../../../mathematical-logic.md#first-order-formula), or the [Tarski-Vaught test](../../../mathematical-logic.md#tarski-vaught-test), gives elementarity. Its reduct is therefore a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of $\operatorname{Th}(A)$. In the version without diagram constants its [cardinality](../../../set-theory.md#cardinality) is at most $\max(|I|,|\mathcal L|,\aleph_0)$.

For an [order automorphism](../../../set.md#order-automorphism) $\rho:I\to I$, define

$$
\widehat\rho\bigl(t(c_{i_1},\ldots,c_{i_m})\bigr)
=t(c_{\rho(i_1)},\ldots,c_{\rho(i_m)}).
$$

This is well defined. If two terms represent the same element, express their equality as a [first-order formula](../../../mathematical-logic.md#first-order-formula) on the increasing [union](../../../set.md#set-union) of their generator indices. Indiscernibility and preservation of the index order carry that equality to the transported terms. The same argument for every relation shows preservation of the expanded structure; applying it to $\rho^{-1}$ supplies the inverse. Every element is a term in the generators, so no other [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) of the specified expansion can have the same action on them. Hence

$$
\boxed{\text{order automorphisms of }I\text{ extend uniquely to the generated Skolem expansion.}}
$$

For an application requiring the generators to lie in a definable infinite ordered class, impose that class predicate and its increasing-order [first-order formulas](../../../mathematical-logic.md#first-order-formula) too. The finite-fragment proof uses an increasing [sequence](../../../real-analysis.md#sequence) in that class, so all these additional conditions are preserved. In particular the integer index order and its shift give the [structure automorphism](../../../mathematical-logic.md#automorphism-of-a-first-order-structure) used in the [NFU](../../../set-theory.md#new-foundations-with-urelements) construction. The constants are order indiscernibles, not necessarily indiscernibles under arbitrary permutations of the index [set](../../../set.md).

<h3 id="7/ii">ii</h3>

↑ **Parent:** [7](#7)

<h4 id="7/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#7/ii)

In the game $G(A)$, where $A\subseteq\omega^\omega$, the players alternately choose [natural numbers](../../../arithmetic.md#natural-number) and produce a [sequence](../../../real-analysis.md#sequence) $x$. Player I wins exactly when $x\in A$. A [strategy in an infinite game](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) assigns a move to every finite position where its player is to move; it is winning if every play following it is won by that player. A game is determined if one player has a [winning strategy](../../../descriptive-set-theory.md#winning-strategy-in-an-infinite-game). Both cannot have [winning strategies](../../../descriptive-set-theory.md#winning-strategy-in-an-infinite-game), since their joint play would have to be won by both. The [axiom of determinacy](../../../descriptive-set-theory.md#axiom-of-determinacy) asserts

$$
\boxed{\mathsf{AD}:\quad \text{every }G(A),\ A\subseteq\omega^\omega,\ \text{is determined}.}
$$

Without assuming [AD](../../../descriptive-set-theory.md#axiom-of-determinacy), one can prove determinacy for finite games by backward induction, and for games with open or closed payoffs by the following argument. Give $\omega^\omega$ its [product topology](../../../geometry-and-topology.md#product-topology) of discrete move coordinates. If $A$ is open, let $W_0$ be the finite positions whose entire cylinder of extensions lies in $A$. Form a [winning-position attractor in an infinite game](../../../descriptive-set-theory.md#winning-position-attractor-in-an-infinite-game) by [transfinite recursion](../../../set-theory.md#transfinite-recursion): add an I-position if some child has already been added, and add an II-position if all its children have already been added. Take [unions](../../../set.md#set-union) at limits. The process stabilizes because there are only set-many positions and each genuine successor change adds a new one.

An added nonterminal position receives its least entry [ordinal](../../../set-theory.md#ordinal). At an I-position in the stable attractor, choose a child of smaller rank; at an II-position every child has smaller rank. Thus every play following I's rank-decreasing [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) must reach $W_0$: an infinite strictly descending [sequence](../../../real-analysis.md#sequence) of [ordinals](../../../set-theory.md#ordinal) cannot exist. The resulting play is in $A$, so I wins from any position in the attractor.

Outside the attractor, every child of an I-position remains outside, and an II-position has some child outside. Otherwise the ranks of all its children would have a set-sized [supremum](../../../real-analysis.md#supremum) and the parent would have been added at a later stage. II chooses such a child and keeps the play outside $W_0$ forever. If its outcome were in the [open set](../../../topology.md#open-set) $A$, some finite prefix would have its entire cylinder in $A$, contrary to this avoidance. Therefore II wins from outside. With natural-number moves the least suitable child may be chosen at each position, so no [choice](../../../set-theory.md#axiom-of-choice) axiom is needed for these [strategies](../../../descriptive-set-theory.md#strategy-in-an-infinite-game). This proves [open determinacy](../../../descriptive-set-theory.md#open-determinacy). For a closed payoff, apply the same argument to its open complement with the players' winning roles interchanged. Clopen payoffs are included in both results.

Now assume [AC](../../../set-theory.md#axiom-of-choice) and construct an undetermined game. The [set](../../../set.md) of [strategies](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) for either player has [cardinality](../../../set-theory.md#cardinality) $\mathfrak c=2^{\aleph_0}$, since a [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) is a [function](../../../function.md) on a countably infinite [set](../../../set.md) of positions. Each fixed [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) is compatible with $\mathfrak c$ plays: the other player's [sequence](../../../real-analysis.md#sequence) of freely chosen moves determines distinct full plays. Use [choice](../../../set-theory.md#axiom-of-choice) to enumerate I's [strategies](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) as $(\sigma_\alpha)_{\alpha<\mathfrak c}$ and II's as $(\tau_\alpha)_{\alpha<\mathfrak c}$, and [well-order](../../../set.md#well-order) the space of plays.

Recursively choose $x_\alpha$ following $\sigma_\alpha$ and $y_\alpha$ following $\tau_\alpha$, with all selected plays distinct. At stage $\alpha$ fewer than $\mathfrak c$ plays have been used, while each compatible-play [set](../../../set.md) has size $\mathfrak c$, so fresh choices exist; take the least ones in the fixed [well-order](../../../set.md#well-order). This does not require regularity of $\mathfrak c$, since $|\alpha|<\mathfrak c$ for every $\alpha$ below its initial [ordinal](../../../set-theory.md#ordinal).

Put $A=\{y_\alpha:\alpha<\mathfrak c\}$. Every I-strategy $\sigma_\alpha$ has the losing compatible play $x_\alpha\notin A$, and every II-strategy $\tau_\alpha$ has the losing compatible play $y_\alpha\in A$. Therefore neither player has a [winning strategy](../../../descriptive-set-theory.md#winning-strategy-in-an-infinite-game). This [choice diagonalization of an undetermined game](../../../descriptive-set-theory.md#choice-diagonalization-of-an-undetermined-game) proves

$$
\boxed{\mathsf{ZF}\vdash\mathsf{AC}\Rightarrow\neg\mathsf{AD}.}
$$

The elementary determinacy proofs above concern specified definable payoff classes; the diagonal construction explains why extending them to every arbitrary [subset](../../../set.md#subset) of the play space is incompatible with [choice](../../../set-theory.md#axiom-of-choice).

## 8

↑ **Parent:** [Paper 19](paper-19.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

For [Fodor's theorem](../../../set-theory.md#fodor-lemma), let $\kappa$ be regular uncountable, $S\subseteq\kappa$ stationary, and $f:S\to\kappa$ regressive: $f(\alpha)<\alpha$ for every nonzero $\alpha\in S$. A [club set](../../../set-theory.md#club-set) is unbounded in $\kappa$ and closed under limits below $\kappa$; a [stationary set](../../../set-theory.md#stationary-set) meets every club. Removing $0$ preserves stationarity. We prove that some fibre of $f$ is stationary, not merely that one fibre is large.

We first check the club facts used in the argument. An [intersection](../../../set.md#set-intersection) of fewer than $\kappa$ club [subsets](../../../set.md#subset) of $\kappa$ is club. Closure is immediate. For unboundedness, given $\gamma$ and clubs $(C_i)_{i<\mu}$ with $\mu<\kappa$, choose an increasing [sequence](../../../real-analysis.md#sequence) $\gamma_n$ starting above $\gamma$, such that $\gamma_{n+1}$ is above a point of every $C_i$ beyond $\gamma_n$. Regularity bounds the [supremum](../../../real-analysis.md#supremum) of the fewer-than-$\kappa$ points at each step. Then $\delta=\sup_{n<\omega}\gamma_n<\kappa$, and the chosen points in each $C_i$ are cofinal in $\delta$; closure puts $\delta$ in their [intersection](../../../set.md#set-intersection).

For a [sequence](../../../real-analysis.md#sequence) $(C_\xi)_{\xi<\kappa}$ of clubs its [diagonal intersection](../../../set-theory.md#diagonal-intersection)

$$
\Delta_{\xi<\kappa}C_\xi
=\{\delta<\kappa:\forall\xi<\delta\ (\delta\in C_\xi)\}
$$

is also club. To obtain a point above $\gamma$, recursively choose $\gamma_{n+1}>\gamma_n$ in $\bigcap_{\xi\le\gamma_n}C_\xi$, possible by the preceding result, and take the [supremum](../../../real-analysis.md#supremum) $\delta$ of the [sequence](../../../real-analysis.md#sequence). For each $\xi<\delta$, every sufficiently late $\gamma_n$ belongs to $C_\xi$, so $\delta\in C_\xi$. For closure, if diagonal-intersection points are cofinal in $\delta<\kappa$, then for each $\xi<\delta$ their sufficiently late points lie in $C_\xi$, and closure again puts $\delta$ there.

Suppose every fibre $S_\xi=\{\alpha\in S:f(\alpha)=\xi\}$ were nonstationary. Choose a club $C_\xi$ disjoint from each fibre. Stationarity supplies $\alpha\in S\cap\Delta_{\xi<\kappa}C_\xi$, with $\alpha>0$. Put $\xi=f(\alpha)<\alpha$. By diagonal membership $\alpha\in C_\xi$, but by its definition $\alpha\in S_\xi$, a contradiction. Thus

$$
\boxed{\exists\xi<\kappa\quad \{\alpha\in S:f(\alpha)=\xi\}\text{ is stationary}.}
$$

This is precisely the pressing-down assertion. Regularity and uncountability were used to keep the club-building suprema below $\kappa$.

For the [Cantor normal form](../../../set-theory.md#cantor-normal-form) theorem, every nonzero [ordinal](../../../set-theory.md#ordinal) has a unique expression

$$
\boxed{\alpha=\omega^{\beta_0}n_0+\cdots+\omega^{\beta_{m-1}}n_{m-1},
\qquad \beta_0>\cdots>\beta_{m-1},\quad 0<n_i<\omega.}
$$

All operations are [ordinal](../../../set-theory.md#ordinal) operations, so the order of the terms matters. The [ordinal](../../../set-theory.md#ordinal) zero has the empty expression. We give the greedy existence proof and then prove uniqueness.

The powers $\omega^\beta$ are strictly increasing and continuous at limit exponents, and satisfy $\omega^\beta\ge\beta$. Hence the [set](../../../set.md) of exponents with $\omega^\beta\le\alpha$ is nonempty and bounded, and its [supremum](../../../real-analysis.md#supremum) $\beta_0$ belongs to it by continuity (or is already its last successor member). Thus there is a largest such exponent and

$$
\omega^{\beta_0}\le\alpha<\omega^{\beta_0+1}
=\omega^{\beta_0}\cdot\omega.
$$

Since the last product is the [supremum](../../../real-analysis.md#supremum) of the finite multiples, there is a unique positive finite $n_0$ satisfying

$$
\omega^{\beta_0}n_0\le\alpha<\omega^{\beta_0}(n_0+1).
$$

The initial segment of $\alpha$ of length $\omega^{\beta_0}n_0$ leaves a tail of unique order type $\rho$, so

$$
\alpha=\omega^{\beta_0}n_0+\rho,\qquad \rho<\omega^{\beta_0}.
$$

The bound follows from strict increase of [ordinal addition](../../../set-theory.md#ordinal-addition) in its right argument: a tail at least $\omega^{\beta_0}$ would contradict the preceding interval. This is the relevant instance of the [ordinal division algorithm](../../../set-theory.md#ordinal-division-algorithm).

If $\rho>0$, apply the same construction to it. Its leading exponent must be below $\beta_0$. Continue with the remainder. An infinite continuation would produce an infinite strictly descending [sequence](../../../real-analysis.md#sequence) of [ordinals](../../../set-theory.md#ordinal), impossible by [well-foundedness](../../../set-theory.md#well-founded-relation). Thus the process terminates after finitely many steps and gives the required form.

To prove uniqueness, first observe that a finite decreasing-exponent suffix with leading exponent $\gamma$ is smaller than $\omega^{\gamma+1}$. This follows by induction on its number of terms: the later tail is below $\omega^\gamma$, so adding it to a finite multiple of $\omega^\gamma$ stays below the next finite multiple and hence below $\omega^\gamma\cdot\omega$. Consequently the tail after a term with exponent $\beta$ is below $\omega^\beta$.

Any proposed normal form therefore places $\alpha$ in exactly the interval

$$
\omega^{\beta_0}n_0\le\alpha<\omega^{\beta_0}(n_0+1)
<\omega^{\beta_0+1}.
$$

Its first exponent is recoverable as the largest exponent whose power does not exceed $\alpha$, and its first coefficient is recoverable as the largest finite multiple not exceeding $\alpha$. The right remainder is unique because [ordinal addition](../../../set-theory.md#ordinal-addition) is strictly increasing in its right argument. Apply the same reasoning to the remainder, successively fixing every exponent and coefficient. This proves uniqueness without treating [ordinal addition](../../../set-theory.md#ordinal-addition) as commutative or cancelling arbitrary left summands.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
