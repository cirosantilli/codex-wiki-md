# Diffraction-limited resolution

↑ **Parent:** [Diffraction-limited system](diffraction-limited-system.md)

[Diffraction-limited resolution](diffraction-limited-resolution.md) is a scale for distinguishing details with a specified ideal [diffraction](diffraction.md) response and a specified criterion. For two equally bright, mutually incoherent [optical point sources](optical-point-source.md) imaged through a uniformly transmitting, unobscured circular [optical pupil](optical-pupil.md), the [Rayleigh criterion](rayleigh-criterion.md) places the centre of one [Airy disk](airy-disk.md) at the first zero of the other. At small [angles](angle.md) in air this separation is

$$
\theta_{\rm R}=\frac{j_{1,1}}{\pi}\frac{\lambda}{D}\simeq1.22\frac{\lambda}{D},\qquad j_{1,1}\simeq3.831706.
$$

Here $D$ is pupil [diameter](diameter.md), $\lambda$ is [wavelength](wavelength.md) in air, and $j_{1,1}$ is the first positive zero of the order-one [Bessel function of the first kind](bessel-function-of-the-first-kind.md). This is the radius to the first zero, not the diameter of the central spot. [Fraunhofer diffraction](fraunhofer-diffraction.md) gives the radial peak-normalized [light intensity](light-intensity.md)

$$
P(q)=\left[\frac{2J_1(q)}q\right]^2,\qquad q=\frac{\pi D\theta}{\lambda},\qquad P(0)=1.
$$

The removable value at zero follows from $J_1(q)\sim q/2$. The pupil [Fourier transform](fourier-transform.md) reduces to a radial [integral](integral.md) by circular symmetry, which produces the [Bessel function of the first kind](bessel-function-of-the-first-kind.md); its first zero supplies the factor $1.22$.[Two-Dimensional Fourier Optics](oscillations-and-waves-by-richard-fitzpatrick/two-dimensional-fourier-optics.md)

In the usual scalar circular-pupil approximation for a [fluorescence microscope](fluorescence-microscope.md), the corresponding object-plane [Rayleigh criterion](rayleigh-criterion.md) is

$$
r_{\rm R}=\frac{j_{1,1}}{2\pi}\frac{\lambda_0}{\mathrm{NA}}\simeq0.61\frac{\lambda_0}{\mathrm{NA}},\qquad q=\frac{2\pi\mathrm{NA}\,r}{\lambda_0}.
$$

Here $\lambda_0$ is the vacuum emission [wavelength](wavelength.md), and the object-side [numerical aperture](numerical-aperture.md) already includes the medium's [refractive index](refractive-index.md). Do not divide $\lambda_0$ by $n$ again. For small cone [angles](angle.md) in air, $\mathrm{NA}\simeq D/(2f)$ and image-plane radius $f\theta_{\rm R}$ agrees with this form. The assumptions include a single [wavelength](wavelength.md), ideal [optical focus](focus-optics.md), and mutually incoherent emitters. High [numerical aperture](numerical-aperture.md) can require a vector description with [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) and emitter orientation; [confocal microscopy](confocal-microscopy.md) has its own excitation-and-detection response. The same $0.61$ formula therefore does not describe every microscope or illumination method.[Resolution by Michael W. Davidson](resolution-by-michael-w-davidson.md)

<a id="image-doubling-numerical-aperture-halves-the-ideal-circular-pupil-point-response-scale-at-fixed-wavelength"></a>
![](circular-pupil-point-spread-scale.png)

**[Figure 36](#image-doubling-numerical-aperture-halves-the-ideal-circular-pupil-point-response-scale-at-fixed-wavelength). Doubling numerical aperture halves the ideal circular-pupil point-response scale at fixed wavelength**.

In this original model, $\lambda_0=550\,\mathrm{nm}$ and [numerical apertures](numerical-aperture.md) $0.25$ and $0.50$ give first-zero radii $1.342\,\mathrm{\mu m}$ and $0.671\,\mathrm{\mu m}$. Each [point spread function](point-spread-function.md) is divided by its own peak to compare shape. The pupil axes are transverse [wave vector](wavevector.md) components multiplied by $\lambda_0/(2\pi)$, so pupil radius equals [numerical aperture](numerical-aperture.md). A wider pupil accepts a wider range of transverse [wave vectors](wavevector.md), producing a narrower image. Increasing [magnification](magnification.md) alone enlarges the same spot and does not reduce its object-plane radius.

The [Rayleigh criterion](rayleigh-criterion.md) is a useful visual convention, not an absolute information barrier. For equal incoherent sources with total detected [radiant flux](radiant-flux.md) $F$ and separation vector $\mathbf s$, the ideal image is

$$
I(\mathbf x)=\frac F2\left[p(\mathbf x-\mathbf s/2)+p(\mathbf x+\mathbf s/2)\right].
$$

Below the [Rayleigh criterion](rayleigh-criterion.md) this still differs from $Fp(\mathbf x)$; for small $\mathbf s$, symmetry cancels the linear change and the first change is quadratic in separation. Estimating two unknown source positions is then increasingly sensitive to [noise](noise-signal-processing.md), background, relative brightness and uncertainty in the [point spread function](point-spread-function.md). Localizing one isolated source and recovering an arbitrary extended object are different inference tasks. Measurements that separate optical modes can also extract separation information differently from direct image [light intensity](light-intensity.md) measurement.[Quantum Theory of Superresolution for Two Incoherent Optical Point Sources by Mankei Tsang and others](quantum-theory-of-superresolution-for-two-incoherent-optical-point-sources-by-mankei-tsang-and-others.md)

There remains a real limit for arbitrary images in this model: the [optical transfer function](optical-transfer-function.md) is zero above the transmitted [spatial frequency](spatial-frequency.md) band. Its cutoff for scalar [incoherent imaging](incoherent-imaging.md) is $\nu_c=2\mathrm{NA}/\lambda_0$ in object-plane cycles per unit length. The [Nyquist–Shannon sampling theorem](nyquist-shannon-sampling-theorem.md) therefore suggests object-referred [detector pixel](optical-detector-pixel.md) pitch $p_{\rm pix}\leq\lambda_0/(4\mathrm{NA})$, with finer sampling providing margin. Finite [detector pixels](optical-detector-pixel.md) also integrate over their [area](surface-area.md), suppressing contrast; coarse sampling can cause [aliasing](aliasing.md). Finer sampling cannot alone recover [spatial frequencies](spatial-frequency.md) removed by the optics, and [Fourier deconvolution](fourier-deconvolution.md) amplifies [noise](noise-signal-processing.md) where the [optical transfer function](optical-transfer-function.md) is small. [Photon shot noise](photon-shot-noise.md), [read noise](read-noise.md), [optical aberrations](optical-aberration.md) and [defocus](defocus-aberration.md) can all worsen practical discrimination. A useful resolution claim therefore reports the object model, criterion, [wavelength](wavelength.md), [numerical aperture](numerical-aperture.md), sampling and [signal-to-noise ratio in photon counting](signal-to-noise-ratio-in-photon-counting.md).

**Table of contents**

- [Rayleigh criterion](rayleigh-criterion.md)
- [Spatial resolution element](spatial-resolution-element.md)

## ↑ Ancestors (7)

1. [Diffraction-limited system](diffraction-limited-system.md)
2. [Point spread function](point-spread-function.md)
3. [Physical optics](physical-optics.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Adaptive optics](adaptive-optics.md)
- [Aperture](aperture.md)
- [Confocal optical sectioning](confocal-optical-sectioning.md)
- [Diffraction limit of a telescope](diffraction-limit-of-a-telescope.md)
- [Diffraction-limited resolution](diffraction-limited-resolution.md)
- [Diffraction-limited system](diffraction-limited-system.md)
- [Field of view](field-of-view.md)
- [Magnification](magnification.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-338/2/a/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-338/2/b/iv/solution.md)
- [Seidel coma pupil mapping](seidel-coma-pupil-mapping.md)
- [Single-slit diffraction](single-slit-diffraction.md)
- [Thin lens](thin-lens.md)
