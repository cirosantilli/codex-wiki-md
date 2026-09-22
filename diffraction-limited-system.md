# Diffraction-limited system

↑ **Parent:** [Point spread function](point-spread-function-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diffraction-limited_system)

A [diffraction-limited system](diffraction-limited-system.md) has an optical response close to the ideal [diffraction](diffraction.md) response for its specified [optical pupil](optical-pupil.md), [wavelength](wavelength.md) and [optical focus](focus-optics.md). Improving the [optical aberrations](optical-aberration.md) further makes little difference to that response. This describes the optics: a poorly sampled or noisy detector can still deliver an image with much worse usable [diffraction-limited resolution](diffraction-limited-resolution.md).

The [optical pupil](optical-pupil.md) determines which [wave amplitudes](wave-amplitude.md) and [wave phases](phase-waves.md) contribute to an image point. In a scalar, [paraxial approximation](paraxial-approximation.md) at the [focal plane](focal-plane.md) of an [optical lens](lens-optics.md) in air, write the pupil transmission as $T(u,v)e^{i\phi(u,v)}$, after removing the ideal focusing phase. The [amplitude spread function](amplitude-spread-function.md) is proportional to its scaled [Fourier transform](fourier-transform-split.md):

$$
h(x,y)\propto\iint T(u,v)e^{i\phi(u,v)}\exp\left[-\frac{2\pi i}{\lambda f}(ux+vy)\right]\,du\,dv.
$$

Here $(u,v)$ are pupil coordinates, $(x,y)$ are image coordinates, $f$ is [focal length](focal-length.md), and $\lambda$ is the [wavelength](wavelength.md) in air. For a uniformly transmitting, unobscured circular [optical pupil](optical-pupil.md) at ideal [optical focus](focus-optics.md), the result is an [Airy disk](airy-disk.md) with surrounding rings. A blocked centre, support structures, or nonuniform transmission changes the ideal [point spread function](point-spread-function-split.md); “diffraction limited” does not specify one universal spot shape. The existing [Fourier model of a Lyot coronagraph](fourier-model-of-a-lyot-coronagraph.md) illustrates how pupil and focal masks deliberately alter this response.[pp. 6–8, §§D(c), E: lens Fourier transform and pupil transfer function](mit-2-71-and-2-710-optics-spring-2014-by-nicholas-x-fang/review-for-optics.md)

[Optical aberrations](optical-aberration.md) add pupil [wave phase](phase-waves.md) errors. [Defocus](defocus-aberration.md) contributes a quadratic pupil [wave phase](phase-waves.md) in the [paraxial approximation](paraxial-approximation.md), redistributing [light intensity](light-intensity.md) from the best-focused spot. The [Strehl ratio](strehl-ratio.md) compares the peak with the ideal response for the same pupil and total [radiant flux](radiant-flux.md). A broad [optical spectrum](optical-spectrum.md) produces a weighted sum of wavelength-dependent [point spread functions](point-spread-function-split.md); [chromatic aberration](chromatic-aberration.md) can additionally change [optical focus](focus-optics.md) with [wavelength](wavelength.md). Thus the operating conditions belong with any claim that a system is diffraction limited.

**Table of contents**

- [Numerical aperture](numerical-aperture.md)
- [Diffraction-limited resolution](diffraction-limited-resolution.md)
  - [Rayleigh criterion](rayleigh-criterion.md)
    - [Incoherent two-source Airy profile](incoherent-two-source-airy-profile.md)
  - [Spatial resolution element](spatial-resolution-element.md)

## ↑ Ancestors (6)

1. [Point spread function](point-spread-function-split.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Diffraction-limited system](diffraction-limited-system.md)
- [Solution](past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-2/6/i/solution.md)
- [Strehl ratio](strehl-ratio.md)
