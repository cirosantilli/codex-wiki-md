<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Consider the discrete map

$$
(t,r,\psi,\theta,\phi)\longmapsto
(t,r,\psi,\pi-\theta,\,2\phi_0-\phi).
$$

It is an [isometry](../../../../../../isometry.md): $\cos\theta$ and $d\phi$ both change sign, leaving $\cos\theta\,d\phi$ unchanged, while $d\theta^2$ and $\sin^2\theta\,d\phi^2$ are also unchanged. A local component of its [fixed-point set](../../../../../../fixed-point-set.md) is $\theta=\pi/2$, $\phi=\phi_0$.

If a [geodesic](../../../../../../geodesic.md) starts tangent to that component, the [isometry](../../../../../../isometry.md) fixes both its initial position and its initial tangent. Applying the [isometry](../../../../../../isometry.md) therefore gives a [geodesic](../../../../../../geodesic.md) with the same initial data. Uniqueness of the [geodesic equation](../../../../../../geodesic-equation.md) makes it the same curve, so it remains in the fixed component. This proves that the selected submanifold is a [totally geodesic submanifold](../../../../../../totally-geodesic-submanifold.md); it has dimension three, not two. The proof continues through a horizon when expressed in regular coordinates, so coordinate singularities of the original chart do not invalidate it.

The [geodesic conserved quantities from Killing vectors](../../../../../../geodesic-conserved-quantity-from-a-killing-vector.md) associated with $\partial_\psi$ and $\partial_\phi$ are

$$
L_\psi=r^2h\left(\dot\psi+\frac12\cos\theta\,\dot\phi-\Omega\dot t\right),\qquad
L_\phi=\frac12\cos\theta\,L_\psi+\frac{r^2\sin^2\theta}{4}\dot\phi.
$$

Dots denote [derivatives](../../../../../../derivative.md) with respect to an [affine parameter](../../../../../../affine-parameter.md). On the chosen submanifold $\dot\phi=0$ and $\cos\theta=0$, so $L_\phi=0$. Requiring also $L_\psi=0$ gives

$$
\boxed{\dot\psi=\Omega(r)\dot t.}
$$

More generally, away from the polar-coordinate axes, both displayed angular charges being zero imply $\dot\phi=0$ and the same relation. In particular, zero conserved [angular momentum](../../../../../../angular-momentum.md) does not imply constant $\psi$: the motion follows the local dragging of the angular coordinate by the rotating geometry.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
