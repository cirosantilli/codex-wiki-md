<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [complex structure](../../../../../../complex-structure.md) splits the complexified [cotangent bundle](../../../../../../cotangent-bundle.md) into its $(1,0)$ and $(0,1)$ parts. Thus the space of smooth [differential forms of type (p, q)](../../../../../../differential-form-of-type-p-q.md) is

$$
\boxed{\mathcal A^{p,q}(M)=\Gamma\left(M,\bigwedge^p(T^{1,0}M)^*\otimes\bigwedge^q(T^{0,1}M)^*\right).}
$$

Here $\Gamma$ denotes smooth [sections of a vector bundle](../../../../../../section-of-a-vector-bundle.md); exterior multiplication identifies the displayed bundle with a subbundle of the complexified exterior algebra. In [holomorphic coordinates](../../../../../../holomorphic-coordinate.md), such a [differential form of type (p, q)](../../../../../../differential-form-of-type-p-q.md) has the expression

$$
\alpha=\sum_{|I|=p,\,|J|=q}a_{IJ}(z,\bar z)\,dz_I\wedge d\bar z_J,
$$

where the coefficients are smooth and both multi-indices are increasing. Negative bidegrees, or bidegrees exceeding the complex dimension, give the zero space.

On a [complex manifold](../../../../../../complex-manifold.md), the [exterior derivative](../../../../../../exterior-derivative.md) has just two type components, $d=\partial+\bar\partial$. The [conjugate Dolbeault operator](../../../../../../conjugate-dolbeault-operator.md) and the [Dolbeault operator](../../../../../../dolbeault-operator.md) are, respectively,

$$
\partial\alpha=\sum_{I,J,k}\frac{\partial a_{IJ}}{\partial z_k}\,dz_k\wedge dz_I\wedge d\bar z_J,
\qquad
\bar\partial\alpha=\sum_{I,J,k}\frac{\partial a_{IJ}}{\partial\bar z_k}\,d\bar z_k\wedge dz_I\wedge d\bar z_J.
$$

Keeping the differentiating factor at the front fixes the signs. These definitions are intrinsic because holomorphic coordinate changes preserve type. **The two operators are the type projections of the exterior derivative**, raising $p$ and $q$, respectively.

For a [holomorphic map](../../../../../../holomorphic-map.md) $f:M\to N$, its differential is a [complex-linear map](../../../../../../complex-linear-map.md), so the [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) sends $(1,0)$ covectors to $(1,0)$ covectors and $(0,1)$ covectors to $(0,1)$ covectors. In coordinates $w$ on $N$,

$$
f^*dw_a=\sum_j\frac{\partial f_a}{\partial z_j}dz_j,
\qquad f^*d\bar w_a=\sum_j\overline{\frac{\partial f_a}{\partial z_j}}d\bar z_j.
$$

The [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) commutes with the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md), so it preserves the counts of these factors. Consequently

$$
\boxed{f^*:\mathcal A^{p,q}(N)\longrightarrow\mathcal A^{p,q}(M).}
$$

It also commutes separately with the [Dolbeault operator](../../../../../../dolbeault-operator.md) and the [conjugate Dolbeault operator](../../../../../../conjugate-dolbeault-operator.md), because it commutes with $d$ and preserves type.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
