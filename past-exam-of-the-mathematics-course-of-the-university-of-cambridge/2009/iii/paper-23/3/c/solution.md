<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Yoneda embedding](../../../../../../yoneda-embedding.md) preserves [categorical products](../../../../../../product-category-theory.md): for any $a$, maps $a\to c\times Y$ correspond naturally to pairs of maps $a\to c$ and $a\to Y$. Hence $H_{c\times Y}\cong H_c\times H_Y$. Using the [exponential in a presheaf category](../../../../../../exponential-in-a-presheaf-category.md), the [Yoneda lemma](../../../../../../yoneda-lemma.md) and the exponential [universal property](../../../../../../universal-property.md) in $\mathcal C$ gives

$$
\begin{aligned}
((H_Z)^{H_Y})(c)
&=\operatorname{Nat}(H_c\times H_Y,H_Z)\\
&\cong\operatorname{Nat}(H_{c\times Y},H_Z)\\
&\cong\mathcal C(c\times Y,Z)\\
&\cong\mathcal C(c,Z^Y)=H_{Z^Y}(c).
\end{aligned}
$$

Every [bijection](../../../../../../bijection.md) is natural in $c$, since it is given by precomposition or the natural exponential [adjunction](../../../../../../adjoint-functors.md). Thus these component [bijections](../../../../../../bijection.md) are a [natural isomorphism](../../../../../../natural-isomorphism.md) of [categorical presheaves](../../../../../../presheaf-category-theory.md):

$$
\boxed{(H_Z)^{H_Y}\cong H_{Z^Y}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
