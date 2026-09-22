<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In [resistive-force theory](../../../../../resistive-force-theory.md) ([RFT](../../../../../resistive-force-theory.md)), the hydrodynamic force per unit arclength exerted by the fluid on a slender filament is

$$
\boxed{\mathbf f=-\xi_\parallel(\mathbf u\cdot\mathbf t)\mathbf t
-\xi_\perp[\mathbf u-(\mathbf u\cdot\mathbf t)\mathbf t]
=-[\xi_\perp I+(\xi_\parallel-\xi_\perp)\mathbf t\mathbf t^T]\mathbf u}.
$$

Here $\mathbf t$ is the unit tangent and $\mathbf u$ the local velocity relative to the background fluid. The [parallel and perpendicular drag coefficients of a slender filament](../../../../../parallel-and-perpendicular-drag-coefficients-of-a-slender-filament.md) are positive and generally satisfy $\xi_\perp>\xi_\parallel$; their leading logarithmic ratio is about two. This local approximation assumes a small filament radius compared with length and curvature scales, negligible fluid inertia, and a [Newtonian fluid](../../../../../newtonian-fluid.md). It represents drag by the local tangent direction and neglects nonlocal [hydrodynamic interactions](../../../../../hydrodynamic-interaction.md) between separated filament segments. Boundaries, close approaches and end corrections may require [slender-body theory](../../../../../slender-body-theory.md) or a more complete flow calculation. In this problem the background fluid is at rest, and the drag coefficients are taken uniform along the filament.

The [rigid-body velocity in a deforming swimmer frame](../../../../../rigid-body-velocity-in-a-deforming-swimmer-frame.md) is the sum of translation, rotation and material deformation. With $\mathbf r=x\mathbf e_x+\epsilon g\mathbf e_y$,

$$
\mathbf u=U\mathbf e_x+V\mathbf e_y+\Omega\mathbf e_z\times\mathbf r+\epsilon g_t\mathbf e_y,
$$

so, in instantaneous swimmer-frame components,

$$
\boxed{\mathbf u=(U-\epsilon\Omega g)\mathbf e_x+(V+\Omega x+\epsilon g_t)\mathbf e_y}.
$$

The reference-frame conditions $g(0,t)=g_x(0,t)=0$ attach the origin and orientation to the filament's base and base tangent. They prevent arbitrary shape translations or tilts from being absorbed into the definition of $g$.

The exact tangent and arclength element are

$$
\mathbf t=\frac{\mathbf e_x+\epsilon g_x\mathbf e_y}{\sqrt{1+\epsilon^2g_x^2}},\qquad
 ds=\sqrt{1+\epsilon^2g_x^2}\,dx.
$$

Since $U,V,\Omega=O(\epsilon)$, the local velocity is $O(\epsilon)$. Changing the drag tensor by its $O(\epsilon)$ tangent correction therefore changes $\mathbf f$ only at $O(\epsilon^2)$. The arclength correction is smaller still at this order. Also $-\epsilon\Omega g=O(\epsilon^2)$. Thus **$\mathbf t=\mathbf e_x$ is sufficient at order $\epsilon$**. This assumes the small-slope expansion is uniform, $\epsilon|g_x|\ll1$.

Put $G_0(t)=\langle g_t\rangle_x$ and $G_1(t)=\langle xg_t\rangle_x$, with $\langle h\rangle_x=L^{-1}\int_0^Lh\,dx$. The first-order local force is

$$
\mathbf f=-\epsilon\xi_\parallel U_1\mathbf e_x
-\epsilon\xi_\perp(V_1+\Omega_1x+g_t)\mathbf e_y+O(\epsilon^2).
$$

Its total hydrodynamic forces are

$$
\boxed{F_x=-\epsilon\xi_\parallel L U_1+O(\epsilon^2),\qquad
F_y=-\epsilon\xi_\perp L\left(V_1+\frac L2\Omega_1+G_0\right)+O(\epsilon^2)}.
$$

Taking the moment about the swimmer-frame origin, $M_z=\int(xf_y-\epsilon gf_x)\,ds$, the second term is beyond first order. Hence

$$
\boxed{M_z=-\epsilon\xi_\perp L\left(\frac L2V_1+\frac{L^2}{3}\Omega_1+G_1\right)+O(\epsilon^2)}.
$$

For [force-free](../../../../../force-free.md) and [torque-free](../../../../../torque-free.md) motion, the three leading coefficients vanish. The longitudinal force immediately gives **$U_1=0$**. The two transverse equations are

$$
V_1+\frac L2\Omega_1=-G_0,\qquad
\frac L2V_1+\frac{L^2}{3}\Omega_1=-G_1.
$$

Their determinant is $L^2/12>0$. Solving yields the [first-order free swimming of a planar filament](../../../../../first-order-free-swimming-of-a-planar-filament.md):

$$
\boxed{V_1=-4\langle g_t\rangle_x+\frac6L\langle xg_t\rangle_x,\qquad
\Omega_1=\frac6L\langle g_t\rangle_x-\frac{12}{L^2}\langle xg_t\rangle_x}.
$$

The [resistive-force theory](../../../../../resistive-force-theory.md) coefficient cancels because both equations use the same transverse drag. Another interpretation is the [least-squares projection of filament deformation velocity](../../../../../least-squares-projection-of-filament-deformation-velocity.md): $-V_1-\Omega_1x$ is the best affine approximation to $g_t$ on $[0,L]$. Zero transverse force and torque mean that the residual is orthogonal to $1$ and $x$.

If $g$ is sufficiently differentiable and periodic with period $T$, each $g_t(x,t)$ has zero temporal mean. More explicitly,

$$
V_1=\frac d{dt}\left[-4\langle g\rangle_x+\frac6L\langle xg\rangle_x\right],\qquad
\Omega_1=\frac d{dt}\left[\frac6L\langle g\rangle_x-\frac{12}{L^2}\langle xg\rangle_x\right].
$$

Both bracketed quantities return to their initial values over a period. Thus the [first-order periodic transverse swimming velocity](../../../../../first-order-periodic-transverse-swimming-velocity.md) satisfies

$$
\boxed{\langle V_1\rangle_t=\langle\Omega_1\rangle_t=0}.
$$

These results concern first order and swimmer-frame components. Changes of orientation can affect laboratory displacements at second order; higher-order net swimming is not ruled out.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 334](../../paper-334-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
