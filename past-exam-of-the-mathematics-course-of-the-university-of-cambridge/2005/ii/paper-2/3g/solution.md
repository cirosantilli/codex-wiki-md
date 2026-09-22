<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

Use the curvature-minus-one [Poincare disc model](../../../../../poincare-disk-model.md), whose [Riemannian metric](../../../../../riemannian-metric.md) is

$$
ds^2=\frac{4(dx^2+dy^2)}{(1-x^2-y^2)^2}.
$$

Its [geodesics](../../../../../geodesic.md) are Euclidean diameters and arcs of circles meeting the boundary circle orthogonally. The [hyperbolic area](../../../../../hyperbolic-area.md) of a measurable region $D$ is

$$
\operatorname{Area}(D)=\int_D\frac4{(1-x^2-y^2)^2}\,dx\,dy.
$$

An [isometry](../../../../../isometry.md) can move the center of a circle to the origin. Its hyperbolic radius $r$ and Euclidean radius $\rho$ then satisfy $r=\int_0^\rho2\,du/(1-u^2)=2\operatorname{artanh}\rho$, so $\rho=\tanh(r/2)$. Integrating the [area element of a surface](../../../../../area-element-of-a-surface.md) in [polar coordinates](../../../../../polar-coordinates.md) yields

$$
A(r)=\int_0^{2\pi}\int_0^\rho\frac{4u}{(1-u^2)^2}\,du\,d\theta
=\frac{4\pi\rho^2}{1-\rho^2}
=\boxed{2\pi(\cosh r-1)}.
$$

Integrating the line element around the circle gives

$$
C(r)=\frac{4\pi\rho}{1-\rho^2}=\boxed{2\pi\sinh r},
\qquad A'(r)=2\pi\sinh r=C(r).
$$

A geometric definition of [Pi](../../../../../pi.md) valid in this geometry is

$$
\boxed{\pi=\lim_{r\downarrow0}\frac{C(r)}{2r}
=\lim_{r\downarrow0}\frac{A(r)}{r^2}.}
$$

Indeed $\sinh r=r+O(r^3)$ and $\cosh r=1+r^2/2+O(r^4)$. The circumference-to-diameter ratio at a fixed positive radius is not constant, so the limiting qualification is necessary.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
