<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

This is a [Gaussian thermostat](../../../../../../gaussian-thermostat.md), with generator and angular acceleration

$$
F=X+\lambda V,\qquad \lambda(x,v)=\langle E(x),iv\rangle.
$$

The canonical fields $X$ and $V$ preserve [Liouville volume of a surface geodesic flow](../../../../../../liouville-volume-of-a-surface-geodesic-flow.md). To check this directly, use the [canonical coframe of a surface unit tangent bundle](../../../../../../canonical-coframe-of-a-surface-unit-tangent-bundle.md) $(\alpha,\beta,\omega)$, with dual frame $(X,H,V)$ and

$$
d\alpha=\omega\wedge\beta,\qquad d\beta=\alpha\wedge\omega,\qquad d\omega=-K\alpha\wedge\beta.
$$

For the positive volume $\mu=\alpha\wedge\beta\wedge\omega$, contraction gives $\iota_X\mu=\beta\wedge\omega$ and $\iota_V\mu=\alpha\wedge\beta$. Both two-forms are closed by the displayed structure equations, so the [Cartan formula for the Lie derivative](../../../../../../cartan-s-magic-formula.md) gives $\mathcal L_X\mu=\mathcal L_V\mu=0$.

The [product rule for divergence](../../../../../../product-rule-for-divergence.md) now yields

$$
\operatorname{div}_\mu F=\operatorname{div}_\mu X+
\lambda\operatorname{div}_\mu V+V\lambda=V\lambda.
$$

The [vertical vector field of a surface unit tangent bundle](../../../../../../vertical-vector-field-of-a-surface-unit-tangent-bundle.md) fixes the base point and satisfies $V(v)=iv$, $V(iv)=-v$. Since $E$ depends only on the base point,

$$
\boxed{\operatorname{div}_\mu F(x,v)=-\langle E(x),v\rangle.}
$$

This is the [divergence of a Gaussian thermostat](../../../../../../divergence-of-a-gaussian-thermostat.md). Reversing the overall sign of the chosen volume form does not change its divergence, so the answer is also valid if Liouville volume is written as the oppositely oriented contact volume.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
