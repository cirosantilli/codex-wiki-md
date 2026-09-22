# First-order optical coherence

↑ **Parent:** [Optical coherence](optical-coherence.md)

Consider one selected [polarization of waves](polarization-waves.md), represented by complex fields $E_1(t)$ and $E_2(t)$ at two sampling positions. Suppose their second moments are finite and stationary: $J_j=\langle|E_j(t)|^2\rangle$ and the following uncentered [wave-field correlation](uncentered-wave-field-correlation.md) do not depend on the absolute time $t$. Define

$$
\Gamma_{12}(\tau)=\langle E_1^*(t)E_2(t+\tau)\rangle,
\qquad g^{(1)}_{12}(\tau)=\frac{\Gamma_{12}(\tau)}{\sqrt{J_1J_2}},
\qquad J_1,J_2>0.
$$

The star denotes the [complex conjugate](complex-conjugate.md); brackets denote an [ensemble average](expected-value-split.md). A long detector average estimates this quantity only if it adequately samples the fluctuations. The superscript $1$ identifies a field correlation: it does not mean the [autocorrelation](autocorrelation.md) of the measured [light intensity](light-intensity.md). The one-position version is $g^{(1)}(\tau)=\langle E^*(t)E(t+\tau)\rangle/\langle|E|^2\rangle$, so $g^{(1)}(0)=1$ for every nonzero field covered by this definition; this alone says nothing about its correlation at nonzero delay. [Rüdiger Paschotta, RP Photonics Encyclopedia, Coherence Time: stationary complex field correlation](https://www.rp-photonics.com/coherence_time.html).

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $0\leq|g^{(1)}_{12}(\tau)|\leq1$. At a specified delay, magnitude one means $E_2(t+\tau)=aE_1(t)$ in mean square for a fixed nonzero complex $a$: the samples have a reproducible relation in both [wave amplitude](wave-amplitude.md) and [wave phase](phase-waves.md). Magnitude zero means the averaged field cross term vanishes. It need not mean statistical [independence](independent-random-variables.md). A deterministic [phase difference](phase-difference.md) changes the argument of $g^{(1)}$, not its [complex modulus](complex-modulus.md); a distorted but fixed [wavefront](wavefront.md) can therefore remain fully coherent. [Paschotta, Coherence: static distortions versus fluctuating distortions](https://www.rp-photonics.com/coherence.html).

To see the observable, recombine the samples in the same detected spatial mode with matched [wave polarizations](polarization-waves.md). With a common positive conversion factor $C$, let $I_j=CJ_j$ be the single-arm [light intensities](light-intensity.md) reaching that detector. Adding $E_1(t)+e^{i\phi}E_2(t+\tau)$ gives

$$
I(\phi,\tau)=I_1+I_2+2\sqrt{I_1I_2}\,\operatorname{Re}\!\left[e^{i\phi}g^{(1)}_{12}(\tau)\right],
\qquad \mathcal V(\tau)=\frac{2\sqrt{I_1I_2}}{I_1+I_2}|g^{(1)}_{12}(\tau)|.
$$

This follows simply by expanding the squared [complex modulus](complex-modulus.md) and averaging, then taking the maximum and minimum as $\phi$ spans a full cycle. The extra [wave phase](phase-waves.md) scan must leave $I_1,I_2$ and the magnitude of the correlation effectively unchanged. Thus [interferometric visibility](interferometric-visibility.md) equals $|g^{(1)}|$ only for equal nonzero [light intensities](light-intensity.md) and ideal mode matching. For $I_2/I_1=1/4$, perfectly coherent beams have [interferometric visibility](interferometric-visibility.md) $0.8$; a measured value $0.4$ would imply $|g^{(1)}|=0.5$ under these assumptions. Orthogonal [linear polarizations](linear-polarization.md), background light, unresolved [interference fringes](interference-fringe.md) or vibrations can reduce measured contrast further. One absent arm gives zero contrast and makes the normalized two-sample correlation undefined.

**Table of contents**

- [Polarization overlap in interferometric visibility](polarization-overlap-in-interferometric-visibility.md)
- [Temporal optical coherence](temporal-optical-coherence.md)
  - [Unequal-line visibility in a spectral doublet](unequal-line-visibility-in-a-spectral-doublet.md)
  - [Delayed-fibre linewidth measurement](delayed-fibre-linewidth-measurement.md)
  - [Two-line coherence beating](two-line-coherence-beating.md)
    - [Spectral doublet from Michelson visibility revivals](spectral-doublet-from-michelson-visibility-revivals.md)
  - [Temporal coherence from crossed beams](temporal-coherence-from-crossed-beams.md)
    - [Optical path delay in crossed-beam interference](optical-path-delay-in-crossed-beam-interference.md)
  - [Optical coherence time](optical-coherence-time.md)
    - [Optical coherence length](optical-coherence-length.md)
      - [Coherence length from a finite spectral band](coherence-length-from-a-finite-spectral-band.md)
  - [Michelson interferometer](michelson-interferometer.md)
    - [Two-wavelength Michelson rephasing](two-wavelength-michelson-rephasing.md)
    - [Common-arm phase cancellation in a balanced interferometer](common-arm-phase-cancellation-in-a-balanced-interferometer.md)
    - [Round-trip phase in a Michelson interferometer](round-trip-phase-in-a-michelson-interferometer.md)
    - [Precision displacement measurement with a Michelson interferometer](precision-displacement-measurement-with-a-michelson-interferometer.md)
    - [Michelson measurement of length in cadmium wavelengths](michelson-measurement-of-length-in-cadmium-wavelengths.md)
- [Spatial optical coherence](spatial-optical-coherence.md)
  - [Van Cittert-Zernike theorem](van-cittert-zernike-theorem.md)
  - [Uniform-disk spatial coherence](uniform-disk-spatial-coherence.md)
  - [Transverse optical coherence length](transverse-optical-coherence-length.md)

## ↑ Ancestors (6)

1. [Optical coherence](optical-coherence.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Coherence length from a finite spectral band](coherence-length-from-a-finite-spectral-band.md)
- [Coherent beam splitter recombination](coherent-beam-splitter-recombination.md)
- [Delayed-fibre linewidth measurement](delayed-fibre-linewidth-measurement.md)
- [Double-slit interference](double-slit-interference.md)
- [Michelson interferometer](michelson-interferometer.md)
- [Optical coherence](optical-coherence.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2017/1/b/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2021/section-b/b5/a/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022/section-a/3/solution.md)
- [Quantum theory of optical coherence](quantum-theory-of-optical-coherence.md)
- [Siegert relation](siegert-relation.md)
- [Spatial optical coherence](spatial-optical-coherence.md)
- [Two-line coherence beating](two-line-coherence-beating.md)
- [Uniform-disk stellar visibility](uniform-disk-stellar-visibility.md)
