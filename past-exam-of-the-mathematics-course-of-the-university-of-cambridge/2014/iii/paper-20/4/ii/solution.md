<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [representable functor](../../../../../../representable-functor.md) $yC$ is an [indecomposable projective object](../../../../../../indecomposable-projective-object.md). Given an [epimorphism](../../../../../../epimorphism.md) $\coprod_iB_i\twoheadrightarrow yC$, evaluate at $C$. [Epimorphisms](../../../../../../epimorphism.md) and [coproducts](../../../../../../coproduct.md) in a [presheaf category](../../../../../../presheaf-category.md) are pointwise, so $1_C\in yC(C)$ is the image of some element of a particular $B_i(C)$. By the [Yoneda lemma](../../../../../../yoneda-lemma.md), that element defines $s:yC\to B_i$, and its composite into $yC$ corresponds to $1_C$, hence is the identity. The selected component is split epic. More generally, evaluation sends any epimorphism to a surjection, so a map from $yC$ lifts through any epimorphism; this also proves its ordinary projectivity.

Conversely, every presheaf $A$ has the canonical [epimorphism](../../../../../../epimorphism.md)

$$
\coprod_{(C,x),\ x\in A(C)}yC\twoheadrightarrow A,
$$

whose component is the [natural transformation](../../../../../../natural-transformation.md) named by $x$. It is pointwise surjective, since an element at $D$ is reached from its own summand $(D,x)$ at $1_D$. If $A$ is indecomposable projective, one component $r:yC\to A$ has a section $s:A\to yC$. The endomorphism $sr$ of $yC$ is idempotent and therefore corresponds to an [idempotent morphism](../../../../../../idempotent-morphism.md) $e:C\to C$.

If idempotents split in $\mathcal C$, choose $C\xrightarrow{p}D\xrightarrow{i}C$ with $ip=e$, $pi=1_D$. Then $A\cong yD$: the mutually inverse maps are $y(p)s:A\to yD$ and $r\,y(i):yD\to A$. Thus

$$
\boxed{\text{indecomposable projectives are exactly representables when idempotents split}.}
$$

Without that hypothesis the argument still proves that every such object is a retract of a [representable](../../../../../../representable-functor.md). The initial presheaf is not indecomposable projective, since its identity is the empty-[coproduct](../../../../../../coproduct.md) [epimorphism](../../../../../../epimorphism.md) and has no component to select.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
