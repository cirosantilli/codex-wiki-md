<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

For the printed integration formula, $J$ must mean the [Jacobian determinant](../../../../../jacobian-determinant.md) of the inverse coordinate map:

$$
\boxed{J=\frac{\partial(x,y,z)}{\partial(u,v,w)}=\det\begin{pmatrix}x_u&x_v&x_w\\y_u&y_v&y_w\\z_u&z_v&z_w\end{pmatrix}}.
$$

If instead one calls $\partial(u,v,w)/\partial(x,y,z)$ the forward Jacobian, its [determinant](../../../../../determinant.md) is $1/J$ where the derivative is invertible. This convention distinction resolves the direction of the arrow in the printed wording.

To derive the [change of variables formula](../../../../../change-of-variables-formula.md), a small rectangular cell of side lengths $du,dv,dw$ maps under the inverse transformation, to first order, to a parallelepiped with edge vectors $\mathbf r_u\,du$, $\mathbf r_v\,dv$, $\mathbf r_w\,dw$. Its volume is the absolute [scalar triple product](../../../../../scalar-triple-product.md) of those vectors:

$$
dx\,dy\,dz=|\mathbf r_u\cdot(\mathbf r_v\times\mathbf r_w)|\,du\,dv\,dw=|J|\,du\,dv\,dw.
$$

For a one-to-one continuously differentiable coordinate map with continuously differentiable inverse, summing these local volume contributions and taking the partition limit gives

$$
\boxed{\int_D f(x,y,z)\,dx\,dy\,dz=\int_\Delta f(x(u,v,w),y(u,v,w),z(u,v,w))\,|J|\,du\,dv\,dw}.
$$

The absolute value removes an orientation reversal; injectivity ensures that each volume element is counted once.

For positive semi-axes, take $u=x/a$, $v=y/b$, $w=z/c$. The [solid ellipsoid](../../../../../solid-ellipsoid.md) becomes the unit ball and the inverse [Jacobian determinant](../../../../../jacobian-determinant.md) is $abc$. Thus

$$
\int_Dx^2\,dV=a^3bc\int_{u^2+v^2+w^2\le1}u^2\,du\,dv\,dw.
$$

Rotational symmetry gives equal integrals of $u^2,v^2,w^2$ over the ball. Their sum is the integral of $r^2$, so [spherical coordinates](../../../../../spherical-coordinate-system.md) give $\int u^2\,dV=\frac13\int_0^1 4\pi r^4\,dr=4\pi/15$. The [Cartesian second moment of a solid ellipsoid](../../../../../cartesian-second-moment-of-a-solid-ellipsoid.md) is therefore

$$
\boxed{\int_Dx^2\,dx\,dy\,dz=\frac{4\pi}{15}a^3bc}.
$$

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
