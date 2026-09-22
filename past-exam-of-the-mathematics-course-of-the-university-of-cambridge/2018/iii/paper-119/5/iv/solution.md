<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $P$ be a [tiny object](../../../../../../tiny-object.md) of $[\mathcal C,\mathbf{Set}]$, and let $0$ be the [initial object](../../../../../../initial-object.md) of $\mathcal C$. The [representable functor](../../../../../../representable-functor.md) $h_0=\mathcal C(0,-)$ is the terminal functor, since each of its values is a singleton. The exponential adjunction and the [Yoneda lemma](../../../../../../yoneda-lemma.md) give

$$
\operatorname{Nat}(P,F)\cong\operatorname{Nat}(h_0,F^P)\cong(F^P)(0).
$$

Since $P$ is tiny, $E_P:F\mapsto F^P$ is itself a [left adjoint](../../../../../../adjoint-functors.md), so preserves all [colimits](../../../../../../colimit.md). Evaluation at $0$ also preserves colimits, because they are pointwise in a set-valued [functor category](../../../../../../functor-category.md). Therefore $\operatorname{Nat}(P,-)$ preserves the coproduct construction.

It also preserves [epimorphisms](../../../../../../epimorphism.md). Indeed, every such epimorphism is a [pointwise epimorphism in a functor category](../../../../../../pointwise-epimorphism-in-a-functor-category.md), hence the [coequalizer](../../../../../../coequalizer.md) of its [kernel pair](../../../../../../kernel-pair.md), as can be checked pointwise in sets. A left adjoint preserves that coequalizer and therefore sends it to a [regular epimorphism](../../../../../../regular-epimorphism.md), which is an epimorphism; evaluation at zero preserves surjectivity. Thus $P$ is an [irreducible projective in a set-valued functor category](../../../../../../irreducible-projective-in-a-set-valued-functor-category.md).

A [Cauchy-complete category](../../../../../../cauchy-complete-category.md) is one in which every [idempotent morphism](../../../../../../idempotent-morphism.md) splits. By the characterization allowed in the question, irreducible projectives are [representable functors](../../../../../../representable-functor.md) for such an indexing category. Applying it to $P$ proves the [tiny covariant functor on a Cauchy-complete category with an initial object is representable](../../../../../../tiny-covariant-functor-on-a-cauchy-complete-category-with-an-initial-object-is-representable.md) conclusion:

$$
\boxed{P\text{ tiny}\ \Longrightarrow\ P\cong\mathcal C(A,-)\text{ for some }A.}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
