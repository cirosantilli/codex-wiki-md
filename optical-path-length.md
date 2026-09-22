# Optical path length

↑ **Parent:** [Wavefront](wavefront.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Optical_path_length)

An [optical path length](optical-path-length.md) measures how much propagation [wave phase](phase-waves.md) a path accumulates, expressed as the distance that would accumulate the same [wave phase](phase-waves.md) in [vacuum](vacuum.md). A centimetre in a uniform medium with [refractive index](refractive-index.md) $3/2$ has [optical path length](optical-path-length.md) $1.5\,\mathrm{cm}$, although its geometric length remains $1\,\mathrm{cm}$. This makes [optical path length](optical-path-length.md) useful whenever two contributions must arrive with matching [wave phases](phase-waves.md), from an [optical lens](lens-optics.md) to a [Michelson interferometer](michelson-interferometer.md). [Optical Path Length](rp-photonics-encyclopedia-by-rudiger-paschotta/optical-path-length.md)

For a specified path $\gamma$ at fixed [angular frequency](angular-frequency.md) $\omega$, the [optical path length](optical-path-length.md) is the [line integral](line-integral.md)

$$
\operatorname{OPL}_\gamma(\omega)=\int_\gamma n(\mathbf r,\omega)\,ds,\qquad
ds=|d\mathbf r|,\qquad
\operatorname{OPL}=\sum_j n_jL_j\ \text{for uniform segments}.
$$

Here $s$ is geometric [arc length](arc-length.md), and $n$ is the phase [refractive index](refractive-index.md), evaluated at the same [frequency](frequency.md) everywhere. The propagation interpretation assumes a stationary linear medium with [isotropy](isotropy.md), a real positive scalar [refractive index](refractive-index.md) and negligible loss, on a valid [geometrical optics](geometrical-optics-split.md) branch. The path can curve; at sharp interfaces apply the appropriate matching conditions to each segment. A prescribed curve has a mathematical [line integral](line-integral.md), but it predicts a propagation [wave phase](phase-waves.md) only when it represents the physical branch. [Lecture Notes on Geometrical Optics](mit-2-71-and-2-710-optics-spring-2014-by-nicholas-x-fang/lecture-notes-on-geometrical-optics.md) [Optical fibers](optical-fiber.md) can require a mode [wavenumber](wavenumber.md) rather than the bulk [refractive index](refractive-index.md) along a guessed [light ray](light-ray.md). [Optical Path Length](rp-photonics-encyclopedia-by-rudiger-paschotta/optical-path-length.md)

Fix the [vacuum](vacuum.md) [wavelength](wavelength.md) $\lambda_0=c/f=2\pi c/\omega$, with [frequency](frequency.md) $f=\omega/(2\pi)$ and [vacuum](vacuum.md) [wavenumber](wavenumber.md) $k_0=2\pi/\lambda_0$. In a locally uniform medium the [wavelength](wavelength.md) is $\lambda=\lambda_0/n$, while the [frequency](frequency.md) stays unchanged at a stationary interface. With the convention $\Phi=k_0S-\omega t+\phi_0$, propagation from a specified starting [wave phase](phase-waves.md) contributes

$$
\phi_{\mathrm{prop}}=k_0\operatorname{OPL},\qquad
\delta=\delta_{\mathrm{ref}}+k_0\bigl(\operatorname{OPL}_2-\operatorname{OPL}_1\bigr)\pmod{2\pi}.
$$

The relative reference $\delta_{\mathrm{ref}}$ includes launch [wave phases](phase-waves.md) and any extra [wave phase](phase-waves.md) from mirrors, [beam splitters](beam-splitter.md) or coatings. Thus $k_0\operatorname{OPL}$ is a propagation contribution, not an absolute detector [wave phase](phase-waves.md) independent of the apparatus. If the reference contributions stay fixed, a change in [optical path difference](optical-path-difference.md) $h$ changes the [phase difference](phase-difference.md) by $2\pi h/\lambda_0$. Using the material [wavelength](wavelength.md) again in this formula would count the [refractive index](refractive-index.md) twice. [Laws of Geometric Optics](electromagnetism-lecture-notes-by-richard-fitzpatrick/laws-of-geometric-optics.md)

<a id="optical-path-michelson-phase-readout"></a>
![](optical-path-michelson-phase-readout.png)

**[Figure 8](#optical-path-michelson-phase-readout). Optical path difference in a Michelson interferometer: apparatus schematic and a calculated phase difference readout**.

A motivating measurement turns invisible optical oscillations into a slowly changing electrical signal. MIT's teaching experiment uses a [laser](laser-split.md), a [beam splitter](beam-splitter.md), two returning mirrors, an amplified [photodiode](photodiode.md), an oscilloscope and a calibrated mirror actuator driven by a function generator. The returning beams overlap on the [photodiode](photodiode.md); one channel records detector voltage and another the actuator drive. The measured observable is the changing [light intensity](light-intensity.md), including its maxima and minima, rather than direct timing of an optical cycle. A calibrated displacement per drive voltage and the spacing of the extrema relate geometric motion to the [phase difference](phase-difference.md). The guide infers the [laser](laser-split.md) [wavelength](wavelength.md) from known actuator calibration; conversely, with independently known [vacuum](vacuum.md) [wavelength](wavelength.md) and ambient [refractive index](refractive-index.md), the same relation calibrates mirror motion. These two unknowns cannot both be inferred from fringe spacing alone. [Optical Interferometry](mit-8-13-14-experimental-physics-i-and-ii-junior-lab-fall-2016-spring-2017-by-mit-department-of-physics/optical-interferometry.md)

For a proposed change-of-medium measurement, keep the mirrors fixed and put a transparent cell of internal length $L$ in one arm. Compare its contents at [refractive indices](refractive-index.md) $n_a$ and $n_b$, leaving its windows in place. At normal incidence the two traversals give

$$
\Delta\operatorname{OPL}=2L(n_b-n_a),\qquad
\Delta\delta=\frac{4\pi L(n_b-n_a)}{\lambda_0},\qquad
N=\frac{\Delta\delta}{2\pi}=\frac{2L(n_b-n_a)}{\lambda_0}.
$$

Here $N$ is the signed number of whole [interference fringe](interference-fringe.md) cycles plus any resolved fractional cycle, counted continuously. A mirror displacement $x$ instead gives $\Delta\operatorname{OPL}=2n_{\mathrm{amb}}x$; distinguish this double-pass factor from a single pass in a [Mach-Zehnder interferometer](mach-zehnder-interferometer.md). OpenStax's gas-cell worked example provides the same double-pass reasoning; it is a teaching calculation rather than a published measurement dataset.[Example 3.6: mirror displacement and a gas cell](university-physics-volume-3-by-samuel-j-ling-and-others/3-5-the-michelson-interferometer.md)

An exact toy calculation makes the sensitivity visible. Stipulate $\lambda_0=600\,\mathrm{nm}$, $L=10\,\mathrm{mm}$ and $n_b-n_a=3/100000=0.00003$. Then $\Delta\operatorname{OPL}=600\,\mathrm{nm}$ and $\Delta\delta=2\pi$: a full [interference fringe](interference-fringe.md) cycle, despite unchanged geometric lengths. For a continuous change $n_b-n_a=q(3/100000)$, let $0\leq q\leq2$ and choose the initial detector [phase difference](phase-difference.md) to be zero. Equal coherent detected arm contributions of [light intensity](light-intensity.md) $I_0$ predict

$$
\frac{I(q)}{4I_0}=\frac{1+\cos(2\pi q)}{2}=\cos^2(\pi q).
$$

The plot is this stipulated model: $q=1/2$ gives a minimum, $q=1$ restores a maximum, and the reference level is chosen by adjustment of the apparatus. It contains no measured values or assigned properties of a real gas. The equivalent mirror travel in [vacuum](vacuum.md) is $300\,\mathrm{nm}$ per cycle. A single endpoint [light intensity](light-intensity.md) cannot distinguish $q=0$ from $q=1$; the continuous fringe count carries the missing information.

For an interpretable cell measurement, establish the initial [phase difference](phase-difference.md) with a small calibrated mirror scan, then track slow changes through successive [interference fringes](interference-fringe.md). Measure the dark signal and each arm separately, keep [photodiode](photodiode.md) gain within its linear range, align both beams on the same region and match their [linear polarizations](linear-polarization.md). Monitor [interferometric visibility](interferometric-visibility.md) and keep arm delays within the useful [optical coherence time](optical-coherence-time.md). Record cell length, contents, [pressure](pressure-split.md) and [temperature](temperature-split.md); return to the starting condition to check drift. Changes in window deformation, cell length, external air or mirror position also change [optical path length](optical-path-length.md), so a reference cell or an independently monitored mechanical path is needed to isolate the contents' [refractive index](refractive-index.md). These controls are deductions from the model, not a claim that the illustrated apparatus was operated. Loss of fringe count leaves a whole-cycle ambiguity; at an intensity extremum the first [derivative](derivative.md) with respect to [phase difference](phase-difference.md) vanishes, so a scan around [phase quadrature](phase-quadrature.md) is more sensitive to small changes. Broadband illumination, unstable [optical coherence](optical-coherence.md), vibration and strong loss can invalidate a simple one-[frequency](frequency.md) inference.

**Table of contents**

- [Optical path difference](optical-path-difference.md)
  - [Full-cycle phase-plate invisibility](full-cycle-phase-plate-invisibility.md)
- [Group refractive index](group-refractive-index.md)
  - [Group index from refracted-angle dispersion](group-index-from-refracted-angle-dispersion.md)
  - [Group delay](group-delay.md)
    - [Group delay dispersion](group-delay-dispersion.md)
      - [Third-order dispersion](third-order-dispersion.md)

## ↑ Ancestors (6)

1. [Wavefront](wavefront.md)
2. [Physical optics](physical-optics-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (36)

- [Absorption spectrum](absorption-spectrum.md)
- [Atmospheric turbulence](atmospheric-turbulence.md)
- [Beam splitter](beam-splitter.md)
- [Beer-Lambert law](beer-lambert-law.md)
- [Deformable mirror](deformable-mirror.md)
- [Division of amplitude](division-of-amplitude.md)
- [Fabry–Pérot transmission from multiple reflections](fabry-perot-transmission-from-multiple-reflections.md)
- [Fourier transform spectroscopy](fourier-transform-spectroscopy.md)
- [Geometrical optics](geometrical-optics-split.md)
- [Group refractive index](group-refractive-index.md)
- [Interference (wave propagation)](interference-wave-propagation.md)
- [Mirror segment phasing](mirror-segment-phasing.md)
- [Optical interferometry](optical-interferometry.md)
- [Optical path difference](optical-path-difference.md)
- [Optical path length](optical-path-length.md)
- [Optical rays in a reciprocal-height refractive index](optical-rays-in-a-reciprocal-height-refractive-index.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2014/paper-1/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-338/2/a/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-338/1/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-338/2/a/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-338/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-338/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-1/10/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/9/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/9/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/9/a/i/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2/section-a/3/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2/section-b/b7/d/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/section-d/12/solution.md)
- [Phase object](phase-object.md)
- [Photon gas](photon-gas.md)
- [Refractive index](refractive-index.md)
- [Speckle contrast of a sinusoidal wavefront error](speckle-contrast-of-a-sinusoidal-wavefront-error.md)
- [Thin phase-plate cancellation by phase conjugation](thin-phase-plate-cancellation-by-phase-conjugation.md)
- [Wavefront](wavefront.md)
- [Wavefront error](wavefront-error.md)
