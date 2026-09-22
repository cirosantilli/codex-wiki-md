<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start in an inertial frame with the inviscid [magnetohydrodynamic momentum equation](../../../../magnetohydrodynamic-momentum-equation.md),

$$
\rho D_t\mathbf v=-\nabla P+\mathbf J\times\mathbf B-\rho\nabla\Phi.
$$

Here $\rho$ is [mass density](../../../../density.md), $P$ is the isotropic fluid [pressure](../../../../pressure-split.md), $\mathbf v$ is inertial-frame [velocity](../../../../velocity.md), $\mathbf J$ is [electric current density](../../../../current-density.md), $\mathbf B$ is the [magnetic field](../../../../magnetic-field-split.md), and $\Phi$ is [gravitational potential](../../../../newtonian-potential-of-a-point-mass.md) per unit [mass](../../../../mass.md). In the low-frequency approximation to [Ampère's law](../../../../ampere-s-circuital-law.md), $\mathbf J=\nabla\times\mathbf B/\mu_0$. The [vector calculus identity](../../../../vector-calculus-identity.md)

$$
(\nabla\times\mathbf B)\times\mathbf B=(\mathbf B\cdot\nabla)\mathbf B-\nabla(B^2/2)
$$

separates the [Lorentz force density](../../../../lorentz-force-density.md) into [magnetic tension](../../../../magnetic-tension.md) and a [magnetic pressure](../../../../magnetic-pressure.md) gradient. Transform the material [acceleration](../../../../acceleration.md) to a rigid frame rotating with constant [angular velocity](../../../../angular-velocity.md) $\boldsymbol\Omega_0$, using the stated frame transformation. The [rotating-frame magnetohydrodynamic momentum equation](../../../../rotating-frame-magnetohydrodynamic-momentum-equation.md) is

$$
\boxed{\rho D_t\mathbf u=-\nabla\left(P+\frac{B^2}{2\mu_0}\right)+\frac{(\mathbf B\cdot\nabla)\mathbf B}{\mu_0}-\rho\nabla\Phi-2\rho\boldsymbol\Omega_0\times\mathbf u-\rho\boldsymbol\Omega_0\times(\boldsymbol\Omega_0\times\mathbf r).}
$$

The final terms are the [Coriolis force](../../../../coriolis-force.md) and [centrifugal force](../../../../centrifugal-force.md) densities; $\mathbf u$ is the [velocity](../../../../velocity.md) relative to the rotating frame, and $D_t=\partial_t+\mathbf u\cdot\nabla$ uses that frame.

This requires a smooth conducting-fluid continuum with nonrelativistic motion, a constant [magnetic permeability](../../../../permeability-electromagnetism.md) $\mu_0$, the [solenoidal magnetic-field constraint](../../../../solenoidal-magnetic-field-constraint.md), a negligible [displacement current](../../../../displacement-current.md) and negligible net electric-charge force. Viscous forces and anisotropic fluid stresses are omitted. A time-dependent frame would add an [Euler force](../../../../euler-force.md). [Incompressible flow](../../../../incompressible-flow.md) is not needed for this force equation. Finite [electrical resistivity](../../../../electrical-resistivity.md) does not change its displayed instantaneous magnetic force; the later frozen-field calculation additionally uses [ideal magnetohydrodynamics](../../../../ideal-magnetohydrodynamics-split.md). A differentially rotating fluid does not define a single rigid frame with spatially varying $\boldsymbol\Omega_0$: choose a fixed local reference rate and retain the fluid's shear in $\mathbf u$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
