<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

On an oriented pseudo-Riemannian vector space $(\mathbb R^n,\eta,\operatorname{vol})$, the [Hodge star operator](../../../../../hodge-star-operator.md) is the unique linear map

$$
*:\Lambda^p\longrightarrow\Lambda^{n-p}
$$

satisfying

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle_\eta\operatorname{vol}
$$

for all $p$-forms $\alpha,\beta$. If $s$ is the number of negative metric directions, then

$$
*^2=(-1)^{p(n-p)+s}
$$

on $p$-forms under this convention. For the two-forms in the question,

$$
\sigma\wedge\mu=(*\sigma)\wedge\mu
=\langle\mu,\sigma\rangle_\eta\operatorname{vol},
$$

whereas

$$
\sigma\wedge\mu=-\sigma\wedge(*\mu)
=-\langle\sigma,\mu\rangle_\eta\operatorname{vol}.
$$

The induced inner product is symmetric, so these expressions are negatives of one another. Hence a [self-dual differential form](../../../../../self-dual-differential-form.md) and an [anti-self-dual differential form](../../../../../anti-self-dual-differential-form.md) are orthogonal and

$$
\boxed{\sigma\wedge\mu=0}.
$$

Write $w=x^1+ix^2$ and $z=x^3+ix^4$. The metric is conformal to the standard Euclidean metric, and the [Hodge star on middle-degree differential forms is conformally invariant](../../../../../hodge-star-on-middle-degree-differential-forms-is-conformally-invariant.md). Taking $e^{ij}=dx^i\wedge dx^j$, the three real forms are

$$
\omega_1=e^{13}-e^{24},
\qquad
\omega_2=e^{14}+e^{23},
\qquad
\omega_3=2(e^{12}+e^{34}),
$$

because $\omega_1+i\omega_2=dw\wedge dz$. For the orientation specified by  
$dw\wedge dz\wedge d\bar w\wedge d\bar z$, one has

$$
*e^{13}=-e^{24},\qquad
*e^{14}=e^{23},\qquad
*e^{12}=e^{34}.
$$

The corresponding relations for the complementary basis forms immediately give

$$
\boxed{*\omega_k=\omega_k,\qquad k=1,2,3}.
$$

Thus these forms give a real basis of the self-dual two-forms.

Let $D_\alpha=\partial_\alpha+A_\alpha$ be the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md). In these complex coordinates the [Anti-self-dual Yang-Mills equations](../../../../../anti-self-dual-yang-mills-equations.md) are

$$
F_{wz}=0,\qquad
F_{\bar w\bar z}=0,\qquad
F_{w\bar w}+F_{z\bar z}=0.
$$

Introduce the [spectral parameter](../../../../../spectral-parameter.md) $\lambda$ and the linear operators

$$
L(\lambda)=D_w-\lambda D_{\bar z},
\qquad
M(\lambda)=D_z+\lambda D_{\bar w}.
$$

Their commutator is

$$
[L,M]
=F_{wz}
+\lambda(F_{w\bar w}+F_{z\bar z})
+\lambda^2F_{\bar w\bar z}.
$$

Therefore the [Lax pair for the anti-self-dual Yang-Mills equations](../../../../../lax-pair-for-the-anti-self-dual-yang-mills-equations.md)

$$
L(\lambda)\Psi=0,\qquad M(\lambda)\Psi=0
$$

is compatible for every $\lambda$ exactly when the ASDYM equations hold.

In particular, $F_{wz}=0$ says that the connection restricted to each $(w,z)$ surface is a [flat connection](../../../../../flat-connection.md). On a simply connected coordinate patch, the compatible equations

$$
(\partial_w+A_w)g=0,
\qquad
(\partial_z+A_z)g=0
$$

have an invertible solution $g$. Applying the associated [gauge transformation](../../../../../gauge-transformation.md) sets

$$
\boxed{A_w=A_z=0}.
$$

This conclusion is local; global topology can obstruct a single such gauge over the whole space.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
