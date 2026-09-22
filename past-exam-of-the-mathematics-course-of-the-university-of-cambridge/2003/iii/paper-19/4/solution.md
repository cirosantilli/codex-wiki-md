<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [inner model](../../../../../inner-model.md) of a universe of [ZF](../../../../../zermelo-fraenkel-set-theory.md) is a [transitive class](../../../../../transitive-class.md) $M$ containing every [ordinal](../../../../../ordinal.md) and satisfying the required set-theoretic axioms with the inherited membership relation. Transitivity means that every member of a member of $M$ belongs to $M$. Requiring all [ordinals](../../../../../ordinal.md) distinguishes an [inner model](../../../../../inner-model.md) from a [transitive set](../../../../../transitive-set.md) [first-order model](../../../../../model-of-a-first-order-theory.md) such as $V_\kappa$: a [set](../../../../../set-split.md) [first-order model](../../../../../model-of-a-first-order-theory.md) has bounded [ordinal](../../../../../ordinal.md) height. One may specify an [inner model](../../../../../inner-model.md) of [ZF](../../../../../zermelo-fraenkel-set-theory.md), [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) or a stronger theory; [choice](../../../../../axiom-of-choice.md) is not built into the term unless specified.

The fundamental example is the [constructible universe](../../../../../constructible-universe.md). Form the [constructible hierarchy](../../../../../constructible-hierarchy.md)

$$
L_0=\varnothing,\qquad L_{\alpha+1}=\operatorname{Def}(L_\alpha),\qquad
L_\lambda=\bigcup_{\alpha<\lambda}L_\alpha,
\qquad L=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha.
$$

Here [definable power set](../../../../../definable-power-set-split.md) means [subsets](../../../../../subset.md) definable over the [set](../../../../../set-split.md) structure $(L_\alpha,\in)$ by [first-order formulas](../../../../../first-order-formula.md) with finitely many parameters from that level. Each level is transitive, the levels increase, and $\operatorname{Ord}\cap L_\alpha=\alpha$, by induction. Thus $L$ is transitive and contains all [ordinals](../../../../../ordinal.md).

The construction supplies a definable [well-order](../../../../../well-order.md): order objects first by their earliest construction stage, then by a least [first-order formula](../../../../../first-order-formula.md) code and a finite tuple of parameters in the already constructed level's [well-order](../../../../../well-order.md). Recursively extend the earlier [well-order](../../../../../well-order.md) at each successor stage and unite compatible orders at limits. [First-order formula](../../../../../first-order-formula.md) codes and finite tuples of well-ordered parameters are well-orderable. This yields a canonical global ordering definable within $L$; its restrictions to [sets](../../../../../set-split.md) will give [choice](../../../../../axiom-of-choice.md) once the [ZF](../../../../../zermelo-fraenkel-set-theory.md) axioms are checked.

For that check, a useful reflection argument is explicit. Given finitely many [first-order formulas](../../../../../first-order-formula.md) and a starting level, pass to a higher level containing witnesses for their existential subformulas on all parameter tuples from the current level, choosing least witnesses in the canonical order. There are set-many tuples, so ambient [replacement](../../../../../axiom-schema-of-replacement.md) bounds their witness stages. Repeat for $\omega$ steps and take the [union](../../../../../set-union.md) level $L_\theta$. Every relevant witness with parameters in that level appears at a later step. Induction on [first-order formulas](../../../../../first-order-formula.md), with this witness property for the existential case, proves that $L_\theta$ reflects the chosen finite list of [first-order formulas](../../../../../first-order-formula.md) of $L$.

[Separation](../../../../../axiom-schema-of-specification.md) on a constructible [set](../../../../../set-split.md) is then definability over a sufficiently large reflecting level, so its [subset](../../../../../subset.md) appears at the next level. For [replacement](../../../../../axiom-schema-of-replacement.md), reflect the [first-order formula](../../../../../first-order-formula.md) specifying a functional image and its required existence statements. All inputs belong to a level containing the domain as a [set](../../../../../set-split.md); all their unique outputs then lie in one reflecting level. The image is definable there and hence is constructible. For [power set](../../../../../power-set.md), the ambient [set](../../../../../set-split.md) of constructible [subsets](../../../../../subset.md) of $x$ has bounded construction stages by [replacement](../../../../../axiom-schema-of-replacement.md) in the ambient universe. At a level containing them all, this internal collection is definable by the bounded condition $y\subseteq x$, and therefore is itself in $L$. Pairing, [union](../../../../../set-union.md) and [axiom of infinity](../../../../../axiom-of-infinity.md) follow directly from definability over sufficiently large levels, while [extensionality](../../../../../axiom-of-extensionality.md) and [foundation](../../../../../axiom-of-regularity.md) follow from transitivity. Thus $L\models\mathsf{ZF}$, and its canonical ordering gives $L\models\mathsf{AC}$.

This proves the important relative-consistency application

$$
\boxed{\operatorname{Con}(\mathsf{ZF})\Rightarrow\operatorname{Con}(\mathsf{ZFC}).}
$$

One does not conclude that [choice](../../../../../axiom-of-choice.md) is true in the original universe. Instead the [inner model](../../../../../inner-model.md) supplies a possibly smaller universe in which [choice](../../../../../axiom-of-choice.md) holds.

Constructibility also supplies [GCH](../../../../../generalized-continuum-hypothesis.md). Here is the cardinal-counting argument, making clear the role of the [condensation lemma for the constructible universe](../../../../../condensation-lemma-for-the-constructible-universe.md). Work inside $L$. If $x\subseteq\kappa$ is constructible, take a large limit $L_\theta$ containing $x$ and an elementary hull of $\kappa\cup\{\kappa,x\}$ of size $\kappa$. Its transitive collapse is $L_\beta$ by condensation. The collapse fixes every [ordinal](../../../../../ordinal.md) below $\kappa$, and hence fixes $x$ and $\kappa$. Since the hull has size $\kappa$, $\beta<\kappa^+$. Therefore every constructible [subset](../../../../../subset.md) of $\kappa$ appears below $L_{\kappa^+}$.

The condensation fact expresses the rigidity of this definability construction: [first-order formula](../../../../../first-order-formula.md) codes, finite parameter tuples and satisfaction in set-sized lower levels are preserved by the collapse. Inducting over the hull's [ordinal](../../../../../ordinal.md) indices identifies each collapsed lower level with the corresponding $L$-level; elementarity supplies every definable [subset](../../../../../subset.md) coded by parameters in that collapsed lower level. Taking [unions](../../../../../set-union.md) identifies the entire collapsed hull with a level $L_\beta$.

Induction on construction stages gives $|L_\gamma|\le |\gamma|+\aleph_0$: each successor has only countably many [first-order formula](../../../../../first-order-formula.md) schemes with finite parameter tuples, and limits take [unions](../../../../../set-union.md). Hence $|L_{\kappa^+}|=\kappa^+$ for infinite $\kappa$. The preceding containment gives $2^\kappa\le\kappa^+$ in $L$, and Cantor's theorem gives the reverse inequality. Consequently

$$
\boxed{L\models\mathsf{ZFC}+\mathsf{GCH},\qquad
\operatorname{Con}(\mathsf{ZF})\Rightarrow
\operatorname{Con}(\mathsf{ZFC}+\mathsf{GCH}).}
$$

All these [cardinal](../../../../../cardinal-number.md) computations are internal to $L$; they need not equal the ambient [cardinal](../../../../../cardinal-number.md) computations.

[Inner models](../../../../../inner-model.md) are also useful for analyzing stronger axioms. If $\kappa$ is inaccessible in $V$, it remains an uncountable [regular cardinal](../../../../../regular-cardinal.md) in $L$, because a shorter cofinal [sequence](../../../../../sequence.md) in $L$ would already be one in $V$. For each [ordinal](../../../../../ordinal.md) $\lambda<\kappa$, its constructible [subsets](../../../../../subset.md) are fewer than $\kappa$ even in the internal [cardinal](../../../../../cardinal-number.md) comparison: in $V$, $\mathcal P(\lambda)$ has size below $\kappa$, so its constructible part cannot have an $L$-well-order of length at least $\kappa$. Thus it remains strong limit. Accordingly $L$ supplies relative-consistency information compatible with inaccessibles and [GCH](../../../../../generalized-continuum-hypothesis.md). Stronger embedding or measure properties require extra analysis, since the witnessing objects may disappear upon passing to an [inner model](../../../../../inner-model.md).

There is a useful limitation: **no uniform inner-model construction can refute [choice](../../../../../axiom-of-choice.md) from every starting [ZF](../../../../../zermelo-fraenkel-set-theory.md) universe**. Every [inner model](../../../../../inner-model.md) $M$ of [ZF](../../../../../zermelo-fraenkel-set-theory.md) contains the ambient $L$. Indeed, induction gives $L_\alpha^M=L_\alpha$: the same set-sized level has the same satisfaction relation for definitions, and limit stages take the same [unions](../../../../../set-union.md). If the starting universe already satisfies $V=L$, any [inner model](../../../../../inner-model.md) containing all [ordinals](../../../../../ordinal.md) must therefore be the whole universe, where [choice](../../../../../axiom-of-choice.md) holds. To obtain a choice-failing [first-order model](../../../../../model-of-a-first-order-theory.md) uniformly one needs a different method, such as the symmetry restriction in the preceding solution. Inner-model arguments establish consistency and preservation through carefully controlled smaller universes; they do not freely manufacture arbitrary desired axiom failures.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
