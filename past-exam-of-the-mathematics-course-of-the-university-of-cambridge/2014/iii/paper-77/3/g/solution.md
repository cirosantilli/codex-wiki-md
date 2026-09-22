<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Take $\mathbf e=\mathbf e_x$ and the surface normal $\mathbf e_z$. Under reflection in the free surface, polar vectors transform by $M=\operatorname{diag}(1,1,-1)$ and an axial [torque](../../../../../../torque.md) transforms by $\det(M)M$. A parallel [torque](../../../../../../torque.md) therefore reverses sign, while the separation direction $\mathbf e_x$ does not. The [free-surface image of a rotlet dipole](../../../../../../free-surface-image-of-a-rotlet-dipole.md) is a dipole of strength $-D$ at $z=+h$.

The observation point at the cell is directly below the image, so $\mathbf e\cdot\mathbf r=0$ and the image [velocity](../../../../../../velocity.md) vanishes. A symmetry proof of the vanishing normal drift is also useful: reflection in the vertical plane containing $\mathbf e$ reverses the axial dipole moment, preserves the normal component of a polar [velocity](../../../../../../velocity.md), and leaves the geometry unchanged. Linearity would make that same component change sign with $D$, forcing it to be zero. Thus **this singularity alone produces no attraction or repulsion**.

Write $X,Y,Z$ relative to the image, so the cell is at $(0,0,-2h)$. The image field is

$$
\mathbf u_{\mathrm{im}}=\frac{3D}{8\pi\mu}
\frac{X(0,-Z,Y)}{(X^2+Y^2+Z^2)^{5/2}}.
$$

Although its value at the cell is zero, its [velocity](../../../../../../velocity.md) gradient is not. In particular, the [surface-induced yaw of a rotlet dipole](../../../../../../surface-induced-yaw-of-a-rotlet-dipole.md) has

$$
\boxed{\omega_z=(\partial_Xu_Y-\partial_Yu_X)_{\mathrm{cell}}
=\frac{3D}{128\pi\mu h^4}\ne0\quad(D\ne0).}
$$

A spherical [torque](../../../../../../torque.md)-free body rotates with the local fluid angular [velocity](../../../../../../velocity.md) $\Omega_z=\omega_z/2$. Its swimming direction therefore turns in the surface plane and, at fixed height and speed, it traces a circle with radius $V_{\mathrm{swim}}/|\Omega_z|$. The sign of $D$ sets the sense of turning in this convention. An elongated swimmer also responds to strain; its rotation coefficient depends on its shape and need not equal one half of the [vorticity](../../../../../../vorticity.md). When the [stresslet](../../../../../../force-dipole-flow.md) is included, its changing height produces a changing turning rate rather than an exactly fixed-radius circle.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
