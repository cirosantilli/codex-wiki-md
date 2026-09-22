# Airy disk

↑ **Parent:** [Point spread function](point-spread-function-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Airy_disk)

The [Airy disk](airy-disk.md) is the central bright region, up to the first dark ring, in the scalar [diffraction](diffraction.md) pattern of a uniformly illuminated, unobscured circular [aperture](aperture.md). The whole pattern includes the weaker surrounding rings; its radius is distinct from its [full width at half maximum](full-width-at-half-maximum.md).

For a circular [optical pupil](optical-pupil.md) of [diameter](diameter.md) $D$ under normal, uniform monochromatic [plane wave](plane-wave.md) illumination, [Fraunhofer diffraction](fraunhofer-diffraction.md) gives

$$
\frac{I(\theta)}{I_0}=P(u)=\left[\frac{2J_1(u)}{u}\right]^2,\qquad u=\frac{\pi D\sin\theta}{\lambda},\qquad P(0)=1.
$$

Here $I_0$ is the on-axis [light intensity](light-intensity.md), $\theta$ is the [angle](angle.md) from the [optical axis](optical-axis.md), $\lambda$ is the [wavelength](wavelength.md) in the propagation medium, and $J_1$ is the order-one [Bessel function of the first kind](bessel-function-of-the-first-kind.md). The [paraxial approximation](paraxial-approximation.md) replaces $\sin\theta$ by $\theta$, measured in [radians](radian.md). The first positive zero $j_{1,1}=3.831705970\ldots$ gives

$$
\sin\theta_1=\frac{j_{1,1}}{\pi}\frac{\lambda}{D},\qquad \theta_1\simeq1.219669891\frac{\lambda}{D}\simeq1.22\frac{\lambda}{D}.
$$

This is the angular radius of the [Airy disk](airy-disk.md); the angular diameter is twice as large. The [Airy disk derivation](airy-disk-derivation.md) explains the origin of the [Bessel function of the first kind](bessel-function-of-the-first-kind.md) and of the numerical coefficient.[equations 10.78–10.85 and Table 10.1: circular-aperture response and first zero](oscillations-and-waves-by-richard-fitzpatrick/two-dimensional-fourier-optics.md)

<a id="image-ideal-circular-aperture-intensity-central-disk-dark-rings-and-radial-profile"></a>
![](airy-disk-radial-intensity.png)

**[Figure 2](#image-ideal-circular-aperture-intensity-central-disk-dark-rings-and-radial-profile). Ideal circular-aperture intensity: central disk, dark rings and radial profile**.

The image and both radial curves show the same calculated [light intensity](light-intensity.md), divided by its peak. The image's [logarithmic scale](logarithmic-scale.md) makes the weak rings visible; its colour is a display choice. The linear curve shows how small the ring peaks are compared with the centre. A dark ring marks a zero of [wave amplitude](wave-amplitude.md), produced by cancellation across the [optical pupil](optical-pupil.md); it is not the edge of all transmitted [light](light.md). The first [Airy disk](airy-disk.md) contains about $83.78\%$ of the total [radiant flux](radiant-flux.md), as calculated in [Airy disk normalization and encircled energy](airy-disk-normalization-and-encircled-energy.md).

For an original design example, take an ideal [optical lens](lens-optics.md) in air with [focal length](focal-length.md) $f=100\,\mathrm{mm}$, circular [optical pupil](optical-pupil.md) [diameter](diameter.md) $D=5.00\,\mathrm{mm}$ and [wavelength](wavelength.md) $\lambda=550\,\mathrm{nm}$. In the [focal plane](focal-plane.md), the radial coordinate $r\simeq f\theta$ gives

$$
\theta_1\simeq1.34164\times10^{-4}\,\mathrm{rad},\qquad r_1\simeq1.219669891\frac{\lambda f}{D}=13.4164\,\mathrm{\mu m}.
$$

The first-zero diameter is $26.8327\,\mathrm{\mu m}$. Solving $P(u_{1/2})=1/2$ gives $u_{1/2}=1.616339948\ldots$, so the diameter measured by [full width at half maximum](full-width-at-half-maximum.md) is only

$$
w_{1/2}=\frac{2u_{1/2}}{\pi}\frac{\lambda f}{D}\simeq1.028993970\frac{\lambda f}{D}=11.3189\,\mathrm{\mu m}.
$$

Thus a quoted “spot diameter” is incomplete without its definition. Doubling $D$ halves both widths at fixed [wavelength](wavelength.md) and [focal length](focal-length.md); increasing [magnification](magnification.md) alone changes the image scale without improving object-space discrimination.

The [Airy disk](airy-disk.md) supplies a calculable reference for a [point spread function](point-spread-function-split.md), allowing [diffraction](diffraction.md) to be distinguished from [defocus](defocus-aberration.md) and [optical aberrations](optical-aberration.md). Its beauty is that one circular boundary determines an entire sequence of bright and dark rings through a [Fourier transform](fourier-transform-split.md). The ideal formula assumes an unobscured pupil, uniform illumination, ideal [optical focus](focus-optics.md), a single [wavelength](wavelength.md), and a scalar description with small output [angles](angle.md). A blocked centre, nonuniform pupil transmission or a significant pupil [wave phase](phase-waves.md) error changes the response. High [numerical aperture](numerical-aperture.md) may require [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) and a vector field description. The [circular-aperture diffraction laboratory experiment](circular-aperture-diffraction-laboratory-experiment.md) tests the far-field pattern directly; the [Rayleigh criterion](rayleigh-criterion.md) uses its first zero to define a two-source convention.

**Table of contents**

- [Airy disk derivation](airy-disk-derivation.md)
- [Airy disk normalization and encircled energy](airy-disk-normalization-and-encircled-energy.md)
- [Circular-aperture diffraction laboratory experiment](circular-aperture-diffraction-laboratory-experiment.md)

## ↑ Ancestors (6)

1. [Point spread function](point-spread-function-split.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Airy disk](airy-disk.md)
- [Airy disk derivation](airy-disk-derivation.md)
- [Circular-aperture diffraction laboratory experiment](circular-aperture-diffraction-laboratory-experiment.md)
- [Confocal excitation and detection point spread function](confocal-excitation-and-detection-point-spread-function.md)
- [Confocal pinhole throughput](confocal-pinhole-throughput.md)
- [Diffraction-limited resolution](diffraction-limited-resolution.md)
- [Diffraction-limited system](diffraction-limited-system.md)
- [Fabry–Pérot transmission from multiple reflections](fabry-perot-transmission-from-multiple-reflections.md)
- [Incoherent two-source Airy profile](incoherent-two-source-airy-profile.md)
- [Microscope scale calibration](microscope-scale-calibration.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-1/section-a/3/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1/section-d/d12/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2/section-d/d13/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2/section-a/2/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2/section-d/d12/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2/section-a/a1/solution.md)
- [Point spread function](point-spread-function-split.md)
- [Rayleigh criterion](rayleigh-criterion.md)
