# Constant-pressure-ratio vertical disk model

↑ **Parent:** [Radiation-to-gas pressure ratio](radiation-to-gas-pressure-ratio.md)

Assume a [thin disk](thin-disk.md) has height-independent [opacity](opacity.md) $\kappa_{\rm op}$ and [radiation-to-gas pressure ratio](radiation-to-gas-pressure-ratio.md) $\beta$, with vertical gravity $-\Omega_z^2z$. [Hydrostatic equilibrium](hydrostatic-equilibrium.md) and [radiative diffusion](radiative-diffusion.md) imply

$$
F_z=\frac\beta{1+\beta}\frac{c\Omega_z^2}{\kappa_{\rm op}}z.
$$

Balancing its derivative against viscous heating $\rho\nu q^2\Omega^2$ fixes the [dynamic viscosity](dynamic-viscosity.md)

$$
\rho\nu=\frac\beta{1+\beta}\frac{c}{q^2\kappa_{\rm op}}\frac{\Omega_z^2}{\Omega^2}.
$$

It is independent of height under these assumptions. For a [spherically symmetric potential](spherically-symmetric-potential.md), $\Omega_z=\Omega$. Integrating $\rho\nu$ through the full surface-to-surface thickness $2H$ gives $\bar\nu\Sigma=2H\rho\nu$, which determines the thickness from the radial [accretion rate](accretion-rate.md) solution.

## ↑ Ancestors (8)

1. [Radiation-to-gas pressure ratio](radiation-to-gas-pressure-ratio.md)
2. [Vertical structure of an astrophysical disk](vertical-structure-of-an-astrophysical-disk.md)
3. [Thin disk](thin-disk.md)
4. [Astrophysical disk](astrophysical-disk.md)
5. [Astrophysics](astrophysics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-321/1/c/solution.md)
