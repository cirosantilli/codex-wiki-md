<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $\mathcal C$ has finite products and every [idempotent morphism](../../../../../../idempotent-morphism.md) splits. For a representable presheaf $yA$, the exponential formula gives

$$
(F^{yA})(C)
=\operatorname{Nat}(yC\times yA,F)
\cong F(C\times A).
$$

Thus exponentiation by $yA$ is precomposition with $-\times A$. Precomposition has a [Right Kan extension](../../../../../../right-kan-extension.md) as right adjoint, so every representable presheaf is a [tiny object](../../../../../../tiny-object.md).

Conversely, let $P$ be tiny. Then $(-)^P$ is a left adjoint and preserves all small [colimits](../../../../../../colimit.md). Since $\mathcal C$ has a terminal object $1$, the terminal presheaf is $y1$, and evaluation at $1$ preserves colimits. Therefore

$$
\operatorname{Nat}(P,F)
\cong\operatorname{Nat}(y1,F^P)
\cong(F^P)(1)
$$

preserves all small colimits as a functor of $F$. By the result supplied in the question, splitting idempotents implies that $P$ is representable. Hence the [representable presheaves are the tiny objects of an idempotent-complete finite-product category](../../../../../../representable-presheaves-are-the-tiny-objects-of-an-idempotent-complete-finite-product-category.md), and Yoneda identifies $\mathcal C$ with the full subcategory of tiny objects of its presheaf topos.

## ↑ Ancestors (11)

1. [C](../c.md)
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
