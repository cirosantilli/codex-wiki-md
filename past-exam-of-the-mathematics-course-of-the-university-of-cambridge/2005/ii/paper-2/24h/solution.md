<h1 id="24h/solution">Solution</h1>

↑ **Parent:** [24H](../24h.md)

The plane [planar isoperimetric inequality](../../../../../planar-isoperimetric-inequality.md) says that a simple closed curve of length $L$ enclosing area $A$ satisfies $L^2\geq4\pi A$, with equality for circles.

For sufficiently small $r$, below the [injectivity radius](../../../../../injectivity-radius.md) at $p$, [geodesic polar coordinates](../../../../../geodesic-polar-coordinates.md) give the surface metric $dr^2+j(r,\theta)^2d\theta^2$. The radial variation field is a [Jacobi field](../../../../../jacobi-field.md), so

$$
j_{rr}+K(\gamma_\theta(r))j=0,\qquad j(0,\theta)=0,\quad j_r(0,\theta)=1.
$$

Its integral equation is $j=r-\int_0^r(r-u)K(\gamma_\theta(u))j(u,\theta)\,du$. [Continuity](../../../../../continuous-function.md) of [curvature](../../../../../curvature.md) and $j(u,\theta)=u+o(u)$, uniformly in direction, give

$$
j(r,\theta)=r-\frac{K(p)}6r^3+o(r^3).
$$

The [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md) makes the angular metric factor both the circle line element and the polar area factor. Therefore

$$
L=\int_0^{2\pi}j(r,\theta)\,d\theta
=2\pi r-\frac\pi3K(p)r^3+o(r^3),
$$



$$
A=\int_0^r\int_0^{2\pi}j(u,\theta)\,d\theta\,du
=\pi r^2-\frac\pi{12}K(p)r^4+o(r^4).
$$

Squaring the length expansion and subtracting gives

$$
\boxed{4\pi A-L^2=\pi^2K(p)r^4+o(r^4).}
$$

This identifies the requested remainder and proves its ratio to $r^4$ tends to zero. For $K(p)>0$, sufficiently small [geodesic](../../../../../geodesic.md) disks have **$L^2<4\pi A$**, the opposite strict inequality to the planar bound. Their positive [curvature](../../../../../curvature.md) allows more area for the same perimeter; the Euclidean inequality is not a universal inequality for curved surfaces.

## ↑ Ancestors (10)

1. [24H](../24h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
