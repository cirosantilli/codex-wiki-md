# Focal ratio

↑ **Parent:** [Optical instrument](optical-instrument-split.md)

The [focal ratio](focal-ratio.md), or f-number, of a converging [optical instrument](optical-instrument-split.md) focused at infinity is the [dimensionless quantity](dimensionless-quantity.md)

$$
N=F=\frac{f}{D},
$$

where $f>0$ is effective [focal length](focal-length.md) and $D$ is the on-axis [entrance pupil](entrance-pupil.md) [diameter](diameter.md). The notation f/4 means $N=4$, not $f=4$ in a particular unit. A $100\,\mathrm{mm}$ [focal length](focal-length.md) with $D=25\,\mathrm{mm}$ gives f/4. Closing the [aperture stop](aperture-stop.md) until $D=12.5\,\mathrm{mm}$ gives f/8 while retaining the same [focal length](focal-length.md). The mechanical opening need not equal $D$. [Gregory Hollows and Nicholas James, Edmund Optics, System Throughput, f-number, and Numerical Aperture](https://www.edmundoptics.com/knowledge-center/application-notes/imaging/lens-iris-aperture-setting/).

For a [thin lens](thin-lens.md) in air with a circular [aperture stop](aperture-stop.md) at the [thin lens](thin-lens.md), the converging bundle from a distant on-axis point has half-[angle](angle.md) $\alpha$ satisfying

$$
\tan\alpha=\frac{D}{2f}=\frac{1}{2N},\qquad \alpha\simeq\frac{1}{2N}\quad\hbox{in radians}.
$$

The last step uses the [small-angle approximation](small-angle-approximation.md). For a compound [optical lens](lens-optics.md), the cone is set by the image-side [optical pupil](optical-pupil.md) and its distance from the receiving plane; the simple triangle is not an exact high-[angle](angle.md) rule. At finite object distance a [thin lens](thin-lens.md) instead gives $v=f(1+|m|)$, by its imaging equation and [transverse magnification](transverse-magnification.md), so its working cone corresponds to $v/D=N(1+|m|)$. Nominal [focal ratio](focal-ratio.md) therefore does not alone specify close-range image [irradiance](irradiance.md). [Hollows and James, working f-number and image-space cone](https://www.edmundoptics.com/knowledge-center/application-notes/imaging/lens-iris-aperture-setting/).

Two useful scalings follow under stated conditions. For a fixed uniform incident beam and unchanged transmission, collected [radiant flux](radiant-flux.md) scales as $D^2$. For an extended source with fixed [radiance](radiance.md), the central image [irradiance](irradiance.md) scales approximately as $N^{-2}$ in the [paraxial approximation](paraxial-approximation.md): the [solid angle](solid-angle.md) of the cone scales as $(D/f)^2$. For an ideal uniformly illuminated unobscured circular [entrance pupil](entrance-pupil.md), the first dark ring of the [point spread function](point-spread-function-split.md) has angular [radius](radius.md) and [focal plane](focal-plane.md) [radius](radius.md)

$$
\theta_1\simeq1.22\frac{\lambda}{D},\qquad r_1\simeq f\theta_1=1.22\lambda N.
$$

Here $\lambda$ is [wavelength](wavelength.md). These are first-zero radii, not diameters or a universal rule for resolving arbitrary objects. A proof outline evaluates the circular [aperture](aperture.md)'s [Fraunhofer diffraction](fraunhofer-diffraction.md) using its [Fourier transform](fourier-transform-split.md), then uses the first zero of the resulting [Bessel function](bessel-function-split.md). [Richard Fitzpatrick, University of Texas at Austin, Two-Dimensional Fourier Optics, circular-aperture first minimum](oscillations-and-waves-by-richard-fitzpatrick/two-dimensional-fourier-optics.md).

At $\lambda=0.55\,\mathrm{\mu m}$, the example's f/4 and f/8 first-ring radii are $2.684$ and $5.368\,\mathrm{\mu m}$. Closing the [aperture stop](aperture-stop.md) halves $D$, quarters collected [radiant flux](radiant-flux.md) and doubles this [diffraction](diffraction.md) radius. It can also reduce [optical aberrations](optical-aberration.md) by excluding outer [light rays](light-ray.md); actual sharpness reflects both effects. This explains why a smaller [aperture](aperture.md) need not produce a sharper image. [Gregory Hollows and Nicholas James, Edmund Optics, The Airy Disk and Diffraction Limit](https://www.edmundoptics.com/knowledge-center/application-notes/imaging/limitations-on-resolution-and-contrast-the-airy-disk/).

<a id="image-aperture-and-focal-ratio-a-common-optical-focus-reduced-collection-and-increased-diffraction-radius"></a>
![](aperture-focal-ratio-field-view-cone-scaling.png)

**[Figure 1](#image-aperture-and-focal-ratio-a-common-optical-focus-reduced-collection-and-increased-diffraction-radius). Aperture and focal ratio: a common optical focus, reduced collection and increased diffraction radius**. Original analytical illustration. Left: equal-scale [thin lens](thin-lens.md) geometry with $f=100\,\mathrm{mm}$ and $D=25$ or $12.5\,\mathrm{mm}$. Right: collected [radiant flux](radiant-flux.md) relative to f/4 is $(4/N)^2$, and first-ring [radius](radius.md) relative to f/4 is $N/4$. The [wavelength](wavelength.md) is $0.55\,\mathrm{\mu m}$; the [entrance pupil](entrance-pupil.md) is circular, uniformly illuminated and unobscured. These are calculated quantities, not measurements.

A proposed [optical bench](optical-bench.md) check puts a fixed [collimator](collimator.md) before a converging [thin lens](thin-lens.md) and a [photodetector](photodetector.md) large enough to collect the entire image behind it. Compare two centred [aperture stops](aperture-stop.md) of known [diameters](diameter.md) while fixing source output, detector gain and integration time. The integrated signal tests the $D^2$ collection law; a spatially resolved [optical camera](optical-camera.md) at the [focal plane](focal-plane.md) can separately measure the [point spread function](point-spread-function-split.md). Repeat a dark reading and the first [aperture stop](aperture-stop.md), and check that neither the incoming beam nor detector clips either bundle. A resolved pinhole source, imperfect collimation, [optical aberrations](optical-aberration.md) and detector pixel size can dominate the apparent spot width; a single peak reading does not measure total collected [radiant flux](radiant-flux.md).

## ↑ Ancestors (5)

1. [Optical instrument](optical-instrument-split.md)
2. [Optics](optics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Aperture](aperture.md)
- [Field of view](field-of-view.md)
- [Focal ratio](focal-ratio.md)
- [Integral-field spectrograph volume scaling](integral-field-spectrograph-volume-scaling.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/2/b/i/solution.md)
