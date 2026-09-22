<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a locally small [category](../../../../../category-split.md) $\mathcal C$, an object $A$, and a [functor](../../../../../functor.md) $F:\mathcal C\to\mathbf{Set}$, the covariant form of the [Yoneda lemma](../../../../../yoneda-lemma.md) is the natural [bijection](../../../../../bijection.md)

$$
\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A),\qquad \alpha\longmapsto\alpha_A(1_A).
$$

For $x\in F(A)$ define $\alpha^x_B(f)=F(f)(x)$, where $f:A\to B$. For $u:B\to D$, functoriality gives $F(u)\alpha^x_B(f)=F(uf)(x)=\alpha^x_D(uf)$, so this is a [natural transformation](../../../../../natural-transformation.md). Conversely, naturality of $\alpha$ at $f:A\to B$ gives $\alpha_B(f)=F(f)\alpha_A(1_A)$. The two constructions are inverse. They are natural in $F$, because a [natural transformation](../../../../../natural-transformation.md) $F\Rightarrow G$ commutes with evaluation. They are also natural in $A$: an arrow $v:A'\to A$ induces $\mathcal C(A,-)\to\mathcal C(A',-)$ by precomposition, and the resulting map $\operatorname{Nat}(\mathcal C(A',-),F)\to\operatorname{Nat}(\mathcal C(A,-),F)$ corresponds to $F(v):F(A')\to F(A)$. Applying the result to the [opposite category](../../../../../opposite-category.md) gives $\operatorname{Nat}(\mathcal C(-,A),H)\cong H(A)$ for $H:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$.

Now let $\mathcal C$ be a [small category](../../../../../small-category.md), and let $F,G:\mathcal C\to\mathbf{Set}$. Finite [products in a category](../../../../../product-category-theory.md) in $[\mathcal C,\mathbf{Set}]$ exist pointwise; the terminal [functor](../../../../../functor.md) is the constant singleton [functor](../../../../../functor.md). Define the [exponential of covariant set-valued functors](../../../../../exponential-of-covariant-set-valued-functors.md) by

$$
(G^F)(C)=\operatorname{Nat}(\mathcal C(C,-)\times F,G).
$$

Smallness ensures that these [natural transformations](../../../../../natural-transformation.md) form a set. For $u:C\to D$, define $(G^F)(u)(\alpha)$ at $E$ by

$$
\bigl((G^F)(u)(\alpha)\bigr)_E(v,x)=\alpha_E(vu,x),\qquad v:D\to E.
$$

Precomposition respects identities and composition, so this defines a [functor](../../../../../functor.md). Its [evaluation map of an exponential object](../../../../../evaluation-map-of-an-exponential-object.md) is

$$
\mathrm{ev}_C:(G^F)(C)\times F(C)\to G(C),\qquad (\alpha,x)\mapsto\alpha_C(1_C,x).
$$

To check naturality, for $u:C\to D$ both sides give $\alpha_D(u,F(u)x)$: one side uses naturality of $\alpha$, and the other uses the defining action of $G^F$.

Here is the full [universal property](../../../../../universal-property.md). Given $\theta:H\times F\Rightarrow G$, define $\widehat\theta:H\Rightarrow G^F$ by

$$
\bigl(\widehat\theta_C(h)\bigr)_D(v,x)=\theta_D(H(v)h,x),\qquad v:C\to D.
$$

For $w:D\to E$, naturality of $\theta$ makes this commute with $G(w)$, so $\widehat\theta_C(h)$ is a [natural transformation](../../../../../natural-transformation.md). Replacing $h$ by $H(u)h$ is the same as precomposing $v$ by $u$, proving naturality in $C$. Conversely, $\beta:H\Rightarrow G^F$ gives $\theta_C(h,x)=\beta_C(h)_C(1_C,x)$. Starting with $\theta$ recovers it immediately. Starting with $\beta$, its naturality at $v:C\to D$ yields

$$
\beta_D(H(v)h)_D(1_D,x)=\beta_C(h)_D(v,x),
$$

so it too is recovered. The formulas are natural in $H$ and $G$, giving the required [adjunction](../../../../../adjoint-functors.md) $(-)\times F\dashv(-)^F$. Therefore **the covariant functor category is cartesian closed**. This proof supplies the actual exponential and does not need a colimit presentation of its arguments.

Finally suppose $\mathcal C$ itself is a [small category](../../../../../small-category.md) which is a [Cartesian closed category](../../../../../cartesian-closed-category.md). In its [presheaf category](../../../../../presheaf-category.md), the same construction, applied to $\mathcal C^{\mathrm{op}}$, gives

$$
\begin{aligned}
((YB)^{YA})(C)
&=\operatorname{Nat}(YC\times YA,YB)\\
&\cong\operatorname{Nat}(Y(C\times A),YB)\\
&\cong\mathcal C(C\times A,B)\\
&\cong\mathcal C(C,B^A)\\
&=Y(B^A)(C).
\end{aligned}
$$

The first [isomorphism](../../../../../isomorphism.md) uses the product's [universal property](../../../../../universal-property.md): a map into $C\times A$ is precisely a pair of maps into $C$ and $A$. The next is the [Yoneda lemma](../../../../../yoneda-lemma.md), and the last is the exponential [adjunction](../../../../../adjoint-functors.md) in $\mathcal C$. Each step is natural in $C$, $A$, and $B$. Under these identifications, evaluation corresponds to $Y$ of the evaluation $B^A\times A\to B$. Hence **the Yoneda embedding preserves exponentials**, with the natural identification $\boxed{Y(B^A)\cong(YB)^{YA}}$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
