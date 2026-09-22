<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the perturbation phase be $\vartheta=\mathbf k(t)\cdot\mathbf r$ and write $\psi=\psi_0+\operatorname{Re}[\Pi(t)e^{i\vartheta}]$. [Incompressible flow](../../../../../../incompressible-flow.md) imposes $\mathbf k\cdot\mathbf v=0$. Applying the background advective derivative to the phase gives

$$
(\partial_t+\mathbf u_0\cdot\nabla)\vartheta=\dot{\mathbf k}\cdot\mathbf r-2Axk_y.
$$

Cancel this position-dependent phase by choosing

$$
\boxed{\dot k_x=2Ak_y,\qquad \dot k_y=\dot k_z=0,\qquad k_x(t)=k_x(t_0)+2Ak_y(t-t_0).}
$$

The perturbation acting on the basic flow gives $(\mathbf u'\cdot\nabla)\mathbf u_0=-2Au_x'\mathbf e_y$. Its self-advection vanishes exactly: the physical velocity $\mathbf u'$ is perpendicular to $\mathbf k$, while every spatial derivative of $\mathbf u'$ is proportional to a component of $\mathbf k$. Thus $\mathbf u'\cdot\nabla\mathbf u'=0$, including the products between the complex mode and its conjugate. Substituting into the full [Navier-Stokes equation](../../../../../../navier-stokes-equation.md) therefore gives an [exact incompressible shearing wave](../../../../../../exact-incompressible-shearing-wave.md), with no small-amplitude approximation:

$$
\boxed{\dot{\mathbf v}-2Av_x\mathbf e_y+2\Omega\mathbf e_z\times\mathbf v=-i\mathbf k\Pi-\nu k^2\mathbf v,\qquad \mathbf k\cdot\mathbf v=0.}
$$

In components these equations are

$$
\begin{aligned}
\dot v_x-2\Omega v_y&=-ik_x\Pi-\nu k^2v_x,\\
\dot v_y+2(\Omega-A)v_x&=-ik_y\Pi-\nu k^2v_y,\\
\dot v_z&=-ik_z\Pi-\nu k^2v_z.
\end{aligned}
$$

Differentiating the transversality constraint closes the [pressure](../../../../../../pressure.md):

$$
\boxed{ik^2\Pi=2\Omega k_xv_y+(4A-2\Omega)k_yv_x.}
$$

The coefficient $4A$ includes both the shear term in the momentum equation and $\dot{\mathbf k}\cdot\mathbf v$; treating the [wavevector](../../../../../../wavevector.md) as fixed would miss one contribution. Initial data with $\mathbf k(t_0)\cdot\mathbf v(t_0)=0$ remain transverse under this closed evolution. These [shearing waves](../../../../../../shearing-wave.md) are exact in an unbounded local shear flow or with compatible shearing-periodic boundaries; arbitrary rigid [boundary conditions](../../../../../../boundary-condition.md) need not admit a single such wave.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
