<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the density as a hydrostatic reference profile $\widehat\rho(z)$ plus a small perturbation $\rho'$, and define buoyancy and [buoyancy frequency](../../../../../../buoyancy-frequency.md) by

$$
b=-\frac g{\rho_0}\rho',
\qquad
N^2=-\frac g{\rho_0}\frac{d\widehat\rho}{dz}>0.
$$

The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) to the [Navier-Stokes equation](../../../../../../navier-stokes-equation.md), together with [mass conservation](../../../../../../mass-conservation.md), is

$$
\nabla\mathbin\cdot\mathbf u=0,
$$



$$
\frac{D\mathbf u}{Dt}
=-\nabla\pi+b\mathbf e_z+\nu\nabla^2\mathbf u,
\qquad
\frac{Db}{Dt}+N^2w=\kappa\nabla^2b,
$$

where $D/Dt$ is the [material derivative](../../../../../../material-derivative.md), $\nu$ is [kinematic viscosity](../../../../../../kinematic-viscosity.md), and $\kappa$ is [mass diffusivity](../../../../../../mass-diffusivity.md). Linearizing about rest and eliminating pressure and buoyancy gives

$$
\left[(\partial_t-\kappa\nabla^2)(\partial_t-\nu\nabla^2)\nabla^2
+N^2\partial_x^2\right]w=0.
$$

For a [plane wave](../../../../../../plane-wave.md) proportional to $e^{i(kx+mz-\omega t)}$, with $K^2=k^2+m^2$, the viscous-diffusive [dispersion relation](../../../../../../dispersion-relation.md) is

$$
(-i\omega+\nu K^2)(-i\omega+\kappa K^2)K^2+N^2k^2=0.
$$

In the inviscid limit this becomes

$$
\omega_0^2=\frac{N^2k^2}{k^2+m^2}.
$$

For weak diffusion the two oscillatory roots are

$$
\omega=\pm\omega_0-\frac i2(\nu+\kappa)K^2
+O\bigl((\nu-\kappa)^2K^4/\omega_0\bigr),
$$

so a freely evolving Fourier mode decays.

A single plane wave is also an exact solution of the nonlinear equations. Every field depends only on its phase $\Theta=\mathbf k\mathbin\cdot\mathbf x-\omega t$, while [incompressible flow](../../../../../../incompressible-flow.md) gives $\mathbf u\mathbin\cdot\mathbf k=0$. Therefore $\mathbf u\mathbin\cdot\nabla$ annihilates both $\mathbf u(\Theta)$ and $b(\Theta)$, and all nonlinear advection terms vanish.

For a boundary-forced wave with real $\omega$, nonzero $\nu$ or $\kappa$ instead makes the bulk vertical wavenumber complex, attenuating the propagating beam. Because diffusion raises the spatial order of the equations, additional short vertical-wavenumber roots form viscous and scalar [boundary layers](../../../../../../boundary-layer.md); they allow a no-slip velocity condition and a scalar no-flux condition to accompany impermeability. These layers and bulk attenuation become essential near [critical internal-wave reflection](../../../../../../critical-internal-wave-reflection.md), where the inviscid reflected wavelength collapses.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
