<h1 id="24h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) says that the radial and angular directions of the [exponential map](../../../../../../exponential-map-riemannian-geometry.md) are orthogonal, with radial lengths preserved. On a surface it gives

$$
\boxed{\langle\Phi_r,\Phi_r\rangle=1,\qquad
\langle\Phi_r,\Phi_\theta\rangle=0,}
$$

so the metric in [geodesic polar coordinates](../../../../../../geodesic-polar-coordinates.md) is $dr^2+G(r,\theta)d\theta^2$.

To prove it, consider a smooth variation $\gamma(r,s)=\exp_p(rv(s))$ of [geodesics](../../../../../../geodesic.md) with unit initial vectors $v(s)$. Put $T=\gamma_r$ and $J=\gamma_s$. Each radial [geodesic](../../../../../../geodesic.md) has constant unit speed, and the Levi-Civita connection is torsion free. Hence

$$
\frac d{dr}\langle T,J\rangle
=\langle\nabla_TT,J\rangle+\langle T,\nabla_TJ\rangle
=\langle T,\nabla_JT\rangle
=\frac12\partial_s\langle T,T\rangle=0.
$$

At $r=0$, $J=0$ because all [geodesics](../../../../../../geodesic.md) start at $p$, so the constant [inner product](../../../../../../inner-product.md) is zero. Unit radial length follows from [constant speed](../../../../../../constant-speed.md). General initial-vector variations split into a radial component, whose image has the same length, and a component tangent to the initial sphere, whose image is orthogonal to it. This proves the full [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [24H](../../24h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
