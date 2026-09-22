<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [inner model](../../../../../inner-model.md) of [ZF](../../../../../zermelo-fraenkel-set-theory.md) is a [transitive class](../../../../../transitive-class.md) $M$ containing every [ordinal](../../../../../ordinal.md), with inherited membership, such that each [ZF](../../../../../zermelo-fraenkel-set-theory.md) axiom holds with all quantifiers restricted to $M$. Here transitivity means $x\in y\in M\Rightarrow x\in M$. For a proper class this is an axiom-by-axiom assertion, not an internal truth predicate for the whole class. An [inner model](../../../../../inner-model.md) can have fewer [subsets](../../../../../subset.md) of a given [set](../../../../../set-split.md) than the surrounding universe; it need not have the same [cardinals](../../../../../cardinal-number.md) or the same continuum function.

[Inner models](../../../../../inner-model.md) prove [relative consistency](../../../../../relative-consistency.md). If a theory $T$ proves that a definable class $M$ satisfies every axiom of $S$, an inconsistency proof from $S$ could be relativized to $M$ and become an inconsistency proof from $T$. Thus **$\operatorname{Con}(T)\Rightarrow\operatorname{Con}(S)$**. This reasoning concerns formal interpretations and needs no assumption that a given model of $T$ is externally well-founded.

The central example is the [constructible universe](../../../../../constructible-universe.md). Define

$$
L_0=\varnothing,\qquad L_{\alpha+1}=\operatorname{Def}(L_\alpha),\qquad L_\lambda=\bigcup_{\alpha<\lambda}L_\alpha,\qquad L=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha,
$$

where $\operatorname{Def}(X)$ contains exactly the [subsets](../../../../../subset.md) definable over $(X,\in)$ using parameters from $X$. [Satisfaction for a set structure](../../../../../satisfaction-for-a-set-structure.md) is definable, so this recursion is available in [ZF](../../../../../zermelo-fraenkel-set-theory.md). [Induction](../../../../../mathematical-induction.md) shows that the levels are transitive and increasing: if $a\in L_\alpha$, the [subset](../../../../../subset.md) $\{x\in L_\alpha:x\in a\}$ is $a$, so $a\in L_{\alpha+1}$. The [ordinal](../../../../../ordinal.md) part of $L_\alpha$ is $\alpha$, giving all [ordinals](../../../../../ordinal.md) in $L$.

For completeness, the main axiom mechanisms explain why this example works. Finite [set](../../../../../set-split.md) operations on constructible parameters are definable at finitely many further stages. For a fixed finite family of formulas and parameters, close a [sequence](../../../../../sequence.md) of levels under their least constructible witness stages and take its [union](../../../../../set-union.md); [induction](../../../../../mathematical-induction.md) on formulas gives a reflecting level. [Separation](../../../../../axiom-schema-of-specification.md) of a constructible [set](../../../../../set-split.md) then occurs at the next definability stage. For [replacement](../../../../../axiom-schema-of-replacement.md), ambient [replacement](../../../../../axiom-schema-of-replacement.md) bounds the construction stages of the unique constructible outputs; a reflecting level above that bound makes the range definable. For the internal [power set](../../../../../power-set.md) of $a\in L$, use ambient [separation](../../../../../axiom-schema-of-specification.md) to form $\mathcal P(a)\cap L$, bound the construction stages of its members, and at a sufficiently high level define the family of all [subsets](../../../../../subset.md) of $a$ in that level. Thus the internal [power set](../../../../../power-set.md) is constructible even though some ambient [subsets](../../../../../subset.md) may not be. [Foundation](../../../../../axiom-of-regularity.md) is inherited by transitivity, and [infinity](../../../../../infinity.md) comes from $L_\omega$ and its successor stages.

There is a canonical [well-order](../../../../../well-order.md) of $L$: order by first construction stage, then by the least definition code and finite parameter tuple, using the previously constructed [well-orders](../../../../../well-order.md) for parameters. Each [set](../../../../../set-split.md) in $L$ can be well-ordered by the restriction of this set-like class order; hence $L$ satisfies [AC](../../../../../axiom-of-choice.md). Moreover the hierarchy computed inside $L$ is the same hierarchy, because definability over a fixed [set](../../../../../set-split.md) structure and limit unions are absolute. Thus $L$ satisfies $V=L$. The further [cardinal](../../../../../cardinal-number.md) analysis of this hierarchy, encapsulated in the [constructible universe theorem](../../../../../constructible-universe-theorem.md), gives [GCH](../../../../../generalized-continuum-hypothesis.md). Consequently

$$
\boxed{\operatorname{Con}(\mathrm{ZF})\Longrightarrow\operatorname{Con}(\mathrm{ZFC}+V=L+\mathrm{GCH}).}
$$

This proves the [relative consistency](../../../../../relative-consistency.md) of choice, [CH](../../../../../continuum-hypothesis.md) and [GCH](../../../../../generalized-continuum-hypothesis.md); in particular none can be refuted by [ZF](../../../../../zermelo-fraenkel-set-theory.md) if [ZF](../../../../../zermelo-fraenkel-set-theory.md) is consistent. The assertions here are internal to $L$: they do not assert [CH](../../../../../continuum-hypothesis.md) in the ambient universe.

[Inner models](../../../../../inner-model.md) also isolate definable information. The [relative constructible universe](../../../../../relative-constructible-universe.md) built with a [set](../../../../../set-split.md) parameter retains that parameter and all [ordinals](../../../../../ordinal.md) while discarding unrelated [sets](../../../../../set-split.md). Such constructions help compare [relative consistency](../../../../../relative-consistency.md) strengths and identify which hypotheses survive passage to smaller universes; preservation of a large-cardinal property must be checked separately, not inferred merely from transitivity.

There is an important limitation, the [constructible-universe obstruction to a uniform inner-model proof of failure of choice](../../../../../constructible-universe-obstruction-to-a-uniform-inner-model-proof-of-failure-of-choice.md). Every [inner model](../../../../../inner-model.md) $M$ of [ZF](../../../../../zermelo-fraenkel-set-theory.md) contains the ambient $L$. Indeed $L_\alpha^M=L_\alpha$ by [induction](../../../../../mathematical-induction.md): the same [set](../../../../../set-split.md) structure has the same definable [subsets](../../../../../subset.md) at a successor stage, and both hierarchies take the same [union](../../../../../set-union.md) at a limit. If the ambient universe satisfies $V=L$, this forces $M=V$. Thus [inner models](../../../../../inner-model.md) cannot uniformly produce a model of $\neg\mathrm{AC}$ or $V\ne L$ from every [ZF](../../../../../zermelo-fraenkel-set-theory.md) universe. To prove the opposite independence directions one needs an outer-model or other interpretation technique, such as [forcing](../../../../../forcing-split.md) or the non-well-founded symmetry construction in Question 2.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
