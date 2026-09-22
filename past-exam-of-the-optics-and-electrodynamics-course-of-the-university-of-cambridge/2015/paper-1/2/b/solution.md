<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [spectral line](../../../../../spectral-line.md) has finite width when the emitted or absorbed field loses coherence, or when different emitters have different transition frequencies. It is useful to distinguish [homogeneous spectral broadening](../../../../../homogeneous-spectral-broadening.md) of each emitter from [inhomogeneous spectral broadening](../../../../../inhomogeneous-spectral-broadening.md) across the ensemble.

**Finite lifetime and [dephasing](../../../../../dephasing-channel.md).** For an upper-state population lifetime $\tau$ and a stable lower state, the radiating [amplitude](../../../../../wave-amplitude.md) decays as $e^{-t/(2\tau)}$. Its Fourier spectrum is Lorentzian, with [full width at half maximum](../../../../../full-width-at-half-maximum.md)

$$
\Delta\omega_{\rm nat}=\frac1\tau,\qquad
\Delta\nu_{\rm nat}=\frac1{2\pi\tau}.
$$

More generally, an [optical coherence time](../../../../../optical-coherence-time.md) $T_2$ gives $\Delta\omega_{\rm hom}=2/T_2$. Both level lifetimes and pure [dephasing](../../../../../dephasing-channel.md) can contribute to $1/T_2$. Distinguishing population lifetime from [amplitude](../../../../../wave-amplitude.md) coherence time prevents the usual factor-of-two error.

**Thermal motion.** To first order in velocity, $\delta\nu=\nu_0v_\parallel/c$. A [Maxwell-Boltzmann velocity distribution](../../../../../maxwell-boltzmann-velocity-distribution.md) therefore produces a Gaussian profile, with

$$
\sigma_\nu=\frac{\nu_0}{c}\sqrt{\frac{k_BT}{M}},\qquad
\boxed{\Delta\nu_D=\frac{\nu_0}{c}\sqrt{\frac{8k_BT\ln2}{M}}}.
$$

This is inhomogeneous [doppler broadening](../../../../../doppler-broadening.md): different velocity classes have different [resonance](../../../../../resonance.md) frequencies. A distribution of bulk velocities can add further broadening, while a common bulk velocity shifts the line.

**Interactions with the surroundings.** Collisions can interrupt the dipole [wave phase](../../../../../phase-waves.md) and perturb the [energy](../../../../../energy-split.md) levels, producing [pressure broadening](../../../../../pressure-broadening.md) and shifts. In the impact approximation, approximately exponential [wave phase](../../../../../phase-waves.md) relaxation produces a Lorentzian contribution; its rate increases with perturber density times an appropriate velocity-averaged collision cross section. Slowly varying electric microfields can instead produce non-Lorentzian Stark profiles. Neutral perturbers, charged perturbers and [resonance](../../../../../resonance.md) interactions need not produce the same line shape. These mechanisms and the Gaussian thermal limit are distinguished in NIST's atomic-spectroscopy compendium.[section 20, Spectral Line Shapes, Widths, and Shifts: Doppler and pressure broadening](../../../../../atomic-spectroscopy-a-compendium-of-basic-ideas-notation-data-and-formulas-by-william-c-martin-and-wolfgang-wiese.md)

Finite observation time limits coherence; [transit-time broadening](../../../../../transit-time-broadening.md) also occurs for particles crossing a narrow optical beam. Strong resonant excitation causes [power broadening](../../../../../power-broadening.md): for an ideal lifetime-limited two-level transition, $\Delta\omega=\Gamma\sqrt{1+s}$ with population decay rate $\Gamma$ and [saturation parameter](../../../../../saturation-parameter.md) $s$. Unresolved [fine structure](../../../../../fine-structure.md), [hyperfine structure](../../../../../hyperfine-structure.md), isotope components, or spatially varying Zeeman and Stark shifts may look like a single broadened feature even though several frequencies are present.

The observed spectrum is additionally convolved with the instrument response. A Gaussian Doppler contribution convolved with Lorentzian homogeneous broadening gives a [Voigt profile](../../../../../voigt-profile.md); their full widths do not generally add in quadrature. An informative experiment varies temperature, perturber pressure and excitation intensity separately, calibrates the spectrometer response with a narrower reference, and checks optical thickness or self-absorption. Extrapolation to weak excitation and low pressure helps isolate the lifetime contribution, while a Doppler-free technique is needed if velocity spread still dominates.

<a id="2/b/image-original-normalized-gaussian-lorentzian-and-voigt-line-shape-comparison"></a>
![](../../../../../past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2015/paper-1-line-profiles.png)

**[Figure 1](#2/b/image-original-normalized-gaussian-lorentzian-and-voigt-line-shape-comparison). Original normalized Gaussian, Lorentzian and Voigt line-shape comparison**.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
