<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [Cartesian closed category](../../../../../../cartesian-closed-category.md) has finite [categorical products](../../../../../../product-category-theory.md) and, for every $P,Q$, an [exponential object](../../../../../../exponential-object.md) $Q^P$ with an evaluation [morphism](../../../../../../morphism.md) $\operatorname{ev}:Q^P\times P\to Q$ such that composition with evaluation gives [natural bijections](../../../../../../natural-bijection.md)

$$
\mathcal E(R,Q^P)\cong\mathcal E(R\times P,Q).
$$

Finite [categorical products](../../../../../../product-category-theory.md) in the [presheaf category](../../../../../../presheaf-category.md) are pointwise; in particular its [terminal object](../../../../../../terminal-object.md) is the constant singleton [categorical presheaf](../../../../../../presheaf-category-theory.md). For [categorical presheaves](../../../../../../presheaf-category-theory.md) $P,Q$ define

$$
\boxed{(Q^P)(c)=\operatorname{Nat}(H_c\times P,Q).}
$$

For $u:d\to c$, restriction sends $\alpha$ to $\alpha\circ(H_u\times1_P)$. Composition and identity laws follow from those of the [Yoneda embedding](../../../../../../yoneda-embedding.md), so this is a [categorical presheaf](../../../../../../presheaf-category-theory.md).

Define evaluation at $c$ by $\operatorname{ev}_c(\alpha,x)=\alpha_c(1_c,x)$. For $u:d\to c$, [naturality](../../../../../../naturality.md) of $\alpha$ gives $Q(u)\alpha_c(1_c,x)=\alpha_d(u,P(u)x)$, which is the evaluation of the restricted pair. Hence evaluation is a [natural transformation](../../../../../../natural-transformation.md).

Given $t:R\times P\to Q$, its [currying](../../../../../../currying.md) sends $z\in R(c)$ to the transformation whose component at $a$ is

$$
(\widehat t_c(z))_a(v,x)=t_a(R(v)z,x)\qquad(v:a\to c,\ x\in P(a)).
$$

[Naturality](../../../../../../naturality.md) in $a$ follows from that of $t$, and [naturality](../../../../../../naturality.md) in $c$ follows by composing $v$ with the relevant arrow. Evaluating $\widehat t$ at $(1_c,x)$ recovers $t_c(z,x)$. Conversely, if $s:R\to Q^P$, [naturality](../../../../../../naturality.md) of $s$ along $v:a\to c$ says that evaluating $s_a(R(v)z)$ at $(1_a,x)$ gives $(s_c(z))_a(v,x)$. Thus [currying](../../../../../../currying.md) the evaluation of $s$ recovers $s$. These constructions are inverse and natural, proving the [universal property](../../../../../../universal-property.md). This is the [exponential in a presheaf category](../../../../../../exponential-in-a-presheaf-category.md), and proves **the [presheaf category](../../../../../../presheaf-category.md) is [Cartesian closed](../../../../../../cartesian-closed-category.md)**.

## ↑ Ancestors (11)

1. [B](../b.md)
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
