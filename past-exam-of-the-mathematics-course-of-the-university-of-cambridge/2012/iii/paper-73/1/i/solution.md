<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work with an incompressible [Newtonian fluid](../../../../../../newtonian-fluid.md) of constant [kinematic viscosity](../../../../../../kinematic-viscosity.md). The [vorticity equation](../../../../../../vorticity-equation.md) is $D\boldsymbol\omega/Dt=(\boldsymbol\omega\cdot\nabla)\mathbf u+\nu\nabla^2\boldsymbol\omega$. In the axisymmetric [Burgers vortex](../../../../../../burgers-vortex.md) the swirl does not advect the axial [vorticity](../../../../../../vorticity.md), and the stretching rate is $\partial_z u_z=\alpha$. Put $s(t)=\delta^2(t)$ and $W=\omega_z$. The Gaussian profile has

$$
\frac{\partial_tW}{W}=\dot s\left(-\frac1s+\frac{r^2}{s^2}\right),\quad
\frac{u_r\partial_rW}{W}=\frac{\alpha r^2}{s},\quad
\frac{\nabla^2W}{W}=-\frac4s+\frac{4r^2}{s^2}.
$$

Substitution into $\partial_tW+u_r\partial_rW=\alpha W+\nu\nabla^2W$ matches both the constant and $r^2$ terms precisely when

$$
\boxed{\dot s+\alpha s=4\nu}.
$$

For every finite positive initial $s_0$,

$$
\boxed{\delta^2(t)=\frac{4\nu}{\alpha}+\left(s_0-\frac{4\nu}{\alpha}\right)e^{-\alpha t}},\qquad
\delta(t)\longrightarrow\sqrt{4\nu/\alpha}.
$$

The strain compresses the cross-section and stretches its [vorticity](../../../../../../vorticity.md), while [kinematic viscosity](../../../../../../kinematic-viscosity.md) spreads the core. The attracting radius is the balance of these effects; its relaxation time is $\alpha^{-1}$. Total [circulation](../../../../../../circulation-physics.md) stays fixed because stretching increases the [vorticity](../../../../../../vorticity.md) as the cross-sectional area decreases.

At the steady core radius, the swirl speed is of order $\Gamma_0/\delta$, and its [velocity gradient tensor](../../../../../../velocity-gradient-tensor.md) is of order $\Gamma_0/\delta^2$. Its [viscous dissipation](../../../../../../viscous-dissipation.md) integrated over a cross-section therefore scales as

$$
\mathcal D_{\rm tube}\sim\nu\left(\frac{\Gamma_0}{\delta^2}\right)^2\delta^2
\sim\boxed{\alpha\Gamma_0^2}.
$$

This is per unit length and per unit density. More precisely, for the swirl contribution, [integration by parts](../../../../../../integration-by-parts.md) relates the integrated strain [viscous dissipation](../../../../../../viscous-dissipation.md) to $\nu\int W^2\,dA$; the boundary term vanishes for the $1/r$ swirl velocity. Thus

$$
\boxed{\mathcal D_{\rm tube}=\frac{\nu\Gamma_0^2}{2\pi\delta^2}=\frac{\alpha\Gamma_0^2}{8\pi}}.
$$

Multiply by density for power per physical length. Here the azimuthal velocity's [circulation](../../../../../../circulation-physics.md) $\Gamma$ is $\Gamma_0$, as follows by integrating $W$ over the cross-section. The result is finite as $\nu\to0$ with strain and [circulation](../../../../../../circulation-physics.md) held fixed. Local core [viscous dissipation](../../../../../../viscous-dissipation.md) grows like $\nu^{-1}$ while its area shrinks like $\nu$. For $\Gamma_0/\nu\gg1$, the swirl gradients dominate the background strain within the core.

This finite quantity is the excess [viscous dissipation](../../../../../../viscous-dissipation.md) due to the vortex. The uniform straining flow alone dissipates $3\nu\alpha^2$ per unit volume, and integrating that over an infinite cross-section diverges. The total [viscous dissipation](../../../../../../viscous-dissipation.md) of the complete idealized flow is therefore not a finite tube power unless the background is subtracted or spatially bounded.

A [Burgers vortex sheet](../../../../../../burgers-vortex-sheet.md) instead smooths a fixed velocity jump $U$ across a layer of thickness $\delta_s\sim\sqrt{\nu/\alpha}$. Its [viscous dissipation](../../../../../../viscous-dissipation.md) per sheet area is of order

$$
\mathcal D_{\rm sheet}\sim\nu(U/\delta_s)^2\delta_s\sim U^2\sqrt{\nu\alpha}\longrightarrow0.
$$

**A tube with fixed [circulation](../../../../../../circulation-physics.md) supports finite [viscous dissipation](../../../../../../viscous-dissipation.md) in a vanishingly small core; a sheet with fixed velocity jump does not.** This makes strained [vortex tubes](../../../../../../vortex-tube.md) plausible intense dissipative structures at high [Reynolds number](../../../../../../reynolds-number.md). It does not assert that sheets are absent from [turbulence](../../../../../../turbulence-split.md): sheets can carry [inertial range](../../../../../../inertial-range.md) organization and become unstable, producing finer vortical structures.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
