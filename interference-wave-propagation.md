# Interference (wave propagation)

↑ **Parent:** [Physical optics](physical-optics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interference_(wave_propagation))

[Wave interference](interference-wave-propagation.md) is the reinforcement or cancellation that occurs when overlapping [wave amplitudes](wave-amplitude.md) add by the [superposition principle](superposition-principle.md). For two [monochromatic waves](monochromatic-wave.md) of the same [frequency](frequency.md), mutual [optical coherence](optical-coherence.md) means that their relative [wave phase](phase-waves.md) is stable during the observation. Equal [wave phases](phase-waves.md) give [constructive interference](constructive-interference.md); a half-cycle [phase difference](phase-difference.md) gives the [destructive interference intensity](destructive-interference-intensity.md) minimum. [Wave amplitudes](wave-amplitude.md) add before their squares determine [wave intensity](intensity-physics.md). [Ling, Sanny and Moebs, University Physics Volume 3, §3.1: coherent waves and interference](https://openstax.org/books/university-physics-volume-3/pages/3-1-youngs-double-slit-interference).

Consider two overlapping beams in a homogeneous medium, with the same [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) and individual local time-averaged [light intensities](light-intensity.md) $I_1,I_2$. Their [phase difference](phase-difference.md) $\delta$ is measured in [radians](radian.md). In the scalar detection convention, the combined local time-averaged [wave intensity](intensity-physics.md) is

$$
I=I_1+I_2+2\sqrt{I_1I_2}\cos\delta.
$$

The last term records [wave interference](interference-wave-propagation.md); adding $I_1+I_2$ alone misses it. The formula describes [irradiance](irradiance.md) when both fields propagate along the same direction, or when the same detector geometry factor is included in all three intensities. For crossing beams it describes the squared [electric field](electric-field-split.md) response, proportional to [scalar wave intensity](scalar-wave-intensity.md); a specified component of the [Poynting vector](poynting-vector.md) also requires the propagation geometry. The ideal crossing [plane waves](plane-wave.md) below make that distinction explicit.

For equal individual [light intensities](light-intensity.md) $I_1=I_2=I_0>0$, the [cosine](cosine.md) half-angle identity gives

$$
I=2I_0(1+\cos\delta)=4I_0\cos^2(\delta/2).
$$

The [constructive interference intensity](constructive-interference-intensity.md) is $4I_0$ at $\delta=0$ modulo $2\pi$, and the [destructive interference intensity](destructive-interference-intensity.md) is zero at $\delta=\pi$ modulo $2\pi$. At [phase quadrature](phase-quadrature.md), $\delta=\pi/2$, it is $2I_0$. With $I_1=1$ and $I_2=0.25$ in the same arbitrary [wave intensity](intensity-physics.md) unit, the maximum is $2.25$, the minimum is $0.25$, and the [phase quadrature](phase-quadrature.md) value is $1.25$: unequal [wave amplitudes](wave-amplitude.md) cannot cancel completely.

<a id="image-two-beam-wave-intensity-versus-phase-difference-equal-beams-reach-4-and-0-unequal-beams-reach-2-25-and-0-25"></a>
![](interference-intensity-versus-phase.png)

**[Figure 9](#image-two-beam-wave-intensity-versus-phase-difference-equal-beams-reach-4-and-0-unequal-beams-reach-2-25-and-0-25). Two-beam wave intensity versus phase difference: equal beams reach 4 and 0; unequal beams reach 2.25 and 0.25**.

Both curves use the same [wave intensity](intensity-physics.md) unit and a horizontal [angle](angle.md) in [radians](radian.md). The dashed levels are the averages over a full [phase difference](phase-difference.md) cycle. Equal beams have [interferometric visibility](interferometric-visibility.md) one; the unequal example has [interferometric visibility](interferometric-visibility.md) $0.8$.

A spatially varying [phase difference](phase-difference.md) turns the same law into [interference fringes](interference-fringe.md). Take two ideal [plane electromagnetic waves](plane-electromagnetic-wave.md) with common [wavelength](wavelength.md) $\lambda$, equal individual [light intensities](light-intensity.md) $I_0$, and propagation directions at [angles](angle.md) $+\theta$ and $-\theta$ from the $z$ axis in the $xz$ plane, with $0<\theta<\pi/2$. Both have [linear polarization](linear-polarization.md) along $y$, perpendicular to both propagation directions. Choose equal initial [wave phases](phase-waves.md); their [wavevectors](wavevector.md) and [phase difference](phase-difference.md) are

$$
\mathbf k_\pm=k(\pm\sin\theta,0,\cos\theta),\qquad k=\frac{2\pi}{\lambda},\qquad
\phi_\pm=\pm kx\sin\theta+kz\cos\theta-\omega t,\qquad
\delta=\phi_+-\phi_-=2kx\sin\theta.
$$

Here $k$ is the [wavenumber](wavenumber.md) and $\omega$ the [angular frequency](angular-frequency.md). The common $z$ and time terms cancel, so the [interference fringes](interference-fringe.md) stay at fixed $x$ for every $z$. Their [interference fringe spacing](interference-fringe-spacing.md) is

$$
\Lambda=\frac{2\pi}{2k\sin\theta}=\frac{\lambda}{2\sin\theta},\qquad
\frac{I(x,z)}{I_0}=4\cos^2(kx\sin\theta).
$$

Set the length unit to $\lambda$, so that $\lambda=1$, and take $\theta=30^\circ=\pi/6$: then $\Lambda=1$. The [constructive interference intensity](constructive-interference-intensity.md) bands lie at integer $x/\lambda$; the [destructive interference intensity](destructive-interference-intensity.md) bands lie at half-integer $x/\lambda$.

<a id="image-ideal-crossing-plane-waves-at-pm30-circ-stationary-interference-fringes-with-spacing-one-wavelength"></a>
![](two-beam-interference-fringes.png)

**[Figure 10](#image-ideal-crossing-plane-waves-at-pm30-circ-stationary-interference-fringes-with-spacing-one-wavelength). Ideal crossing plane waves at $\pm30^\circ$: stationary interference fringes with spacing one wavelength**.

The grid covers $-3\leq x/\lambda\leq3$ and $0\leq z/\lambda\leq4$; both axes are dimensionless lengths in [wavelength](wavelength.md) units. The colour scale is $I/I_0$ from zero to four, using the same single-beam normalization as the equal-beam curve above. This is an ideal [plane wave](plane-wave.md) superposition, with no slits or point sources and no near-field approximation. For these $y$-polarized [plane electromagnetic waves](plane-electromagnetic-wave.md) in [vacuum](vacuum.md), the longitudinal time-averaged [Poynting vector](poynting-vector.md) obeys $\langle S_z\rangle=I\cos\theta$; the plotted scalar $I$ therefore differs from the [irradiance](irradiance.md) through a plane normal to $z$ by that common factor. This relation follows by adding the [magnetic fields](magnetic-field-split.md) as well as the [electric fields](electric-field-split.md).

The bright peaks do not create [energy](energy-split.md). Averaging over one [interference fringe spacing](interference-fringe-spacing.md), or equivalently over one full [phase difference](phase-difference.md) cycle, gives

$$
\frac1{2\pi}\int_0^{2\pi}I(\delta)\,d\delta=I_1+I_2,
$$

because the [integral](integral-split.md) of the [cosine](cosine.md) is zero, with [sine](sine.md) as its [antiderivative](antiderivative.md). Equal beams thus average to $2I_0$, despite bright bands at $4I_0$. For the crossing-wave geometry, the average longitudinal [energy flux](energy-flux.md) is correspondingly $2I_0\cos\theta$. Bright and dark regions redistribute the incoming [energy](energy-split.md); [conservation of energy](conservation-of-energy.md) concerns the full [energy flux](energy-flux.md), rather than the height of one peak.

[Wave interference](interference-wave-propagation.md) is useful because [phase differences](phase-difference.md) convert small changes in [optical path length](optical-path-length.md) into measurable changes of [wave intensity](intensity-physics.md), as in a [Mach-Zehnder interferometer](mach-zehnder-interferometer.md). Its beauty is that the same [superposition principle](superposition-principle.md) produces both complete cancellation and fourfold brightening; adding more coherent contributions also produces the narrow peaks of a [diffraction grating](diffraction-grating.md). Feynman's treatment connects this many-source pattern directly to addition of [complex amplitudes](complex-amplitude.md). [Feynman, Leighton and Sands, The Feynman Lectures on Physics, I §30–1: the resultant amplitude of identical oscillators](https://www.feynmanlectures.caltech.edu/I_30.html#Ch30-S1).

A short proof outline uses local real fields $E_j(t)=A_j\cos(\omega t+\phi_j)$ with parallel [linear polarizations](linear-polarization.md). Write $I=C\langle(E_1+E_2)^2\rangle_t$ and $I_j=CA_j^2/2$ for the same positive conversion factor $C$. Averaging over many [wave periods](wave-period.md) while the [phase difference](phase-difference.md) stays fixed uses $\langle\cos^2(\omega t+\phi_j)\rangle_t=1/2$ and $\langle\cos(\omega t+\phi_1)\cos(\omega t+\phi_2)\rangle_t=\cos\delta/2$, giving the stated law. Equivalently, add the [complex amplitudes](complex-amplitude.md) and take the squared [complex modulus](complex-modulus.md). [Feynman, Leighton and Sands, The Feynman Lectures on Physics, I §29–5: the mathematics of interference](https://www.feynmanlectures.caltech.edu/I_29.html#Ch29-S5).

For different fixed [linear polarizations](linear-polarization.md) in a common transverse plane, the cross term acquires the [dot product](dot-product.md) of their real [unit vectors](unit-vector.md), equal to $\cos\alpha$ for relative [angle](angle.md) $\alpha$. Orthogonal [linear polarizations](linear-polarization.md) remove the cross term in polarization-insensitive scalar detection; different orientations generally only reduce it. A common [polarizer](polarizer.md) can select overlapping components and recover [wave interference](interference-wave-propagation.md). Likewise, rapid random variation of the [phase difference](phase-difference.md) removes the observed cross term only when the detector's time average has $\langle e^{i\delta(t)}\rangle_t=0$. Slowly varying [wave phases](phase-waves.md) can instead move resolved [interference fringes](interference-fringe.md), and biased or incompletely sampled [wave phases](phase-waves.md) can leave residual contrast. Finite [optical coherence](optical-coherence.md) therefore depends on the observation time as well as the fields.

**Table of contents**

- [Interferometry](interferometry.md)
  - [Optical interferometry](optical-interferometry.md)
    - [Atmospheric piston in interferometry](atmospheric-piston-in-interferometry.md)
    - [Fringe tracking](fringe-tracking.md)
- [Moiré pattern](moire-pattern.md)
  - [Moiré fringe](moire-fringe.md)
    - [Moiré fringe spacing formula](moire-fringe-spacing-formula.md)
- [Destructive interference](destructive-interference.md)
- [Thin-film interference](thin-film-interference.md)
  - [Adjacent reflected minima of an air-film-air layer](adjacent-reflected-minima-of-an-air-film-air-layer.md)
  - [Antireflection coating](antireflection-coating.md)
    - [Spectral colour of an antireflection coating](spectral-colour-of-an-antireflection-coating.md)
  - [Angular fringe spacing of a transparent film](angular-fringe-spacing-of-a-transparent-film.md)
  - [Newton's rings](newton-s-rings.md)
- [Double-slit experiment](double-slit-experiment.md)
  - [Incidence-independent adjacent-fringe wavelength](incidence-independent-adjacent-fringe-wavelength.md)
    - [Unknown incidence offset in double-slit phase](unknown-incidence-offset-in-double-slit-phase.md)
  - [Single-electron interference pattern buildup](single-electron-interference-pattern-buildup.md)
  - [Double-slit interference](double-slit-interference.md)
    - [Fraunhofer diffraction of unequal slits](fraunhofer-diffraction-of-unequal-slits.md)
      - [Fringe-count convention inside a diffraction envelope](fringe-count-convention-inside-a-diffraction-envelope.md)
    - [Phase-reversed double-slit diffraction](phase-reversed-double-slit-diffraction.md)
      - [Half-slit phase-step diffraction factorization](half-slit-phase-step-diffraction-factorization.md)
- [Phase matching](phase-matching.md)
  - [Type-II phase matching](type-ii-phase-matching.md)
  - [Type-I phase matching](type-i-phase-matching.md)
  - [Quasi-phase-matching](quasi-phase-matching.md)
    - [Periodically poled lithium niobate](periodically-poled-lithium-niobate.md)
  - [Phase mismatch](phase-mismatch.md)
    - [Nonlinear optical coherence length](nonlinear-optical-coherence-length.md)
- [Beat](beat.md)
  - [Two-tone output of a linear resonant circuit](two-tone-output-of-a-linear-resonant-circuit.md)
- [Constructive interference intensity](constructive-interference-intensity.md)
- [Destructive interference intensity](destructive-interference-intensity.md)
- [Interference fringe](interference-fringe.md)
  - [Fringe shift](fringe-shift.md)
  - [Interference fringe spacing](interference-fringe-spacing.md)
- [Which-path information](which-path-information.md)
- [Interferometric visibility](interferometric-visibility.md)
  - [Signed coherence and fringe visibility](signed-coherence-and-fringe-visibility.md)

## ↑ Ancestors (5)

1. [Physical optics](physical-optics-split.md)
2. [Optics](optics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
