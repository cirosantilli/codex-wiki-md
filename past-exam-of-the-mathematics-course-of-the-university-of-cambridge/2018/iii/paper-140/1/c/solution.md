<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There is an [orientation](../../../../../../orientation-of-a-simplex.md) convention in this statement: the two [volume forms](../../../../../../volume-form.md) must be positive for one fixed [orientation](../../../../../../orientation-of-a-simplex.md), as is usual in [Moser theorem for volume forms](../../../../../../moser-theorem-for-volume-forms.md). Without that convention, the stated necessity is false. For example, on an oriented [two-sphere](../../../../../../two-sphere.md), take a positive [volume form](../../../../../../volume-form.md) $\beta_0$ and an [orientation-reversing diffeomorphism](../../../../../../orientation-reversing-diffeomorphism.md) $r$, and set $\beta_1=r^*\beta_0$. Then $(r^{-1})^*\beta_1=\beta_0$ but $\int\beta_1=-\int\beta_0$. We prove the intended result with a common [orientation](../../../../../../orientation-of-a-simplex.md).

If $\phi^*\beta_1=\beta_0$, positivity forces $\phi$ to preserve the [orientation](../../../../../../orientation-of-a-simplex.md), and integration of the [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) gives equality of the integrals.

For sufficiency, [top-degree de Rham cohomology](../../../../../../top-degree-de-rham-cohomology.md) gives a [differential form](../../../../../../differential-form-split.md) $\alpha$ of degree $n-1$ with $\beta_1-\beta_0=d\alpha$. Put $\beta_t=(1-t)\beta_0+t\beta_1$. Positivity makes every $\beta_t$ a [volume form](../../../../../../volume-form.md). The [interior product of a differential form](../../../../../../interior-product.md) gives an [linear isomorphism](../../../../../../linear-isomorphism.md)

$$
T_pM\longrightarrow\Lambda^{n-1}T_p^*M,\qquad v\longmapsto\iota_v\beta_t.
$$

Thus there is a unique smooth time-dependent [vector field](../../../../../../vector-field.md) $X_t$ satisfying $\iota_{X_t}\beta_t=-\alpha$. Since $M$ is [compact](../../../../../../compact-space.md), its [local flow](../../../../../../local-flow.md) exists throughout $0\leq t\leq1$ and defines a [smooth isotopy](../../../../../../smooth-isotopy.md) $\phi_t$ starting at the identity. By [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md), and since a top-degree [differential form](../../../../../../differential-form-split.md) has zero [exterior derivative](../../../../../../exterior-derivative.md),

$$
\frac{d}{dt}\phi_t^*\beta_t
=\phi_t^*\bigl(d\alpha+\mathcal L_{X_t}\beta_t\bigr)
=\phi_t^*\bigl(d\alpha+d\iota_{X_t}\beta_t\bigr)=0.
$$

Hence

$$
\boxed{\phi_1^*\beta_1=\beta_0.}
$$

The zero-dimensional case, a single point, is immediate from equality of the integrals.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 140](../../../paper-140-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
