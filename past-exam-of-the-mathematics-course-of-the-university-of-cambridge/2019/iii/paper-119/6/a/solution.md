<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [locally small category](../../../../../../locally-small-category.md) $\mathcal C$, the [Yoneda lemma](../../../../../../yoneda-lemma.md) states that

$$
\operatorname{Nat}(\mathcal C(-,A),F)\cong F(A),
\qquad \alpha\longmapsto\alpha_A(1_A),
$$

naturally in both $A\in\mathcal C$ and $F:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$. Taking $F=\mathcal C(-,B)$ gives

$$
\operatorname{Nat}(yA,yB)\cong\mathcal C(A,B),
$$

so the [Yoneda embedding](../../../../../../yoneda-embedding.md) is full and faithful.

For small $\mathcal C$, the [presheaf category](../../../../../../presheaf-category.md) has pointwise finite limits and colimits, exponential

$$
(G^F)(C)=\operatorname{Nat}(yC\times F,G),
$$

and a [subobject classifier](../../../../../../subobject-classifier.md) whose elements at $C$ are sieves on $C$. Hence it is a [presheaf topos](../../../../../../presheaf-topos.md).

If $\mathcal C$ has finite limits, the Yoneda embedding preserves them: maps into a limiting object are the corresponding limits of hom-sets. Its essential image is therefore a full subcategory of the presheaf topos closed under finite limits. Since Yoneda is full and faithful, this proves the assertion up to equivalence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
