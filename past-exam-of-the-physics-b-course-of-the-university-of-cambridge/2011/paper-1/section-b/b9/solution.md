<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

A [fluid](../../../../../fluid.md) is described on a continuum scale by [density](../../../../../density.md), [pressure](../../../../../pressure-split.md) and [velocity](../../../../../velocity.md) fields. An Eulerian field is measured at fixed position; a material element changes at rate $D/Dt=\partial_t+\mathbf v\cdot\nabla$. [mass](../../../../../mass.md) conservation requires

$$
\partial_t\rho+\nabla\cdot(\rho\mathbf v)=0.
$$

For [incompressible flow](../../../../../incompressible-flow.md) this becomes $\nabla\cdot\mathbf v=0$. A [streamline](../../../../../streamline.md) is instantaneously tangent to [velocity](../../../../../velocity.md), whereas a [pathline](../../../../../pathline.md) follows a particle through time; they coincide in a steady [flow](../../../../../flow.md) but need not in an unsteady one.

For an ideal inviscid [fluid](../../../../../fluid.md), [pressure](../../../../../pressure-split.md) and body [forces](../../../../../force-split.md) give the Euler equation. In the constant-density gravitational case,

$$
\rho\frac{D\mathbf v}{Dt}=-\nabla p+\rho\mathbf g.
$$

A stationary impermeable boundary requires zero normal [velocity](../../../../../velocity.md), but inviscid theory does not impose no slip. Taking its steady projection along a [streamline](../../../../../streamline.md) gives $p/\rho+v^2/2+gz=\mathrm{constant}$. If the [flow](../../../../../flow.md) is also irrotational in the connected region, that constant is shared between [streamlines](../../../../../streamline.md). Inviscid does not mean irrotational: rotating ideal-fluid [flows](../../../../../flow.md) are possible. A [velocity](../../../../../velocity.md) potential exists locally for an irrotational field, and in [incompressible flow](../../../../../incompressible-flow.md) it obeys [Laplace's equation](../../../../../laplace-equation.md). The Bernoulli assumptions must be checked before converting a [pressure](../../../../../pressure-split.md) difference into a [speed](../../../../../speed.md).[Restrictions and Common Assumptions: inviscid, steady, incompressible flow and streamline dependence](../../../../../bernoulli%E2%80%99s-equation-by-nasa-glenn-research-center.md)

Real [fluids](../../../../../fluid.md) transmit shear stress. An incompressible [Newtonian fluid](../../../../../newtonian-fluid.md) with constant [dynamic viscosity](../../../../../dynamic-viscosity-split.md) $\eta$ obeys

$$
\rho\frac{D\mathbf v}{Dt}=-\nabla p+\eta\nabla^2\mathbf v+\rho\mathbf g.
$$

The constitutive shear stress is proportional to strain rate, and stationary solid boundaries usually impose no slip. [viscosity](../../../../../dynamic-viscosity-split.md) diffuses [vorticity](../../../../../vorticity-split.md) and converts organized mechanical [energy](../../../../../energy-split.md) into [heat](../../../../../heat-split.md); its local dissipation $2\eta e_{ij}e_{ij}$ is nonnegative. It cannot generally be included merely by changing the constant in a lossless Bernoulli equation.

In a long straight circular tube, steady fully developed [laminar flow](../../../../../laminar-flow.md) has

$$
v_z(r)=\frac{\Delta p}{4\eta L}(a^2-r^2),\qquad
Q=\frac{\pi a^4\Delta p}{8\eta L}.
$$

This [Hagen-Poiseuille equation](../../../../../hagen-poiseuille-equation.md) follows by balancing the axial [pressure](../../../../../pressure-split.md) [gradient](../../../../../gradient.md) with viscous shear and setting $v_z(a)=0$. The parabolic profile, the fourth-power [radius](../../../../../radius.md) sensitivity and the pumping power $\Delta p\,Q$ are experimentally distinct consequences. Entrance regions, rough walls, non-Newtonian response or a changing [temperature](../../../../../temperature-split.md) require additional modelling.

The [Reynolds number](../../../../../reynolds-number.md) $\mathrm{Re}=\rho UL/\eta$ compares inertia with [viscosity](../../../../../dynamic-viscosity-split.md). Small values favor creeping-flow balances; high values permit thin [boundary layers](../../../../../boundary-layer.md), separation and [turbulence](../../../../../turbulence-split.md), although transition depends on geometry and perturbations, not one universal critical number. At high [Reynolds number](../../../../../reynolds-number.md) an outer [flow](../../../../../flow.md) can be approximately inviscid while near-wall [viscosity](../../../../../dynamic-viscosity-split.md) still determines drag. This resolves why a zero-drag ideal potential-flow model cannot predict the resistance of an ordinary moving body. In turbulent [flow](../../../../../flow.md), fluctuating [Reynolds stresses](../../../../../reynolds-stress.md) redistribute momentum and increase the required [pressure](../../../../../pressure-split.md) drop; averaging the equations introduces closure requirements.

A controlled tube experiment measures [pressure](../../../../../pressure-split.md) difference and collected [volume](../../../../../volume.md) per time while changing forcing. Use tracers or a [velocity](../../../../../velocity.md) probe to test profile shape, allow sufficient entrance [length](../../../../../length.md), and monitor [radius](../../../../../radius.md) and [temperature](../../../../../temperature-split.md) independently. Repeat with reversed [flow](../../../../../flow.md) and at several rates to test offsets and linearity. Dye mixing alone does not measure [viscosity](../../../../../dynamic-viscosity-split.md) or establish a fully developed [velocity](../../../../../velocity.md) profile. The original figure below separates a specified laminar velocity profile from an independent pressure/discharge measurement.

<a id="section-b/b9/image-ideal-and-viscous-fluid-flow"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1-fluid-flow.png)

**[Figure 3](#section-b/b9/image-ideal-and-viscous-fluid-flow). Ideal and viscous fluid flow**.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
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
