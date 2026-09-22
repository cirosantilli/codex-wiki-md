<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**$\boxed{\text{(a): two-photon excitation; (b): one-photon/confocal excitation.}}$** The compact emitting region in (a) indicates that excitation itself is strongly localized. In (b), the illuminated path generates out-of-focus [fluorescence](../../../../../fluorescence-split.md) as well as fluorescence near the focus. A confocal detection pinhole can reject much of that unwanted emission from the recorded image; it does not prevent the dye solution from emitting it.

In ordinary one-photon excitation, the local fluorescence-generation rate is approximately proportional to excitation [light intensity](../../../../../light-intensity.md) $I$. In unsaturated [two-photon excitation microscopy](../../../../../two-photon-excitation-microscopy.md), it is proportional to $I^2$. Simultaneous absorption is appreciable only in the high-intensity focal region, generally produced using a pulsed [laser](../../../../../laser-split.md). Two lower-energy photons jointly excite the fluorophore; the excitation [wavelength](../../../../../wavelength.md) is therefore typically substantially longer than in its one-photon experiment. This reduces out-of-focus excitation and permits detection without a confocal pinhole.[pp. 73–75, quadratic excitation, optical sectioning and pulsed illumination](../../../../../two-photon-laser-scanning-fluorescence-microscopy-by-winfried-denk-and-others.md)

For a small detection pinhole, the effective confocal [point spread function](../../../../../point-spread-function-split.md) is approximately

$$
\boxed{h_{\rm conf}(\mathbf r)\propto h_{\rm exc}(\mathbf r)h_{\rm det}(\mathbf r)}.
$$

Here each factor denotes an intensity response. Excitation and detection jointly select the focal region. Enlarging the pinhole increases collected signal but weakens axial rejection and changes the effective [point spread function](../../../../../point-spread-function-split.md). In [two-photon excitation microscopy](../../../../../two-photon-excitation-microscopy.md) with broad collection, the spatial response is dominated by

$$
\boxed{h_{2p}(\mathbf r)\propto[h_{\rm exc,2p}(\mathbf r)]^2}.
$$

The pinhole product and excitation square are different physical mechanisms even when simplified mathematical profiles resemble one another.[Confocal formation and conjugate focal selection, Fig. 3; discussion of excitation and detection responses](../../../../../confocal-microscopy-chapter-manuscript-by-brad-amos-and-others.md)

**Compare both lateral and axial widths using the actual wavelengths and objective.** For a [diffraction-limited system](../../../../../diffraction-limited-system.md), their characteristic scalings are

$$
\delta_{xy}\sim\frac{\lambda}{\mathrm{NA}},\qquad
\delta_z\sim\frac{n_{\rm med}\lambda}{\mathrm{NA}^2},
$$

where $\mathrm{NA}$ is [numerical aperture](../../../../../numerical-aperture.md) and $n_{\rm med}$ is the medium's [refractive index](../../../../../refractive-index.md). Numerical prefactors depend on the width criterion and high-aperture optical model. Axial resolution is generally worse than lateral resolution. A small confocal pinhole improves axial sectioning and can narrow the lateral response, at the cost of photon throughput.

As a simple [Gaussian function](../../../../../gaussian-function.md) example, $h(x)=\exp[-x^2/(2\sigma^2)]$ has squared profile $h(x)^2=\exp[-x^2/\sigma^2]$, so its width is reduced by $1/\sqrt2$. However, the two-photon illumination spot itself is broader at its longer excitation [wavelength](../../../../../wavelength.md). **Two-photon excitation is not automatically higher-resolution than confocal microscopy**, and ordinary two-photon sectioning is not intrinsically super-resolution. Compare measured [point spread functions](../../../../../point-spread-function-split.md), pinhole settings, [numerical apertures](../../../../../numerical-aperture.md), scattering and [optical aberrations](../../../../../optical-aberration.md), not just the fact that one profile is squared.

The original model figure below separates focal confinement from wavelength-dependent width. It is an illustrative one-dimensional [Gaussian function](../../../../../gaussian-function.md) calculation, not a reproduction or quantitative fit of the supplied photograph.

<a id="6/i/image-local-excitation-nonlinearity-and-wavelength-dependent-point-spread-widths"></a>
![](../../../../../past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-2-optical-response.png)

**[Figure 1](#6/i/image-local-excitation-nonlinearity-and-wavelength-dependent-point-spread-widths). Local excitation nonlinearity and wavelength-dependent point-spread widths**. Left: squaring the same normalized Gaussian illumination narrows the local generation profile. Right: a longer-wavelength illumination profile can remain broader after squaring than an illustrative confocal excitation-times-detection response. All widths are synthetic; peak normalization does not equate photon throughput or excitation dose.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
