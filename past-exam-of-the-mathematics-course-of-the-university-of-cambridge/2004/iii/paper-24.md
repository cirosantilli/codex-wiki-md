# Paper 24

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper24.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper24.pdf)

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

## 1

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Independence here is a [relative consistency](../../../mathematical-logic.md#relative-consistency) assertion: from a ground [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) satisfying [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice), construct a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory) of each remaining theory in which the omitted [axiom](../../../mathematical-logic.md#axiom) fails. The ground [axiom of choice](../../../set-theory.md#axiom-of-choice) is a tool for constructing these countermodels, not an extra [axiom](../../../mathematical-logic.md#axiom) imposed on the theories being tested. The [constructible universe](../../../definable-power-set.md#constructible-universe) supplies the usual relative-consistency implication from ZF to ZFC, so this ground [choice](../../../set-theory.md#axiom-of-choice) assumption requires no additional consistency strength. These constructions can be formalized inside an arbitrary ground model; they do not require the stronger assumption that a [transitive model](../../../set-theory.md#transitive-model) exists.

**[Union](../../../set.md#set-union).** Put $\lambda=\beth_\omega$ and use the [hereditarily locally small membership model](../../../set-theory.md#hereditarily-locally-small-membership-model)

$$
B_\lambda=\{x:(\forall y\in\operatorname{TC}(\{x\}))\ |y|<\lambda\}.
$$

The ground [cardinal](../../../set-theory.md#cardinal-number) $\lambda$ is a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal) of [countable](../../../set-theory.md#countable-set) [cofinality](../../../set-theory.md#cofinality). This [transitive class](../../../set-theory.md#transitive-class) contains the [empty set](../../../set.md#empty-set) and $\omega$. [Pairing](../../../set-theory.md#axiom-of-pairing) preserves the bound, as does taking a [subset](../../../set.md#subset), so [separation](../../../set-theory.md#axiom-schema-of-specification) holds for every formula relativized to this class. If an internally definable [function](../../../function.md) has domain $a\in B_\lambda$, ground [replacement](../../../set-theory.md#axiom-schema-of-replacement) collects its range $r$. Since $|r|\leq|a|<\lambda$ and every descendant of an element of $r$ already has fewer than $\lambda$ members, $r\in B_\lambda$. Thus the full functional [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) holds. For $x\in B_\lambda$, every actual [subset](../../../set.md#subset) of $x$ belongs to the class and

$$
|\mathcal P(x)|=2^{|x|}<\lambda.
$$

Consequently its entire [power set](../../../set.md#power-set) belongs to the class. [Extensionality](../../../set-theory.md#axiom-of-extensionality) and [foundation](../../../set-theory.md#axiom-of-regularity) are inherited from the ground membership relation; $\omega$ witnesses [infinity](../../../mathematics.md#infinity). However $a=\{\beth_n:n<\omega\}$ belongs to $B_\lambda$, while its only possible [union](../../../set.md#set-union) is $\lambda$, which does not. **All the other ZF [axioms](../../../mathematical-logic.md#axiom) hold, and [union](../../../set.md#set-union) fails.** Bounding the entire [transitive closure](../../../set-theory.md#transitive-closure) by $<\lambda$ instead would give the wrong model: functional ranges at this singular bound need not be hereditarily small.

**[Power set](../../../set.md#power-set).** Use the [transitive class](../../../set-theory.md#transitive-class) $H_{\omega_1}$ of [hereditarily countable sets](../../../set-theory.md#hereditarily-countable-set). [Pairing](../../../set-theory.md#axiom-of-pairing), [union](../../../set.md#set-union) and [separation](../../../set-theory.md#axiom-schema-of-specification) preserve hereditary countability. A functional image of a [countable](../../../set-theory.md#countable-set) domain is [countable](../../../set-theory.md#countable-set), and its members have [countable](../../../set-theory.md#countable-set) [transitive closures](../../../set-theory.md#transitive-closure); their [countable](../../../set-theory.md#countable-set) [union](../../../set.md#set-union) is [countable](../../../set-theory.md#countable-set) in the ground [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) model. This proves [replacement](../../../set-theory.md#axiom-schema-of-replacement). The remaining structural [axioms](../../../mathematical-logic.md#axiom) and [infinity](../../../mathematics.md#infinity) are inherited. Every actual [subset](../../../set.md#subset) of $\omega$ belongs to $H_{\omega_1}$, but a putative internal [power set](../../../set.md#power-set) of $\omega$ would contain all these [subsets](../../../set.md#subset) and hence be uncountable by [Cantor's theorem](../../../set.md#cantor-s-theorem). **[Power set](../../../set.md#power-set) fails in $H_{\omega_1}$, with every other ZF [axiom](../../../mathematical-logic.md#axiom) intact.**

**[Replacement](../../../set-theory.md#axiom-schema-of-replacement).** Use $V_{\omega+\omega}$ in the [cumulative hierarchy](../../../set-theory.md#cumulative-hierarchy). At a limit [ordinal](../../../set-theory.md#ordinal) cutoff, [pairing](../../../set-theory.md#axiom-of-pairing), [union](../../../set.md#set-union), [power set](../../../set.md#power-set) and every instance of [separation](../../../set-theory.md#axiom-schema-of-specification) remain below the cutoff; [foundation](../../../set-theory.md#axiom-of-regularity), [extensionality](../../../set-theory.md#axiom-of-extensionality) and [infinity](../../../mathematics.md#infinity) hold as well. With parameter $V_\omega$, define $f(n)=V_{\omega+n}$ by $n$ finite iterations of [power set](../../../set.md#power-set). The finite iteration witnesses and each value are inside $V_{\omega+\omega}$, so this is an internally definable total [function](../../../function.md) on $\omega$. Its range has [rank of a set](../../../set-theory.md#rank-of-a-set) $\omega+\omega$ and is absent from the model. **This instance of [replacement](../../../set-theory.md#axiom-schema-of-replacement) fails.**

**[Extensionality](../../../set-theory.md#axiom-of-extensionality).** Build well-founded coded [sets](../../../set.md) over one [urelement](../../../set-theory.md#urelement) $a$, retaining a distinct ordinary [empty set](../../../set.md#empty-set) $e$. Membership of an atom is always false, and membership of a [set](../../../set.md) code is its coded extension. Thus $a\ne e$ but they have identical empty extensions. [Pairing](../../../set-theory.md#axiom-of-pairing), [union](../../../set.md#set-union), [separation](../../../set-theory.md#axiom-schema-of-specification) and [replacement](../../../set-theory.md#axiom-schema-of-replacement) are performed on [set](../../../set.md) codes; pure $\omega$ witnesses [infinity](../../../mathematics.md#infinity), and the well-founded construction gives [foundation](../../../set-theory.md#axiom-of-regularity). There is a small point concerning the unmodified, untyped [Axiom of power set](../../../set-theory.md#axiom-of-power-set): the atom is vacuously a [subset](../../../set.md#subset) of every object. Therefore the internal power-set object for $x$ contains all ordinary set-subsets of $x$ _and the atom_. It has exactly the required extension. **All remaining ZF [axioms](../../../mathematical-logic.md#axiom) hold, but [extensionality](../../../set-theory.md#axiom-of-extensionality) fails.** In the usual typed atom theory, the power-set [axiom](../../../mathematical-logic.md#axiom) instead quantifies only over set-subsets.

**[Foundation](../../../set-theory.md#axiom-of-regularity).** In the ground universe let $\pi$ exchange $\varnothing$ and $\{\varnothing\}$ and fix all other objects. On the same domain define the [Rieger-Bernays permutation model](../../../set-theory.md#rieger-bernays-permutation-model)

$$
x\mathrel E y\quad\Longleftrightarrow\quad x\in\pi(y).
$$

Since $\pi$ is a [bijection](../../../function.md#bijection), two objects with the same $E$-members are equal, so [extensionality](../../../set-theory.md#axiom-of-extensionality) holds. Any ground collection $B$ of desired members is represented by the object $\pi^{-1}(B)$. In particular, an $E$-pair is $\pi^{-1}(\{a,b\})$ and the $E$-union of $a$ is

$$
\pi^{-1}\left(\bigcup_{b\in\pi(a)}\pi(b)\right).
$$

An $E$-subset of $a$ is an object $z$ with $\pi(z)\subseteq\pi(a)$, so its $E$-power-set object is

$$
\pi^{-1}\bigl(\{\pi^{-1}(u):u\subseteq\pi(a)\}\bigr).
$$

Translate every formula by replacing membership with $E$; ground [separation](../../../set-theory.md#axiom-schema-of-specification) and [replacement](../../../set-theory.md#axiom-schema-of-replacement) collect the required extensions and the same representation supplies their internal witnesses. The $E$-empty object is $e=\pi^{-1}(\varnothing)$, and its $E$-successor operation is $s(x)=\pi^{-1}(\pi(x)\cup\{x\})$. Ground [well-founded recursion](../../../set-theory.md#well-founded-recursion) and [replacement](../../../set-theory.md#axiom-schema-of-replacement) collect the iterates of $s$ from $e$; representing this collection gives an $E$-inductive object. Thus [infinity](../../../mathematics.md#infinity) holds. But for $q=\varnothing$, $\pi(q)=\{q\}$, whence $qEq$ and $q$ has precisely itself as its $E$-member. **[Foundation](../../../set-theory.md#axiom-of-regularity) fails.**

**[Infinity](../../../mathematics.md#infinity).** The [hereditarily finite sets](../../../set-theory.md#hereditarily-finite-set) $V_\omega$ satisfy [extensionality](../../../set-theory.md#axiom-of-extensionality), [foundation](../../../set-theory.md#axiom-of-regularity), [pairing](../../../set-theory.md#axiom-of-pairing), [union](../../../set.md#set-union), [power set](../../../set.md#power-set) and [separation](../../../set-theory.md#axiom-schema-of-specification). Each internal domain is externally finite, so every internally definable functional image is finite and belongs to $V_\omega$, proving [replacement](../../../set-theory.md#axiom-schema-of-replacement). No finite object can contain the [empty set](../../../set.md#empty-set) and all its successive [Finite von Neumann ordinals](../../../set-theory.md#finite-von-neumann-ordinal). **[Infinity](../../../mathematics.md#infinity) fails, and all other ZF [axioms](../../../mathematical-logic.md#axiom) hold.**

**[Choice](../../../set-theory.md#axiom-of-choice) with atoms.** For the negative model use the [Basic Fraenkel permutation model](../../../set-theory.md#basic-fraenkel-permutation-model). Let $A$ be an infinite [set](../../../set.md) of [urelements](../../../set-theory.md#urelement) and let every [permutation](../../../combinatorics.md#permutation) of $A$ act recursively on [sets](../../../set.md). Keep precisely the hereditarily finitely supported objects: an object has a [finite support](../../../group-theory.md#finite-support-in-a-permutation-action) $F\subseteq A$ if every [permutation](../../../combinatorics.md#permutation) fixing $F$ pointwise fixes the object, and every object occurring in its membership ancestry must also have such a support. The class of these objects contains the pure universe and $A$ itself.

Supports for a [pair](../../../set.md#pair) are united; [union](../../../set.md#set-union) preserves a support; a formula defining a [subset](../../../set.md#subset) uses the finite [union](../../../set.md#set-union) of the supports of its domain and parameters. An internally definable functional range has the same support, since its values are uniquely specified, and its elements are already hereditarily supported. This proves the full [separation](../../../set-theory.md#axiom-schema-of-specification) and [replacement](../../../set-theory.md#axiom-schema-of-replacement) schemas. All hereditarily supported set-subsets of a fixed [set](../../../set.md) form its symmetric internal [power set](../../../set.md#power-set); this collection is invariant under the pointwise stabilizer of a support of the original [set](../../../set.md). For the untyped version add all the atoms, as above. Pure $\omega$, ground well-foundedness and set-extensionality give the remaining [axioms](../../../mathematical-logic.md#axiom).

The family $[A]^2$ of [unordered pairs](../../../set.md#unordered-pair) of atoms is hereditarily supported. If it had a [choice function](../../../set-theory.md#choice-function) $f$, let $F$ be a finite support of $f$. Choose distinct $a,b\in A\setminus F$. The [transposition](../../../combinatorics.md#transposition-permutation) exchanging $a,b$ fixes $F$ and $\{a,b\}$, but exchanges its two possible chosen elements. Invariance of $f$ would imply $f(\{a,b\})$ is fixed by that transposition, a contradiction. Conversely, the full well-founded universe over the atoms, before restricting to finite supports, satisfies [choice](../../../set-theory.md#axiom-of-choice) when the ground universe does. **Both [choice](../../../set-theory.md#axiom-of-choice) and its negation are relatively consistent with the stated weakening of [extensionality](../../../set-theory.md#axiom-of-extensionality).**

## 2

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [partition relation](../../../set-theory.md#partition-relation) $\lambda\to(\mu)^r_\nu$ says that every [colouring](../../../set.md#colouring-of-a-set) of the $r$-element [subsets](../../../set.md#subset) of a [set](../../../set.md) of [cardinality](../../../set-theory.md#cardinality) $\lambda$ into $\nu$ colours has a [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) of [cardinality](../../../set-theory.md#cardinality) $\mu$. Define the [beth numbers](../../../set-theory.md#beth-number) over an infinite [cardinal](../../../set-theory.md#cardinal-number) $\kappa$ by $\beth_0(\kappa)=\kappa$ and $\beth_{n+1}(\kappa)=2^{\beth_n(\kappa)}$. The [Erdős-Rado theorem for finite arities](../../../set-theory.md#erdos-rado-theorem-for-finite-arities) gives the precise bound

$$
\boxed{\beth_n(\kappa)^+\longrightarrow(\kappa^+)^{n+1}_\kappa\qquad(n<\omega).}
$$

Thus any fixed finite arity and any fixed infinite number of colours admit arbitrarily large infinite [monochromatic sets](../../../ramsey-theory.md#monochromatic-set) once the starting [cardinal](../../../set-theory.md#cardinal-number) is sufficiently large. For pairs, the especially useful case is $(2^\kappa)^+\to(\kappa^+)^2_\kappa$. The successor in this bound matters: a binary first-difference colouring on a suitably ordered [set](../../../set.md) of binary [sequences](../../../real-analysis.md#sequence) supplies the familiar obstruction at $2^\kappa$. Also, a theorem for every fixed finite arity is not a theorem homogenizing all arities simultaneously.

The mechanism is to build an [end-homogeneous routing tree](../../../set-theory.md#end-homogeneous-routing-tree): each new vertex is routed according to its colours to earlier vertices on its branch. A long branch is end-homogeneous, meaning the colour from a fixed earlier vertex is independent of the later vertex. There are at most $\kappa^\alpha\leq2^\kappa$ routes of length $\alpha<\kappa^+$, and the whole collection of short routes has size at most $2^\kappa$. Inserting $(2^\kappa)^+$ vertices therefore forces a branch of length $\kappa^+$. One colour occurs at $\kappa^+$ earlier vertices on that branch, giving the pair theorem. Iterating the higher-arity version of this routing construction explains the successive powers in the [Erdős-Rado theorem for finite arities](../../../set-theory.md#erdos-rado-theorem-for-finite-arities).

A [weakly compact cardinal](../../../set-theory.md#weakly-compact-cardinal) is an uncountable [strongly inaccessible cardinal](../../../set-theory.md#strongly-inaccessible-cardinal) $\kappa$ with

$$
\kappa\longrightarrow(\kappa)^2_2.
$$

Equivalent formulations include the [tree property](../../../set.md#tree-property) at the inaccessible [cardinal](../../../set-theory.md#cardinal-number) and compactness for theories of size at most $\kappa$ in the infinitary language $L_{\kappa,\kappa}$: if every subtheory of size $<\kappa$ has a [first-order model](../../../mathematical-logic.md#model-of-a-first-order-theory), so does the theory.

A [measurable cardinal](../../../set-theory.md#measurable-cardinal) is an uncountable $\kappa$ carrying a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) [closed](../../../topology.md#closed-set) under intersections of fewer than $\kappa$ members. Such an [ultrafilter](../../../set-theory.md#ultrafilter) contains no [set](../../../set.md) of size $<\kappa$, since all singletons have complements in it and it is [kappa-complete](../../../set-theory.md#kappa-complete-filter). Consequently a cofinal [sequence](../../../real-analysis.md#sequence) of length $<\kappa$ would partition $\kappa$ into too few small pieces, so $\kappa$ is [regular cardinal](../../../set-theory.md#regular-cardinal). If $\lambda<\kappa$ and $\kappa$ distinct [subsets](../../../set.md#subset) of $\lambda$ existed, choose, for each coordinate of $\lambda$, the bit selected by the [ultrafilter](../../../set-theory.md#ultrafilter). [Kappa-completeness](../../../set-theory.md#kappa-complete-filter) would make all those bits simultaneously constant on a large [set](../../../set.md) of indices; only one distinct [subset](../../../set.md#subset) could have that bit pattern, a contradiction. Hence $2^\lambda<\kappa$: $\kappa$ is also a [strong limit cardinal](../../../set-theory.md#strong-limit-cardinal).

A [supercompact cardinal](../../../set-theory.md#supercompact-cardinal) $\kappa$ has, for every $\lambda\geq\kappa$, a [fine ultrafilter](../../../set-theory.md#fine-ultrafilter) that is a [normal ultrafilter on small subsets](../../../set-theory.md#normal-ultrafilter-on-small-subsets) and is [kappa-complete](../../../set-theory.md#kappa-complete-filter) on

$$
P_\kappa(\lambda)=\{x\subseteq\lambda:|x|<\kappa\}.
$$

Fine means $\{x:\alpha\in x\}$ is large for every $\alpha<\lambda$. Normal means that a [function](../../../function.md) $f$ with $f(x)\in x$ on a large [set](../../../set.md) is constant on some large [set](../../../set.md). Equivalently, for every such $\lambda$ there is an [elementary embedding](../../../set-theory.md#elementary-embedding) $j:V\to M$ with [critical point](../../../analysis.md#critical-point) $\kappa$, $j(\kappa)>\lambda$, and $M$ [closed](../../../topology.md#closed-set) under $\lambda$-sequences from the universe.

These notions form the implication chain **supercompact $\Rightarrow$ measurable $\Rightarrow$ weakly compact**. For the first implication, an embedding as above gives the measure $U=\{X\subseteq\kappa:\kappa\in j(X)\}$. For the second, use a [normal ultrafilter on a cardinal](../../../set-theory.md#normal-ultrafilter-on-a-cardinal) obtained by normalizing its measure. Indeed the [ultrapower embedding](../../../set-theory.md#ultrapower-embedding) gives the measure $U=\{X\subseteq\kappa:\kappa\in j(X)\}$; for a regressive $f$, $j(f)(\kappa)<\kappa$ is a fixed [ordinal](../../../set-theory.md#ordinal), yielding the required constant large fibre. Given a pair-colouring, select for each $\alpha$ the measure-one colour on the tail above $\alpha$. One selected colour occurs on a measure-one [set](../../../set.md) of $\alpha$'s. Normality makes the diagonal intersection of their selected tails measure one; any two members of that intersection have the selected colour. This gives the required [partition relation](../../../set-theory.md#partition-relation), and the preceding regularity and strong-limit argument gives inaccessibility.

## 3

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

[Forcing](../../../forcing.md) constructs new [first-order models](../../../mathematical-logic.md#model-of-a-first-order-theory) while controlling which ground-model properties survive. Fix a ground model $M$ and a [partially ordered set](../../../set.md#partially-ordered-set) $P\in M$, writing $q\leq p$ when $q$ is the stronger condition. A [generic filter](../../../forcing.md#generic-filter) is upward [closed](../../../topology.md#closed-set), directed towards stronger conditions, and meets every ground-model [dense subset of a forcing order](../../../forcing.md#dense-subset-of-a-forcing-order). If $M$ is externally a [countable transitive model](../../../forcing.md#countable-transitive-model), enumerate its dense [subsets](../../../set.md#subset) and successively choose stronger conditions in them. The resulting filter is $M$-generic. External countability is crucial: this is not a claim that the ground model regards its own universe as [countable](../../../set-theory.md#countable-set).

A [forcing name](../../../forcing.md#forcing-name) is built recursively from pairs $(\sigma,p)$ of earlier names and conditions. For a generic filter $G$, its [evaluation of a forcing name](../../../forcing.md#evaluation-of-a-forcing-name) is

$$
\tau_G=\{\sigma_G:(\sigma,p)\in\tau,\ p\in G\},\qquad
M[G]=\{\tau_G:\tau\in M\}.
$$

The [canonical forcing name](../../../forcing.md#canonical-forcing-name) $\check x=\{(\check y,1):y\in x\}$ evaluates to $x$, so $M\subseteq M[G]$. Recursive evaluation also proves transitivity. Name ranks bound the ranks of their evaluations, so an [ordinal](../../../set-theory.md#ordinal) in the extension is below some ground [ordinal](../../../set-theory.md#ordinal) and is already a ground [ordinal](../../../set-theory.md#ordinal). Thus [forcing preserves ordinals](../../../forcing.md#forcing-preserves-ordinals).

The central link between syntax and generic interpretation is the [forcing theorem](../../../forcing.md#forcing-theorem). The relation $p\Vdash\varphi(\tau_1,\ldots,\tau_n)$ is definable in the ground model, and the [forcing truth lemma](../../../forcing.md#forcing-truth-lemma) says

$$
M[G]\models\varphi((\tau_1)_G,\ldots,(\tau_n)_G)
\quad\Longleftrightarrow\quad
(\exists p\in G)\ p\Vdash\varphi(\tau_1,\ldots,\tau_n).
$$

For an atomic membership assertion, densely many refinements must witness equality with a member-name whose associated condition is compatible with the refinement. Equality is obtained by recursive mutual inclusion of names. For [negation](../../../computer-science.md#negation), $p\Vdash\neg\varphi$ means no stronger condition forces $\varphi$; for an [existential quantification](../../../mathematical-logic.md#existential-quantification), witnesses must be obtainable densely below $p$. Induction on name rank establishes the atomic clauses, and induction on formulas establishes definability and the truth lemma. The generic filter meets the relevant dense [sets](../../../set.md) at the existential step. An arbitrary semantic assertion about one chosen generic filter is insufficient: the definable relation must work uniformly for all generic interpretations.

This explains preservation of [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). [Extensionality](../../../set-theory.md#axiom-of-extensionality) and [foundation](../../../set-theory.md#axiom-of-regularity) follow from transitivity; canonical names supply [infinity](../../../mathematics.md#infinity). Pair and [union](../../../set.md#set-union) names give [pairing](../../../set-theory.md#axiom-of-pairing) and [union](../../../set.md#set-union). For [separation](../../../set-theory.md#axiom-schema-of-specification), restrict a name's members to conditions [forcing](../../../forcing.md) the defining formula. For [replacement](../../../set-theory.md#axiom-schema-of-replacement), the definable [forcing](../../../forcing.md) relation lets ground [axiom schema of collection](../../../set-theory.md#axiom-schema-of-collection) bound a [set](../../../set.md) of names for all possible witnesses to the unique outputs; evaluating their collected name gives the range. For [power set](../../../set.md#power-set), let $\tau$ name the given [set](../../../set.md) and let $D$ be the [set](../../../set.md) of its member-names. Every [subset](../../../set.md#subset) of $\tau_G$ has an equivalent name drawn from $\mathcal P(D\times P)$, by the truth lemma, so a ground [set](../../../set.md) of candidate names collects all its [subsets](../../../set.md#subset). Finally choose a ground [well-order](../../../set.md#well-order) of the relevant names; its evaluated image surjects onto the desired [set](../../../set.md), and choosing the first name for each value well-orders that [set](../../../set.md). This is why ordinary [forcing](../../../forcing.md) over a [choice](../../../set-theory.md#axiom-of-choice) model preserves [choice](../../../set-theory.md#axiom-of-choice).

For a concrete example, [Cohen forcing](../../../forcing.md#cohen-forcing) consists of finite partial [functions](../../../function.md) $\omega\to2$, ordered by extension. The generic [union](../../../set.md#set-union) $c=\bigcup G$ is total because deciding each coordinate is dense. For every ground real $x$, the [set](../../../set.md) of conditions disagreeing with $x$ somewhere is dense, so $c\ne x$. This construction changes the universe by adding a genuinely new real without changing its [ordinals](../../../set-theory.md#ordinal).

The size and compatibility of conditions determine what else changes. With the [countable chain condition for forcing](../../../forcing.md#countable-chain-condition-for-forcing), an ordinal-valued name has only countably many possible values at each coordinate: take a maximal antichain deciding that value. Therefore the possible range of a name for a map with infinite ground domain of [cardinality](../../../set-theory.md#cardinality) $\mu$ lies in a ground [set](../../../set.md) of size at most $\mu\cdot\aleph_0=\mu$. This prevents [cardinal](../../../set-theory.md#cardinal-number) collapse and changes of uncountable regular [cofinalities](../../../set-theory.md#cofinality). [Forcing](../../../forcing.md) by finite partial [functions](../../../function.md) $\lambda\times\omega\to2$ is ccc: the [delta-system lemma](../../../set-theory.md#delta-system-lemma) thins any uncountable family of finite domains to a delta-system, and a further thinning makes their values agree on its finite root. Two remaining conditions are compatible. Distinct coordinates add distinct reals.

For example, start with [GCH](../../../set-theory.md#generalized-continuum-hypothesis) and take $\lambda=\aleph_2$. This [forcing](../../../forcing.md) has size $\lambda$ and adds $\lambda$ distinct reals. A [nice name for a real](../../../forcing.md#nice-name-for-a-real) uses countably many antichains, and each antichain is [countable](../../../set-theory.md#countable-set). The ground arithmetic $\lambda^{\aleph_0}=\lambda$ bounds the number of such names by $\lambda$. Hence

$$
\boxed{M[G]\models 2^{\aleph_0}=\aleph_2,}
$$

giving a relative-consistency example of the failure of [CH](../../../set-theory.md#continuum-hypothesis). The ground [choice](../../../set-theory.md#axiom-of-choice) of GCH is available through the [constructible universe](../../../definable-power-set.md#constructible-universe); no claim that every starting model has this arithmetic is needed.

By contrast, [countably closed forcing](../../../forcing.md#countably-closed-forcing) adds no new [countable](../../../set-theory.md#countable-set) [sequences](../../../real-analysis.md#sequence) of ground [ordinals](../../../set-theory.md#ordinal). Given a name, recursively strengthen a condition to decide each coordinate, then take a lower bound of the descending [sequence](../../../real-analysis.md#sequence). That condition decides the entire [sequence](../../../real-analysis.md#sequence). Closure and chain conditions thus control different features; neither should be silently substituted for the other.

Further applications include changing [cofinalities](../../../set-theory.md#cofinality), adding branches through trees, and constructing prescribed continuum patterns. If the aim is to violate [choice](../../../set-theory.md#axiom-of-choice), an ordinary generic extension of a [choice](../../../set-theory.md#axiom-of-choice) model will not do: one restricts to a suitable symmetric collection of names, checking the [axioms](../../../mathematical-logic.md#axiom) again. These examples also mark a limitation: [forcing](../../../forcing.md) proves relative consistency, not absolute consistency of the background theory. The countable-transitive-model picture gives a concrete semantic construction; the definable [forcing](../../../forcing.md) relation and Boolean-valued formulation supply the corresponding formal consistency arguments without asserting that a transitive ground model can be proved to exist.

## 4

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use the [rooted-tree homeomorphic embedding](../../../combinatorics.md#homeomorphic-embedding-of-a-rooted-tree) relation: an injective map of vertices preserves [lowest common ancestors](../../../combinatorics.md#lowest-common-ancestor), so edges may become paths and the source root may map below the target root. We prove the stronger labelled statement for labels in any [well-quasi-ordering](../../../set.md#well-quasi-ordering) $Q$, with labels increasing under the embedding. Forgetting labels gives [Kruskal's tree theorem](../../../set.md#kruskal-s-tree-theorem).

First every infinite [sequence](../../../real-analysis.md#sequence) in a [well-quasi-ordering](../../../set.md#well-quasi-ordering) has an infinite nondecreasing [subsequence](../../../real-analysis.md#subsequence). Colour its index pairs according as the earlier term is or is not below the later term. [Ramsey's theorem](../../../ramsey-theory.md#ramsey-s-theorem) gives an infinite constant-colour [subsequence](../../../real-analysis.md#subsequence); the bad colour would contradict [well-quasi-ordering](../../../set.md#well-quasi-ordering). Applying this successively in each coordinate proves [finite product closure of well-quasi-orderings](../../../set.md#finite-product-closure-of-well-quasi-orderings).

We need [Higman lemma](../../../set.md#higman-s-lemma) with its proof. Order finite [words](../../../foundations-of-mathematics.md#string) over $Q$ by [subsequence](../../../real-analysis.md#subsequence) embedding with increased letters. If there were a [bad sequence](../../../set.md#bad-sequence), choose one $w_0,w_1,\ldots$ minimally: at each position choose a shortest word admitting a bad continuation of the fixed prefix. No word is empty. Write $w_n=u_na_n$, separating the last letter, and choose $n_0<n_1<\cdots$ with $a_{n_0}\leq a_{n_1}\leq\cdots$. Consider

$$
w_0,\ldots,w_{n_0-1},u_{n_0},u_{n_1},\ldots.
$$

An earlier prefix word cannot embed in a later $u_{n_j}$, since it would then embed in $w_{n_j}$. Nor can $u_{n_i}$ embed in $u_{n_j}$: adding the comparable last letters would embed $w_{n_i}$ in $w_{n_j}$. Thus the displayed [sequence](../../../real-analysis.md#sequence) is bad, contradicting minimality at $n_0$, since $u_{n_0}$ is shorter. **Finite words over a well-quasi-order are [well-quasi-ordered](../../../set.md#well-quasi-ordering).**

Now suppose labelled [rooted trees](../../../combinatorics.md#rooted-tree) admit a bad [sequence](../../../real-analysis.md#sequence) $T_0,T_1,\ldots$, chosen minimally in vertex count at each position. Let $\mathcal A$ consist of all proper rooted subtrees of these trees, rooted at a descendant and containing all its descendants. We claim $\mathcal A$ is [well-quasi-ordered](../../../set.md#well-quasi-ordering). Otherwise take a bad [sequence](../../../real-analysis.md#sequence) $S_0,S_1,\ldots$ from $\mathcal A$. Only finitely many subtrees come from any fixed finite prefix of the $T_n$'s, and a bad [sequence](../../../real-analysis.md#sequence) cannot repeat an object. Thin it so that $S_i$ comes from $T_{m_i}$ with $m_0<m_1<\cdots$. The [sequence](../../../real-analysis.md#sequence)

$$
T_0,\ldots,T_{m_0-1},S_0,S_1,\ldots
$$

is bad: $T_j\preceq S_i$ would imply $T_j\preceq T_{m_i}$, since a rooted subtree embeds in its host; comparisons within the $S_i$'s are excluded by their [choice](../../../set-theory.md#axiom-of-choice). But $S_0$ is strictly smaller than $T_{m_0}$, contradicting minimality. This proves the claim.

Choose an arbitrary ordering of the children of each $T_n$. Record its root label and the finite word of rooted child-subtrees:

$$
\left(\ell_n,\ (T_{n,1},\ldots,T_{n,r_n})\right)\in Q\times\mathcal A^*.
$$

By [Higman lemma](../../../set.md#higman-s-lemma) and finite product closure, two records, with indices $i<j$, are comparable. Map the root of $T_i$ to the root of $T_j$, and map its selected child-subtrees into the distinct selected branches of $T_j$. Within a branch the embeddings preserve lowest common ancestors; between different branches both lowest common ancestors are the roots. Labels increase everywhere. This gives $T_i\preceq_Q T_j$, contradicting badness. **Finite labelled [rooted trees](../../../combinatorics.md#rooted-tree) are [well-quasi-ordered](../../../set.md#well-quasi-ordering) by label-monotone homeomorphic embedding.** In particular, this proves the unlabelled theorem. A root-preserving variant follows by giving the root a special incomparable label unavailable at nonroot vertices; the general labelled theorem then forces root to root. Adjacency-preserving embeddings are a different, more restrictive relation and do not satisfy the same assertion.

For [Friedman's finite form of Kruskal's theorem](../../../set.md#friedman-s-finite-form-of-kruskal-s-theorem), fix $k\in\mathbb N$ and consider finite bad [sequences](../../../real-analysis.md#sequence) satisfying $|T_i|\leq k+i$, with indices starting at $1$. Their prefixes form a [finite bad-sequence tree](../../../set.md#finite-bad-sequence-tree). At each depth there are only finitely many possible unlabelled tree isomorphism types below the size bound, so this tree is finitely branching. If bad [sequences](../../../real-analysis.md#sequence) existed at every finite length, [König infinity lemma](../../../combinatorics.md#konig-s-lemma) would yield an infinite branch, hence an infinite bad [sequence](../../../real-analysis.md#sequence) of [rooted trees](../../../combinatorics.md#rooted-tree), contrary to what was just proved. Therefore

$$
\boxed{\forall k\ \exists N\ \forall(T_1,\ldots,T_N)\
\left[(\forall i\leq N)\ |T_i|\leq k+i\ \Longrightarrow\
(\exists i<j\leq N)\ T_i\preceq T_j\right].}
$$

The same proof works with any fixed finite label [set](../../../set.md). The finite size bounds are what make the bad-prefix tree finitely branching; the proof does not claim a small effective numerical bound.

## 5

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Work in [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). The move alphabet need not be [countable](../../../set-theory.md#countable-set); [choice](../../../set-theory.md#axiom-of-choice) permits the selections of moves, strategies and witnesses used below. Assume $A\ne\varnothing$; with the usual convention that a player unable to move loses, the empty alphabet is a trivial terminal game. We prove [Borel determinacy theorem](../../../descriptive-set-theory.md#borel-determinacy-theorem) by strengthening the assertion to the existence of [game coverings](../../../descriptive-set-theory.md#covering-of-an-infinite-game) that unravel payoffs. Simply asserting that determined payoffs are [closed](../../../topology.md#closed-set) under [countable](../../../set-theory.md#countable-set) unions would not be a proof.

It is useful to allow a tree of legal finite plays with terminal nodes explicitly labelled as losses for either player. For an infinite branch, I wins exactly when it belongs to the payoff $C$. Projection of a game tree is length-preserving and respects prefixes. At a projected original terminal node the outcome is inherited, but the new tree may also have artificial terminal losses.

A [covering of an infinite game](../../../descriptive-set-theory.md#covering-of-an-infinite-game) has such a projection $\pi:S\to T$ and maps $\Phi$ taking a [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) on $S$ to a [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) of the same player on $T$. Its crucial lifting condition is this: each maximal play $x$ on $T$ following $\Phi(\sigma)$ has a $\sigma$-compatible lift $y$ on $S$, either projecting exactly to $x$ with its inherited terminal outcome, or projecting to a prefix of $x$ and ending in a loss for the player using $\sigma$. Its [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) maps must be local in depth: choices up to a given depth use only the upstairs [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) up to that depth. A $k$-covering preserves the initial $k$ levels and choices. If $\pi^{-1}(C)$ is [clopen](../../../topology.md#clopen-set), call it an [unravelling of a game payoff](../../../descriptive-set-theory.md#unravelling-of-a-game-payoff). A winning upstairs [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) cannot have a compatible premature losing lift; hence any such covering transfers winning strategies downstairs, for the payoff pulled back by $\pi$.

First, [clopen determinacy with terminal losses](../../../descriptive-set-theory.md#clopen-determinacy-with-terminal-losses) holds on any set-sized tree. At a node where all infinite extensions have one fixed winner, the other player can win only by [forcing](../../../forcing.md) a terminal loss for that winner. Decide that reachability game by the [winning-position attractor in an infinite game](../../../descriptive-set-theory.md#winning-position-attractor-in-an-infinite-game): begin with the desired losing terminals, add the attacking player's positions with a successor already in the attractor and the defending player's positions with every successor in it, and take unions at limit stages. Entry ranks give a [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) reaching the target; outside the attractor the defender avoids it. If there are no infinite extensions the same reachability analysis still applies. At every remaining position there are infinite extensions in both $C$ and its complement. This remaining tree is [well-founded](../../../set-theory.md#well-founded-relation), since an infinite branch through it would contradict clopenness at that branch. [Well-founded recursion](../../../set-theory.md#well-founded-recursion) now assigns a winner upwards from the already decided nodes, choosing a winning successor when the player to move has one. These choices give an actual winning [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game).

Next we construct an [announcement-and-challenge covering of a closed payoff](../../../descriptive-set-theory.md#announcement-and-challenge-covering-of-a-closed-payoff). Let $C\subseteq[T]$ be [closed](../../../topology.md#closed-set), and choose an even depth $l>k$. Play initially follows $T$ unchanged. At a nonterminal position $p$ of length $l$, replace I's next move $a$ by $(a,X)$, where $X$ is any [subset](../../../set.md#subset) of the following [set](../../../set.md) $Z_{p,a}$ of exit positions: $r$ strictly extends $pa$, is nonterminal, and is a shortest such extension along its branch satisfying $[T_r]\cap C=\varnothing$. If $[T_{pa}]\cap C=\varnothing$ already, the first nonterminal extension beyond $pa$ counts as an exit. Distinct exits form a prefix antichain. An original terminal move always keeps its original outcome.

Player II now either accepts and makes an ordinary next move $b$, or challenges an $r\in X$ and makes the move $b$ prescribed by that $r$. On acceptance, continue the original play until the first exit $r$: it is an artificial win for I if $r\in X$, and an artificial loss for I otherwise. On a challenge, both players are forced to follow $r$ until it is reached, after which the original game resumes without the acceptance stopping rule. The projection forgets the announcements and challenge flags.

An infinite accepted play avoids all exits. Every sufficiently long prefix of its projection therefore has a continuation in $C$, so closedness implies that the projection is in $C$. Every infinite challenged play passes through an exit cylinder disjoint from $C$. Thus among infinite plays the pulled-back payoff is decided by II's acceptance or challenge: it is [clopen](../../../topology.md#clopen-set). This remains true when a particular branch reaches an inherited terminal position before either case produces an infinite play.

Here is the strategy-transfer proof, which also fixes the artificial terminal labels. Given an I-strategy $\sigma$ upstairs, use its announced ordinary move $a$ downstairs and initially simulate an accepting response. If the projected play never exits, this is an exact lift. If its first exit $r$ is not in the announced $X$, the accepting lift ends in a loss for I, as allowed. If $r\in X$, switch to the simulation in which II challenged this particular $r$. The earlier ordinary prefix is unchanged: all moves through $r$ in the challenged simulation are forced and agree with the observed prefix. Beyond $r$ follow $\sigma$ in that simulation. This gives an exact compatible lift. Original terminal outcomes are inherited throughout.

For an II-strategy $\tau$ upstairs, after seeing $pa$ downstairs, let

$$
Y=\{r\in Z_{p,a}:\text{no announcement }X
\text{ makes }\tau\text{ challenge }r\}.
$$

For the announcement $X=Y$, the [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) $\tau$ must accept, since a challenge would have to name an element of $Y$. Use its accepting ordinary response downstairs and simulate that acceptance until an exit. If the exit $r$ belongs to $Y$, the accepting lift is an artificial loss for II, as required. If $r\notin Y$, choose an announcement $X_r$ for which $\tau$ challenges $r$, and switch to that simulation. Its first ordinary response and all the intervening forced moves agree with the actual prefix $r$; after $r$ use $\tau$ there. This gives an exact lift. Choices of $X_r$ use [choice](../../../set-theory.md#axiom-of-choice). No switch uses unseen future moves, and the definition of $Y$ uses only the [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game)'s responses at the fixed announcement level. Thus the maps are local in depth. The unchanged initial segment makes this a $k$-covering.

We now establish the stronger assertion: **every Borel payoff on every such game tree admits a $k$-unravelling for every finite $k$**. [Closed](../../../topology.md#closed-set) payoffs were just handled. Complements need no new construction, since the complement of a [clopen](../../../topology.md#clopen-set) pulled-back payoff is [clopen](../../../topology.md#clopen-set).

For [countable](../../../set-theory.md#countable-set) unions, suppose $C=\bigcup_{n<\omega}C_n$ and the stronger assertion is known for each constituent and for its continuous pullbacks. Starting with $T_0=T$, choose a covering $T_{n+1}\to T_n$ that unravels the current pullback of $C_n$ and preserves at least the first $k+n$ levels and choices. Previously unravelled payoffs remain [clopen](../../../topology.md#clopen-set) under further continuous projections. There is a [depth-stabilizing inverse limit of game coverings](../../../descriptive-set-theory.md#depth-stabilizing-inverse-limit-of-game-coverings): each finite level eventually ceases to change, and these stable levels form a tree $T_\infty$.

For completeness, the limit retains the covering property, not just the topology. Compose the projections and the depth-local [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) maps; their finite restrictions stabilize. To lift a play following the limit-projected [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game), lift it successively, coherently, from $T_n$ to $T_{n+1}$. If all lifts are exact, the stabilized finite prefixes give a compatible play on $T_\infty$. If a premature losing terminal lift occurs, every further lift is either exact or another losing terminal prefix, so its length cannot increase; lengths and then its finite position stabilize. This produces the permitted losing terminal lift in the limit. The choices needed to select successive lifts are available in [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). Projections, inherited terminal outcomes and depth-local [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) maps consequently make $T_\infty\to T$ a genuine $k$-covering.

On $T_\infty$, the pullbacks of all the $C_n$ are [clopen](../../../topology.md#clopen-set), so their [union](../../../set.md#set-union) is [open](../../../topology.md#open-set). Its complement is [closed](../../../topology.md#closed-set). Apply the closed-payoff construction once more to unravel this complement; it unravels the [union](../../../set.md#set-union) too. Composition gives the desired covering of $T$. This proves the induction step. Induction on a well-founded construction of a [Borel set](../../../measure-theory.md#borel-set), whose operations are complementation and [countable](../../../set-theory.md#countable-set) [union](../../../set.md#set-union) starting from [open](../../../topology.md#open-set) [sets](../../../set.md), proves the assertion for every Borel payoff. Continuous preimages of a constituent have the same type of construction, so the induction hypothesis used at successive covers is justified. No countability of the move alphabet was used; all enlarged alphabets and trees remain [sets](../../../set.md).

Finally apply this result to $T=A^{<\omega}$. The unravelled [clopen](../../../topology.md#clopen-set) game has a winning [strategy](../../../descriptive-set-theory.md#strategy-in-an-infinite-game) by the first argument. The covering lifting condition transfers it to the original game. Therefore

$$
\boxed{\text{for every Borel }C\subseteq A^\omega,
\text{ one player has a winning strategy in }G(C).}
$$

This is a theorem in the usual background [set](../../../set.md) theory with [choice](../../../set-theory.md#axiom-of-choice); it does not assert unrestricted determinacy for arbitrary, non-Borel payoffs.

## 6

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Identify the [space of infinite subsets of the natural numbers](../../../ramsey-theory.md#space-of-infinite-subsets-of-the-natural-numbers) with their increasing enumerations, with the [ordinary topology on infinite subsets](../../../ramsey-theory.md#ordinary-topology-on-infinite-subsets) inherited from the discrete product $\omega^\omega$. This is the [sequence](../../../real-analysis.md#sequence) convention in the [Open Ramsey theorem](../../../ramsey-theory.md#open-ramsey-theorem). For a general infinite ground [set](../../../set.md), first choose a countably infinite [subset](../../../set.md#subset) and use its enumeration. The theorem cannot mean unrestricted [sequences](../../../real-analysis.md#sequence) with repetitions: the [clopen](../../../topology.md#clopen-set) partition according as the first two entries agree or differ has both colours over every infinite ground [set](../../../set.md).

For a finite [finite stem](../../../ramsey-theory.md#finite-stem-of-an-infinite-subset) $s$ and an infinite tail $B$ above $\max s$, write

$$
[s,B]=\{s\cup X:X\in[B]^\omega\},
$$

where the enumeration of $s$ precedes the tail. Let $O$ be [open](../../../topology.md#open-set). The tail $B$ accepts $s$ if $[s,B]\subseteq O$; it rejects $s$ if no infinite subtail accepts it. Both properties persist on infinite subtails, and any stem can be decided by thinning: choose an accepting subtail if one exists; otherwise the current tail already rejects it.

Use [deciding all finite stems by fusion](../../../ramsey-theory.md#deciding-all-finite-stems-by-fusion). At stage $n$, choose a new element $b_n$ from the current tail, then thin the remaining tail to decide each of the finitely many [subsets](../../../set.md#subset) of $\{b_0,\ldots,b_n\}$. First decide the empty stem as well. The final selected [set](../../../set.md) $B$ decides every finite stem from $B$, because all subsequent selections lie in the tail that decided that stem. If $B$ accepts the empty stem, $[B]^\omega\subseteq O$ and we are done.

Otherwise the empty stem is rejected. If a stem $s\subset B$ is rejected, only finitely many $a\in B$ above $\max s$ can have the tail $B/a$ accepting $s\cup\{a\}$. Indeed, if infinitely many such $a$ formed $D$, then every $X\in[D]^\omega$ starts with one of them and has its remaining tail in $B/a$. It follows that $[s,D]\subseteq O$, contradicting rejection of $s$. All other one-point extensions are rejected, since the first fusion has already decided them.

Build an infinite $C\subseteq B$ recursively. Maintain that every [subset](../../../set.md#subset) of the finite selected prefix is rejected. To select its next element, avoid the finite [union](../../../set.md#set-union) of the finitely many accepting-extension obstructions for these rejected stems. Such an element exists, and all the new stems remain rejected. Hence every finite stem from $C$ is rejected. If some $X\in[C]^\omega$ were in $O$, openness would supply a finite initial segment $s$ of $X$ whose entire ordinary cylinder is contained in $O$. The tail $C/\max s$ would accept $s$, a contradiction. Thus

$$
\boxed{[C]^\omega\cap O=\varnothing
\quad\text{or}\quad[B]^\omega\subseteq O.}
$$

In particular every [open](../../../topology.md#open-set) payoff has an infinite [homogeneous set](../../../ramsey-theory.md#homogeneous-set-for-a-colouring). A finite partition into [open](../../../topology.md#open-set) colour classes can be handled by successive application of this two-colour assertion.

For an arbitrary partition use [finite-symmetric-difference parity colouring](../../../ramsey-theory.md#finite-symmetric-difference-parity-colouring). On the infinite [subsets](../../../set.md#subset) of the ground [set](../../../set.md), declare $X\sim Y$ when $X\mathbin\triangle Y$ is finite, and choose a representative $R$ from each [equivalence class](../../../set-theory.md#equivalence-class). Colour $X$ by

$$
c(X)=|X\mathbin\triangle R_{[X]}|\pmod2.
$$

For any infinite $H$, removing one member gives an infinite $H'$ in the same class and reverses the parity. Thus $H$ and $H'$ have opposite colours, so neither colour contains all infinite [subsets](../../../set.md#subset) of any infinite ground [set](../../../set.md). **This two-colouring has no infinite homogeneous [set](../../../set.md).** Representative selection uses [choice](../../../set-theory.md#axiom-of-choice); the construction is deliberately unrestricted by topological regularity.

## 7

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

An [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) converts coordinatewise finite information into a single [first-order structure](../../../mathematical-logic.md#first-order-structure). Let $(M_i)_{i\in I}$ be nonempty structures in a common [first-order language](../../../mathematical-logic.md#first-order-language), and let $U$ be an [ultrafilter](../../../set-theory.md#ultrafilter) on $I$. In $\prod_iM_i$, [set](../../../set.md)

$$
f\sim_U g\quad\Longleftrightarrow\quad\{i:f(i)=g(i)\}\in U.
$$

The [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) $\prod_iM_i/U$ has these [equivalence classes](../../../set-theory.md#equivalence-class) as its elements. [Functions](../../../function.md) are interpreted coordinatewise; a relation holds of classes exactly when it holds on a $U$-large [set](../../../set.md) of indices. Intersecting finitely many large agreement [sets](../../../set.md) shows that these interpretations are independent of representatives.

The [Łoś theorem](../../../foundations-of-mathematics.md#los-theorem), which explains the construction's usefulness, says

$$
\prod_iM_i/U\models\varphi([f_1],\ldots,[f_r])
\quad\Longleftrightarrow\quad
\{i:M_i\models\varphi(f_1(i),\ldots,f_r(i))\}\in U.
$$

Here is the proof. Induction on terms establishes the coordinatewise interpretation of atomic formulas. Finite intersections handle conjunction, and the [ultrafilter](../../../set-theory.md#ultrafilter) property handles negation, since precisely one of a [set](../../../set.md) and its complement is large. For an [existential quantification](../../../mathematical-logic.md#existential-quantification), a witness class gives coordinate witnesses on a large [set](../../../set.md). Conversely, when the coordinate existential truth [set](../../../set.md) is large, select a witness in each of those structures and a default element elsewhere. Its class is a witness in the [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct). This uses [choice](../../../set-theory.md#axiom-of-choice). Structural induction on formulas now proves the theorem, with universal quantification obtained by negation.

**Compactness.** If every finite [subset](../../../set.md#subset) of a first-order theory $T$ has a model, take $I$ to be the finite [subsets](../../../set.md#subset) $\Gamma\subseteq T$ and choose $M_\Gamma\models\Gamma$. The cones $\{\Gamma:\Delta\subseteq\Gamma\}$ for finite $\Delta$ have the finite intersection property. Extend their filter to an [ultrafilter](../../../set-theory.md#ultrafilter) by the [ultrafilter lemma](../../../set-theory.md#ultrafilter-lemma). For each $\varphi\in T$, its cone is large, so the Łoś theorem makes the [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) satisfy $\varphi$. This proves the [compactness theorem](../../../mathematical-logic.md#compactness-theorem), including theories of arbitrary [set](../../../set.md) size.

**Elementary extensions and nonstandard elements.** An [ultrapower](../../../foundations-of-mathematics.md#ultrapower) uses a fixed structure at every coordinate. The diagonal map sending $a$ to the class of the constant [function](../../../function.md) $a$ is an [elementary embedding](../../../set-theory.md#elementary-embedding) by the Łoś theorem. For a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter) on $\omega$, the class of $i\mapsto i$ in an [ultrapower](../../../foundations-of-mathematics.md#ultrapower) of the natural numbers exceeds every standard integer, because each corresponding tail is large. In an [ultrapower](../../../foundations-of-mathematics.md#ultrapower) of the real ordered field, the reciprocal of this element is positive and smaller than every positive standard reciprocal integer: an infinitesimal. These examples implement ordinary finite statements in a larger structure without claiming that every external [subset](../../../set.md#subset) or second-order assertion transfers.

**Saturation.** Such an [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) over $\omega$ is countably saturated. To see the actual diagonal argument, list a finitely satisfiable type $\varphi_0(x),\varphi_1(x),\ldots$ with parameters in the [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) and fix representatives for those parameters. For each $n$, the [set](../../../set.md) $E_n$ of coordinates admitting a simultaneous witness to its first $n$ formulas belongs to $U$ by the Łoś theorem. Arrange that the $E_n$ decrease and put $D_n=E_n\cap\{i:i\geq n\}$. The $D_n$ decrease, belong to $U$, and have empty intersection. At coordinate $i$, choose a witness to the first $m(i)$ formulas, where $m(i)$ is the largest $n$ with $i\in D_n$, or choose a default element if there is no such $n$. For each fixed $n$, $m(i)\geq n$ on the large [set](../../../set.md) $D_n$. Therefore the resulting class realizes every formula. This proves [countable saturation of an ultraproduct over omega](../../../foundations-of-mathematics.md#countable-saturation-of-an-ultraproduct-over-omega); it does not assert saturation at all larger cardinalities.

**Algebraic limits.** Take finite fields $\mathbb F_p$ indexed by the primes and a nonprincipal [ultrafilter](../../../set-theory.md#ultrafilter). Their [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) is a field of characteristic zero: for every fixed positive integer $n$, only finitely many primes divide $n$, so $n\cdot1\ne0$ on a large [set](../../../set.md). Every first-order sentence true in all finite fields holds in this infinite field, and more generally so does any sentence true for all but finitely many of the factors. This is a way to create an infinite field retaining uniform first-order information from finite fields. It does not make the field algebraically [closed](../../../topology.md#closed-set): the first-order sentence that every element is a square already fails in infinitely many of the factors.

**Large [cardinals](../../../set-theory.md#cardinal-number).** A [countably complete ultrafilter](../../../set-theory.md#countably-complete-ultrafilter) gives a well-founded membership [ultrapower](../../../foundations-of-mathematics.md#ultrapower) of the universe. If it had an infinite descending chain represented by $f_n$, each [set](../../../set.md)

$$
A_n=\{i:f_{n+1}(i)\in f_n(i)\}
$$

would be large. [Countable](../../../set-theory.md#countable-set) completeness makes $\bigcap_nA_n$ nonempty, giving an actual infinite membership descent at any index in the intersection, contrary to [foundation](../../../set-theory.md#axiom-of-regularity). The [Mostowski collapse](../../../set-theory.md#mostowski-collapse) therefore gives a transitive target and an [ultrapower embedding](../../../set-theory.md#ultrapower-embedding) $j:V\to M$.

For a measure on a [measurable cardinal](../../../set-theory.md#measurable-cardinal) $\kappa$, every [function](../../../function.md) $\kappa\to\alpha$ with $\alpha<\kappa$ is constant on a large [set](../../../set.md): otherwise intersect the fewer than $\kappa$ complements of all its fibres. Consequently $j$ fixes the [ordinals](../../../set-theory.md#ordinal) below $\kappa$. The class of the identity [function](../../../function.md) is below $j(\kappa)$ and above every constant class below $\kappa$, since all tails are large. Thus $j(\kappa)>\kappa$ and its [critical point](../../../analysis.md#critical-point) is $\kappa$. [Fine ultrafilters](../../../set-theory.md#fine-ultrafilter) on $P_\kappa(\lambda)$ that are [normal ultrafilters on small subsets](../../../set-theory.md#normal-ultrafilter-on-small-subsets) and [kappa-complete](../../../set-theory.md#kappa-complete-filter) yield the stronger embeddings witnessing [supercompact cardinals](../../../set-theory.md#supercompact-cardinal).

These applications share a single principle: **an [ultraproduct](../../../foundations-of-mathematics.md#ultraproduct) preserves precisely the first-order information seen by its [ultrafilter](../../../set-theory.md#ultrafilter)**. Principal [ultrafilters](../../../set-theory.md#ultrafilter) merely select a factor; nonprincipal ones can produce new sizes, elements and saturation. Existence of the needed [ultrafilters](../../../set-theory.md#ultrafilter) and selection of coordinate witnesses are set-theoretic assumptions, and changing the [ultrafilter](../../../set-theory.md#ultrafilter) may change the resulting model.

## 8

↑ **Parent:** [Paper 24](paper-24.md)

<h3 id="8/solution">Solution</h3>

↑ **Parent:** [8](#8)

A [BQO](../../../set.md#better-quasi-ordering), or [better-quasi-ordering](../../../set.md#better-quasi-ordering), strengthens a [well-quasi-ordering](../../../set.md#well-quasi-ordering) by testing arrays indexed by arbitrary barriers, rather than just [sequences](../../../real-analysis.md#sequence). Let $Q$ be a [preorder](../../../set.md#preorder). A [barrier in better-quasi-order theory](../../../set.md#barrier-in-better-quasi-order-theory) on an infinite $A\subseteq\omega$ is a family $B$ of nonempty finite increasing [sequences](../../../real-analysis.md#sequence) such that no member is properly contained in another and every infinite [subset](../../../set.md#subset) of $A$ has a member of $B$ as its initial segment.

For barrier members write $s\triangleleft t$ if a finite increasing [sequence](../../../real-analysis.md#sequence) $u$ has $s$ as an initial segment and has $t$ as an initial segment after deleting the first entry of $u$. A map $f:B\to Q$ is good when some $s\triangleleft t$ satisfy $f(s)\leq f(t)$. The definition is

$$
\boxed{Q\text{ is BQO }\Longleftrightarrow
\text{ every map from every barrier into }Q\text{ is good}.}
$$

Both quantifiers matter: testing only barriers of one fixed finite length is insufficient.

For the singleton barrier $B=[A]^1$, shifted pairs are just $\{a\}\triangleleft\{b\}$ with $a<b$. Thus the BQO condition implies the ordinary [well-quasi-ordering](../../../set.md#well-quasi-ordering) condition. Barrier arrays can also be viewed through [continuous arrays in better-quasi-order theory](../../../set.md#continuous-array-in-better-quasi-order-theory) $F:[A]^\omega\to Q$, with $Q$ discrete: [set](../../../set.md) $F(X)=f(s)$ for the unique barrier initial segment $s$ of $X$. This is continuous because that value is fixed by a finite prefix, and comparing $X$ with $X\setminus\{\min X\}$ is exactly the shift comparison. The general continuous-array formulation is equivalent to the barrier definition; its converse uses refinement of fronts to barriers, rather than the incorrect assertion that every prefix-decision family is already a barrier.

For an illustrative positive example, every [well-order](../../../set.md#well-order) is a BQO. If a barrier array into a [well-order](../../../set.md#well-order) were bad, its induced $F$ would satisfy

$$
F(X)>F(X\setminus\{\min X\})
>F(X\setminus\{\text{first two entries}\})>\cdots
$$

for every infinite $X$. This is an infinite strict descent in a [well-order](../../../set.md#well-order), a contradiction. A finite antichain with equality is also a BQO: the finitely many fibres of the induced continuous array are [open](../../../topology.md#open-set), so repeated use of the [Open Ramsey theorem](../../../ramsey-theory.md#open-ramsey-theorem) gives an infinite $A'$ on which the array is constant. The comparison of an infinite [subset](../../../set.md#subset) of $A'$ with its shift is then good.

The implication to a well-quasi-order is strict. The [Rado order](../../../set.md#rado-order) is

$$
R=\{(m,n)\in\omega^2:m<n\},\qquad
(m,n)\leq_R(k,l)\ \Longleftrightarrow\
(m=k\text{ and }n\leq l)\text{ or }n<k.
$$

It is [well-quasi-ordered](../../../set.md#well-quasi-ordering): if one first coordinate occurs infinitely often, its second coordinates have an increasing pair; otherwise the first coordinates are unbounded, and a later one exceeds the second coordinate of a chosen earlier pair. But take the barrier $[\omega]^2$ and $f(\{m,n\})=(m,n)$. For $m<n<l$, the shift compares $(m,n)$ with $(n,l)$; their first coordinates differ and $n<n$ is false. Every shifted comparison therefore fails. This [bad barrier array for the Rado order](../../../set.md#bad-barrier-array-for-the-rado-order) proves **[well-quasi-ordering](../../../set.md#well-quasi-ordering) does not imply [better-quasi-ordering](../../../set.md#better-quasi-ordering)**.

The stronger notion is designed for infinitary closure operations, such as powerset and infinite-sequence constructions, where a mere well-quasi-order can develop new bad arrays. The barrier definition records variable finite amounts of information from an infinite object and is consequently more robust than checking [sequences](../../../real-analysis.md#sequence) alone.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
