<h1 id="3/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conversely, suppose $p\in G$ and $p\Vdash^*\sigma\in\tau$. The [syntactic forcing relation](../../../../../../../syntactic-forcing-relation.md) says that

$$
D=\{s\leq p:\exists(\rho,r)\in\tau\ (s\leq r\land s\Vdash^*\sigma=\rho)\}
$$

is [dense below a forcing condition](../../../../../../../dense-below-a-forcing-condition.md) $p$. This is a [set](../../../../../../../set-split.md) in $M$ by definability of forcing and [axiom schema of separation](../../../../../../../axiom-schema-of-specification.md). The [dense-below generic meeting lemma](../../../../../../../dense-below-generic-meeting-lemma.md) gives $s\in G\cap D$: augment $D$ by all [incompatible forcing conditions](../../../../../../../incompatible-forcing-conditions.md) with $p$ to obtain a globally dense ground-model [set](../../../../../../../set-split.md), and use $p\in G$ to exclude the incompatible part.

Choose the witnessing $(\rho,r)\in\tau$. Since $s\leq r$ and $s\in G$, upward closure gives $r\in G$. The assumed equality truth lemma gives $\sigma^G=\rho^G$, while $r\in G$ gives $\rho^G\in\tau^G$. Combining both directions,

$$
\boxed{\sigma^G\in\tau^G\ \Longleftrightarrow\ \exists p\in G\ (p\Vdash^*\sigma\in\tau).}
$$

This completes the [atomic membership truth lemma for forcing](../../../../../../../atomic-membership-truth-lemma-for-forcing.md); no separate assumption of the membership truth lemma was made.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [3](../../../3.md)
4. [Paper 121](../../../../paper-121-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
