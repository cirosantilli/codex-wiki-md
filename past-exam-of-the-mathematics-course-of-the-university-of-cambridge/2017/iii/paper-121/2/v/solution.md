<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The assumed [beth number](../../../../../../beth-number.md) equality $\beth_1=\aleph_2$ means $2^{\aleph_0}=\aleph_2$ in the ambient universe. Put $W=L(X)$ with $X=\mathcal P(\omega)$, using the [relative constructible hierarchy](../../../../../../relative-constructible-hierarchy.md) defined above.

The base $X$ is transitive because every member of a member of $X$ is a finite [ordinal](../../../../../../ordinal.md), hence itself a [subset](../../../../../../subset.md) of $\omega$. Moreover $X\subseteq W$ and $X\in W$, and $W$ is an [inner model](../../../../../../inner-model.md) of [ZF](../../../../../../zermelo-fraenkel-set-theory.md). The latter standard fact follows from the hierarchy and reflection: bounded-rank witnesses give pairing and union; reflection gives separation and replacement; ambient replacement bounds the stages of all relatively constructible [subsets](../../../../../../subset.md) of any fixed [set](../../../../../../set-split.md), giving power set. It does not require [axiom of choice](../../../../../../axiom-of-choice.md) inside $W$. Since no new [subsets](../../../../../../subset.md) of $\omega$ can appear in an inner class,

$$
\mathcal P^W(\omega)=X=\mathcal P(\omega).
$$

Since [inner models with all reals preserve omega-one](../../../../../../inner-models-with-all-reals-preserve-omega-one.md), it suffices to check that their real-code argument applies to $W$. Every ambient countably infinite [ordinal](../../../../../../ordinal.md) has a [well-order code](../../../../../../well-order-code.md) on $\omega$, coded by a [subset](../../../../../../subset.md) of $\omega$ in $X$. Finite [ordinals](../../../../../../ordinal.md) and $\omega$ are already shared. This code belongs to $W$, is well-founded there, and its [Mostowski collapse theorem](../../../../../../mostowski-collapse-theorem.md) interpretation inside $W$ is the same [ordinal](../../../../../../ordinal.md) as outside. Hence the [ordinal](../../../../../../ordinal.md) is countable in $W$. Conversely, any countability witness in $W$ remains a witness in the ambient universe. Thus $\omega_1^W=\omega_1$.

If $W$ satisfied the [Continuum hypothesis](../../../../../../continuum-hypothesis.md) in its usual well-orderable formulation, it would contain a [bijection](../../../../../../bijection.md) from $\omega_1^W$ onto its [power set](../../../../../../power-set.md) of $\omega$. The same [bijection](../../../../../../bijection.md) would exist externally from $\omega_1$ onto $X$, contradicting $|X|=\aleph_2$. Therefore

$$
\boxed{L(\mathcal P(\omega))\models\neg\mathsf{CH}.}
$$

This proof uses agreement on all reals and on $\omega_1$, not an unwarranted assertion that $L(X)$ satisfies [axiom of choice](../../../../../../axiom-of-choice.md) or computes every higher [cardinal number](../../../../../../cardinal-number.md) correctly.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
