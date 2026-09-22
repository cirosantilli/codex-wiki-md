<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [Cartesian closed category](../../../../../../cartesian-closed-category.md) has finite [products in a category](../../../../../../product-category-theory.md) and, for all $X,Y$, an [exponential object](../../../../../../exponential-object.md) $Y^X$ with a [natural bijection](../../../../../../natural-bijection.md)

$$
\mathcal E(Z,Y^X)\cong\mathcal E(Z\times X,Y).
$$

Equivalently the [functor](../../../../../../functor.md) $-\times X$ has a [right adjoint](../../../../../../adjoint-functors.md). Its [counit of an adjunction](../../../../../../counit-of-an-adjunction.md) is the [evaluation map of an exponential object](../../../../../../evaluation-map-of-an-exponential-object.md) $Y^X\times X\to Y$.

For the [presheaf category](../../../../../../presheaf-category.md), define the [exponential in a presheaf category](../../../../../../exponential-in-a-presheaf-category.md) by

$$
\boxed{(Y^X)(C)=\operatorname{Nat}(h_C\times X,Y).}
$$

For $f:D\to C$, its restriction sends $\alpha$ to $\alpha\circ(h_f\times1_X)$. Composition of these restriction maps follows from composition of the $h_f$, so this is a [categorical presheaf](../../../../../../presheaf-category-theory.md). Define [evaluation map of an exponential object](../../../../../../evaluation-map-of-an-exponential-object.md) by

$$
e_C(\alpha,x)=\alpha_C(1_C,x).
$$

For $f:D\to C$, naturality of $\alpha$ gives

$$
Y(f)\alpha_C(1_C,x)=\alpha_D(f,X(f)x)
=e_D\bigl((Y^X)(f)\alpha,X(f)x\bigr).
$$

Thus $e$ is a [natural transformation](../../../../../../natural-transformation.md).

Given a [natural transformation](../../../../../../natural-transformation.md) $\beta:Z\times X\to Y$, define its [currying](../../../../../../currying.md) by

$$
\widehat\beta_C(z)_D(g,x)=\beta_D(Z(g)z,x),
\qquad g:D\to C,\quad x\in X(D).
$$

[Naturality](../../../../../../naturality.md) of $\beta$ proves that $\widehat\beta_C(z)$ is a natural transformation $h_C\times X\to Y$. For $f:C'\to C$, the same formula proves that $\widehat\beta:Z\to Y^X$ is natural. Evaluating at $g=1_C$ gives $e(\widehat\beta\times1_X)=\beta$.

Conversely, if $\gamma:Z\to Y^X$ and $\beta=e(\gamma\times1_X)$, then

$$
\widehat\beta_C(z)_D(g,x)=\gamma_D(Z(g)z)_D(1_D,x)
=\gamma_C(z)_D(g,x),
$$

by naturality of $\gamma$. Hence the two constructions are inverse and natural in $Z,Y$. Products are available pointwise, including the terminal singleton presheaf, so **the presheaf category is Cartesian closed**. The exponential uses [natural transformations](../../../../../../natural-transformation.md) out of $h_C\times X$; simply exponentiating the individual values generally does not give this object.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
