<h1 id="14e/solution">Solution</h1>

↑ **Parent:** [14E](../14e.md)

The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) for the kinetic [Lagrangian](../../../../../lagrangian.md) are

$$
\frac d{dt}(g_{ab}\dot x^b)-\frac12\partial_a g_{bc}\dot x^b\dot x^c=0.
$$

Expanding and multiplying by the [inverse metric](../../../../../inverse-metric.md) gives the [geodesic equation](../../../../../geodesic-equation.md)

$$
\boxed{\ddot x^a+\Gamma^a_{bc}\dot x^b\dot x^c=0,\qquad
\Gamma^a_{bc}=\frac12g^{ad}(\partial_b g_{dc}+\partial_c g_{db}-\partial_d g_{bc}).}
$$

The kinetic variational principle uses an [affine parameter](../../../../../affine-parameter.md); the energy $g_{ab}\dot x^a\dot x^b/2$ is constant along its solutions. Constant curves are also [geodesics](../../../../../geodesic.md).

For the [Poincaré half-plane model](../../../../../poincare-half-plane-model.md), translation in $x$ gives the [conserved quantity](../../../../../conserved-quantity.md) $p=\dot x/y^2$, and the energy is $E=(\dot x^2+\dot y^2)/(2y^2)$. If $p=0$, the nonconstant [geodesics](../../../../../geodesic.md) are vertical lines, with $y=y_0e^{\pm\sqrt{2E}t}$. If $p\ne0$,

$$
\left(\frac{dy}{dx}\right)^2=\frac{2E}{p^2y^2}-1.
$$

Writing $R^2=2E/p^2$ and integrating $dx/dy=\pm y/\sqrt{R^2-y^2}$ yields $(x-x_0)^2+y^2=R^2$. Thus nonconstant [geodesic](../../../../../geodesic.md) images are vertical lines or upper semicircles meeting the real axis orthogonally.

For the two specified points, the circle centre is $(6,0)$ and the radius is five:

$$
\boxed{(x-6)^2+y^2=25,\qquad y>0.}
$$

For example, an affine unit-speed parametrization is $x=6+5\tanh t$, $y=5\operatorname{sech}t$. The endpoints on the real axis are $(1,0)$ and $(11,0)$, outside the hyperbolic surface.

<a id="14e/image-the-upper-half-plane-geodesic-through-the-two-specified-points"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4-geodesic.png)

**[Figure 2](#14e/image-the-upper-half-plane-geodesic-through-the-two-specified-points). The upper-half-plane geodesic through the two specified points**.

## ↑ Ancestors (10)

1. [14E](../14e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
