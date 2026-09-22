<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $q_*=k\tau_{\rm dec}/\sqrt3$ and $E_D=\exp(-k^2/k_D^2)$ at last scattering. For random oscillator amplitudes, define spectra $P_A,P_B$ and cross-spectrum $P_{AB}$ using the same Fourier normalization as the density spectrum. Averaging the solution's squared modulus gives

$$
P_{\delta_\gamma}=E_D^2\left[P_A\cos^2q_*+P_B\sin^2q_*+2\operatorname{Re}P_{AB}\sin q_*\cos q_*\right].
$$

Consequently the intrinsic-temperature source has variance spectrum $P_{\delta_\gamma}/16$. **A common acoustic phase is necessary for pronounced peaks in the variance.** Equal independent sine/cosine amplitudes would erase them. A regular growing [adiabatic mode](../../../../../../adiabatic-mode.md) begins with negligible velocity outside the sound horizon and selects approximately the cosine phase, $B\simeq0$, preserving a $\cos^2q_*$ sequence. This illustrates [coherent initial phases are needed for acoustic variance peaks](../../../../../../coherent-initial-phases-are-needed-for-acoustic-variance-peaks.md).

From continuity, $\theta_\gamma=3\delta_\gamma'/(4k^2)$. Ignoring the small damping correction in this velocity relation, the coherent cosine solution gives

$$
\theta_\gamma\simeq-\frac{\sqrt3}{4k}A E_D\sin q_*,\qquad
\mathbf v_\gamma=i\mathbf k\theta_\gamma.
$$

The [Doppler CMB anisotropy](../../../../../../doppler-cmb-anisotropy.md) source therefore has directional variance $3\mu^2P_AE_D^2\sin^2q_*/16$, where $\mu=\hat{\mathbf n}\cdot\hat{\mathbf k}$. Its velocity maxima lie between density maxima: compression and bulk motion are a quarter acoustic period apart.

Angular projection must also be included. Let $\chi_*=\tau_0-\tau_{\rm dec}$, assume a thin last-scattering surface, and choose the emission phase $e^{ik\chi_*\mu}$. The coherent intrinsic-plus-Doppler radial response is proportional to

$$
\Theta_\ell(k)=\frac{E_D}{4}\left[\cos q_*\,j_\ell(k\chi_*)-\sqrt3\sin q_*\,j_\ell'(k\chi_*)\right].
$$

The derivative follows from $i\mu e^{ix\mu}=\partial_x e^{ix\mu}$ and the velocity sign above. A reversed line-of-sight convention reverses the corresponding Doppler sign consistently. The [CMB angular power spectrum](../../../../../../cosmic-microwave-background-power-spectrum.md) is $C_\ell=(2/\pi)\int k^2dk\,P_A(k)|\Theta_\ell(k)|^2$ in this simplified model. Squaring the combined response keeps its correlated density–velocity cross term; adding two independent angular powers would discard that correlation. The derivative Bessel projection also spreads the Doppler contribution differently from the density contribution.

The [sound horizon](../../../../../../sound-horizon.md) here is $r_s\simeq\tau_{\rm dec}/\sqrt3$. Intrinsic acoustic extrema occur near $kr_s=n\pi$, mapping roughly to $\ell_n\simeq n\pi\chi_*/r_s$, with interleaved velocity extrema and projection broadening. [Cosmic microwave background diffusion damping](../../../../../../cosmic-microwave-background-diffusion-damping.md) suppresses both contributions exponentially at $k\gtrsim k_D$, or multipoles $\ell\gtrsim k_D\chi_*$. Modes outside the sound horizon have no completed acoustic oscillation.

The metric integral represents gravitational redshift, including contributions that in another gauge are separated into endpoint [Sachs-Wolfe effects](../../../../../../sachs-wolfe-effect.md) and [Integrated Sachs-Wolfe effects](../../../../../../integrated-sachs-wolfe-effect.md). It is not correct to call the entire synchronous metric integral only a late-time integrated effect. Large-scale metric/curvature fluctuations remain important where photon pressure cannot redistribute matter causally and produce the broad large-angle signal rather than just the pressure-oscillation sequence. Potential evolution during radiation-to-matter transition also drives and shifts acoustic amplitudes near horizon entry; late accelerating-era evolution adds a large-angle integrated signal. These effects are excluded by the oscillator's instruction to ignore metric perturbations. Even if the Newtonian-gauge potential is constant in matter domination, synchronous $h'_{ij}$ need not vanish, and the complete observable requires the consistent density, velocity and metric combination.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
