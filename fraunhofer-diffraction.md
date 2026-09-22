# Fraunhofer diffraction

↑ **Parent:** [Physical optics](physical-optics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fraunhofer_diffraction)

[Fraunhofer diffraction](fraunhofer-diffraction.md) is the far-field approximation for [diffraction](diffraction.md): contributions from an [aperture](aperture.md) reach a selected observation direction with approximately linear path-dependent [wave phases](phase-waves.md). Adding their [complex amplitudes](complex-amplitude.md) gives a [Fourier transform](fourier-transform.md) of the field across the [aperture](aperture.md). It also describes the appropriate rear [focal plane](focal-plane.md) of an ideal [optical lens](lens-optics.md) under coherent plane-wave illumination. The [diffraction grating](diffraction-grating.md) examples use this regime. [Richard Fitzpatrick, Wave Optics, §10.9: Two-dimensional Fourier optics](https://farside.ph.utexas.edu/teaching/315/Waves/node98.html); [MIT 2.71/2.710 Optics, The ideal thin lens as a Fourier transform engine, slides 12–14: back focal plane diffraction](https://web.mit.edu/2.710/Fall06/2.710-wk10-a-sl.pdf).

For a slit of width $a$, [wavelength](wavelength.md) $\lambda$ and screen distance $L$, sufficient conditions near the forward direction are

$$
L\gg a,\qquad L\gg\frac{a^2}{\lambda},\qquad \frac{a^2}{\lambda L}\ll1.
$$

The last two statements are equivalent: the important comparison is with $a^2/\lambda$, rather than just with the slit width. For a finite rectangular [aperture](aperture.md), check the corresponding condition for both transverse dimensions. The [single-slit diffraction](single-slit-diffraction.md) calculation treats the transverse cut associated with width $a$. [Richard Fitzpatrick, Wave Optics, §10.10, equations 10.93–10.96: far-field conditions](https://farside.ph.utexas.edu/teaching/315/Waves/node99.html).

A short explanation is that the distance from slit coordinate $x$ to an observation point at distance $R$ and [angle](angle.md) $\theta$ is

$$
r(x)=\sqrt{R^2-2Rx\sin\theta+x^2}=R-x\sin\theta+\frac{x^2\cos^2\theta}{2R}+O(a^3/R^2).
$$

The linear term supplies the [phase difference](phase-difference.md); the quadratic term supplies a [wave phase](phase-waves.md) error of order $a^2/(\lambda R)$, since the [wavenumber](wavenumber.md) is $2\pi/\lambda$. Near the forward direction $R\approx L$, so the stated condition makes this error small. This is why a distant screen permits the simple [single-slit diffraction](single-slit-diffraction.md) formula. [Fitzpatrick, §10.9, equations 10.70–10.74: path expansion and aperture superposition](https://farside.ph.utexas.edu/teaching/315/Waves/node98.html).

**Table of contents**

- [Single-slit diffraction](single-slit-diffraction.md)

## ↑ Ancestors (5)

1. [Physical optics](physical-optics.md)
2. [Optics](optics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Diffraction grating](diffraction-grating.md)
- [Diffraction-limited resolution](diffraction-limited-resolution.md)
- [Focal ratio](focal-ratio.md)
- [Fourier model of a Lyot coronagraph](fourier-model-of-a-lyot-coronagraph.md)
- [Fraunhofer diffraction](fraunhofer-diffraction.md)
- [Single-slit diffraction](single-slit-diffraction.md)
