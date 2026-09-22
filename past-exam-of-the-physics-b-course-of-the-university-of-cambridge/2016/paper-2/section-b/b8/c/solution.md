<h1 id="section-b/b8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Newtonian fluid](../../../../../../newtonian-fluid.md) exerts viscous [shear stress](../../../../../../shear-stress.md) proportional to the rate of strain. For an incompressible fluid of constant [dynamic viscosity](../../../../../../dynamic-viscosity-split.md) $\eta$,

$$
\boldsymbol\sigma=-p\mathbf I+\eta[\nabla\mathbf u+(\nabla\mathbf u)^T].
$$

The local momentum balance is the [Navier-Stokes equation](../../../../../../navier-stokes-equation.md):

$$
\boxed{\rho\left(\frac{\partial\mathbf u}{\partial t}+\mathbf u\cdot\nabla\mathbf u\right)=-\nabla p+\eta\nabla^2\mathbf u+\rho\mathbf g.}
$$

The left side is density times [material acceleration](../../../../../../material-acceleration.md). A steady velocity field can still have convective [acceleration](../../../../../../acceleration.md) when a moving parcel changes speed or direction; setting $\partial\mathbf u/\partial t=0$ does not eliminate it.

The [Reynolds number](../../../../../../reynolds-number.md) $\mathrm{Re}=\rho UL/\eta$ compares inertia with viscous effects. At low [Reynolds number](../../../../../../reynolds-number.md), the fluid's own inertia can often be neglected, giving [Stokes flow](../../../../../../stokes-flow-split.md). This does not say that every immersed body has zero [acceleration](../../../../../../acceleration.md): its [mass](../../../../../../mass.md) and the net pressure, viscous and body [forces](../../../../../../force-split.md) still enter its own [equation of motion](../../../../../../equation-of-motion.md).

For a small rigid sphere moving through a slowly varying viscous background, [Stokes drag](../../../../../../stokes-s-law.md) is $-6\pi\eta a(\mathbf v-\mathbf u)$. In still fluid, a simple settling model includes [weight](../../../../../../weight-representation-theory.md), [buoyancy](../../../../../../buoyancy.md) and drag:

$$
m\dot v=(m-\rho_fV_s)g-6\pi\eta av.
$$

Ignoring fluid added mass and unsteady history forces, this gives relaxation time $m/(6\pi\eta a)$ and [terminal velocity](../../../../../../terminal-velocity.md)

$$
\boxed{v_t=\frac{2a^2(\rho_s-\rho_f)g}{9\eta}.}
$$

At the terminal [velocity](../../../../../../velocity.md) the net [force](../../../../../../force-split.md) and [acceleration](../../../../../../acceleration.md) vanish, while viscous drag and gravity remain individually nonzero. The dissipated [power](../../../../../../power.md) $6\pi\eta av_t^2$ is supplied by the loss of gravitational [potential energy](../../../../../../potential-energy.md) relative to buoyant support. The creeping-flow and quasisteady-drag assumptions must be checked before applying this expression at large speed or immediately after a rapid start.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
