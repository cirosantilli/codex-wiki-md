<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The independence statements are [relative consistency](../../../../../relative-consistency.md) statements. We construct models from an ambient model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md); the construction is an interpretation and does not assume that the ambient model is transitive. [Foundation](../../../../../axiom-of-regularity.md) is already true in the ordinary ambient membership structure, so its positive consistency direction is immediate.

For the negative direction, construct an [extensional cumulative universe over Quine atoms](../../../../../extensional-cumulative-universe-over-quine-atoms.md). Let $A$ be a countably infinite [set](../../../../../set-split.md) of formal symbols $q_a$. Give each $q_a$ the extension $\{q_a\}$. For a [set](../../../../../set-split.md) $X$ of already constructed objects, let $S(X)$ be its unique representative: [set](../../../../../set-split.md) $S(\{q_a\})=q_a$, and otherwise use a fresh tagged code $(1,X)$. Atom codes have a different tag. Begin with $U_0=A$ and put

$$
U_{\alpha+1}=U_\alpha\cup\{S(X):X\subseteq U_\alpha\},\qquad U_\lambda=\bigcup_{\alpha<\lambda}U_\alpha.
$$

[Set](../../../../../set-split.md) $W=\bigcup_\alpha U_\alpha$. The interpreted membership relation $E$ gives $S(X)$ exactly the members $X$, and gives $q_a$ exactly the member $q_a$. This convention matters: creating a second representative for $\{q_a\}$ would violate [extensionality](../../../../../axiom-of-extensionality.md). Every object is uniquely determined by its extension, so $E$ satisfies full [extensionality](../../../../../axiom-of-extensionality.md). Every set-sized collection $X$ of objects has bounded construction rank, by ambient [replacement](../../../../../axiom-schema-of-replacement.md), and hence has its representative $S(X)$ in $W$.

Here are the remaining axiom verifications. [Empty set](../../../../../empty-set.md) and [pairing](../../../../../axiom-of-pairing.md) use $S(\varnothing)$ and $S(\{x,y\})$. If $E(y)=X$, its interpreted [union](../../../../../set-union.md) is $S(\bigcup_{x\in X}E(x))$. Its interpreted [power set](../../../../../power-set.md) is

$$
S\bigl(\{S(Y):Y\subseteq X\}\bigr),
$$

since every [subset](../../../../../subset.md) extension has a unique representative. The pure, atom-free finite hierarchy supplies a copy of $\omega$ and an inductive [set](../../../../../set-split.md). For [separation](../../../../../axiom-schema-of-specification.md), translate an $E$-formula into the ambient language, with quantifiers restricted to the definable class $W$; ambient [separation](../../../../../axiom-schema-of-specification.md) gives the appropriate [subset](../../../../../subset.md) of $X$, and $S$ represents it. For [replacement](../../../../../axiom-schema-of-replacement.md), uniqueness in the interpreted functional relation gives an ambient definable functional image of the [set](../../../../../set-split.md) $X$. Ambient [replacement](../../../../../axiom-schema-of-replacement.md) makes that image set-sized, and $S$ again represents it. These arguments also establish that all the operations used have bounded construction rank.

Ambient choice gives choice in $W$: choose a member from each nonempty extension in a set-sized family and represent the graph, using interpreted [ordered pairs](../../../../../ordered-pair.md). But $q_a E q_a$, and the nonempty [set](../../../../../set-split.md) with extension $\{q_a\}$ has no $E$-minimal member. Thus

$$
\boxed{\operatorname{Con}(\mathrm{ZFC})\Longrightarrow\operatorname{Con}(\mathrm{ZF}-\mathrm{Foundation}+\mathrm{AC}+\neg\mathrm{Foundation}).}
$$

Together with the ordinary model, this proves independence of [foundation](../../../../../axiom-of-regularity.md) from the other [ZF](../../../../../zermelo-fraenkel-set-theory.md) axioms, even when choice is retained.

To extend the construction to failure of choice, let the full [permutation group](../../../../../permutation-group.md) of $A$ act on $W$ by

$$
\pi(q_a)=q_{\pi(a)},\qquad \pi(S(X))=S(\pi``X).
$$

The singleton convention is equivariant, so this is an [automorphism](../../../../../automorphism.md) of $(W,E)$. An object has [finite support](../../../../../finite-support-in-a-permutation-action.md) if some finite $F\subseteq A$ has the property that every [permutation](../../../../../permutation.md) fixing $F$ pointwise fixes the object. Retain objects all of whose membership descendants have [finite support](../../../../../finite-support-in-a-permutation-action.md), stopping the hereditary recursion at the atomic self-loops. This gives the [hereditarily finite-supported Quine-atom model](../../../../../hereditarily-finite-supported-quine-atom-model.md) $\mathcal H$; each $q_a$ belongs to it, with support $\{q_a\}$.

[Extensionality](../../../../../axiom-of-extensionality.md) persists because every retained object's members are retained. [Empty set](../../../../../empty-set.md), [pairing](../../../../../axiom-of-pairing.md), [infinity](../../../../../infinity.md) and [union](../../../../../set-union.md) preserve hereditary [finite support](../../../../../finite-support-in-a-permutation-action.md). For [separation](../../../../../axiom-schema-of-specification.md) on a retained [set](../../../../../set-split.md) $x$, the [union](../../../../../set-union.md) of finite supports for $x$ and the formula's parameters supports the separated extension: [permutations](../../../../../permutation.md) fixing those supports preserve satisfaction in $\mathcal H$. All its members are retained, so its representative is retained. For [replacement](../../../../../axiom-schema-of-replacement.md), the same support fixes the functional range, because an [automorphism](../../../../../automorphism.md) must take the unique output at an input to the unique output at its transported input. Ambient [replacement](../../../../../axiom-schema-of-replacement.md) bounds that range; all its members are in $\mathcal H$, so its representative belongs to $\mathcal H$. Finally, the collection of all retained [subset](../../../../../subset.md) representatives of $x$ is an ambient [set](../../../../../set-split.md), contained in the full interpreted [power set](../../../../../power-set.md) of $x$. A support of $x$ permutes this collection onto itself, and its members are retained. Its representative is therefore the internal [power set](../../../../../power-set.md) in $\mathcal H$. This verifies every [ZF](../../../../../zermelo-fraenkel-set-theory.md) axiom except [foundation](../../../../../axiom-of-regularity.md); [foundation](../../../../../axiom-of-regularity.md) still fails at each $q_a$.

The atom [set](../../../../../set-split.md) $A$ and the family $[A]^2$ of its two-element [subsets](../../../../../subset.md) have empty support and are retained. Suppose a [choice function](../../../../../choice-function.md) $f$ on $[A]^2$ were retained, with [finite support](../../../../../finite-support-in-a-permutation-action.md) $F$. Choose distinct $q_a,q_b$ outside $F$ and transpose them. The transposition fixes $f$ and fixes the unordered pair $\{q_a,q_b\}$, but moves whichever of its two members $f$ selects. Equivariance would require that selected member to be fixed, a contradiction. Hence

$$
\boxed{\operatorname{Con}(\mathrm{ZFC})\Longrightarrow\operatorname{Con}(\mathrm{ZF}-\mathrm{Foundation}+\neg\mathrm{AC}+\neg\mathrm{Foundation}).}
$$

The full universe $W$ gives the corresponding positive-choice model. Choice is therefore independent of [ZF](../../../../../zermelo-fraenkel-set-theory.md) without [foundation](../../../../../axiom-of-regularity.md). Unlike a [permutation](../../../../../permutation.md) model with ordinary [urelements](../../../../../urelement.md), this model retains full pure-set [extensionality](../../../../../axiom-of-extensionality.md): the atomic objects are self-membered [sets](../../../../../set-split.md), not empty objects exempted from [extensionality](../../../../../axiom-of-extensionality.md).

The constructible-universe interpretation gives $\operatorname{Con}(\mathrm{ZF})\Rightarrow\operatorname{Con}(\mathrm{ZFC})$. Thus the consistency assumptions in both displayed conclusions can equivalently be taken to be $\operatorname{Con}(\mathrm{ZF})$; no additional consistency strength is being used.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
