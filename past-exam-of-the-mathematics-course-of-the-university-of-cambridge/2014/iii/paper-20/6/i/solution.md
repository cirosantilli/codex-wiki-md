<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\mathcal A=\mathbb T_{fp}$ be a small skeleton of the [finitely presented models of an algebraic theory](../../../../../../finitely-presented-models-of-an-algebraic-theory.md). The [classifying topos](../../../../../../classifying-topos.md) assertion means that for every [Grothendieck topos](../../../../../../grothendieck-topos.md) $\mathcal F$ there is an equivalence

$$
\boxed{\operatorname{Geom}(\mathcal F,[\mathcal A,\mathbf{Set}])\simeq\mathbb T\text{-}\operatorname{Mod}(\mathcal F),}
$$

natural under inverse image along [geometric morphisms](../../../../../../geometric-morphism.md). On the left, morphisms are transformations between inverse image functors, and on the right they are model homomorphisms. A model in $\mathcal F$ interprets the sorts by objects, the operations by arrows, and the equations by equality of the resulting arrows. Finite products suffice for these algebraic operations.

The [generic model of an algebraic theory](../../../../../../generic-model-of-an-algebraic-theory.md) is the tautological covariant functor: for each sort $S$ its component is

$$
U_S:\mathcal A\to\mathbf{Set},\qquad A\longmapsto A_S,
$$

with all operations interpreted pointwise. Pulling $U$ back by a [geometric morphism](../../../../../../geometric-morphism.md) gives its classified model. For a single-sorted theory, this is simply the underlying-set functor with its pointwise algebraic structure.

The orientation is important: $[\mathcal A,\mathbf{Set}]$ is the presheaf topos on $\mathcal A^{\mathrm{op}}$, and the generic model is covariant on finitely presented algebras. Such an algebra is a finite-generator, finite-relation presentation. In the algebraic syntactic category it corresponds to the formula imposing its relations, with arrows reversed. The finite-presentability/filtered-colimit description of algebraic models gives the above classifying equivalence; a detailed proof is not needed for this part.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [6](../../6.md)
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
