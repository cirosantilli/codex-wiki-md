<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $m=GM/c^2$ and $f(r)=1-2m/r$. A photon follows a [null geodesic](../../../../null-geodesic.md), with an [affine parameter](../../../../affine-parameter.md) $\lambda$ satisfying

$$
\frac{d^2x^\mu}{d\lambda^2}
+\Gamma^\mu{}_{\alpha\beta}
\frac{dx^\alpha}{d\lambda}\frac{dx^\beta}{d\lambda}=0.
$$

The [Christoffel symbols](../../../../christoffel-symbol.md) follow from the supplied [Schwarzschild spacetime](../../../../schwarzschild-spacetime-split.md) [metric tensor](../../../../metric-tensor.md). An efficient equivalent procedure is to use the [geodesic Lagrangian](../../../../geodesic-lagrangian.md)

$$
\mathcal L=\frac12\left[
-fc^2\dot t^2+f^{-1}\dot r^2
+r^2\dot\theta^2+r^2\sin^2\theta\,\dot\phi^2
\right],
$$

where dots denote $d/d\lambda$. Its [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) give the affinely parametrized [geodesic equations](../../../../geodesic-equation.md). The condition $\mathcal L=0$ is imposed after variation; setting the Lagrangian identically to zero before varying would discard the equations.

By [spherical symmetry](../../../../spherical-symmetry.md) the ray's [angular momentum](../../../../angular-momentum.md) fixes an orbital plane through the center. Rotate the angular coordinates so that plane is $\theta=\pi/2$. The $\theta$ [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is

$$
\frac{d}{d\lambda}(r^2\dot\theta)
=r^2\sin\theta\cos\theta\,\dot\phi^2,
$$

so $\theta=\pi/2$, $\dot\theta=0$ is preserved once imposed initially. A radial ray has no unique orbital plane, but any plane through that radial line can be chosen.

The coordinates $t$ and $\phi$ are cyclic. Thus their canonical momenta obey

$$
\frac{d}{d\lambda}(-c^2f\dot t)=0,\qquad
\frac{d}{d\lambda}(r^2\dot\phi)=0.
$$

The two [conserved quantities](../../../../conserved-quantity.md) can be chosen as

$$
\boxed{\varepsilon=f\dot t,\qquad \ell=r^2\dot\phi.}
$$

These are the [geodesic conserved quantities from Killing vectors](../../../../geodesic-conserved-quantity-from-a-killing-vector.md) $\partial_t$ and $\partial_\phi$. With the chosen parameter normalization the conserved energy is $E=c^2\varepsilon$ and axial [angular momentum](../../../../angular-momentum.md) is $\ell$; multiplying the affine tangent by a constant multiplies both quantities by that constant.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
