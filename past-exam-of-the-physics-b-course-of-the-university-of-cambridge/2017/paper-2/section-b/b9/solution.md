<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

**Following the moving [fluid](../../../../../fluid.md).** The Eulerian [velocity field](../../../../../velocity-field.md) $\mathbf u(\mathbf x,t)$ assigns a [velocity](../../../../../velocity.md) to each position. A [fluid](../../../../../fluid.md) [particle](../../../../../particle-physics.md) satisfies $\dot{\mathbf x}=\mathbf u$, so the [chain rule](../../../../../chain-rule.md) gives the [material derivative](../../../../../material-derivative.md), also called the convective [derivative](../../../../../derivative.md),

$$
\boxed{\frac D{Dt}=\frac\partial{\partial t}+\mathbf u\cdot\nabla,
\qquad \mathbf a=\frac{D\mathbf u}{Dt}.}
$$

Even in steady flow a [particle](../../../../../particle-physics.md) can accelerate because it moves between regions with different [velocity](../../../../../velocity.md). For example, flow around a curved obstacle changes direction despite $\partial_t\mathbf u=0$. [Mass](../../../../../mass.md) conservation is

$$
\partial_t\rho+\nabla\cdot(\rho\mathbf u)=0,
\qquad \frac{D\rho}{Dt}+\rho\nabla\cdot\mathbf u=0.
$$

For a constant-density incompressible [fluid](../../../../../fluid.md), $\nabla\cdot\mathbf u=0$.

**[Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid-split.md) and [Bernoulli's equation](../../../../../bernoulli-equation.md).** Neglect [viscosity](../../../../../dynamic-viscosity-split.md) and take the body [force](../../../../../force-split.md) per unit [mass](../../../../../mass.md) to be $-\nabla\Phi$. [Newton's second law](../../../../../newton-s-second-law.md) for a [fluid](../../../../../fluid.md) element gives

$$
\rho\frac{D\mathbf u}{Dt}=-\nabla p-\rho\nabla\Phi.
$$

For steady flow, dot with [displacement](../../../../../displacement.md) along a [streamline](../../../../../streamline.md). The tangential component of $\mathbf u\cdot\nabla\mathbf u$ is the [derivative](../../../../../derivative.md) of $u^2/2$ along that line. For constant density, integration gives

$$
\boxed{\frac p\rho+\frac{u^2}{2}+\Phi=B,\qquad B\text{ constant along a streamline}.}
$$

In uniform gravity, $\Phi=gz$. Thus [pressure](../../../../../pressure-split.md), [kinetic energy](../../../../../kinetic-energy.md) per unit [mass](../../../../../mass.md) and [gravitational potential energy](../../../../../gravitational-energy.md) per unit [mass](../../../../../mass.md) exchange along a [streamline](../../../../../streamline.md). For a barotropic compressible [fluid](../../../../../fluid.md), replace $p/\rho$ by $\int dp/\rho(p)$. Different [streamlines](../../../../../streamline.md) need not have the same Bernoulli constant.

**[Vorticity](../../../../../vorticity-split.md) and [potential flow](../../../../../potential-flow.md).** [Vorticity](../../../../../vorticity-split.md) is $\boldsymbol\omega=\nabla\times\mathbf u$. A small [fluid](../../../../../fluid.md) element rotates locally with [angular velocity](../../../../../angular-velocity.md) $\boldsymbol\omega/2$ after its deformational part is separated. The [vector](../../../../../vector.md) identity

$$
(\mathbf u\cdot\nabla)\mathbf u=\nabla(u^2/2)-\mathbf u\times\boldsymbol\omega
$$

gives $\nabla B=\mathbf u\times\boldsymbol\omega$ for steady constant-density [inviscid flow](../../../../../inviscid-flow.md). Thus an irrotational region has one common Bernoulli constant on each connected region. In a simply connected irrotational domain, introduce a [velocity potential](../../../../../velocity-potential.md) $\mathbf u=\nabla\phi$. [Incompressibility](../../../../../incompressible-flow.md) then gives [Laplace's equation](../../../../../laplace-equation.md), $\nabla^2\phi=0$. For unsteady [irrotational flow](../../../../../irrotational-flow.md),

$$
\partial_t\phi+\frac12|\nabla\phi|^2+\frac p\rho+\Phi=C(t).
$$

An impermeable stationary wall fixes $\partial_n\phi=0$, but ideal [potential flow](../../../../../potential-flow.md) does not enforce no slip. In a multiply connected domain, [irrotational flow](../../../../../irrotational-flow.md) may still have nonzero [circulation](../../../../../circulation-physics.md) around an excluded vortex core, so a globally single-valued potential requires care.

For example, uniform two-dimensional flow past a circular cylinder has $\phi=U(r+a^2/r)\cos\theta$ outside $r=a$. Its normal [velocity](../../../../../velocity.md) vanishes at the cylinder, and its surface tangential [velocity](../../../../../velocity.md) is $-2U\sin\theta$. [Bernoulli's equation](../../../../../bernoulli-equation.md) predicts a symmetric [pressure](../../../../../pressure-split.md) distribution and zero [drag](../../../../../drag-physics.md). This is [D'Alembert's paradox](../../../../../d-alembert-s-paradox.md): the assumptions omit the viscous [boundary layers](../../../../../boundary-layer.md), separation and wake responsible for real [drag](../../../../../drag-physics.md).

For an incompressible [fluid](../../../../../fluid.md) of constant [kinematic viscosity](../../../../../kinematic-viscosity.md) $\nu$, the [curl](../../../../../curl.md) of the motion equation gives

$$
\frac{D\boldsymbol\omega}{Dt}=(\boldsymbol\omega\cdot\nabla)\mathbf u+\nu\nabla^2\boldsymbol\omega.
$$

The first term stretches and tilts [vortex lines](../../../../../vortex-line.md); the second diffuses [vorticity](../../../../../vorticity-split.md). In two-dimensional incompressible [inviscid flow](../../../../../inviscid-flow.md) the stretching term is absent and [vorticity](../../../../../vorticity-split.md) is carried with the [fluid](../../../../../fluid.md). In a three-dimensional [inviscid flow](../../../../../inviscid-flow.md) it can be amplified by stretching. Density gradients not parallel to [pressure](../../../../../pressure-split.md) gradients provide an additional source in a general compressible [fluid](../../../../../fluid.md).

**Viscous flow.** A [Newtonian fluid](../../../../../newtonian-fluid.md)'s shear [stress](../../../../../stress.md) is proportional to rate of [strain](../../../../../strain.md). For constant [viscosity](../../../../../dynamic-viscosity-split.md) and [incompressibility](../../../../../incompressible-flow.md) the [Navier-Stokes equation](../../../../../navier-stokes-equation.md) is

$$
\boxed{\rho\frac{D\mathbf u}{Dt}=-\nabla p-\rho\nabla\Phi+\eta\nabla^2\mathbf u,}
$$

with [dynamic viscosity](../../../../../dynamic-viscosity-split.md) $\eta$ and [kinematic viscosity](../../../../../kinematic-viscosity.md) $\nu=\eta/\rho$. At an ordinary [solid](../../../../../solid.md) wall, the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) sets [fluid](../../../../../fluid.md) [velocity](../../../../../velocity.md) equal to the wall [velocity](../../../../../velocity.md). [Viscosity](../../../../../dynamic-viscosity-split.md) transfers [momentum](../../../../../momentum-split.md) between neighbouring layers and converts mechanical [energy](../../../../../energy-split.md) into [heat](../../../../../heat-split.md); unlike the [pressure](../../../../../pressure-split.md) [force](../../../../../force-split.md), its shear contribution depends on [velocity](../../../../../velocity.md) gradients.

For plane [Couette flow](../../../../../couette-flow.md) between plates $y=0,h$, with the upper plate moving at $U$, the steady solution is $u_x=Uy/h$, with shear [stress](../../../../../stress.md) $\eta U/h$. For pressure-driven flow through a pipe of radius $a$, a constant [pressure](../../../../../pressure-split.md) gradient gives the parabolic Poiseuille profile

$$
u_z(r)=\frac{-dp/dz}{4\eta}(a^2-r^2),\qquad
Q=\frac{\pi a^4}{8\eta}\left(-\frac{dp}{dz}\right).
$$

The [Reynolds number](../../../../../reynolds-number.md) $\mathrm{Re}=\rho UL/\eta$ compares convective inertia with viscous [force](../../../../../force-split.md). Small [Reynolds number](../../../../../reynolds-number.md) often permits the Stokes-flow approximation; large [Reynolds number](../../../../../reynolds-number.md) can produce thin [boundary layers](../../../../../boundary-layer.md) and, under suitable conditions, [turbulence](../../../../../turbulence-split.md). It does not justify neglecting the wall conditions. Bernoulli's inviscid constant is generally not conserved along a viscous [streamline](../../../../../streamline.md), and pipe flow instead shows a [pressure](../../../../../pressure-split.md) loss corresponding to dissipation.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
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
