<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the covariant version of the [Yoneda embedding](../../../../../../yoneda-embedding.md), put $Y(A)=\mathcal C(A,-)$. A [morphism](../../../../../../morphism.md) $u:A\to B$ induces the [natural transformation](../../../../../../natural-transformation.md) $Y(u):Y(B)\to Y(A)$ whose component sends $v:B\to X$ to $vu$. Thus $Y$ is a [functor](../../../../../../functor.md) from the [opposite category](../../../../../../opposite-category.md) $\mathcal C^{\mathrm{op}}$ to the [functor category](../../../../../../functor-category.md) $[\mathcal C,\mathbf{Set}]$. The [locally small category](../../../../../../locally-small-category.md) hypothesis makes each value a [set](../../../../../../set-split.md).

The [Yoneda lemma](../../../../../../yoneda-lemma.md) says that, for a [functor](../../../../../../functor.md) $F:\mathcal C\to\mathbf{Set}$, evaluation at the [identity morphism](../../../../../../identity-morphism.md) gives a [natural bijection](../../../../../../natural-bijection.md)

$$
\boxed{\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A),\qquad \theta\longmapsto\theta_A(1_A).}
$$

Given $a\in F(A)$, define $\theta^a_X(v)=F(v)(a)$. For $w:X\to X'$, the [functor](../../../../../../functor.md) law gives $F(w)\theta^a_X(v)=F(wv)(a)=\theta^a_{X'}(wv)$, proving [naturality](../../../../../../naturality.md). Conversely, [naturality](../../../../../../naturality.md) of $\theta$ at $v:A\to X$ gives $\theta_X(v)=F(v)\theta_A(1_A)$. These two constructions are inverse, because $F(1_A)(a)=a$.

The [bijection](../../../../../../bijection.md) is natural in both variables. A [natural transformation](../../../../../../natural-transformation.md) $\beta:F\to H$ sends the element $a$ to $\beta_A(a)$, matching postcomposition by $\beta$. For $u:A\to B$, precomposing with $Y(u)$ sends $\theta$ to a transformation from $Y(B)$ and its distinguished element is $\theta_B(u)=F(u)(a)$. This is exactly the required dependence on $A$.

Taking $F=Y(B)$ gives $\operatorname{Nat}(Y(A),Y(B))\cong\mathcal C(B,A)$. Consequently **the covariant [Yoneda embedding](../../../../../../yoneda-embedding.md) is [full and faithful](../../../../../../full-and-faithful-functor.md)**, with the reversal of arrows accounted for by its [opposite category](../../../../../../opposite-category.md) domain.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
