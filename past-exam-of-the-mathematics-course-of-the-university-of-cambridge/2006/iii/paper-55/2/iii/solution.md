<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

There is first an angular-scale typo in the PDF: smaller angles correspond to larger multipoles, approximately $\theta\sim\pi/\ell$. Small scales relative to the first acoustic peak therefore have $\ell\gtrsim200$, not the printed inequality in the other direction.

The [photon-baryon acoustic oscillator](../../../../../../photon-baryon-acoustic-oscillator.md) produces rapidly varying density and velocity sources around and below the sound horizon. Treating the emission density as a simple long-wavelength gravitational source misses these acoustic peaks and their phases. [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md) suppresses short-scale perturbations through diffusion before decoupling. The [cosmological visibility function](../../../../../../cosmological-visibility-function.md) has finite width, so different emission times and acoustic phases are averaged rather than sampled on one sharp surface. As [tight coupling](../../../../../../tight-coupling-approximation.md) breaks down, the photon quadrupole and higher moments are generated; [Thomson scattering](../../../../../../thomson-scattering.md) of the quadrupole produces polarization. These require the full [photon Boltzmann hierarchy](../../../../../../photon-boltzmann-hierarchy.md), rather than exactly vanishing emission moments above the dipole. They are the [angular-scale limits of instantaneous photon decoupling](../../../../../../angular-scale-limits-of-instantaneous-photon-decoupling.md).

The distinction is important: acoustic evolution and diffusion can already be included in correctly calculated emission $\delta_\gamma$ and $\mathbf v$. They do not themselves invalidate collisionless propagation after decoupling. The two-moment, single-time initial condition and omission of scattering after that surface are the approximations used in the requested line-of-sight formula.

For the stated assumptions, multiply the [synchronous photon brightness equation](../../../../../../synchronous-photon-brightness-equation.md) by $e^{ik\mu\tau}$ and integrate:

$$
\Delta(\mathbf k,\mathbf n,\tau_0)
=e^{-ik\mu(\tau_0-\tau_d)}\Delta(\mathbf k,\mathbf n,\tau_d)
-2\int_{\tau_d}^{\tau_0}e^{-ik\mu(\tau_0-\tau)}h'_{ij}(\mathbf k,\tau)n^in^j\,d\tau.
$$

Here $\tau_d$ is the decoupling time. Inverse Fourier transformation shifts each source to the unperturbed ray

$$
\mathbf x(\tau)=\mathbf x_0-\mathbf n(\tau_0-\tau),\qquad
\mathbf x_d=\mathbf x_0-\mathbf n(\tau_0-\tau_d).
$$

Insert the initial brightness monopole and Doppler dipole, and divide by four:

$$
\boxed{\frac{\Delta T}{T}(\mathbf x_0,\mathbf n,\tau_0)
=\frac14\delta_\gamma(\mathbf x_d,\tau_d)
+\mathbf n\cdot\mathbf v(\mathbf x_d,\tau_d)
-\frac12\int_{\tau_d}^{\tau_0}h'_{ij}(\mathbf x(\tau),\tau)n^in^j\,d\tau.}
$$

This is the [synchronous Sachs-Wolfe line-of-sight formula](../../../../../../synchronous-sachs-wolfe-line-of-sight-formula.md). The first term is intrinsic emission temperature, the second is the [Doppler effect](../../../../../../doppler-effect.md), and the last is the accumulated gravitational redshift in this gauge. The derivative $h'_{ij}$ is the partial conformal-time derivative evaluated on the ray, not its total derivative along the ray. Its integral contains endpoint gravitational effects as well as evolving-potential effects when rewritten in [Newtonian gauge](../../../../../../newtonian-gauge.md); it should not be identified solely with the [Integrated Sachs-Wolfe effect](../../../../../../integrated-sachs-wolfe-effect.md).

The direction $\mathbf n$ is photon propagation toward the observer. The observer-to-source sky direction is its negative, so changing that convention also changes the displayed Doppler sign and the ray parametrization. Correct emitter positions and this direction convention are needed to interpret the formula.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
