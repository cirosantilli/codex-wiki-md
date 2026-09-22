<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Morita equivalence of geometric theories](../../../../../../morita-equivalence-of-geometric-theories.md) means equivalence of their [classifying toposes](../../../../../../classifying-topos.md). Equivalently, their categories of models in every [Grothendieck topos](../../../../../../grothendieck-topos.md) are equivalent pseudonaturally with respect to inverse image. Agreement only of their set-based model categories, without this natural internal-model structure, is not the definition.

Suppose $\mathbf{Set}[\mathbb T]\simeq\mathbf{Set}[\mathbb S]=\mathcal E$. A property expressed intrinsically in terms of the topos is the same under either presentation. One can therefore translate a [site](../../../../../../site-category-theory.md) or logical characterization of that property from $\mathbb T$ into one for $\mathbb S$. Examples include Booleanity, connectedness, atomicity and the structure of the [subtopos](../../../../../../subtopos.md) lattice. The bridge is the common invariant $\mathcal E$, rather than an assumed literal identification of the two signatures.

The [duality between geometric quotients and subtoposes](../../../../../../duality-between-geometric-quotients-and-subtoposes.md) makes this precise. A [geometric quotient theory](../../../../../../geometric-quotient-theory.md) $\mathbb T'$ of $\mathbb T$ adds geometric axioms over the same signature. Quotients are identified when they prove the same geometric sequents. The theorem gives

$$
\boxed{\{\text{geometric quotients of }\mathbb T\}/\text{provable equivalence}
\ \longleftrightarrow\
\{\text{subtoposes of }\mathbf{Set}[\mathbb T]\}.}
$$

The [subtopos](../../../../../../subtopos.md) corresponding to $\mathbb T'$ is its [classifying topos](../../../../../../classifying-topos.md). Stronger axioms correspond to smaller [subtoposes](../../../../../../subtopos.md) under inclusion.

The [site](../../../../../../site-category-theory.md) mechanism explains the correspondence. On $\mathcal C_{\mathbb T}$, an additional sequent requires the associated family of definable images to cover its antecedent. Adding these covering sieves produces a topology $J'\supseteq J_{\mathbb T}$ and a geometric embedding

$$
\mathbf{Sh}(\mathcal C_{\mathbb T},J')\hookrightarrow
\mathbf{Sh}(\mathcal C_{\mathbb T},J_{\mathbb T}).
$$

Conversely, [subtoposes](../../../../../../subtopos.md) correspond to such larger topologies; requiring their extra definable covers gives the corresponding deductively closed quotient theory. Pulling the universal model into the [subtopos](../../../../../../subtopos.md) supplies the universal model of the quotient.

Given a quotient $\mathbb T'$, transport its [subtopos](../../../../../../subtopos.md) along the chosen equivalence of [classifying toposes](../../../../../../classifying-topos.md). Apply the duality again to obtain a quotient $\mathbb S'$ of $\mathbb S$. Their [classifying toposes](../../../../../../classifying-topos.md) are equivalent, so

$$
\boxed{\mathbb T'\text{ and }\mathbb S'\text{ are Morita-equivalent}.}
$$

This is an explicit transfer principle for whole families of theory extensions and their order relations. Intrinsic constructions such as open, closed or Boolean [subtoposes](../../../../../../subtopos.md) can likewise be described in each syntax. Different descriptions may look unrelated, but their equality is explained by the common [subtopos](../../../../../../subtopos.md). No universal translation of individual formulas is asserted without choosing the relevant equivalence and interpretations.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
