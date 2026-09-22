<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Evaluate the smooth one-form on unit velocities to obtain $f(x,v)=\theta_x(v)$. Its integral along a periodic orbit of the [geodesic flow](../../../../../../geodesic-flow.md) is exactly the one-form integral along the corresponding closed [geodesic](../../../../../../geodesic.md). Negative curvature makes this geodesic flow an [Anosov flow](../../../../../../anosov-flow.md); the geodesic flow of a connected closed negatively curved surface is also [topologically transitive](../../../../../../topological-transitivity.md). Apply the smooth [Livsic theorem](../../../../../../livsic-theorem.md) to obtain $u\in C^\infty(SM)$ with

$$
Xu=\theta_x(v).
$$

If there is more than one connected component, apply this argument to each component separately.

The [vertical vector field of a surface unit tangent bundle](../../../../../../vertical-vector-field-of-a-surface-unit-tangent-bundle.md) differentiates rotation of $v$, so

$$
VXu=\theta_x(iv),\qquad V^2Xu=-\theta_x(v).
$$

For each $x$, writing $\theta_x(v)=A\cos\vartheta+B\sin\vartheta$ shows explicitly that

$$
\int_0^{2\pi}\theta_x(v)^2\,d\vartheta
=\pi(A^2+B^2)
=\int_0^{2\pi}\theta_x(iv)^2\,d\vartheta.
$$

The fibre disintegration of [Liouville volume of a surface geodesic flow](../../../../../../liouville-volume-of-a-surface-geodesic-flow.md) is $d\mu=dA_g\,d\vartheta$. Integrating the displayed equality over the base therefore gives $\|VXu\|_{L^2}^2=\|Xu\|_{L^2}^2$. Substitution into the supplied [Pestov identity for a geodesic flow](../../../../../../pestov-identity-for-a-geodesic-flow.md) yields

$$
\|XVu\|_{L^2}^2+\int_{SM}(-K)(Vu)^2\,d\mu=0.
$$

Both terms are nonnegative and $-K\ge k_0>0$. Thus $Vu=0$ everywhere. Since every unit-circle fibre is connected, $u$ is independent of velocity and descends to a smooth function $h$ on $M$: $u=h\circ\pi$. Its geodesic derivative is

$$
Xu(x,v)=dh_x(v).
$$

Comparison with $Xu=\theta_x(v)$, first on unit vectors and then on all vectors by linearity, proves

$$
\boxed{\theta=dh.}
$$

Thus the one-form is an [exact differential form](../../../../../../exact-differential-form.md). This proves the degree-one [geodesic X-ray transform](../../../../../../geodesic-x-ray-transform.md) conclusion directly from the given integral identity and the stated smooth coboundary theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
