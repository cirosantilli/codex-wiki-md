<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

A [velocity field](../../../../../velocity-field.md) $\mathbf u(\mathbf x,t)$ assigns a [velocity](../../../../../velocity.md) to each point. Following a fluid parcel rather than holding position fixed gives the material or convective [derivative](../../../../../derivative.md)

$$
\boxed{\frac D{Dt}=\partial_t+\mathbf u\cdot\nabla.}
$$

The convective term can accelerate fluid even in a steady flow, for example as a stream narrows. Conservation of [mass](../../../../../mass.md) is $\partial_t\rho+\nabla\cdot(\rho\mathbf u)=0$; constant-density [incompressible flow](../../../../../incompressible-flow.md) has $\nabla\cdot\mathbf u=0$.

For an incompressible [Newtonian fluid](../../../../../newtonian-fluid.md) of constant [density](../../../../../density.md) and [viscosity](../../../../../dynamic-viscosity-split.md), with conservative body-force potential per [mass](../../../../../mass.md) $\Phi$, [momentum](../../../../../momentum-split.md) balance is

$$
\frac{D\mathbf u}{Dt}=-\frac{\nabla p}{\rho}-\nabla\Phi+\nu\nabla^2\mathbf u.
$$

Neglect [viscosity](../../../../../dynamic-viscosity-split.md) and assume steady flow. Dotting with an element along a streamline, or using $(\mathbf u\cdot\nabla)\mathbf u=\nabla(u^2/2)-\mathbf u\times(\nabla\times\mathbf u)$, gives

$$
\boxed{\frac p\rho+\frac{u^2}{2}+\Phi=B\quad\text{along a streamline}.}
$$

This is Bernoulli's equation: [pressure](../../../../../pressure-split.md) [work](../../../../../work.md), [kinetic energy](../../../../../kinetic-energy.md) and gravitational [potential energy](../../../../../potential-energy.md) interconvert. In a connected irrotational region under the same assumptions, $B$ is the same for all streamlines. In a rotational flow it can vary between them. Viscous dissipation, pumps or unsteady motion require the corresponding modified balance; the steady inviscid expression cannot be applied indiscriminately.

[Vorticity](../../../../../vorticity-split.md) $\boldsymbol\zeta=\nabla\times\mathbf u$ measures local fluid rotation. For constant-density [incompressible flow](../../../../../incompressible-flow.md) it evolves by

$$
\frac{D\boldsymbol\zeta}{Dt}=(\boldsymbol\zeta\cdot\nabla)\mathbf u+\nu\nabla^2\boldsymbol\zeta,
$$

showing vortex stretching and viscous diffusion. A [potential flow](../../../../../potential-flow.md) has $\mathbf u=\nabla\phi$ locally, so irrotational incompressible motion satisfies $\nabla^2\phi=0$. Boundary conditions then determine flows around simple shapes. A multiply connected region can have circulation even when its local [vorticity](../../../../../vorticity-split.md) vanishes; ideal [potential flow](../../../../../potential-flow.md) also misses no-slip [boundary layers](../../../../../boundary-layer.md) and viscous drag.

For a [Newtonian fluid](../../../../../newtonian-fluid.md), [shear stress](../../../../../shear-stress.md) is proportional to [strain](../../../../../strain.md) rate. No-slip at solid walls produces [velocity](../../../../../velocity.md) gradients and dissipation. Fully developed laminar pipe flow, for example, has

$$
u_z(s)=\frac{\Delta p}{4\mu\ell}(R^2-s^2),\qquad
Q=\frac{\pi R^4\Delta p}{8\mu\ell}.
$$

The [Reynolds number](../../../../../reynolds-number.md) $\operatorname{Re}=UL/\nu$ compares inertial and viscous terms. Small values favour creeping-flow approximations; large values can permit thin [boundary layers](../../../../../boundary-layer.md) and [turbulence](../../../../../turbulence-split.md), without guaranteeing [turbulence](../../../../../turbulence-split.md) in every geometry. **The appropriate flow model follows from conservation laws, constitutive properties, boundaries and scale comparisons.**

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
