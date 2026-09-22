<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

All independence assertions here are [relative consistency](../../../../../relative-consistency.md) results. Begin with a [first-order model](../../../../../model-of-a-first-order-theory.md) of [ZF](../../../../../zermelo-fraenkel-set-theory.md); for the choice-preserving side use [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). The original [first-order model](../../../../../model-of-a-first-order-theory.md) already gives the side where [foundation](../../../../../axiom-of-regularity.md) holds. We construct the opposite side while checking the other axioms, then add a symmetry restriction to make [choice](../../../../../axiom-of-choice.md) fail.

Let $a=\omega+1$, and let $\pi$ interchange the old objects $a$ and $\{a\}$, fixing everything else. They are distinct. On the same domain define the [Rieger-Bernays permutation model](../../../../../rieger-bernays-permutation-model.md) by

$$
\boxed{x\mathrel E y\quad\Longleftrightarrow\quad x\in\pi(y).}
$$

Write $S(b)=\pi^{-1}(b)$; the $E$-members of $S(b)$ are exactly the old members of $b$. In particular $a\mathrel E a$, and $a$ has no other $E$-member. Thus $a$ is a [Quine atom](../../../../../quine-atom.md), and the nonempty $E$-set $a$ has no member disjoint from itself. [Foundation](../../../../../axiom-of-regularity.md) fails.

Here are the other axioms explicitly. Equal $E$-extensions imply $\pi(y)=\pi(z)$ by old [extensionality](../../../../../axiom-of-extensionality.md), hence $y=z$. An $E$-pair of $x,z$ is $S(\{x,z\})$. An $E$-union of $y$ is

$$
S\left(\bigcup\{\pi(x):x\in\pi(y)\}\right).
$$

Its elements are precisely objects with an $E$-membership chain of length two into $y$. The $E$-power [set](../../../../../set-split.md) of $y$ is

$$
S\left(\{S(b):b\subseteq\pi(y)\}\right),
$$

since $x\subseteq_E y$ means $\pi(x)\subseteq\pi(y)$. These are old [sets](../../../../../set-split.md) by [power set](../../../../../power-set.md) and [replacement](../../../../../axiom-schema-of-replacement.md).

Translate any [first-order formula](../../../../../first-order-formula.md) by replacing its membership symbol with $E$, a definable relation with parameter $a$. [Separation](../../../../../axiom-schema-of-specification.md) on $y$ produces the representative of the old [set](../../../../../set-split.md) $\{x\in\pi(y):\varphi^E(x)\}$. For [replacement](../../../../../axiom-schema-of-replacement.md), functionality in the new structure is exactly functionality of the translated [first-order formula](../../../../../first-order-formula.md) on the old [set](../../../../../set-split.md) $\pi(y)$; old [replacement](../../../../../axiom-schema-of-replacement.md) gives its range, and $S$ represents that range as an $E$-set. Thus the full schemas, not merely their quantifier-free instances, survive. The old finite [ordinals](../../../../../ordinal.md) and $\omega$ are fixed by $\pi$, so their empty-set and successor relations are unchanged; the old $\omega$ witnesses [axiom of infinity](../../../../../axiom-of-infinity.md).

If the original [first-order model](../../../../../model-of-a-first-order-theory.md) satisfies [AC](../../../../../axiom-of-choice.md), the new one does too. For an $E$-family $y$ of nonempty $E$-sets, old [choice](../../../../../axiom-of-choice.md) selects $c(x)\in\pi(x)$ for each $x\in\pi(y)$. The $E$-ordered-pair construction is definable, so old [replacement](../../../../../axiom-schema-of-replacement.md) forms the graph of this selection in $E$-pair codes; applying $S$ makes it an $E$-function. It chooses an $E$-member from each member of the family. Therefore a full membership permutation alone does not refute [choice](../../../../../axiom-of-choice.md). We have proved

$$
\boxed{\operatorname{Con}(\mathsf{ZF})\Rightarrow
\operatorname{Con}(\mathsf{ZF}-\mathsf{Foundation}+\neg\mathsf{Foundation}),}
$$

with [choice](../../../../../axiom-of-choice.md) preserved if it was initially present. Together with the unchanged [well-founded](../../../../../well-founded-relation.md) [first-order model](../../../../../model-of-a-first-order-theory.md), this proves [foundation](../../../../../axiom-of-regularity.md)'s independence from the remaining axioms.

For the choice-failing extension, work in an ambient [first-order model](../../../../../model-of-a-first-order-theory.md) of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) and build the [extensional cumulative universe over Quine atoms](../../../../../extensional-cumulative-universe-over-quine-atoms.md). Let $A$ be a countably infinite collection of distinct tagged objects. Give each $q\in A$ the membership extension $\{q\}$. Adjoin [sets](../../../../../set-split.md) in successive construction ranks, representing a set-sized collection $X$ by a unique new tagged object with extension $X$, except that the representative of $\{q\}$ is the already existing $q$. Denote this representative by $S(X)$ again. Thus $S(\{q\})=q$; adjoining a second, distinct ordinary singleton would incorrectly violate [extensionality](../../../../../axiom-of-extensionality.md).

More formally take atom tags of kind zero, put $D_0=A$, and define

$$
D_{\alpha+1}=D_\alpha\cup\{(1,X):X\subseteq D_\alpha,
\ X\ne\{q\}\text{ for every }q\in A\},\qquad
D_\lambda=\bigcup_{\alpha<\lambda}D_\alpha.
$$

The extension of $(1,X)$ is $X$, and the extension of an atom $q$ is $\{q\}$. Tags of the two kinds are disjoint. Any set-sized collection of objects has bounded construction ranks and hence a representative at a later stage. This proves pairing, [union](../../../../../set-union.md), [power set](../../../../../power-set.md), [separation](../../../../../axiom-schema-of-specification.md) and [replacement](../../../../../axiom-schema-of-replacement.md) by representing their extensions, just as above. For [axiom of infinity](../../../../../axiom-of-infinity.md), recursively construct the pure finite ordinals, collect these representatives in an ambient [set](../../../../../set-split.md) by [replacement](../../../../../axiom-schema-of-replacement.md), and apply $S$ to that collection. The resulting inductive [set](../../../../../set-split.md) is fixed by every atom permutation. Every object has a unique extension, so full [extensionality](../../../../../axiom-of-extensionality.md) holds, although [foundation](../../../../../axiom-of-regularity.md) fails at the atoms.

Let $G$ be the full [symmetric group](../../../../../symmetric-group.md) of $A$. Extend $g\in G$ by $g(S(X))=S(g''X)$, recursively on the non-atomic construction ranks. This preserves membership, including the atomic self-loops. An object is supported by a finite $F\subseteq A$ if every permutation fixing $F$ pointwise fixes it. Retain the [hereditarily finite-supported Quine-atom model](../../../../../hereditarily-finite-supported-quine-atom-model.md) $H$: every object reachable from a retained object by finitely many membership steps has [finite support](../../../../../finite-support-in-a-permutation-action.md). In particular all members of a retained object are retained, every atom is supported by itself, and $S(A)$ is supported by the [empty set](../../../../../empty-set.md).

We verify the schemas in $H$, rather than assuming that an arbitrary invariant class is a [first-order model](../../../../../model-of-a-first-order-theory.md). For [separation](../../../../../axiom-schema-of-specification.md), a [subset](../../../../../subset.md) of a retained [set](../../../../../set-split.md) $x$ definable in $H$ from parameters $p_1,\ldots,p_m$ is fixed by permutations fixing the [union](../../../../../set-union.md) of their finite supports. Its members are already in $H$, so its representative belongs to $H$. For [replacement](../../../../../axiom-schema-of-replacement.md), a definable functional image of $x$ is a [set](../../../../../set-split.md) in the ambient universe. Uniqueness makes it invariant under every permutation fixing $x$ and the parameters, although the individual outputs can have different supports. Those outputs are in $H$ by the relativized [first-order formula](../../../../../first-order-formula.md), so the range representative is hereditarily supported. This proves [replacement](../../../../../axiom-schema-of-replacement.md) without falsely requiring one [finite support](../../../../../finite-support-in-a-permutation-action.md) for every individual value.

The internal [power set](../../../../../power-set.md) is the representative of

$$
\{S(Y):Y\subseteq\operatorname{ext}(x),\ S(Y)\in H\}.
$$

It is an ambient [set](../../../../../set-split.md) and is fixed by the support of $x$, because a permutation carries retained [subsets](../../../../../subset.md) of $x$ to retained [subsets](../../../../../subset.md) of $x$. Every member is retained by its definition. This proves the internal power-set axiom. Finite [unions](../../../../../set-union.md) of supports handle pairing and [union](../../../../../set-union.md); the pure [natural numbers](../../../../../natural-number.md) have empty support; [extensionality](../../../../../axiom-of-extensionality.md) is inherited because $H$ is membership-transitive. Hence $H$ satisfies all [ZF](../../../../../zermelo-fraenkel-set-theory.md) axioms except [foundation](../../../../../axiom-of-regularity.md), which still fails.

In $H$ form the family of all two-element [subsets](../../../../../subset.md) of $A$, a family with empty support. Suppose it had a [choice function](../../../../../choice-function.md) $f\in H$, with [finite support](../../../../../finite-support-in-a-permutation-action.md) $F$. Choose distinct $q,r\in A\setminus F$. Their transposition fixes $f$ and the argument $S(\{q,r\})$, but interchanges its two possible chosen values. Equivariance gives a contradiction. Thus

$$
\boxed{H\models\mathsf{ZF}-\mathsf{Foundation}
+\neg\mathsf{Foundation}+\neg\mathsf{AC}.}
$$

The full construction over $A$, before restricting to $H$, has [choice](../../../../../axiom-of-choice.md) by ambient [choice](../../../../../axiom-of-choice.md) and the representability of [choice](../../../../../axiom-of-choice.md) graphs. Alternatively an ordinary [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) [first-order model](../../../../../model-of-a-first-order-theory.md) gives the positive [choice](../../../../../axiom-of-choice.md) side. This proves the independence of [AC](../../../../../axiom-of-choice.md) from [ZF](../../../../../zermelo-fraenkel-set-theory.md) minus [foundation](../../../../../axiom-of-regularity.md). The required metatheoretic consistency can be expressed using Con([ZF](../../../../../zermelo-fraenkel-set-theory.md)), since the [constructible universe](../../../../../constructible-universe.md) of a [ZF](../../../../../zermelo-fraenkel-set-theory.md) [first-order model](../../../../../model-of-a-first-order-theory.md) supplies [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md), as explained in the next solution. No assumption of a [transitive model](../../../../../transitive-model.md) follows from mere consistency or is needed for these interpreted [first-order model](../../../../../model-of-a-first-order-theory.md) constructions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
