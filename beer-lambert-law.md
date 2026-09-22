# Beer-Lambert law

↑ **Parent:** [Absorbance](absorbance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Beer–Lambert_law)

The [Beer-Lambert law](beer-lambert-law.md) relates [absorbance](absorbance.md) $A$ to an absorbing species' [concentration](concentration.md) $c$ and path length $l$ by $A=\varepsilon lc$ in a homogeneous medium using sufficiently narrow-band light. The coefficient $\varepsilon$ depends on the species, [wavelength](wavelength.md) and [chemical solution](solution-chemistry.md) conditions. This makes [Ellman's reagent](ellman-s-reagent.md) useful for quantitative [thiol](thiol.md) assays once its released colored species has been calibrated. [IUPAC Compendium of Chemical Terminology, fifth edition (Gold Book) by International Union of Pure and Applied Chemistry; IUPAC Gold Book: Beer-Lambert law and validity conditions](iupac-compendium-of-chemical-terminology-fifth-edition-gold-book-by-international-union-of-pure-and-applied-chemistry/beer-lambert-law.md)

Here $c$ is [molar concentration](molar-concentration.md), $l$ is the geometric [length](length.md) through the sample, and $\varepsilon$ is the [molar absorption coefficient](molar-absorption-coefficient.md). The ideal beam has parallel [light rays](light-ray.md), a single [wavelength](wavelength.md), and a medium with uniform composition and [isotropy](isotropy.md); finite spectral width must be small relative to features in the [optical spectrum](optical-spectrum.md).[IUPAC Compendium of Chemical Terminology, fifth edition (Gold Book) by International Union of Pure and Applied Chemistry; Beer–Lambert law, entry B00626: opening definition, equations and spectral-bandwidth qualification](iupac-compendium-of-chemical-terminology-fifth-edition-gold-book-by-international-union-of-pure-and-applied-chemistry/beer-lambert-law.md)

For a [spectrophotometer](spectrophotometer.md), distinguish the source's output from the reference that reaches the [photodetector](photodetector.md). Let $P_0$ be the received [radiant power](radiant-flux.md) through a [reference blank](reference-blank.md) and $P$ the received [radiant power](radiant-flux.md) through the sample, after subtracting the [photodetector](photodetector.md)'s dark response. Both refer to the same selected [wavelength](wavelength.md) band and collection geometry. Define the blank-normalized [transmittance](transmittance.md) and [absorbance](absorbance.md) by

$$
T=\frac{P}{P_0},\qquad A=-\log_{10}T,\qquad T=10^{-A}.
$$

The [reference blank](reference-blank.md) includes the [solvent](solvent.md) and other assay ingredients except the absorbing target. Matching [cuvettes](cuvette.md) and conditions makes their common losses divide out. Thus this $T$ is relative to the [reference blank](reference-blank.md); it is not the absolute [transmittance](transmittance.md) of the entire [cuvette](cuvette.md) and its contents. Both [radiant powers](radiant-flux.md) can be expressed in [watts](watt.md), while their [ratio](ratio.md), $T$, and its [logarithm](logarithm.md), $A$, are [dimensionless](dimensionless-quantity.md). An instrument displaying $40\%$ transmission means $T=0.40$, not $T=40$.

<a id="image-beer-lambert-reference-sample-detector"></a>
![](beer-lambert-reference-sample-detector.png)

**[Figure 7](#image-beer-lambert-reference-sample-detector). The reference blank and sample establish a radiant power ratio**. Original schematic of two successive measurements in the same [spectrophotometer](spectrophotometer.md), not a drawing of a particular commercial instrument. The [monochromator](monochromator.md) selects the same [wavelength](wavelength.md) band; the same [photodetector](photodetector.md) reads the [reference blank](reference-blank.md) and sample. The marked $l$ is geometric [length](length.md) through the [chemical solution](solution-chemistry.md), distinct from [optical path length](optical-path-length.md). Arrow widths are schematic, not measured [radiant powers](radiant-flux.md).

Why take a [logarithm](logarithm.md)? Consider two consecutive identical absorbing layers. Each transmits a fraction $t$ of the [radiant power](radiant-flux.md) entering it, so together they transmit $t^2$. Their [absorbances](absorbance.md) add because $-\log_{10}(t^2)=2(-\log_{10}t)$. Doubling the sample [length](length.md) doubles [absorbance](absorbance.md) while squaring [transmittance](transmittance.md). This turns multiplicative loss into an additive scale and makes a [straight line](straight-line.md) useful for inferring [molar concentration](molar-concentration.md).

A short model derivation makes the assumption explicit. Suppose a thin layer of thickness $dx$ removes the fraction $kc\,dx$ of its incoming [radiant power](radiant-flux.md), where $k$ is a fixed [constant of proportionality](constant-of-proportionality.md) and $c$ is a uniform [molar concentration](molar-concentration.md). The corresponding [ordinary differential equation](ordinary-differential-equation.md), initial condition, and solution are

$$
\frac{dP}{dx}=-kcP,\qquad P(0)=P_0,\qquad
P(l)=P_0 e^{-kcl}.
$$

Taking the base-ten [logarithm](logarithm.md) gives $A=kcl/\ln 10$, so $\varepsilon=k/\ln 10$. The [exponential decay](exponential-decay.md) follows from equal layers removing equal fractions of what remains. Proportionality to [molar concentration](molar-concentration.md) additionally assumes that the absorbing [chemical species](chemical-species.md) retains the same response as its [molar concentration](molar-concentration.md) changes; the geometric argument alone does not establish that.

**Table of contents**

- [Molar absorption coefficient](molar-absorption-coefficient.md)
- [Beer-Lambert calibration model](beer-lambert-calibration-model.md)
- [Beer-Lambert measurement controls](beer-lambert-measurement-controls.md)
  - [Reference blank](reference-blank.md)

## ↑ Ancestors (4)

1. [Absorbance](absorbance.md)
2. [Physical chemistry](physical-chemistry-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Absorbance](absorbance.md)
- [Acetone iodination rate-law experiment](acetone-iodination-rate-law-experiment.md)
- [Beer-Lambert law](beer-lambert-law.md)
- [Beer-Lambert measurement controls](beer-lambert-measurement-controls.md)
- [Chloroplast dye-reduction experiment](chloroplast-dye-reduction-experiment.md)
- [Coupled-enzyme readout of glycolytic ATP formation](coupled-enzyme-readout-of-glycolytic-atp-formation.md)
- [Disulfide bond](disulfide-bond.md)
- [Enzyme inhibition initial-rate assay](enzyme-inhibition-initial-rate-assay.md)
- [Solution](past-exam-of-the-atmospheric-physics-course-of-the-university-of-cambridge/2014/paper-1/1/a/solution.md)
- [Solution](past-exam-of-the-atmospheric-physics-course-of-the-university-of-cambridge/2014/paper-1/1/b/solution.md)
- [Solution](past-exam-of-the-biochemistry-and-molecular-biology-course-of-the-university-of-cambridge/2025/paper-1/section-b/5/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/4/a/i/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/4/a/iii/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-id/3/c/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-id/1/b/solution.md)
- [SEC detector response](sec-detector-response.md)
- [Trypsin colorimetric assay](trypsin-colorimetric-assay.md)
