<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The key fact is that the extra [left adjoint](../../../../../../adjoint-functors.md) $f_!$ sends each [representable](../../../../../../representable-functor.md) $yC$ to an [indecomposable projective object](../../../../../../indecomposable-projective-object.md). Let $\coprod_iB_i\twoheadrightarrow f_!yC$ be epic. The inverse image $f^*$ preserves [epimorphisms](../../../../../../epimorphism.md) and [coproducts](../../../../../../coproduct.md), because it is a [left adjoint](../../../../../../adjoint-functors.md) between toposes. Apply it and lift the unit $\eta:yC\to f^*f_!yC$ through the resulting [epimorphism](../../../../../../epimorphism.md), using projectivity of $yC$. A map from $yC$ to a [coproduct](../../../../../../coproduct.md) selects one component, by evaluation at $C$ and the [Yoneda lemma](../../../../../../yoneda-lemma.md). Thus for some $i$ we obtain $t:yC\to f^*B_i$ with $f^*(B_i\to f_!yC)t=\eta$.

Transpose $t$ across $f_!\dashv f^*$ to $\bar t:f_!yC\to B_i$. The displayed equality says that its composite back to $f_!yC$ is the identity. This proves the required indecomposable-projective property.

Since idempotents split in $\mathcal D$, part (ii) supplies objects $FC\in\mathcal D$ and isomorphisms $f_!yC\cong y(FC)$. Full faithfulness of the [Yoneda embedding](../../../../../../yoneda-embedding.md) transports the action of $f_!$ on [representable](../../../../../../representable-functor.md) arrows to a functor $F:\mathcal C\to\mathcal D$. For $P\in\widehat{\mathcal D}$,

$$
(f^*P)(C)\cong\operatorname{Hom}(yC,f^*P)\cong\operatorname{Hom}(f_!yC,P)\cong P(FC).
$$

These identifications are natural in both $C$ and $P$. Hence

$$
\boxed{f^*\cong(-)\circ F^{\mathrm{op}}.}
$$

Its [right adjoint](../../../../../../adjoint-functors.md) is consequently the right Kan extension from part (i), uniquely up to natural isomorphism. Thus the entire [geometric morphism](../../../../../../geometric-morphism.md) is induced by $F$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Section B](../../section-b.md)
4. [Paper 20](../../../paper-20-split.md)
5. [Iii](../../../split.md)
6. [2014](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
