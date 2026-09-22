<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first mechanism is [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md): finite photon mean free paths allow radiation to diffuse out of compressions, while velocity slip and radiation shear dissipate acoustic motion. A Fourier diffusion equation has $X'=-D(\tau)k^2X$, hence $X\propto\exp[-k^2\int D\,d\tau]$. For the polarization-inclusive tightly coupled plasma, a useful expression is

$$
\boxed{\frac1{k_D^2}=\int^{\tau_*}\frac{d\tau}{6\dot\kappa}
\left[\frac{R^2}{(1+R)^2}+\frac{16}{15(1+R)}\right],\qquad
X\propto e^{-k^2/k_D^2}.}
$$

The positive scattering rate is $\dot\kappa=a n_e\sigma_T$, and $R$ is the [baryon loading parameter](../../../../../../baryon-loading-parameter.md). The two terms represent heat conduction from velocity slip and photon shear viscosity. **The mode amplitude has an approximately Gaussian cutoff in $k$; power is suppressed by $e^{-2k^2/k_D^2}$.** The formula assumes tight coupling and slowly varying coefficients before decoupling.

The second mechanism is [finite-width last-scattering damping](../../../../../../finite-width-last-scattering-damping.md). Photons emerge from a range of times and depths, so rapidly varying sources are averaged rather than observed at one sharply defined phase. Approximate the normalized [cosmological visibility function](../../../../../../cosmological-visibility-function.md) by a Gaussian of width $\sigma_\tau$. For a radial plane-wave phase,

$$
\boxed{\int g(\tau)e^{ik\mu(\tau-\tau_*)}d\tau
=e^{-(k\mu\sigma_\tau)^2/2}.}
$$

The associated power factor is $e^{-(k\mu\sigma_\tau)^2}$. An acoustic factor $e^{\pm ikc_s\tau}$ is likewise averaged, replacing $k\mu$ by $k(\mu\pm c_s)$ in the constant-sound-speed approximation. Thus fine radial structure and rapid acoustic time oscillations are suppressed once their phase changes substantially across the visibility width. This is an averaging effect after the perturbations exist; [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md) physically erases them by diffusion. Angular projection and the evolving source determine the final isotropic damping envelope, so the radial $\mu$ dependence must not be silently discarded.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
