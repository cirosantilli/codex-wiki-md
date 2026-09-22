<h1 id="15f/solution">Solution</h1>

↑ **Parent:** [15F](../15f.md)

An [embedded surface parametrization](../../../../../embedded-surface-parametrization.md) is a smooth map $F:U\subset\mathbb R^2\to\mathbb R^3$, with open $U$, injective differential of rank two at each point, and $F$ a [homeomorphism](../../../../../homeomorphism.md) onto its image with the subspace topology. Its [induced metric](../../../../../induced-metric.md) is

$$
 g_{ij}=\partial_iF\cdot\partial_jF,\qquad ds^2=g_{ij}du^idu^j.
$$

In coordinates, an arc-length-parametrized [geodesic](../../../../../geodesic.md) satisfies

$$
 \boxed{\ddot u^k+\Gamma^k_{ij}\dot u^i\dot u^j=0,\qquad
 g_{ij}\dot u^i\dot u^j=1,}
$$

where the [Christoffel symbols](../../../../../christoffel-symbol.md) are $\Gamma^k_{ij}=\tfrac12g^{k\ell}(\partial_i g_{j\ell}+\partial_j g_{i\ell}-\partial_\ell g_{ij})$. The normalization fixes unit speed; it is compatible with the differential equations because geodesic speed is constant.

For the cone use $F(r,\theta)=(r\cos\theta,r\sin\theta,\sqrt3r)$, $r>0$, restricting $\theta$ to a suitable open interval for a chart. Direct differentiation gives its [first fundamental form](../../../../../first-fundamental-form.md)

$$
 ds^2=4\,dr^2+r^2d\theta^2.
$$

With $\rho=2r$ and $\phi=\theta/2$, this becomes $d\rho^2+\rho^2d\phi^2$, the Euclidean [metric](../../../../../metric.md) in [polar coordinates](../../../../../polar-coordinates.md). The map $(r,\theta)\mapsto(2r\cos(\theta/2),2r\sin(\theta/2))$ is therefore a [local isometry](../../../../../local-isometry.md). It is local rather than global because increasing $\theta$ by $2\pi$ increases $\phi$ by $\pi$.

Given two points, choose their angle representatives so that $|\theta_2-\theta_1|\leq\pi$. Their developed plane angles then differ by at most $\pi/2$. The straight segment between their developed positions stays away from the origin: it lies in an angular sector of width at most $\pi/2$ containing both positive-radius endpoints. Develop that segment back onto the cone. Since [local isometries](../../../../../local-isometry.md) preserve [geodesics](../../../../../geodesic.md), it gives a geodesic joining the two points; it can be parametrized by arc length. This constructs [geodesics on a punctured circular cone](../../../../../geodesics-on-a-punctured-circular-cone.md). For a repeated point the constant curve is the degenerate geodesic. In particular, this argument does not appeal to completeness of the punctured cone.

**The joining geodesic need not be unique.** For endpoints with equal positive radius and opposite azimuth, one may use the angular changes $+\pi$ and $-\pi$. In the plane these give two straight segments from $(\rho,0)$ to $(0,\rho)$ and $(0,-\rho)$, respectively. Both avoid the origin. Their lifts pass on opposite sides of the cone and have distinct images, so a [reparametrization](../../../../../reparametrization.md) cannot identify them.

## ↑ Ancestors (10)

1. [15F](../15f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
