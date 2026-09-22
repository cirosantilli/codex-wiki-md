<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The Yoneda embedding is an exact representation of a category, but does not by itself reduce the subject to the study of arbitrary functor categories.** There are both a size issue and a structure issue.

Let $\mathcal A$ be a [locally small category](../../../../../locally-small-category.md) and set $yA=\mathcal A(-,A)$. For a [categorical presheaf](../../../../../presheaf-category-theory.md) $P:\mathcal A^{\mathrm{op}}\to\mathbf{Set}$, a [natural transformation](../../../../../natural-transformation.md) $\theta:yA\to P$ is determined by $x=\theta_A(1_A)$. Indeed, naturality along $f:B\to A$ forces

$$
\theta_B(f)=P(f)(x).
$$

Conversely this formula defines a natural transformation for each $x\in P(A)$, since functoriality gives naturality along every $g:C\to B$. Taking $P=yA'$ gives

$$
\boxed{\operatorname{Nat}(yA,yA')\cong\mathcal A(A,A').}
$$

Thus the [Yoneda embedding](../../../../../yoneda-embedding.md) is [full and faithful](../../../../../full-and-faithful-functor.md), and $\mathcal A$ is equivalent to its [full subcategory](../../../../../full-subcategory.md) of [representable presheaves](../../../../../representable-functor.md). The indexing [category](../../../../../category-split.md) in the usual version is $\mathcal A^{\mathrm{op}}$, not necessarily a small category chosen independently of $\mathcal A$.

Local smallness makes the values $\mathcal A(B,A)$ [sets](../../../../../set-split.md); it does not make the collection of objects a set. For a large indexing category, the collection of [natural transformations](../../../../../natural-transformation.md) between arbitrary set-valued [functors](../../../../../functor.md) can itself be a proper class. For example, take the discrete category on the class of ordinals and the constant two-element functor. Its endomorphisms include an independently chosen function $\{0,1\}\to\{0,1\}$ at each ordinal. A small functor category cannot encode this collection without changing universes. The [Yoneda lemma](../../../../../yoneda-lemma.md) remains meaningful when the source is representable because the displayed bijection identifies its natural transformations with a set. It does not make the entire large functor category locally small.

Even for a [small category](../../../../../small-category.md), the representable image is usually a very special part of its [presheaf category](../../../../../presheaf-category.md). If $\mathcal A$ is the terminal category, its presheaf category is $\mathbf{Set}$, but its representable image consists only of a singleton. The presheaf category has all small [categorical limits](../../../../../categorical-limit.md) and [colimits](../../../../../colimit.md), whereas an arbitrary full subcategory need have almost none. The Yoneda embedding preserves existing limits because [representable functors](../../../../../representable-functor.md) preserve limits. It generally does not preserve colimits. For example, the coproduct of two singleton sets in [category of finite sets](../../../../../category-of-finite-sets.md) is a two-element set, but evaluating the proposed presheaf coproduct at a two-element set gives

$$
|(y1\amalg y1)(2)|=2,\qquad |y(1\amalg1)(2)|=4.
$$

The pointwise coproduct therefore leaves the representable image. Identifying which presheaves are representable, and which ambient constructions return to the original category, is precisely substantive [category theory](../../../../../category-theory-split.md).

The representation is nonetheless powerful. The [Yoneda lemma](../../../../../yoneda-lemma.md) replaces a morphism by all its probes, converts a [universal property](../../../../../universal-property.md) into a [representation of a functor](../../../../../representation-of-a-functor.md), and makes the presheaf category a natural place to add formal [colimits](../../../../../colimit.md). A small presheaf category is the free [free cocompletion](../../../../../free-cocompletion.md) under small colimits: every presheaf is a colimit of representables indexed by its [category of elements](../../../../../category-of-elements.md). But this is a controlled enlargement of the category, not an identification of its original objects with all functors. The stronger conclusion in the proposed assertion therefore does not follow from the full-faithfulness statement.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
