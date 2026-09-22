<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [large cardinal](../../../../../large-cardinal.md) axiom says that there is an uncountable [cardinal](../../../../../cardinal-number.md) with a strong closure, reflection, combinatorial or embedding property. Its interest is not merely the magnitude of the [cardinal](../../../../../cardinal-number.md): it packages a universe-like portion of [set](../../../../../set-split.md) theory, or a coherent way of comparing the universe with a proper [inner model](../../../../../inner-model.md). Such axioms form a hierarchy extending ordinary [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md), compared through [relative consistency](../../../../../relative-consistency.md) implications. The consistency qualifications are essential; an existence axiom is not a theorem of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) simply because its consequences are attractive.

The basic example is a [strongly inaccessible cardinal](../../../../../strongly-inaccessible-cardinal.md): an uncountable [regular cardinal](../../../../../regular-cardinal.md) $\kappa$ which is a [strong limit cardinal](../../../../../strong-limit-cardinal.md), so

$$
\operatorname{cf}(\kappa)=\kappa,\qquad 2^\lambda<\kappa\quad(\lambda<\kappa).
$$

These conditions imply $|V_\alpha|<\kappa$ for every $\alpha<\kappa$. Prove this by induction along the [cumulative hierarchy](../../../../../cumulative-hierarchy.md): the successor step uses the strong-limit property, and a limit step uses regularity to bound a [union](../../../../../set-union.md) of fewer than $\kappa$ smaller [sets](../../../../../set-split.md). Thus every member of $V_\kappa$ has [cardinality](../../../../../cardinality.md) below $\kappa$.

Consequently **$V_\kappa$ is a [transitive model](../../../../../transitive-model.md) of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md)**. Pairing, [union](../../../../../set-union.md), [power set](../../../../../power-set.md), [separation](../../../../../axiom-schema-of-specification.md), [axiom of infinity](../../../../../axiom-of-infinity.md) and [foundation](../../../../../axiom-of-regularity.md) stay within the hierarchy. For [replacement](../../../../../axiom-schema-of-replacement.md), a definable [function](../../../../../function-split.md) on $x\in V_\kappa$ has fewer than $\kappa$ values; regularity bounds their ranks below $\kappa$, putting the range in $V_\kappa$. Ambient [choice](../../../../../axiom-of-choice.md) supplies a [choice function](../../../../../choice-function.md) for a family in $V_\kappa$, and its graph also has bounded rank. This verifies the substantial closure axiom rather than only saying that the rank is large. It also shows why inaccessible existence cannot be proved in a consistent [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md): it would yield a [set](../../../../../set-split.md) [first-order model](../../../../../model-of-a-first-order-theory.md) of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) and hence its consistency, contrary to the [Gödel second incompleteness theorem](../../../../../godel-second-incompleteness-theorem.md).

An uncountable regular limit [cardinal](../../../../../cardinal-number.md) is a [weakly inaccessible cardinal](../../../../../weakly-inaccessible-cardinal.md); requiring the strong-limit inequality is stronger without additional hypotheses. Under [GCH](../../../../../generalized-continuum-hypothesis.md), every smaller infinite [cardinal](../../../../../cardinal-number.md) satisfies $2^\lambda=\lambda^+<\kappa$, so the two notions coincide. This distinction separates cardinal-arithmetic assumptions from the regularity requirement.

A [Mahlo cardinal](../../../../../mahlo-cardinal.md) is an inaccessible $\kappa$ whose [inaccessible cardinals](../../../../../strongly-inaccessible-cardinal.md) below it form a [stationary set](../../../../../stationary-set.md). Thus every [club set](../../../../../club-set.md) meets those inaccessibles, which strengthens mere unboundedness. There are inaccessible $\lambda<\delta<\kappa$; $V_\delta$ is a [first-order model](../../../../../model-of-a-first-order-theory.md) of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) containing an inaccessible $\lambda$. Mahloness therefore supplies a consistency statement stronger than the bare existence of one inaccessible. Iterating the demand that smaller [cardinals](../../../../../cardinal-number.md) have the same reflection property leads to further levels of the hierarchy.

A [weakly compact cardinal](../../../../../weakly-compact-cardinal.md) is a logical and combinatorial strengthening of inaccessibility. One standard characterization is an inaccessible $\kappa$ with

$$
\kappa\longrightarrow(\kappa)^2_2:
$$

every two-colouring of pairs has a homogeneous [subset](../../../../../subset.md) of size $\kappa$. Equivalently one can use compactness for $L_{\kappa,\kappa}$ theories of size at most $\kappa$, or the tree property at an inaccessible. These viewpoints explain the terminology: a local collection of compatible requirements has a global realization, and tall narrow trees cannot avoid cofinal branches. They are characterization statements; the elementary closure and measure arguments below are separate proofs of the consequences used here.

A [measurable cardinal](../../../../../measurable-cardinal.md) carries a nonprincipal [kappa-complete](../../../../../kappa-complete-filter.md) [ultrafilter](../../../../../ultrafilter.md) $U$ on $\kappa$. Every [set](../../../../../set-split.md) of size less than $\kappa$ is $U$-null, since it is a [union](../../../../../set-union.md) of fewer than $\kappa$ null singletons. Such a [cardinal](../../../../../cardinal-number.md) is regular: a cofinal [sequence](../../../../../sequence.md) of length $\mu<\kappa$ would partition $\kappa$ into $\mu$ bounded, hence null, pieces; completeness would make their [union](../../../../../set-union.md) null, an impossibility.

It is also strong limit. If $\lambda<\kappa$ and there were distinct [sets](../../../../../set-split.md) $A_\alpha\subseteq\lambda$ for $\alpha<\kappa$, choose for each $\xi<\lambda$ the $U$-large side of the partition according to whether $\xi\in A_\alpha$. The [intersection](../../../../../set-intersection.md) of these fewer than $\kappa$ large sides belongs to $U$, but all its indices designate the same [subset](../../../../../subset.md) of $\lambda$, so it has at most one member. This contradicts nonprincipality. Hence $2^\lambda<\kappa$, proving that every [measurable cardinal](../../../../../measurable-cardinal.md) is inaccessible.

The measure gives an [ultrapower embedding](../../../../../ultrapower-embedding.md). Form equivalence classes of [functions](../../../../../function-split.md) $f:\kappa\to V$ under equality on a $U$-large [set](../../../../../set-split.md), with membership defined coordinatewise modulo $U$. Induction on [first-order formulas](../../../../../first-order-formula.md) proves elementarity: Boolean operations use the [ultrafilter](../../../../../ultrafilter.md) laws, and the existential step chooses coordinate witnesses on a large [set](../../../../../set-split.md). Countable completeness makes the [ultrapower](../../../../../ultrapower.md) [well-founded](../../../../../well-founded-relation.md). An infinite descending membership chain would give countably many large coordinate conditions; their [intersection](../../../../../set-intersection.md) would produce an actual infinite membership descent in $V$. Collapse the [ultrapower](../../../../../ultrapower.md) to a [transitive class](../../../../../transitive-class.md) $M$, obtaining $j:V\to M$.

For $\alpha<\kappa$, every [function](../../../../../function-split.md) into $\alpha$ is constant on a large [set](../../../../../set-split.md) by completeness; induction shows $j(\alpha)=\alpha$. The class of the identity [function](../../../../../function-split.md) is larger than every such constant [ordinal](../../../../../ordinal.md) and lies below $j(\kappa)$, so $j(\kappa)>\kappa$. Thus the [critical point of an elementary embedding](../../../../../critical-point-of-an-elementary-embedding.md) is $\kappa$. The measure viewpoint has become a precise self-similarity principle for the universe.

A [supercompact cardinal](../../../../../supercompact-cardinal.md) imposes arbitrarily strong closure on these embeddings: for every $\lambda\ge\kappa$ there is $j:V\to M$ with critical point $\kappa$, $j(\kappa)>\lambda$, and $M^\lambda\subseteq M$. It implies measurability by the derived [ultrafilter](../../../../../ultrafilter.md)

$$
U=\{X\subseteq\kappa:\kappa\in j(X)\}.
$$

Elementarity makes this an [ultrafilter](../../../../../ultrafilter.md); fixed [ordinals](../../../../../ordinal.md) below $\kappa$ show that singletons are null. For $\mu<\kappa$, $j$ fixes the indexing length, so it carries an [intersection](../../../../../set-intersection.md) of $\mu$ [sets](../../../../../set-split.md) to the [intersection](../../../../../set-intersection.md) of their images. If all these images contain $\kappa$, so does their [intersection](../../../../../set-intersection.md), proving $\kappa$-completeness.

These examples illustrate three connected uses of [large cardinals](../../../../../large-cardinal.md): obtaining [set](../../../../../set-split.md) [first-order models](../../../../../model-of-a-first-order-theory.md) and stronger consistency statements, extending finite or countable compactness and partition phenomena to uncountable domains, and constructing [elementary embeddings](../../../../../elementary-embedding.md) with controlled closure. They also interact with [inner models](../../../../../inner-model.md): an inaccessible remains inaccessible in the [constructible universe](../../../../../constructible-universe.md), since it cannot acquire a new short cofinal [sequence](../../../../../sequence.md) there and there are fewer [subsets](../../../../../subset.md) of smaller [ordinals](../../../../../ordinal.md). A [measurable cardinal](../../../../../measurable-cardinal.md)'s measure need not belong to that [inner model](../../../../../inner-model.md), so preservation of the stronger property is a different issue. [Large cardinal](../../../../../large-cardinal.md) axioms are thus structured additional hypotheses, with carefully distinguishable consequences and relative-consistency claims, rather than a single claim that sufficiently big [cardinals](../../../../../cardinal-number.md) exist.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
