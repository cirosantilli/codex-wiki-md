# Prism minimum-deviation index measurement

↑ **Parent:** [Refractive index](refractive-index.md)

A [prism minimum-deviation index measurement](prism-minimum-deviation-index-measurement.md) infers a transparent sample's [relative refractive index](relative-refractive-index.md) from two [angles](angle.md): its known apex [angle](angle.md) $A$ and the smallest deviation $\delta_{\min}$ of a selected [spectral line](spectral-line.md). A [spectrometer](spectrometer.md) combines a source and slit, a [collimator](collimator.md), a rotating [optical prism](prism-optics.md) table, and a viewing [optical telescope](optical-telescope.md) with an angular readout. The [collimator](collimator.md) supplies a nearly parallel beam; the [optical telescope](optical-telescope.md) locates its emergent direction. This turns an otherwise difficult measurement of the [phase velocity](phase-velocity.md) of [light](light.md) into a measurement of [angles](angle.md).

For the symmetric path through a uniform [optical prism](prism-optics.md), with the same external medium at both faces and positive [refractive indices](refractive-index.md),

$$
r_1=r_2=\frac A2,\qquad i=e=\frac{A+\delta_{\min}}2,\qquad n_{\rm rel}=\frac{n_{\rm prism}}{n_{\rm ext}}=\frac{\sin[(A+\delta_{\min})/2]}{\sin(A/2)}.
$$

The [angles](angle.md) $i,e,r_1,r_2$ are measured from face normals. This is the [minimum deviation](minimum-deviation.md) relation, not a formula for an arbitrary prism orientation. An absolute [refractive index](refractive-index.md) additionally requires $n_{\rm ext}$.

<a id="image-prism-minimum-deviation-index-measurement-symmetric-ray-geometry-and-an-independently-calculated-deviation-minimum"></a>
![](refractive-index-prism-minimum-deviation.png)

**[Figure 5](#image-prism-minimum-deviation-index-measurement-symmetric-ray-geometry-and-an-independently-calculated-deviation-minimum). Prism minimum-deviation index measurement: symmetric ray geometry and an independently calculated deviation minimum**. The original model chooses $A=60^\circ$ and $n_{\rm rel}=3/2$ at one fixed [wavelength](wavelength.md). The left panel marks face normals, equal internal [angles](angle.md), apex [angle](angle.md) and deviation from the undeflected incident direction. The right panel calculates deviation versus incidence from two applications of [Snell's law](snell-s-law.md); the marked minimum is the only orientation used for the index inference. No points are experimental observations.

For example, stipulate $A=60^\circ$ and $n_{\rm rel}=3/2$. Then $i=e=\arcsin(3/4)\simeq48.5904^\circ$ and $\delta_{\min}\simeq37.1808^\circ$. Substitution recovers $n_{\rm rel}=1.5$. These synthetic values illustrate the geometry; they are not readings for the prism in the laboratory protocol below.

A Michigan State University teaching experiment uses a mercury lamp, slit, [collimator](collimator.md), prism table and [optical telescope](optical-telescope.md), with a subsidiary angular scale read to one arcminute. First focus the [optical telescope](optical-telescope.md) on a distant object; with the prism removed, align its crosshair to a narrow vertical slit image, focus the [collimator](collimator.md), and establish the direct-beam zero. Insert and centre the prism. Select the green mercury [spectral line](spectral-line.md), tabulated at $546.1\,\mathrm{nm}$, then rotate the prism while tracking its image with the [optical telescope](optical-telescope.md). Locate the turning point where continued prism rotation reverses the image motion, and read the deviation. Re-establish the minimum separately for each other [spectral line](spectral-line.md). The protocol assumes $A=60^\circ$; that assumed apex [angle](angle.md) is not an independently measured result. [introductory-physics-experiments-physics-252-version-4-0-michigan-state-university; Michigan State University, The Prism Spectrometer, Physics 252 v4.0: pp. 2, 5–9; apparatus, vernier readout, alignment, turning point and wavelength table](introductory-physics-experiments-physics-252-version-4-0-michigan-state-university/the-prism-spectrometer.md)

For an uncertainty-aware implementation, repeat the turning-point search from both prism-rotation directions, recheck the direct-beam reference, and record individual readings before averaging. Independently determine $A$ or include its calibration uncertainty; record the chosen [spectral line](spectral-line.md), sample identity, [temperature](temperature-split.md) and surrounding-air conditions. These are proposed controls deduced from the inference, not claimed additional instructions or results of that manual. Finite slit width, unresolved [spectral lines](spectral-line.md), imperfect collimation, table tilt, angular calibration and sample nonuniformity can limit the inferred [refractive index](refractive-index.md). One arcminute readout resolution alone does not establish one arcminute total [measurement uncertainty](measurement-uncertainty.md). A single selected [wavelength](wavelength.md) gives one index, not a measured [optical dispersion](dispersion-optics.md) curve.

A short geometric derivation uses $r_1+r_2=A$ and $\delta=i+e-A$. Reversibility exchanges entrance and exit. At the symmetric stationary path, $i=e$ and $r_1=r_2$; applying [Snell's law](snell-s-law.md) gives the displayed index relation. The plotted calculation checks that this stationary point is a minimum on the chosen transmitting branch. To assess local sensitivity, differentiate the inferred index using [angles](angle.md) in radians:

$$
\frac{dn_{\rm rel}}{n_{\rm rel}}=\frac12\cot\!\left(\frac{A+\delta_{\min}}2\right)d\delta_{\min}+\frac12\left[\cot\!\left(\frac{A+\delta_{\min}}2\right)-\cot\!\left(\frac A2\right)\right]dA.
$$

This first-order relation exposes both angular contributions; it is not an instruction to add signed systematic errors as independent random errors. In the synthetic example, a deviation error of $+1$ arcminute at fixed $A$ changes the inferred [relative refractive index](relative-refractive-index.md) by approximately $+1.92\times10^{-4}$.

## ↑ Ancestors (6)

1. [Refractive index](refractive-index.md)
2. [Electromagnetic wave](electromagnetic-wave-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Prism minimum-deviation index measurement](prism-minimum-deviation-index-measurement.md)
