<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Cartesian closed category](../../../../../../cartesian-closed-category.md) has finite [products in a category](../../../../../../product-category-theory.md) and, for every $F$, an [exponential object](../../../../../../exponential-object.md) $G^F$ characterized naturally by

$$
\mathcal E(K\times F,G)\cong\mathcal E(K,G^F).
$$

In $[\mathcal C,\mathbf{Set}]$, finite products and the terminal functor are computed pointwise. With $h_B=\mathcal C(B,-)$, define

$$
(G^F)(B)=\operatorname{Nat}(h_B\times F,G).
$$

This is a set because $\mathcal C$ is a [small category](../../../../../../small-category.md). For $v:B\to B'$, precomposition $h_{B'}\to h_B$ induces $(G^F)(v)$ by precomposition of [natural transformations](../../../../../../natural-transformation.md), making $G^F$ a covariant [functor](../../../../../../functor.md).

Given $\alpha:K\times F\to G$, define its curry $\widehat\alpha:K\to G^F$ by

$$
\bigl(\widehat\alpha_B(y)\bigr)_C(u,x)=\alpha_C(K(u)y,x)
\qquad(u:B\to C,\ x\in F(C)).
$$

For $a:C\to C'$, naturality of $\alpha$ gives $G(a)\alpha_C(K(u)y,x)=\alpha_{C'}(K(au)y,F(a)x)$, proving that this is a [natural transformation](../../../../../../natural-transformation.md) $h_B\times F\to G$. The same formula with $u$ precomposed proves naturality of $\widehat\alpha$ in $B$.

Conversely, from $\beta:K\to G^F$ define

$$
\alpha_B(y,x)=\bigl(\beta_B(y)\bigr)_B(1_B,x).
$$

Naturality of $\beta$ and its values proves naturality of $\alpha$. Currying this result recovers $\beta$, since $\beta_C(K(u)y)=(G^F)(u)(\beta_B(y))$; uncurrying a curry recovers $\alpha$ by setting $u=1_B$. These mutually inverse constructions are natural in $K,G$, giving the adjunction required for an [exponential object](../../../../../../exponential-object.md). Therefore

$$
\boxed{[\mathcal C,\mathbf{Set}]\text{ is cartesian closed},\quad (G^F)(B)=\operatorname{Nat}(h_B\times F,G).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
