<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $J:\mathcal C\hookrightarrow\mathcal B$ exhibit a [reflective subcategory](../../../../../../reflective-subcategory.md), with [reflector](../../../../../../reflector.md) $K$, and let $E:I\to\mathcal C$ be a small [diagram in a category](../../../../../../diagram-category-theory.md). Completeness of $\mathcal B$ gives a [categorical limit](../../../../../../categorical-limit.md) $L$ of $JE$. For every $B'\in\mathcal B$, the [universal property](../../../../../../universal-property.md) of this [categorical limit](../../../../../../categorical-limit.md) and the reflection [adjunction](../../../../../../adjoint-functors.md) give

$$
\begin{aligned}
\mathcal B(JKB',L)
&\cong\lim_i\mathcal B(JKB',JE_i)\\
&\cong\lim_i\mathcal B(B',JE_i)\\
&\cong\mathcal B(B',L).
\end{aligned}
$$

The composite is precomposition with $\rho_{B'}$, so $L$ satisfies the [hom-set](../../../../../../hom-set.md) condition from the preceding part. Its proof of invertibility of $\rho_L$ did not require repleteness. Thus $L\cong JKL$ whether or not the chosen full reflective subcategory is replete.

Transport the ambient limit cone along $\rho_L^{-1}:JKL\to L$. Its legs lie in the [full subcategory](../../../../../../full-subcategory.md), and their ambient [universal property](../../../../../../universal-property.md), restricted to objects of $\mathcal C$, is exactly the internal [categorical limit](../../../../../../categorical-limit.md) property. Hence **every small diagram in the reflective subcategory has a limit**:

$$
\boxed{\mathcal C\text{ is complete, with a chosen limit }KL.}
$$

For a [replete subcategory](../../../../../../replete-subcategory.md), the ambient limit object $L$ itself belongs to $\mathcal C$. This argument includes the empty diagram and requires no limit-preservation hypothesis on the [reflector](../../../../../../reflector.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
