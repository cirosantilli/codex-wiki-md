<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write the [Yoneda embedding](../../../../../../yoneda-embedding.md) as $h:\mathcal C\to\widehat{\mathcal C}$. For any finite [product in a category](../../../../../../product-category-theory.md), its [universal property](../../../../../../universal-property.md) gives

$$
h_{A\times B}(D)=\mathcal C(D,A\times B)
\cong\mathcal C(D,A)\times\mathcal C(D,B),\qquad h_1(D)\cong1.
$$

These [bijections](../../../../../../bijection.md) are natural, so $h$ preserves finite products. Now use the [exponential in a presheaf category](../../../../../../exponential-in-a-presheaf-category.md), followed by the [Yoneda lemma](../../../../../../yoneda-lemma.md) and the [exponential object](../../../../../../exponential-object.md) property in $\mathcal C$:

$$
\begin{aligned}
(h_B)^{h_A}(D)
&=\operatorname{Nat}(h_D\times h_A,h_B)\\
&\cong\operatorname{Nat}(h_{D\times A},h_B)\\
&\cong\mathcal C(D\times A,B)\\
&\cong\mathcal C(D,B^A)=h_{B^A}(D).
\end{aligned}
$$

Every step is natural in $D$, so these component [bijections](../../../../../../bijection.md) form a [natural isomorphism](../../../../../../natural-isomorphism.md)

$$
\boxed{h_{B^A}\cong(h_B)^{h_A}.}
$$

Under this isomorphism, the image of the evaluation $B^A\times A\to B$ is the presheaf evaluation: both correspond to the same identity of the exponential under the transpose [bijection](../../../../../../bijection.md). Thus the [Yoneda embedding preserves exponentials](../../../../../../yoneda-embedding-preserves-exponentials.md), including their evaluation maps.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
