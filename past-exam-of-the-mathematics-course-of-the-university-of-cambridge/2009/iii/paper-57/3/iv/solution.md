<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A blackbody photon density perturbation gives an intrinsic temperature fluctuation $\Theta_0=\delta_\gamma/4$. The baryon/electron bulk velocity produces a [Doppler effect](../../../../../../doppler-effect.md) at last scattering. In the common-potential convention of part (ii),

$$
\theta_b\simeq\theta_\gamma=\frac3{4k^2}\delta_\gamma'.
$$

Ignoring the slowly varying damping derivative at leading acoustic order, differentiating the density cosine produces a velocity sine. Thus **density and velocity acoustic sources are approximately a quarter cycle out of phase**. For regular adiabatic initial conditions the density oscillation has approximately a common cosine phase across modes; this phase coherence is what makes a sequence of peaks instead of a smooth incoherent superposition.

Let $D_*=\tau_0-\tau_*$ be the comoving distance to last scattering and $r_s(\tau_*)=\int^{\tau_*}c_s\,d\tau$ its [sound horizon](../../../../../../sound-horizon.md). In the present limit $r_s\simeq\tau_*/\sqrt3$. Density extrema have $kr_s\simeq m\pi$, whereas velocity extrema have $kr_s\simeq(m+1/2)\pi$. The projection from spatial wavenumber to high angular multipoles is roughly $\ell\simeq kD_*$, giving an acoustic spacing

$$
\boxed{\Delta\ell\simeq\pi\frac{D_*}{r_s}.}
$$

The [Doppler effect](../../../../../../doppler-effect.md) fills some density troughs and modifies the detailed peak shapes; its different projection prevents treating it as an identical second series of narrow peaks.

For clarity, choose the sightline to point outward from the observer and let its angle to $\mathbf k$ have cosine $\mu$. The intrinsic-plus-emitter-Doppler source is then $[\delta_\gamma/4-ik\mu\theta_b]e^{ik\mu D_*}$. Expanding its angular dependence gives the [angular projection of density and Doppler acoustic sources](../../../../../../angular-projection-of-density-and-doppler-acoustic-sources.md)

$$
\Theta_\ell(k)\simeq\frac{\delta_\gamma(k,\tau_*)}{4}j_\ell(kD_*)
-k\theta_b(k,\tau_*)j_\ell'(kD_*).
$$

The second sign follows from the chosen outward sightline and $v_b^i=ik^i\theta_b$; it changes with the sightline convention together with the velocity projection. The $j_\ell$ are [Spherical Bessel functions](../../../../../../spherical-bessel-function.md). Both sources are proportional to the primordial curvature. If $\mathcal T_\ell=\Theta_\ell/\zeta_*$, their angular spectrum in the usual continuum Fourier normalization is

$$
C_\ell=\frac2\pi\int_0^\infty k^2dk\,P_\zeta(k)|\mathcal T_\ell(k)|^2.
$$

This formula includes the density-velocity cross term, not just a sum of independent source powers.

Photon diffusion multiplies both leading source amplitudes by $e^{-k^2/k_D^2}$, so their power carries $e^{-2k^2/k_D^2}$. The approximate angular damping scale is

$$
\boxed{\ell_D\simeq k_D(\tau_*)D_*;\qquad\text{high-multipole power is exponentially suppressed}.}
$$

This produces the damping tail in the [Cosmic microwave background power spectrum](../../../../../../cosmic-microwave-background-power-spectrum.md). Finite last-scattering thickness adds further small-scale averaging. Gravity, baryon loading and later propagation alter detailed peak locations and heights, but the oscillatory peak sequence, phase-shifted velocity contribution and diffusion damping follow directly from the simplified solution obtained here.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
