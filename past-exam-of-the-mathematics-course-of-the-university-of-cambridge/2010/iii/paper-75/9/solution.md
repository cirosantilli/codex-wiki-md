<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

A [classifying topos](../../../../../classifying-topos.md) for a [coherent theory](../../../../../coherent-theory.md) $\mathbb T$ is a [Grothendieck topos](../../../../../grothendieck-topos.md) $\mathcal B_{\mathbb T}$ with a generic model $U$ such that, for every Grothendieck topos $\mathcal S$, inverse image gives an equivalence

$$
\boxed{\operatorname{Geom}(\mathcal S,\mathcal B_{\mathbb T})
\simeq\mathbb T\text{-}\operatorname{Mod}(\mathcal S),\qquad
f\longmapsto f^*U},
$$

pseudonatural in $\mathcal S$. The equivalence includes model homomorphisms and geometric transformations, not merely a bijection between isomorphism classes of set-based models.

Construct the [coherent syntactic category](../../../../../coherent-syntactic-category.md) $\mathcal C_{\mathbb T}$. Its objects are coherent formulas in finite contexts, modulo provable equivalence, and an arrow is a provably total single-valued coherent relation between their contexts. Composition existentially quantifies the intermediate tuple. Context concatenation, conjunction and equality give [finite limits](../../../../../finite-limit.md); existential quantification gives stable images; finite disjunction gives stable finite unions. Thus it is a small [coherent category](../../../../../coherent-category.md), after choosing representatives.

Equip it with the [coherent topology](../../../../../coherent-topology.md) $J$: a finite family $C_i\to C$ covers when the union of its images is the whole object, equivalently when the associated finite existential disjunction is provable from the target formula. Pullback stability and closure of covers under composition follow from the corresponding properties of images and unions. Set

$$
\boxed{\mathcal B_{\mathbb T}=\operatorname{Sh}(\mathcal C_{\mathbb T},J)}.
$$

The functor $a y:\mathcal C_{\mathbb T}\to\mathcal B_{\mathbb T}$, consisting of the [Yoneda embedding](../../../../../yoneda-embedding.md) followed by [sheafification](../../../../../sheafification.md), interprets each sort, function and relation of the syntax and yields the generic model $U$. It preserves finite limits, images and finite unions: syntactic covers become epimorphic families after sheafification, and the syntactic image factorization thus becomes the image factorization of the corresponding arrow. All the axioms consequently hold in $U$.

Here is the classifying argument. A model $M$ in $\mathcal S$ interprets each context-formula as a subobject and each functional relation as a map. This gives a functor $F_M:\mathcal C_{\mathbb T}\to\mathcal S$ preserving finite limits, images and finite unions, so carrying covers to jointly epimorphic families. Conversely such an interpretation functor recovers exactly a model and all its formula interpretations. Because the source category has finite limits, a finite-limit-preserving functor is [flat](../../../../../flat-module.md); cover preservation says that it is $J$-continuous.

For explicitness, the associated inverse image is the flat tensor extension

$$
P\longmapsto P\otimes_{\mathcal C_{\mathbb T}}F_M
=\int^{C\in\mathcal C_{\mathbb T}}P(C)\cdot F_M(C),
$$

where a set of sections indexes a coproduct and the coend identifies the two actions of every arrow. Flatness makes this extension preserve finite limits. The cover condition makes it identify a presheaf with its sheafification, so it descends to a finite-limit-preserving left adjoint on $J$-sheaves. Its right adjoint sends $N\in\mathcal S$ to $C\mapsto\operatorname{Hom}_{\mathcal S}(F_M(C),N)$; this is a sheaf because matching maps along an interpreted covering family glue uniquely across its jointly epimorphic cover. This is the [Diaconescu equivalence for geometric morphisms](../../../../../diaconescu-equivalence-for-geometric-morphisms.md), with its actual functors displayed.

The resulting geometric inverse image satisfies $f^*(ayC)\cong F_M(C)$, hence $f^*U\cong M$. Conversely any inverse image preserves finite limits and colimits, hence images and unions, and its composite with $ay$ is the interpretation functor of $f^*U$. Since the sheafified representables generate the topos, these constructions recover the geometric morphism up to its unique appropriate isomorphism. Natural transformations of interpretation functors correspond to the model homomorphisms and geometric transformations. This proves the required equivalence and the construction's classifying property.

## ↑ Ancestors (10)

1. [9](../9.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
