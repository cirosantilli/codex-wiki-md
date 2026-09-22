<h1 id="11e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Poincare disc model](../../../../../../poincare-disk-model.md) is

$$
\mathbb D=\{z=x+iy:|z|<1\},
\qquad
ds^2=\frac{4(dx^2+dy^2)}{(1-|z|^2)^2}.
$$

Its geodesics through the origin are the Euclidean diameters. To see directly that the radial segment from $0$ to $re^{i\theta_0}$ minimizes length, write an arbitrary joining curve as $z(t)=r(t)e^{i\theta(t)}$. Its [hyperbolic length](../../../../../../hyperbolic-length-in-the-poincare-disc.md) satisfies

$$
\begin{aligned}
L
&=\int\frac{2\sqrt{\dot r^{\,2}+r^2\dot\theta^{\,2}}}{1-r^2}\,dt\\
&\geq\int\frac{2|\dot r|}{1-r^2}\,dt
\geq2\operatorname{artanh}r.
\end{aligned}
$$

The radial segment has constant $\theta$ and monotone $r$, so equality holds. Hence

$$
\boxed{d_{\mathbb D}(0,z)=2\operatorname{artanh}|z|}
$$

and every radial diameter is length minimizing. Rotational symmetry and uniqueness for the [geodesic equation](../../../../../../geodesic-equation.md) show that these are all geodesics through $0$.

Given any geodesic and a point $p$ on it, a disc-preserving map

$$
T(z)=e^{i\varphi}\frac{z-p}{1-\overline pz}
$$

takes $p$ to the origin. By part (a), $T$ is a hyperbolic isometry and commutes with $J(z)=1/\overline z$. The transformed geodesic is a diameter, hence a generalized circle invariant under $J$. Its inverse image is therefore also a [Generalized circle under a Möbius transformation](../../../../../../generalized-circle-under-a-mobius-transformation.md) invariant under $J$. Thus every hyperbolic geodesic is the part in $\mathbb D$ of a Euclidean line or circle preserved by reflection in the unit circle; equivalently, it is a diameter or a circle orthogonal to the unit circle. This is the [Geodesics of the Poincare disc](../../../../../../geodesics-of-the-poincare-disc.md) description.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
