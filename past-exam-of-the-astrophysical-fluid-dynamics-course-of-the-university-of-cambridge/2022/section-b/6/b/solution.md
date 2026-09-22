<h1 id="section-b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write total [pressure](../../../../../pressure-split.md) and [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) as

$$
p=p_0(r)+\pi(r,z,t),\qquad \Phi=\Phi_0(r)+\psi(r,z,t).
$$

Here $\pi$ is the [Eulerian perturbation of a fluid variable](../../../../../eulerian-perturbation-of-a-fluid-variable.md) applied to [pressure](../../../../../pressure-split.md), while $\psi$ is the corresponding [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) perturbation. They have units $\mathrm{Pa}$ and $\mathrm{m^2\,s^{-2}}$, respectively. The constant interior [mass density](../../../../../density.md) is $\rho$.

The [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid-split.md) are

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u
=-\frac1\rho\nabla(p_0+\pi)-\nabla(\Phi_0+\psi).
$$

Subtract the [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) relation $\nabla p_0/\rho+\nabla\Phi_0=0$ and discard terms quadratic in the perturbation. [Mass conservation](../../../../../mass-conservation.md) gives [incompressible flow](../../../../../incompressible-flow.md), and the gravitational [Poisson equation](../../../../../poisson-s-equation.md) has no bulk density perturbation. Thus, strictly inside the fluid,

$$
\boxed{\partial_t\mathbf u=-\frac{\nabla\pi}{\rho}-\nabla\psi,\qquad
\nabla\cdot\mathbf u=0,\qquad\nabla^2\psi=0.}
$$

The last equation is [Laplace equation](../../../../../laplace-equation.md), not a statement that self-gravity has disappeared. The displaced surface carries a first-order [surface mass density](../../../../../projected-surface-mass-density.md) $\rho\eta$, where $\eta$ is its radial displacement, and this supplies the source and matching conditions for $\psi$ at the moving interface. The [axisymmetric gravitational potential of a displaced cylindrical interface](../../../../../axisymmetric-gravitational-potential-of-a-displaced-cylindrical-interface.md), expressed using [modified Bessel functions](../../../../../modified-bessel-function.md), incorporates that boundary source.

It is useful to define $W=\psi+\pi/\rho$. Taking the [divergence](../../../../../divergence.md) of the momentum equation gives $\nabla^2W=0$. For an axisymmetric [Fourier mode](../../../../../fourier-mode.md) with axial [wavenumber](../../../../../wavenumber.md) $k>0$, regularity at $r=0$ selects radial dependence $I_0(kr)$, the [Modified Bessel function of the first kind](../../../../../modified-bessel-function-of-the-first-kind.md), since $K_0(kr)$ is singular there. In what follows $k=|k_z|$ can always be chosen nonnegative.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
