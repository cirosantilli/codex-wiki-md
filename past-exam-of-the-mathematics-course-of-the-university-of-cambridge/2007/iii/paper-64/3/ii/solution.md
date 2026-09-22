<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Before decoupling, rapid [Thomson scattering](../../../../../../thomson-scattering.md) makes the [photon](../../../../../../photon.md) distribution nearly isotropic in the local photon-fluid rest frame. A local blackbody [temperature](../../../../../../temperature.md) perturbation changes its [energy density](../../../../../../energy-density.md) by $\delta_\gamma=4\delta T/T$. A first-order boost by the fluid [velocity](../../../../../../velocity.md) adds a [temperature](../../../../../../temperature.md) [photon dipole](../../../../../../photon-dipole.md) $\mathbf n\cdot\mathbf v$; it does not generate a [photon quadrupole](../../../../../../photon-quadrupole.md) until second order in that boost. Thus the [photon brightness perturbation](../../../../../../photon-brightness-perturbation.md) at instantaneous decoupling is

$$
\Delta_* =\delta_{\gamma *}+4\mathbf n\cdot\mathbf v_*.
$$

Higher angular moments are suppressed by the [photon](../../../../../../photon.md) mean-free-path to perturbation-length ratio in the [tight-coupling approximation](../../../../../../tight-coupling-approximation.md). The idealized equilibrium assumption neglects those finite-mean-free-path corrections, polarization effects and finite thickness of the last-scattering surface. It is not an assertion that collisionless [photons](../../../../../../photon.md) remain isotropic after decoupling. The distinction between a fluid treatment and the subsequent hierarchy is discussed in [the primary synchronous and Newtonian perturbation treatment](https://arxiv.org/abs/astro-ph/9506072).

Let $\mu=\hat{\mathbf k}\cdot\mathbf n$ and $W(\tau)=e^{ik\mu(\tau-\tau_0)}$. Multiplication of the [synchronous photon brightness equation](../../../../../../synchronous-photon-brightness-equation.md) by its [integrating factor](../../../../../../integrating-factor.md) gives

$$
\left(e^{ik\mu\tau}\Delta\right)'
=-2e^{ik\mu\tau}h'_{ij}n^in^j.
$$

Integration from $\tau_*=\tau_{\rm dec}$ to $\tau_0$ and division by four yield

$$
\boxed{\Theta(\mathbf k,\mu,\tau_0)
=\left(\frac{\delta_{\gamma *}}4+\mathbf n\cdot\mathbf v_*\right)
 e^{-ik\mu(\tau_0-\tau_*)}
-\frac12\int_{\tau_*}^{\tau_0}W(\tau)h'_{ij}n^in^j\,d\tau,
\qquad\Theta=\frac{\Delta T}{T}.}
$$

For the real-space observation point $\mathbf x_0$, the corresponding background ray is $\mathbf x(\tau)=\mathbf x_0-\mathbf n(\tau_0-\tau)$. Fourier inversion gives the [synchronous Sachs-Wolfe line-of-sight formula](../../../../../../synchronous-sachs-wolfe-line-of-sight-formula.md)

$$
\boxed{\Theta(\mathbf x_0,\mathbf n,\tau_0)
=\frac14\delta_\gamma(\mathbf x_*,\tau_*)
+\mathbf n\cdot\mathbf v(\mathbf x_*,\tau_*)
-\frac12\int_{\tau_*}^{\tau_0}
 h'_{ij}(\mathbf x(\tau),\tau)n^in^j\,d\tau,
\quad\mathbf x_*=\mathbf x(\tau_*).}
$$

Every source is evaluated at its appropriate point on the ray, rather than at the observation position. Here $\mathbf n$ is [photon](../../../../../../photon.md) propagation direction, opposite to the outward observer-to-source sky direction; changing that convention changes the written sign of the Doppler projection consistently.

The first term is the intrinsic [photon](../../../../../../photon.md) [temperature](../../../../../../temperature.md) at last scattering. On wavelengths larger than the [sound horizon](../../../../../../sound-horizon.md), it retains primordial adiabatic information; inside that horizon the [photon-baryon fluid](../../../../../../photon-baryon-fluid.md) has acoustic [energy density](../../../../../../energy-density.md) oscillations, producing the acoustic [temperature](../../../../../../temperature.md) peaks. The second term is the [Doppler effect](../../../../../../doppler-effect.md) from the fluid's bulk motion at emission. A regular long-wavelength [velocity](../../../../../../velocity.md) is gradient-suppressed; the Doppler contribution is important near and below the acoustic horizon, with its acoustic phase displaced from that of the [energy density](../../../../../../energy-density.md) oscillation.

The integral is the gravitational energy shift produced by the changing spatial [metric tensor](../../../../../../metric-tensor.md) along the [photon](../../../../../../photon.md) path. In [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md) it includes endpoint gravitational redshifts as well as evolving-potential effects. It must not be identified solely with the [Integrated Sachs-Wolfe effect](../../../../../../integrated-sachs-wolfe-effect.md): in [Newtonian gauge](../../../../../../newtonian-gauge.md) the same total separates into the ordinary last-scattering [Sachs-Wolfe effect](../../../../../../sachs-wolfe-effect.md), local observer terms, and an integral of time-varying potentials. The ordinary contribution is important on scales outside the [sound horizon](../../../../../../sound-horizon.md) at decoupling. A late integrated contribution is strongest on large angular scales when dark energy or curvature changes the potentials; evolution around [matter-radiation equality](../../../../../../matter-radiation-equality.md) also contributes near the first acoustic scales.

The relevant comoving sound scale is $r_s(\tau_*)=\int^{\tau_*}c_s(\tau)d\tau$, while the projection distance is $D_*\simeq\tau_0-\tau_*$. Modes project roughly to [photon temperature multipole](../../../../../../photon-temperature-multipole.md) $\ell\sim kD_*$, and the acoustic scale is $\ell\sim D_*/r_s$, with successive peak spacing of order $\pi D_*/r_s$. At much shorter wavelengths [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md) and the finite last-scattering thickness suppress [energy density](../../../../../../energy-density.md) and [velocity](../../../../../../velocity.md) anisotropies; the instantaneous-decoupling approximation alone does not model that cutoff. These scale distinctions explain why the three terms cannot be assigned one common range of important wavelengths.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
