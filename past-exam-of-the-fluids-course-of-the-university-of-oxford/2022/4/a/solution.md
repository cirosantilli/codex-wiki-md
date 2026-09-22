<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A small [Reynolds number](../../../../reynolds-number.md), $\mathrm{Re}=\rho UL/\eta\ll1$, means that [inertia](../../../../inertia.md) is small compared with viscous forces. It can arise from small speed, small length or large [dynamic viscosity](../../../../dynamic-viscosity-split.md). Examples are the locomotion of a [microswimmer](../../../../microswimmer.md) and the slow [sedimentation](../../../../sedimentation.md) of a small particle in a viscous liquid.

To neglect local [acceleration](../../../../acceleration.md) as well, an externally imposed time scale $T$ must satisfy $\rho L^2/(\eta T)=L^2/(\nu T)\ll1$. This holds for a [steady flow](../../../../steady-flow.md) or a sufficiently slowly varying [quasi-steady Stokes approximation](../../../../quasi-steady-stokes-approximation.md). Small [Reynolds number](../../../../reynolds-number.md) alone is insufficient for that extra step. For an [incompressible flow](../../../../incompressible-flow.md) with constant material coefficients and uniform [gravity](../../../../gravity.md), the [Navier-Stokes equation](../../../../navier-stokes-equation.md) then reduces to the [Stokes equation](../../../../stokes-equation.md):

$$
0=-\nabla p-\rho g\hat{\mathbf z}+\eta\nabla^2\mathbf u,\qquad \nabla\cdot\mathbf u=0.
$$

Taking the [divergence](../../../../divergence.md) and using commuting spatial [derivatives](../../../../derivative.md) gives

$$
0=-\nabla^2p+\eta\nabla^2(\nabla\cdot\mathbf u),\qquad
\boxed{\nabla^2p\simeq0.}
$$

Taking the [curl](../../../../curl.md), which annihilates the [pressure gradient](../../../../pressure-gradient.md) and uniform gravitational force, gives

$$
0=\eta\nabla^2(\nabla\times\mathbf u),\qquad
\boxed{\nabla^2\boldsymbol\omega\simeq0.}
$$

These are the [Harmonic pressure and vorticity in Stokes flow](../../../../harmonic-pressure-and-vorticity-in-stokes-flow.md) results.

A concrete counterexample to inferring both solely from small [Reynolds number](../../../../reynolds-number.md) is [Stokes' second problem](../../../../stokes-second-problem.md): an oscillating plate with arbitrarily small [velocity](../../../../velocity.md) amplitude has negligible [inertia](../../../../inertia.md), but $\partial_t\boldsymbol\omega=\nu\nabla^2\boldsymbol\omega$ is nonzero. Its [vorticity](../../../../vorticity-split.md) is not a [harmonic function](../../../../harmonic-function.md). The quasi-steady qualification is therefore necessary.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
