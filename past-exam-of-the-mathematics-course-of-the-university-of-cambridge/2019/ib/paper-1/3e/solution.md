<h1 id="3e/solution">Solution</h1>

↑ **Parent:** [3E](../3e.md)

The [Poincare disc model](../../../../../poincare-disk-model.md) is

$$
D=\{z\in\mathbb C:|z|<1\},
\qquad
ds^2=\frac{4|dz|^2}{(1-|z|^2)^2}.
$$

This [Riemannian metric](../../../../../riemannian-metric.md) has constant Gaussian curvature $-1$.

For $a\in D$ and $|\eta|=1$, the [Möbius transformation](../../../../../mobius-transformation.md)

$$
T_{a,\eta}(z)=\eta\frac{z-a}{1-\overline a z}
$$

is an [isometry](../../../../../isometry.md) of the disc, and every orientation-preserving disc isometry has this form. In particular, $T_{z_1,1}$ sends $z_1$ to zero and $z_2$ to a point of modulus

$$
\rho=\left|\frac{z_2-z_1}{1-\overline{z_1}z_2}\right|.
$$

Rotations are also isometries, so it remains only to integrate the metric along a radial geodesic from $0$ to $\rho$:

$$
d(0,\rho)=\int_0^\rho\frac{2\,dr}{1-r^2}
=2\operatorname{artanh}\rho.
$$

Thus the [Hyperbolic distance in the Poincare disc](../../../../../hyperbolic-distance-in-the-poincare-disc.md) is

$$
\boxed{d(z_1,z_2)=2\operatorname{artanh}\left|\frac{z_2-z_1}{1-\overline{z_1}z_2}\right|
=\log\frac{1+\rho}{1-\rho}}.
$$

## ↑ Ancestors (10)

1. [3E](../3e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
