<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the layer depth as the length unit, its [thermal diffusion time](../../../../../../thermal-diffusion-time.md) as the time unit, and its imposed [temperature](../../../../../../temperature.md) difference as the [temperature](../../../../../../temperature.md) unit. Then $\mathbf u=(u,0,w)$ is the [velocity field](../../../../../../velocity-field.md), $P$ the [pressure](../../../../../../pressure.md) after the conductive [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) has been subtracted, $\theta$ the departure from the conductive [temperature](../../../../../../temperature.md) $T_0=1-z$, $\mathbf e_z$ the upward [unit vector](../../../../../../unit-vector.md), and $R=g\alpha\Delta T d^3/(\nu\kappa_T)$ the [Rayleigh number](../../../../../../rayleigh-number.md). Here $d$ is the dimensional depth, $\nu$ the [kinematic viscosity](../../../../../../kinematic-viscosity.md), $\kappa_T$ the [thermal diffusivity](../../../../../../thermal-diffusivity.md) and $\alpha$ the [thermal expansion coefficient](../../../../../../thermal-expansion-coefficient.md). The [gradient](../../../../../../gradient.md), [divergence](../../../../../../divergence.md) and [Laplacian](../../../../../../laplacian.md) act on the dimensionless coordinates. The term $w$ in the [heat equation](../../../../../../heat-equation.md) is [advection](../../../../../../advection.md) of the background [gradient](../../../../../../gradient.md), since $-\mathbf u\cdot\nabla T_0=w$. [Mass density](../../../../../../density.md) variations enter only the [buoyancy](../../../../../../buoyancy.md) term under the [Boussinesq approximation](../../../../../../boussinesq-approximation.md); the [incompressible flow](../../../../../../incompressible-flow.md) constraint is $\nabla\cdot\mathbf u=0$.

For fixed, impermeable, stress-free plates, the [no-penetration boundary condition](../../../../../../no-penetration-boundary-condition.md), [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md) and [perfectly conducting thermal boundary condition](../../../../../../perfectly-conducting-thermal-boundary-condition.md) are

$$
\boxed{w=0,\qquad \partial_z u=0,\qquad\theta=0\quad\text{at }z=0,1.}
$$

For a nonzero horizontal [Fourier mode](../../../../../../fourier-mode.md), [incompressibility](../../../../../../incompressible-flow.md) gives $u=i w_z/k$, so the [velocity](../../../../../../velocity.md) conditions are equivalently $w=w_{zz}=0$ on both plates. A uniform horizontal [velocity](../../../../../../velocity.md) is not fixed by these [boundary conditions](../../../../../../boundary-condition.md); take its mean to be zero when discussing the stationary forced pattern.

**The printed small-Prandtl-number label does not generally justify these equations.** In thermal-time units the full momentum equation contains $\operatorname{Pr}^{-1}(\partial_t\mathbf u+\mathbf u\cdot\nabla\mathbf u)$, where the [Prandtl number](../../../../../../prandtl-number.md) is $\operatorname{Pr}=\nu/\kappa_T$. Dropping that term gives [infinite-Prandtl-number convection](../../../../../../infinite-prandtl-number-convection.md) or another explicitly justified [Stokes flow](../../../../../../stokes-flow-split.md) approximation. It is not the general $\operatorname{Pr}\to0$ limit. For example the horizontal shear $u=U_0e^{-\operatorname{Pr}\pi^2t}\cos\pi z$, $w=\theta=0$, satisfies the full linear momentum equation and the plate conditions, and persists at fixed $t$ as $\operatorname{Pr}\to0$. The printed inertia-free equation would instead require this shear to vanish. The following parts solve the equations actually displayed; applying them at small [Prandtl number](../../../../../../prandtl-number.md) needs an additional slaving or creeping-flow ordering.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
