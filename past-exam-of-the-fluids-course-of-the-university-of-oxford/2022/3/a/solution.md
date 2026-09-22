<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Each layer has constant [mass density](../../../../density.md), initially negligible [velocity](../../../../velocity.md) and hence zero [vorticity](../../../../vorticity-split.md). Its [Euler equations for an inviscid fluid](../../../../euler-equations-for-an-inviscid-fluid-split.md) have a conservative gravitational body force, so [Kelvin's circulation theorem](../../../../kelvin-s-circulation-theorem.md) preserves zero bulk [vorticity](../../../../vorticity-split.md). In a simply connected layer, the [irrotational flow](../../../../irrotational-flow.md) therefore has $\mathbf v_i=\nabla\phi_i$. The [incompressible flow](../../../../incompressible-flow.md) condition gives

$$
\boxed{\nabla^2\phi_i=0.}
$$

This applies while the ideal layerwise solution is smooth. It allows an interfacial [vortex sheet](../../../../vortex-sheet.md); it does not assert that the whole two-fluid flow has zero [vorticity](../../../../vorticity-split.md) or that a smooth interface must exist for arbitrarily long times.

The rigid wall [no-penetration boundary conditions](../../../../no-penetration-boundary-condition.md) are

$$
\partial_z\phi_1(r,-h,t)=0,\qquad
\partial_z\phi_2(r,h,t)=0,\qquad
\partial_r\phi_i(a,z,t)=0,
$$

with boundedness and $\partial_r\phi_i=0$ at $r=0$ for regular axisymmetric fields. For a small interface displacement and small slope, linearization of the [kinematic boundary condition](../../../../kinematic-boundary-condition.md) about $z=0$ gives

$$
\boxed{\eta_t=\partial_z\phi_1(r,0,t)=\partial_z\phi_2(r,0,t).}
$$

The small-slope condition is an additional requirement for high-[wavenumber](../../../../wavenumber.md) modes: $|\alpha\eta|\ll1$, not just $|\eta|\ll h,a$.

Choose the unperturbed [hydrostatic pressures](../../../../hydrostatic-pressure.md) as $\bar p_i(z)=p_*-\rho_i gz$. The linearized [Bernoulli equation](../../../../bernoulli-equation.md) gives the [pressure](../../../../pressure-split.md) perturbation $p_i'=-\rho_i\partial_t\phi_i$, after absorbing spatially constant gauges into $\phi_i$. Since [surface tension](../../../../surface-tension-split.md) and viscous [normal stress](../../../../normal-stress.md) vanish, [pressure](../../../../pressure-split.md) continuity on $z=\eta$ gives

$$
-\rho_1\partial_t\phi_1-\rho_1g\eta
=-\rho_2\partial_t\phi_2-\rho_2g\eta,
$$

or

$$
\boxed{\rho_1\partial_t\phi_1-\rho_2\partial_t\phi_2
=(\rho_2-\rho_1)g\eta\quad\text{at }z=0.}
$$

The initial [velocity](../../../../velocity.md) is zero, so $\eta_t(r,0)=0$. Separate [conservation of mass](../../../../mass-conservation.md) in each closed layer also requires $\int_0^a\eta(r,t)r\,dr=0$ relative to the initially horizontal interface.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
