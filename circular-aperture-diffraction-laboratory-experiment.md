# Circular-aperture diffraction laboratory experiment

↑ **Parent:** [Airy disk](airy-disk.md)

An actual teaching setup is described in [Laboratory Exercise No. 4: Diffraction, MIT 6.237, Fall 2024](laboratory-exercise-no-4-diffraction-mit-6-237-fall-2024.md), for MIT's 6.237 Modern Optics Project Laboratory, Fall 2024. Preparation includes predicting the aperture-size dependence and the distinction between [Fraunhofer diffraction](fraunhofer-diffraction.md) and [Fresnel diffraction](fresnel-diffraction.md). A helium–neon [laser](laser-split.md) supplies $632.8\,\mathrm{nm}$ [light](light.md); the far-field setup uses a planar incident [wavefront](wavefront.md), a diffracting object and a distant screen, with beam expansion when needed. Figure 1 also marks an optional [CCD](charge-coupled-device.md) camera. Exercise 4.7 asks students to sketch the circular-aperture pattern, measure the [Airy disk](airy-disk.md) diameter between correctly identified boundaries, and infer the aperture size. No measured values are supplied. As a regime comparison, exercise 4.9 varies the circular opening's position near a microscope objective [optical lens](lens-optics.md), observes near-field patterns and compares them with the far-field case. This tests whether a change in propagation geometry changes the pattern. The coherent illumination measures one aperture's response, rather than the discrimination of two mutually incoherent [optical point sources](optical-point-source.md).[pp. 1–2, introduction, PL4.1 and Fig. 1; p. 5, §4.7; p. 6, §4.9: apparatus, readout and regime comparison](laboratory-exercise-no-4-diffraction-mit-6-237-fall-2024.md)

For a quantitative interpretation, let $L$ be the aperture-to-screen distance and $d_{\rm spot}$ the first-zero diameter on the screen. In the [paraxial approximation](paraxial-approximation.md), the independent calculation is

$$
d_{\rm spot}\simeq2L\theta_1=2\frac{j_{1,1}}\pi\frac{\lambda L}{D},\qquad D\simeq2\frac{j_{1,1}}\pi\frac{\lambda L}{d_{\rm spot}}.
$$

For an explicitly hypothetical measurement, $L=1.80\,\mathrm m$ and $d_{\rm spot}=5.60\,\mathrm{mm}$ at $632.8\,\mathrm{nm}$ would imply $D\simeq0.496\,\mathrm{mm}$. The scale $D^2/\lambda\simeq0.389\,\mathrm m$ is smaller than $L$, but only by a factor of about $4.6$; this alone gives limited confidence in a high-precision [Fraunhofer diffraction](fraunhofer-diffraction.md) approximation. It is not a reported MIT measurement.

Additional recommended controls are to keep [wavelength](wavelength.md) fixed, record $L$, centre and uniformly illuminate the [aperture](aperture.md), and repeat with another $D$. Compare $d_{\rm spot}/L$, which should vary inversely with $D$. A camera readout should include blocked-beam background and avoid saturation. A scaled repetition at larger $L$ tests residual [Fresnel diffraction](fresnel-diffraction.md); nonuniform illumination, [optical aberrations](optical-aberration.md), detector sampling and uncertainty in locating a dark ring limit the inferred $D$. The screen pattern's apparent bright edge depends on display brightness and is not a substitute for the first-zero boundary.

## ↑ Ancestors (7)

1. [Airy disk](airy-disk.md)
2. [Point spread function](point-spread-function-split.md)
3. [Physical optics](physical-optics-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Airy disk](airy-disk.md)
