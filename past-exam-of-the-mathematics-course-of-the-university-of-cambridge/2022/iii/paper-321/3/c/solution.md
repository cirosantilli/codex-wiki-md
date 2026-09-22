<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\mathbf u_0=-3\Omega x\mathbf e_y/2$, advection vanishes and the [Coriolis acceleration](../../../../../../coriolis-acceleration.md) exactly cancels $3\Omega^2x\mathbf e_x$, so constant $P_0$ and $\theta_0=0$ complete the equilibrium.

Write perturbations $(\mathbf v,p,\vartheta)e^{i\mathbf k\cdot\mathbf x-i\omega t}$ with $\mathbf k=(k_x,0,k_z)$. Incompressibility gives $\mathbf k\cdot\mathbf v=0$. It also makes the quadratic terms $\mathbf v\cdot\nabla\mathbf v=i(\mathbf k\cdot\mathbf v)\mathbf v$ and $\mathbf v\cdot\nabla\vartheta$ vanish exactly; the background-advection terms vanish because $k_y=0$. The amplitude equations are

$$
-i\omega v_x=-\frac{ik_xp}{\rho_0}+2\Omega v_y,
\qquad
-i\omega v_y=-\frac12\Omega v_x,
$$



$$
-i\omega v_z=-\frac{ik_zp}{\rho_0}-N^2\vartheta,
\qquad
-i\omega\vartheta=v_z,
\qquad
k_xv_x+k_zv_z=0.
$$

Eliminating the amplitudes yields the [inertia-gravity wave](../../../../../../inertia-gravity-wave.md) dispersion relation

$$
\boxed{\omega^2=\frac{k_z^2}{k^2}\Omega^2
+\frac{k_x^2}{k^2}N^2,
\qquad k^2=k_x^2+k_z^2}.
$$

For $N^2=0$, $\omega=\pm\Omega k_z/k$, so the [group velocity](../../../../../../group-velocity.md) is

$$
\boxed{\mathbf c=\nabla_{\mathbf k}\omega
=\pm k^{-3}[\mathbf k\times(\boldsymbol\Omega\times\mathbf k)]}.
$$

It is perpendicular to $\mathbf k$ and hence to the [phase velocity](../../../../../../phase-velocity.md). An [inertial wave](../../../../../../inertial-wave.md) packet transports energy along beams lying in its phase surfaces.

If $N^2>0$ and $k_x/k_z\to0$, incompressibility suppresses vertical motion and $\omega\to\Omega$: horizontal epicyclic motion and rotation dominate. If $k_z/k_x\to0$, radial motion is suppressed and $\omega\to N$: vertical buoyancy oscillations dominate. Intermediate ratios give hybrid [inertia-gravity waves](../../../../../../inertia-gravity-wave.md).

If $N^2<0$, exponential growth occurs exactly when

$$
\boxed{N^2k_x^2+\Omega^2k_z^2<0
\quad\Longleftrightarrow\quad
\frac{k_x^2}{k_z^2}>\frac{\Omega^2}{-N^2}}.
$$

Only modes with sufficiently large radial wavenumber permit enough vertical displacement for unstable buoyancy to overcome rotational restoration; the other orientations remain stabilized by the Coriolis force.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
