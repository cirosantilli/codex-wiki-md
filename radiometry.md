# Radiometry

↑ **Parent:** [Optics](optics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiometry)

[Radiometry](radiometry.md) measures the [energy](energy.md) and [power](energy.md#power) carried by [electromagnetic radiation](electromagnetic-radiation.md), including [light](optics.md#light). It asks how much radiation a source supplies, where it travels, and how much reaches a receiving surface. The measurements are physical rather than weighted by the sensitivity of the human eye: equal [radiant fluxes](#radiant-flux) at different [wavelengths](wave-equation.md#wavelength) need not look equally bright. [Yoshihiro Ohno, Radiometry and Photometry: Review for Vision Optics, 2000](https://www.nist.gov/publications/radiometry-and-photometry-review-vision-optics).

The five quantities below answer different questions about the same radiation. The [International System of Units](physics.md#international-system-of-units) makes the distinctions visible: a watt is a joule per second, while a steradian measures [solid angle](euclidean-geometry.md#solid-angle). [NIST Guide to the SI, Chapter 4: derived units](https://www.nist.gov/pml/special-publication-811/nist-guide-si-chapter-4-two-classes-si-units-and-si-prefixes).

| Quantity | What is resolved? | Units |
| --- | --- | --- |
| [Radiant flux](#radiant-flux) $\Phi$ | Total radiation [power](energy.md#power) in the specified beam or collection | $\mathrm W$ |
| [Radiant intensity](#radiant-intensity) $I$ | [Power](energy.md#power) per outgoing [solid angle](euclidean-geometry.md#solid-angle) | $\mathrm{W\,sr^{-1}}$ |
| [Radiance](#radiance) $L$ | [Power](energy.md#power) per [projected area](#projected-area) and per [solid angle](euclidean-geometry.md#solid-angle) | $\mathrm{W\,m^{-2}\,sr^{-1}}$ |
| [Irradiance](#irradiance) $E$ | Incident [power](energy.md#power) per receiving [area](differential-geometry.md#surface-area) | $\mathrm{W\,m^{-2}}$ |
| [Radiant exitance](#radiant-exitance) $M$ | Outward emitted [power](energy.md#power) per emitting [area](differential-geometry.md#surface-area) | $\mathrm{W\,m^{-2}}$ |

Resolving [wavelength](wave-equation.md#wavelength) or [frequency](wave.md#frequency) adds a further “per unit interval”, as in [spectral radiance](#spectral-radiance). The notation is consistent with NIST's table of spectral quantities. In particular, [radiant flux](#radiant-flux) is [power](energy.md#power), whereas the existing astronomical [radiative flux](astrophysics.md#radiative-flux) is [power](energy.md#power) per [area](differential-geometry.md#surface-area). [NISTIR 6657, A Rational Methodology for Estimating the Luminous Flux Based upon Color Primaries from Digital Projection Displays, 2009, Table 1](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=901354).

This bookkeeping makes an [optical camera](optical-instrument.md#optical-camera)'s collected signal calculable from a source's [radiance](#radiance) and the geometry of the receiving aperture. It also lets radiation measurements from different instruments be compared. For example, NIST describes separate calibrations of [spectral radiance](#spectral-radiance) and spectral [irradiance](#irradiance) for instruments used to observe Earth. [Johnson, Brown and Rice, Metrology for remote sensing radiometry, §§3.4.1–3.4.2](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=104550).

**Table of contents**

- [Optical haze](#optical-haze)
- [Actinic flux](#actinic-flux)
- [Fluence](#fluence)
- [Radiometer](#radiometer)
  - [Noise temperature](#noise-temperature)
    - [System noise temperature](#system-noise-temperature)
    - [Receiver noise temperature](#receiver-noise-temperature)
  - [Two-load radiometer calibration](#two-load-radiometer-calibration)
- [Reflectance](#reflectance)
- [Absorption (electromagnetic radiation)](#absorption-electromagnetic-radiation)
- [Radiant flux](#radiant-flux)
  - [Radiant flux through an oriented surface](#radiant-flux-through-an-oriented-surface)
  - [Beam collection at fixed radiant flux](#beam-collection-at-fixed-radiant-flux)
  - [Spectral radiant flux](#spectral-radiant-flux)
  - [Calibrated radiant-flux measurement](#calibrated-radiant-flux-measurement)
- [Radiant intensity](#radiant-intensity)
  - [Point emitter](#point-emitter)
- [Radiance](#radiance)
  - [Projected area](#projected-area)
  - [Spectral radiance](#spectral-radiance)
    - [Frequency and wavelength spectral radiance conversion](#frequency-and-wavelength-spectral-radiance-conversion)
    - [Vacuum conservation of specific intensity](#vacuum-conservation-of-specific-intensity)
    - [Limb darkening](#limb-darkening)
      - [Linear limb-darkening law](#linear-limb-darkening-law)
        - [Limb-darkening coefficient](#limb-darkening-coefficient)
      - [Limb-darkened disk flux](#limb-darkened-disk-flux)
      - [Small-planet transit weighting](#small-planet-transit-weighting)
      - [Solar limb-darkening drift-scan experiment](#solar-limb-darkening-drift-scan-experiment)
- [Radiant exitance](#radiant-exitance)
- [Irradiance](#irradiance)
  - [Horizontal versus beam-normal solar irradiance](#horizontal-versus-beam-normal-solar-irradiance)
- [Radiometric absorptance](#radiometric-absorptance)
- [Electrical substitution radiometer](#electrical-substitution-radiometer)
  - [Electrical substitution heat balance](#electrical-substitution-heat-balance)
    - [Radiometer thermal link](#radiometer-thermal-link)
    - [Fixed-temperature electrical substitution example](#fixed-temperature-electrical-substitution-example)
  - [Optical-electrical heating non-equivalence](#optical-electrical-heating-non-equivalence)
  - [Cryogenic radiometer](#cryogenic-radiometer)
    - [Cryogenic laser-power substitution experiment](#cryogenic-laser-power-substitution-experiment)
- [Transmittance](#transmittance)

## Optical haze

↑ **Parent:** [Radiometry](radiometry.md)

The fraction of transmitted light scattered sufficiently far from the forward direction under a specified measurement geometry. A transparent electrode can have high total transmittance yet blur an image if scattering is strong. State the collection angles and wavelength when comparing haze measurements.

## Actinic flux

↑ **Parent:** [Radiometry](radiometry.md)

The photon flux incident from all propagation directions, resolved by wavelength when needed for [photodissociation](chemical-bond.md#photodissociation). It is distinct from the net radiative flux through a horizontal surface; scattered and diffuse photons can contribute even when their net vertical flux cancels.

## Fluence

↑ **Parent:** [Radiometry](radiometry.md)

For an optical beam, time-integrated [light intensity](wave.md#light-intensity), giving incident [energy](energy.md) per unit area.

## Radiometer

↑ **Parent:** [Radiometry](radiometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiometer)

A [radiometer](#radiometer) measures [electromagnetic radiation](electromagnetic-radiation.md) through its received [power](energy.md#power). A radio [radiometer](#radiometer) can express that [power](energy.md#power) as a [noise temperature](#noise-temperature), allowing an unknown source to be compared with calibrated reference [temperatures](temperature.md).

### Noise temperature

↑ **Parent:** [Radiometer](#radiometer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noise_temperature)

A [noise temperature](#noise-temperature) expresses received or internally added noise [power](energy.md#power) on an equivalent [temperature](temperature.md) scale. For one matched receiving channel in the classical thermal limit, an ideal rectangular [bandwidth](electrical-engineering.md#bandwidth-signal-processing) $\Delta\nu$ gives $P=k_{\rm B}T_N\Delta\nu$, with [Boltzmann constant](thermodynamics.md#boltzmann-constant) $k_{\rm B}$. An equivalent [noise temperature](#noise-temperature) need not equal a component's physical [temperature](temperature.md).

#### System noise temperature

↑ **Parent:** [Noise temperature](#noise-temperature)

The [system noise temperature](#system-noise-temperature) includes all noise contributions referred to a specified receiver input. In a simple additive model with negligible intervening losses, $T_{\rm sys}=T_A+T_r$, where $T_A$ is the [antenna temperature](electrical-engineering.md#antenna-temperature) and $T_r$ the [receiver noise temperature](#receiver-noise-temperature).

#### Receiver noise temperature

↑ **Parent:** [Noise temperature](#noise-temperature)

The [receiver noise temperature](#receiver-noise-temperature) represents noise added by the receiver as an equivalent [noise temperature](#noise-temperature) referred to its input. Separating it from the [antenna temperature](electrical-engineering.md#antenna-temperature) prevents internal receiver noise from being mistaken for radiation from the sky.

### Two-load radiometer calibration

↑ **Parent:** [Radiometer](#radiometer)

For a stable [radiometer](#radiometer) with affine output $S=g(T+T_r)$, let $g>0$ be the fixed response coefficient and $T_r$ the [receiver noise temperature](#receiver-noise-temperature). Two reference loads with known equivalent input [noise temperatures](#noise-temperature) $T_c<T_h$ give outputs $S_c$ and $S_h$. Subtracting their outputs eliminates $T_r$; dividing source and reference differences eliminates $g$:

$$
S_h-S_c=g(T_h-T_c),\qquad
T_s=T_c+(T_h-T_c)\frac{S_s-S_c}{S_h-S_c}.
$$

This [two-load radiometer calibration](#two-load-radiometer-calibration) assumes unchanged response and [receiver noise temperature](#receiver-noise-temperature) between readings, with the loads and source referred to the same input. It also eliminates an additional constant output offset. Physical load [temperatures](temperature.md) must first be converted to the applicable equivalent input [noise temperatures](#noise-temperature) when the classical thermal approximation fails. The [Penzias-Wilson microwave background experiment](cosmic-microwave-background.md#penzias-wilson-microwave-background-experiment) gives an original worked example.

## Reflectance

↑ **Parent:** [Radiometry](radiometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reflectance)

The fraction of incident [radiant flux](#radiant-flux) returned by reflection, for specified [wavelength](wave-equation.md#wavelength), [angle of incidence](optics.md#angle-of-incidence) and collection directions.

## Absorption (electromagnetic radiation)

↑ **Parent:** [Radiometry](radiometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Absorption_(electromagnetic_radiation))

The transfer of [energy](energy.md) from [electromagnetic radiation](electromagnetic-radiation.md) to matter. [Reflection](linear-algebra.md#reflection-mathematics) redirects the incident [electromagnetic radiation](electromagnetic-radiation.md), and transmission lets it pass through; absorption transfers some of its [energy](energy.md) to the material instead.

## Radiant flux

↑ **Parent:** [Radiometry](radiometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiant_flux)

[Radiant flux](#radiant-flux) is the [power](energy.md#power) carried by [electromagnetic radiation](electromagnetic-radiation.md): radiation [energy](energy.md) transferred per unit [time](classical-mechanics.md#time-in-physics), measured in [watts](electric-charge.md#watt), $\mathrm W=\mathrm{J\,s^{-1}}$. Specify what is counted: all radiation emitted by a source, radiation within one beam, or radiation intercepted by a [photodetector](optical-instrument.md#photodetector). Writing $Q(t)$ for the cumulative [energy](energy.md) crossing the specified boundary gives

$$
\Phi_e(t)=\frac{dQ}{dt},\qquad
\overline\Phi_e=\frac{Q(t_2)-Q(t_1)}{t_2-t_1},\qquad
Q(t_2)-Q(t_1)=\int_{t_1}^{t_2}\Phi_e(t)\,dt.
$$

The first expression is an instantaneous [derivative](calculus.md#derivative); the second is an average over the stated [time](classical-mechanics.md#time-in-physics) interval. If $0.020\,\mathrm J$ arrives during $0.010\,\mathrm s$, the mean [radiant flux](#radiant-flux) is $2\,\mathrm W$. The [photodetector](optical-instrument.md#photodetector)'s absorbed [power](energy.md#power) equals this incident [radiant flux](#radiant-flux) only if it absorbs all of the incident radiation.

Keeping [radiant flux](#radiant-flux) fixed while widening a beam reduces its [irradiance](#irradiance), the incident [power](energy.md#power) per receiving [area](differential-geometry.md#surface-area). [Radiance](#radiance) additionally resolves the propagation direction and has units $\mathrm{W\,m^{-2}\,sr^{-1}}$; an [optical camera](optical-instrument.md#optical-camera) can collect different [radiant fluxes](#radiant-flux) from sources with the same [radiance](#radiance) but different apparent [solid angles](euclidean-geometry.md#solid-angle). [Luminous flux](optics.md#luminous-flux), measured in lumens, weights the [optical spectrum](optics.md#optical-spectrum) by the human eye's standardized response instead of counting [energy](energy.md) equally at every [wavelength](wave-equation.md#wavelength). Equal [radiant fluxes](#radiant-flux) need not give equal [luminous fluxes](optics.md#luminous-flux).[Radiometry and Photometry: Review for Vision Optics](physics-bibliography.md#osa-handbook-of-optics-volume-iii-visual-optics-and-vision/radiometry-and-photometry-review-for-vision-optics)

[Radiant power](#radiant-flux) also differs from the [optical power](geometrical-optics.md#optical-power) of an [optical lens](geometrical-optics.md#lens-optics), which is reciprocal [focal length](geometrical-optics.md#focal-length) in [dioptres](geometrical-optics.md#dioptre). Likewise, astronomical [radiative flux](astrophysics.md#radiative-flux) is [power](energy.md#power) per [area](differential-geometry.md#surface-area). Stating the units prevents these shared words from hiding different physical quantities.

### Radiant flux through an oriented surface

↑ **Parent:** [Radiant flux](#radiant-flux)

In [geometrical optics](geometrical-optics.md), suppose radiation has a nonnegative [radiance](#radiance) $L(\mathbf x,\mathbf s)$ whose directional contributions add as [power](energy.md#power). Here $\mathbf s$ is the actual propagation [unit vector](vector-space.md#unit-vector), $d\Omega$ is a [solid angle](euclidean-geometry.md#solid-angle) element, and the collecting [oriented surface](differential-geometry.md#oriented-surface) $A$ has chosen [unit normal](differential-geometry.md#unit-normal) $\mathbf n(\mathbf x)$. Assume the following [integrals](integral.md) exist. The outward and inward [radiant fluxes](#radiant-flux) are

$$
\Phi_+=\int_A\!\int_{\mathbf n\cdot\mathbf s>0}
L(\mathbf x,\mathbf s)(\mathbf n\cdot\mathbf s)\,d\Omega\,dA,
\qquad
\Phi_-=\int_A\!\int_{\mathbf n\cdot\mathbf s<0}
L(\mathbf x,\mathbf s)(-\mathbf n\cdot\mathbf s)\,d\Omega\,dA.
$$

Both quantities are nonnegative; their difference is the signed net [radiant flux](#radiant-flux). The [dot product](inner-product.md#dot-product) supplies the [cosine](geometry-and-topology.md#cosine) of the [angle](geometry-and-topology.md#angle) with the [unit normal](differential-geometry.md#unit-normal), hence the [projected area](#projected-area). For incoming radiation the outward [unit normal](differential-geometry.md#unit-normal) gives a negative [dot product](inner-product.md#dot-product); the minus sign makes the collected [power](energy.md#power) positive. Measuring the incoming [angle](geometry-and-topology.md#angle) from a source-facing [unit normal](differential-geometry.md#unit-normal) instead gives the familiar positive $\cos\theta$. The units check is $\mathrm{W\,m^{-2}\,sr^{-1}}\times\mathrm{m^2}\times\mathrm{sr}=\mathrm W$.

Equivalently, the incoming [surface integral](multivariable-calculus.md#surface-integral) is $\Phi_-=\int_A E\,dA$ with local [irradiance](#irradiance) $E$; the emitted part of $\Phi_+$ is $\int_A M\,dA$ with [radiant exitance](#radiant-exitance) $M$. For a small flat patch and a narrow accepted cone, nearly constant [radiance](#radiance) and [angle](geometry-and-topology.md#angle) give $\Phi\simeq LA\cos\theta\,\Delta\Omega$. This approximation requires uniformity across the patch and cone. Direction-independent outgoing [radiance](#radiance) over a whole [hemisphere](euclidean-geometry.md#hemisphere) gives the different exact result $\Phi_+=\pi LA$, by [Lambert's cosine law](optics.md#lambert-s-cosine-law) and the [spherical coordinates](multivariable-calculus.md#spherical-coordinate-system) calculation in [radiant exitance](#radiant-exitance). Replacing the [cosine](geometry-and-topology.md#cosine)-weighted [integral](integral.md) by the [hemisphere](euclidean-geometry.md#hemisphere)'s $2\pi$ [solid angle](euclidean-geometry.md#solid-angle) would double the answer.[Radiometry and Photometry](physics-bibliography.md#radiometry-and-photometry)

These [radiance](#radiance) formulas presume a description in additive directional [power](energy.md#power); they do not reconstruct arbitrary coherent [wave interference](physical-optics.md#interference-wave-propagation) from separate ray contributions. For general [electromagnetic fields](electromagnetism.md#electromagnetic-field), the signed instantaneous [power](energy.md#power) crossing an [oriented surface](differential-geometry.md#oriented-surface) is $\int_A\mathbf S\cdot\mathbf n\,dA$, using the [Poynting vector](electromagnetic-wave.md#poynting-vector) $\mathbf S$; optical measurements commonly average over many [wave periods](wave.md#wave-period). A zero net [radiant flux](#radiant-flux) can conceal equal nonzero incoming and outgoing [radiant fluxes](#radiant-flux).

### Beam collection at fixed radiant flux

↑ **Parent:** [Radiant flux](#radiant-flux)

Consider an ideal parallel circular beam with uniform [irradiance](#irradiance) inside radius $b$, zero outside, and total [radiant flux](#radiant-flux) $P=2\,\mathrm W$. A centred circular collector of radius $a$, perpendicular to the [light rays](geometrical-optics.md#light-ray), intercepts

$$
E_b=\frac{P}{\pi b^2},\qquad
\Phi_{\rm collected}=E_b\pi\min(a,b)^2
=P\min\!\left(1,\frac{a^2}{b^2}\right).
$$

For $b=1\,\mathrm{cm}$ and $a=0.5\,\mathrm{cm}$, $E_b=20000/\pi\,\mathrm{W\,m^{-2}}\simeq6366.20\,\mathrm{W\,m^{-2}}$ and the collected [radiant flux](#radiant-flux) is $0.50\,\mathrm W$. Expanding the beam to $b=2\,\mathrm{cm}$ while keeping $P$ fixed divides [irradiance](#irradiance) and the same collector's [radiant flux](#radiant-flux) by four: $E_b\simeq1591.55\,\mathrm{W\,m^{-2}}$ and $\Phi_{\rm collected}=0.125\,\mathrm W$. A collector covering either entire beam still receives $2\,\mathrm W$.

Tilting a flat collector of actual [area](differential-geometry.md#surface-area) $A$ by an [angle](geometry-and-topology.md#angle) $\theta$ to the beam direction gives $\Phi_{\rm collected}=E_b A\cos\theta$ if its entire [projected area](#projected-area) remains inside the uniform beam. At $60^\circ$ the small collector's [radiant flux](#radiant-flux) halves. A collector large enough to intercept the whole beam after tilting still receives $P$: the footprint on its surface grows as $1/\cos\theta$ and cancels the [irradiance](#irradiance) factor. This model ignores [diffraction](quantum-scattering.md#diffraction), beam-edge structure, and changes in absorption with incidence [angle](geometry-and-topology.md#angle); it counts incident rather than absorbed [power](energy.md#power).

<a id="radiant-flux-beam-collection-geometry"></a>
![](radiant-flux-beam-collection-geometry.png)

**[Figure 1](#radiant-flux-beam-collection-geometry). Fixed radiant flux, different beam widths and collecting projected areas**. Original ideal geometry, not measurements. The beam cross-sections use the same centimetre scale and total [radiant flux](#radiant-flux) of $2\,\mathrm W$; both collectors have radius $0.5\,\mathrm{cm}$. The side view shows a collector's cross-section at $60^\circ$: its projection perpendicular to the [light rays](geometrical-optics.md#light-ray) has half the width, with depth unchanged. The stated half-power result requires the projected collector to stay inside the uniform beam.

### Spectral radiant flux

↑ **Parent:** [Radiant flux](#radiant-flux)

[Spectral radiant flux](#spectral-radiant-flux) resolves [radiant flux](#radiant-flux) by [wavelength](wave-equation.md#wavelength) or [frequency](wave.md#frequency):

$$
\Phi_e=\int_0^\infty\Phi_{e,\lambda}(\lambda)\,d\lambda
=\int_0^\infty\Phi_{e,\nu}(\nu)\,d\nu.
$$

Its units are $\mathrm{W\,m^{-1}}$ per metre of [wavelength](wave-equation.md#wavelength) or $\mathrm{W\,Hz^{-1}}$ per hertz of [frequency](wave.md#frequency). A density quoted per nanometre must be integrated with [wavelength](wave-equation.md#wavelength) intervals in nanometres; its numerical value is $10^{-9}$ times the per-metre density. The [frequency and wavelength spectral radiance conversion](#frequency-and-wavelength-spectral-radiance-conversion) applies equally to [spectral radiant flux](#spectral-radiant-flux), through the [change of variables formula](multivariable-calculus.md#change-of-variables-formula):

$$
\Phi_{e,\nu}(\nu)=\Phi_{e,\lambda}(c/\nu)\frac{c}{\nu^2},
$$

with $c$ the [speed of light](special-relativity.md#speed-of-light) in [vacuum](physics.md#vacuum) and $\Phi_{e,\lambda}$ expressed per metre. The [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) preserves integrated [power](energy.md#power) rather than the height or location of an [optical spectrum](optics.md#optical-spectrum)'s peak.

For two explicitly synthetic [optical spectra](optics.md#optical-spectrum), let $x=\lambda/(1\,\mathrm{nm})$ and quote the following densities in $\mathrm{mW\,nm^{-1}}$:

$$
f_A(x)=\begin{cases}0.020(1-|x-500|/100),&400\leq x\leq600,\\0,&\text{otherwise},\end{cases}
\qquad
f_B(x)=\begin{cases}0.010,&600\leq x\leq800,\\0,&\text{otherwise}.\end{cases}
$$

The [triangle](euclidean-geometry.md#triangle) under $f_A$ and the [rectangle](euclidean-geometry.md#rectangle) under $f_B$ both have [area](differential-geometry.md#surface-area) $2\,\mathrm{mW}$: $200\times0.020/2=200\times0.010=2$. Their band [radiant fluxes](#radiant-flux) differ: $450$–$550\,\mathrm{nm}$ contains $1.5\,\mathrm{mW}$ of $A$, while $650$–$750\,\mathrm{nm}$ contains $1.0\,\mathrm{mW}$ of $B$. These are specified functions, not measured source spectra.

<a id="radiant-flux-synthetic-spectral-integrals"></a>
![](radiant-flux-synthetic-spectral-integrals.png)

**[Figure 2](#radiant-flux-synthetic-spectral-integrals). Equal total radiant flux can hide different band radiant fluxes and detector signals**. Original synthetic [optical spectra](optics.md#optical-spectrum) with exact total [radiant flux](#radiant-flux) $2\,\mathrm{mW}$ each. Darker shading marks the stated 100 nm bands. The lower panel uses a stipulated linear [spectral responsivity](optical-instrument.md#spectral-responsivity) $R(\lambda)=\bigl(0.2+0.001(x-400)\bigr)\,\mathrm{A\,W^{-1}}$; integrating it against the two [spectral radiant fluxes](#spectral-radiant-flux) gives dark-subtracted [electric currents](electric-charge.md#electric-current) $0.60$ and $1.00\,\mathrm{mA}$. The response is illustrative and is not a calibration curve for a real [photodiode](optical-instrument.md#photodiode).

The dark-subtracted [electric current](electric-charge.md#electric-current) of a linear [photodiode](optical-instrument.md#photodiode) is

$$
i=\int R(\lambda)\Phi_{e,\lambda}(\lambda)\,d\lambda,
\qquad [R]=\mathrm{A\,W^{-1}},
$$

using its [spectral responsivity](optical-instrument.md#spectral-responsivity). The figure's stipulated $R$ gives $i_A=0.60\,\mathrm{mA}$ and $i_B=1.00\,\mathrm{mA}$ despite equal total [radiant flux](#radiant-flux). Symmetry places $A$'s mean [wavelength](wave-equation.md#wavelength) at $500\,\mathrm{nm}$ and $B$'s at $700\,\mathrm{nm}$; a linear $R$ averages to its value at that mean. A single [electric current](electric-charge.md#electric-current) therefore cannot determine an unknown broadband [radiant flux](#radiant-flux) without additional spectral information or a sufficiently flat calibrated response.

### Calibrated radiant-flux measurement

↑ **Parent:** [Radiant flux](#radiant-flux)

An [optical power meter](optical-instrument.md#optical-power-meter) makes the definition operational: collect a specified beam on a calibrated [photodiode](optical-instrument.md#photodiode), measure its [electric current](electric-charge.md#electric-current), and infer incident [radiant flux](#radiant-flux) using [spectral responsivity](optical-instrument.md#spectral-responsivity). In the manufacturer-authored [Model 1830-R Series Optical Power Meters User's Manual by Newport Corporation](physics-bibliography.md#model-1830-r-series-optical-power-meters-user-s-manual-by-newport-corporation), §5.5.1 specifies a concrete sequence: connect the detector and its calibration module, select watt mode and the source [wavelength](wave-equation.md#wavelength), block the beam and press ZERO, then unblock it and read the display. The stored background includes [dark current](optical-instrument.md#dark-current-physics) and ambient [light](optics.md#light) present during zeroing. For narrowband radiation,

$$
\Phi_{\rm indicated}=\frac{i_{\rm illuminated}-i_{\rm zero}}{R(\lambda)}.
$$

The [electric current](electric-charge.md#electric-current) difference divided by [spectral responsivity](optical-instrument.md#spectral-responsivity) has units $\mathrm A/(\mathrm{A\,W^{-1}})=\mathrm W$. For a stipulated $R=0.40\,\mathrm{A\,W^{-1}}$ and difference $0.20\,\mathrm{mA}$, the inferred [radiant flux](#radiant-flux) is $0.50\,\mathrm{mW}$; these numbers illustrate the inference and are not reported measurements. The entire beam must hit the active [area](differential-geometry.md#surface-area), and §5.6 calls for correct [wavelength](wave-equation.md#wavelength), background subtraction, and operation below detector saturation. If an [optical attenuator](optical-instrument.md#optical-attenuator) is fitted, §5.4 requires the calibrated detector–attenuator pair and the matching meter setting.

The calibration itself must connect [electric current](electric-charge.md#electric-current) to independently known incident [power](energy.md#power). NIST's [Spectroradiometric Detector Measurements: Ultraviolet, Visible, and Near-Infrared Detectors for Spectral Power by Thomas C. Larason and others](physics-bibliography.md#spectroradiometric-detector-measurements-ultraviolet-visible-and-near-infrared-detectors-for-spectral-power-by-thomas-c-larason-and-others) describes this chain. A [cryogenic radiometer](#cryogenic-radiometer), an [electrical substitution radiometer](#electrical-substitution-radiometer), compares [temperature](temperature.md) changes from absorbed [light](optics.md#light) with those from known [Joule heating](electric-charge.md#joule-heating) (§5.2). Transfer and working detectors carry that [watt](electric-charge.md#watt) scale to a spectral comparator (§5.1). A source, [monochromator](optical-instrument.md#monochromator), focusing optics, shutter, [beam splitter](optical-instrument.md#beam-splitter), and monitor [photodiode](optical-instrument.md#photodiode) illuminate a standard and test detector in turn; calibrated current-to-voltage electronics and voltmeters provide the readout (§§3.2.2–3.2.4, 4.3.1). At each [wavelength](wave-equation.md#wavelength), subtract blocked-beam signals and normalize each detector signal by the simultaneously sampled monitor signal. Comparison with the standard yields the test detector's [spectral responsivity](optical-instrument.md#spectral-responsivity). NIST uses two working standards and alignment normal to the beam (§6.1.1).

Controls distinguish a smaller collected [radiant flux](#radiant-flux) from a faulty conversion: block and unblock the beam to check the baseline; check that its footprint fits the active [area](differential-geometry.md#surface-area); verify the calibrated [optical attenuator](optical-instrument.md#optical-attenuator) configuration; and test proportional response within the specified operating range. Source drift faster than monitor sampling is not removed. NIST discusses finite spectral bandwidth, stray [light](optics.md#light), [temperature](temperature.md), and spatial response variations (§§3.1.1, 6.2, 7.2). A broadband [optical spectrum](optics.md#optical-spectrum) requires the weighted [integral](integral.md) in [spectral radiant flux](#spectral-radiant-flux), rather than dividing by an arbitrary single [spectral responsivity](optical-instrument.md#spectral-responsivity). These limitations explain why the meter's displayed [watts](electric-charge.md#watt) need a stated collection boundary, spectral assumptions, and calibration conditions.

## Radiant intensity

↑ **Parent:** [Radiometry](radiometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiant_intensity)

[Radiant intensity](#radiant-intensity) describes how a source distributes its [radiant flux](#radiant-flux) over directions. A small cone of [solid angle](euclidean-geometry.md#solid-angle) $\Delta\Omega$ carries approximately $I\Delta\Omega$ when $I$ varies little across it; integrating $I$ over all emitting directions recovers the total [radiant flux](#radiant-flux). For a source with [isotropy](continuum-mechanics.md#isotropy) emitting $4\pi\,\mathrm W$ over a full [sphere](euclidean-geometry.md#sphere), $I=1\,\mathrm{W\,sr^{-1}}$ and a $0.01\,\mathrm{sr}$ cone carries $0.01\,\mathrm W$. A planar source satisfying [Lambert's cosine law](optics.md#lambert-s-cosine-law) instead has direction-dependent [radiant intensity](#radiant-intensity), even though its [radiance](#radiance) is direction-independent.

### Point emitter

↑ **Parent:** [Radiant intensity](#radiant-intensity)

An ideal [point emitter](#point-emitter) emits [radiant flux](#radiant-flux) from one location. It approximates a physical source when its emitting dimensions are small relative to the distances relevant to the calculation. With [isotropy](continuum-mechanics.md#isotropy), its [radiant intensity](#radiant-intensity) is $I=\Phi/(4\pi)$ for total [radiant flux](#radiant-flux) $\Phi$. An extended source generally requires integrating contributions from different emitting positions.

## Radiance

↑ **Parent:** [Radiometry](radiometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiance)

[Radiance](#radiance) resolves both position and direction: it is [radiant flux](#radiant-flux) per [projected area](#projected-area) and per [solid angle](euclidean-geometry.md#solid-angle). For a surface element of [area](differential-geometry.md#surface-area) $dA$, and a small outgoing cone $d\Omega$ at [angle](geometry-and-topology.md#angle) $0\leq\theta<\pi/2$ to its outward [unit normal](differential-geometry.md#unit-normal),

$$
d^2\Phi=L(\mathbf x,\mathbf s)\cos\theta\,dA\,d\Omega,
\qquad [L]=\mathrm{W\,m^{-2}\,sr^{-1}}.
$$

Here $\mathbf x$ locates the patch and $\mathbf s$ is a [unit vector](vector-space.md#unit-vector) along the outgoing direction. The factor $dA\cos\theta$ is the patch's apparent [area](differential-geometry.md#surface-area) viewed along that direction. The same local definition applies to transmitted or received radiation, choosing the positive [projected area](#projected-area) for the crossing direction. [Marianne Breinig, University of Tennessee, Radiometry: radiance and Lambert's law](https://labs.phys.utk.edu/mbreinig/phys421/modules/m5/Radiometry.html).

For a planar patch of [area](differential-geometry.md#surface-area) $A$ with spatially uniform, direction-independent [radiance](#radiance) $L$, integrating over the patch gives

$$
I(\theta)=LA\cos\theta.
$$

Take $L=10\,\mathrm{W\,m^{-2}\,sr^{-1}}$ and $A=0.020\,\mathrm{m^2}$. The [radiant intensities](#radiant-intensity) are $I(0)=0.20\,\mathrm{W\,sr^{-1}}$ and $I(60^\circ)=0.10\,\mathrm{W\,sr^{-1}}$. A sufficiently narrow $0.010\,\mathrm{sr}$ cone therefore carries approximately $2.0\,\mathrm{mW}$ or $1.0\,\mathrm{mW}$, respectively. Both views have the same [radiance](#radiance) $L$: the oblique view presents half the [projected area](#projected-area). This is [Lambert's cosine law](optics.md#lambert-s-cosine-law), not a loss of [radiance](#radiance) with viewing [angle](geometry-and-topology.md#angle).

<a id="image-one-uniform-patch-halving-projected-area-halves-radiant-intensity-while-preserving-radiance"></a>
![](projected-area-radiance.png)

**[Figure 3](#image-one-uniform-patch-halving-projected-area-halves-radiant-intensity-while-preserving-radiance). One uniform patch: halving projected area halves radiant intensity while preserving radiance**. The geometric panels show a cross-section of a rectangular patch with the same depth perpendicular to the page. Parallel projection onto a plane perpendicular to the viewing direction changes its width by $\cos\theta$. The graph gives $I(\theta)=LA\cos\theta$ for the stated patch and marks the exact $0^\circ$ and $60^\circ$ cases.

[Radiance](#radiance) is useful because it separates a source's local directional output from the geometry of an observation. Integrating over outgoing directions gives [radiant exitance](#radiant-exitance); integrating incoming [radiance](#radiance) at a receiver gives [irradiance](#irradiance). In the stationary [vacuum](physics.md#vacuum) setting of [vacuum conservation of specific intensity](#vacuum-conservation-of-specific-intensity), a resolved uniform source retains its [radiance](#radiance) along each [light ray](geometrical-optics.md#light-ray), while the [radiant flux](#radiant-flux) received from the whole source can decrease as its apparent [solid angle](euclidean-geometry.md#solid-angle) shrinks.

### Projected area

↑ **Parent:** [Radiance](#radiance)

The [projected area](#projected-area) of a planar patch viewed from a direction is the [area](differential-geometry.md#surface-area) of its perpendicular shadow onto a plane normal to that direction. If $\mathbf n$ and $\mathbf s$ are its [unit normal](differential-geometry.md#unit-normal) and viewing [unit vector](vector-space.md#unit-vector), then $A_\perp=A|\mathbf n\cdot\mathbf s|$ by the [dot product](inner-product.md#dot-product). On the outward side, this is $A\cos\theta$. For a [rectangle](euclidean-geometry.md#rectangle) tilted around one edge, the width perpendicular to that edge contracts by $\cos\theta$ and the edge length stays fixed, proving the formula. At grazing view $A_\perp=0$; interpret the [radiance](#radiance) definition by a limit rather than dividing by zero.

### Spectral radiance

↑ **Parent:** [Radiance](#radiance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectral_radiance)

[Spectral radiance](#spectral-radiance) is [radiance](#radiance) per unit [frequency](wave.md#frequency) or [wavelength](wave-equation.md#wavelength) interval. Its astronomical synonym [specific intensity](#spectral-radiance) is usually written $I_\nu=L_\nu$ or $I_\lambda=L_\lambda$; this $I_\nu$ is a spectral [radiance](#radiance), distinct from the [radiant intensity](#radiant-intensity) $I$ in [radiometry](radiometry.md). For positive small intervals,

$$
d^3\Phi=L_\nu\cos\theta\,dA\,d\Omega\,d\nu
=L_\lambda\cos\theta\,dA\,d\Omega\,d\lambda.
$$

The two expressions refer to the same spectral slice, with the positive widths related through [frequency](wave.md#frequency) $\nu$ and [wavelength](wave-equation.md#wavelength) $\lambda$. For [frequency](wave.md#frequency) measured in hertz, $\mathrm{Hz}=\mathrm{s^{-1}}$, the units are $[L_\nu]=\mathrm{W\,m^{-2}\,sr^{-1}\,Hz^{-1}}$. For [wavelength](wave-equation.md#wavelength) measured in metres, $[L_\lambda]=\mathrm{W\,m^{-2}\,sr^{-1}\,m^{-1}}$. Integrating over a spectral band gives its [radiance](#radiance), and then multiplying by the collecting [projected area](#projected-area) and accepted [solid angle](euclidean-geometry.md#solid-angle) gives a small uniform beam's [radiant flux](#radiant-flux). A spectral measurement therefore retains information that the band-integrated [power](energy.md#power) alone loses.

For an ideal [blackbody](astrophysics.md#blackbody), [Planck's law](statistical-physics.md#planck-s-law) gives $L_\nu=B_\nu(T)$ and $L_\lambda=B_\lambda(T)$ at [temperature](temperature.md) $T$, independent of outgoing direction. Its existing [frequency and wavelength peaks of Planck's law](statistical-physics.md#frequency-and-wavelength-peaks-of-planck-s-law) illustrate why the coordinate matters. The simpler flat-band calculation below isolates that same [change of variables](multivariable-calculus.md#change-of-variables-formula) without the thermal physics.

#### Frequency and wavelength spectral radiance conversion

↑ **Parent:** [Spectral radiance](#spectral-radiance)

In [vacuum](physics.md#vacuum), $\nu=c/\lambda$, where $c$ is the [speed of light](special-relativity.md#speed-of-light). Increasing [wavelength](wave-equation.md#wavelength) decreases [frequency](wave.md#frequency), so the ordinary signed [differentials](smooth-manifold.md#differential-of-a-smooth-map) satisfy $d\nu=-c\lambda^{-2}d\lambda$. A spectral slice's positive contribution to [radiance](#radiance) must be unchanged. The [change of variables formula](multivariable-calculus.md#change-of-variables-formula) therefore gives the absolute [Jacobian determinant](multivariable-calculus.md#jacobian-determinant)

$$
L_\nu(\nu)=L_\lambda(c/\nu)\left|\frac{d\lambda}{d\nu}\right|
=L_\lambda(c/\nu)\frac{c}{\nu^2},
\qquad
L_\lambda(\lambda)=L_\nu(c/\lambda)\frac{c}{\lambda^2}.
$$

These formulas use $L_\lambda$ per metre and $L_\nu$ per hertz. The factor $c/\nu^2$ has units $\mathrm{m\,s}=\mathrm{m\,Hz^{-1}}$, which converts the former density into the latter. If $\ell_{\rm nm}$ denotes the numerical density per nanometre in $\mathrm{W\,m^{-2}\,sr^{-1}\,nm^{-1}}$, its per-metre value is $10^9\ell_{\rm nm}$. Conversely, the per-nanometre value is $10^{-9}$ times the per-metre value. Likewise, a density per terahertz is $10^{12}$ times its per-hertz value because $1\,\mathrm{THz}=10^{12}\,\mathrm{Hz}$.

For a concrete stipulated spectrum, let $L_\lambda=C=10^9\,\mathrm{W\,m^{-2}\,sr^{-1}\,m^{-1}}$ between $\lambda_1=500\,\mathrm{nm}$ and $\lambda_2=600\,\mathrm{nm}$, and zero outside. This is exactly $1\,\mathrm{W\,m^{-2}\,sr^{-1}\,nm^{-1}}$ throughout the band. Using the exact [International System of Units](physics.md#international-system-of-units) value $c=299792458\,\mathrm{m\,s^{-1}}$, the corresponding [frequency](wave.md#frequency) bounds are

$$
\nu_1=\frac{c}{\lambda_2}=499.654096666\ldots\,\mathrm{THz},
\qquad
\nu_2=\frac{c}{\lambda_1}=599.584916\,\mathrm{THz}.
$$

The transformed [spectral radiance](#spectral-radiance) is $L_\nu=Cc/\nu^2$ on this interval. At $\nu_1$ it is approximately $1.200830743\times10^{-12}\,\mathrm{W\,m^{-2}\,sr^{-1}\,Hz^{-1}}$, and at $\nu_2$ it is $8.339102380\times10^{-13}$ in the same units. These are respectively $1.200830743$ and $0.833910238$ per terahertz. Thus a flat [wavelength](wave-equation.md#wavelength) density becomes a decreasing [frequency](wave.md#frequency) density; relabelling the horizontal axis alone would miss both the shape and the units. [NIST, Meet the Constants: exact speed of light](https://www.nist.gov/si-redefinition/meet-constants).

The equality of band [radiances](#radiance) has a short exact proof:

$$
\int_{\lambda_1}^{\lambda_2}C\,d\lambda
=C(\lambda_2-\lambda_1)
=100\,\mathrm{W\,m^{-2}\,sr^{-1}},
$$



$$
\int_{\nu_1}^{\nu_2}\frac{Cc}{\nu^2}\,d\nu
=Cc\left(\frac1{\nu_1}-\frac1{\nu_2}\right)
=C(\lambda_2-\lambda_1).
$$

The reversed bounds and the [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) preserve the same spectral measure. Each half-band, $500$–$550\,\mathrm{nm}$ and $550$–$600\,\mathrm{nm}$, carries $50\,\mathrm{W\,m^{-2}\,sr^{-1}}$, although the corresponding [frequency](wave.md#frequency) widths are about $54.508$ and $45.423\,\mathrm{THz}$.

<a id="image-a-flat-wavelength-spectrum-becomes-curved-in-frequency-with-equal-band-radiances"></a>
![](spectral-radiance-variable-change.png)

**[Figure 4](#image-a-flat-wavelength-spectrum-becomes-curved-in-frequency-with-equal-band-radiances). A flat wavelength spectrum becomes curved in frequency, with equal band radiances**. Matching colours identify the same two spectral half-bands. The shaded areas are $50\,\mathrm{W\,m^{-2}\,sr^{-1}}$ each in either coordinate. The right-hand density is plotted per terahertz; the longer-wavelength half-band occupies the lower-frequency, narrower interval. Both total shaded areas are exactly $100\,\mathrm{W\,m^{-2}\,sr^{-1}}$.

A spectrum's peak is consequently a statement about a particular density and coordinate. The [frequency and wavelength peaks of Planck's law](statistical-physics.md#frequency-and-wavelength-peaks-of-planck-s-law) differ for precisely this reason. Integrated [radiance](#radiance) over a specified physical band supplies a comparison that survives the [change of variables](multivariable-calculus.md#change-of-variables-formula).

#### Vacuum conservation of specific intensity

↑ **Parent:** [Spectral radiance](#spectral-radiance)

In a transparent, stationary [vacuum](physics.md#vacuum) with [Euclidean geometry](euclidean-geometry.md) and observers at rest in the same frame, the [radiative transfer equation](astrophysics.md#radiative-transfer-equation) has zero absorption and emission, so $dI_\nu/ds=0$ along a [light ray](geometrical-optics.md#light-ray). The same [specific intensity](#spectral-radiance) reaches the observer without geometric dilution. More generally, $I_\nu/\nu^3$ is a [Lorentz invariant](special-relativity.md#lorentz-invariance); collisionless propagation preserves this ratio along a ray even with gravitational or cosmological [redshift](optics.md#redshift), rather than preserving $I_\nu$ at shifted [frequencies](wave.md#frequency). [John Peacock, Radiation and Matter, 2018–2019, §4.1, Conservation of intensity and equation (140)](https://www.roe.ac.uk/japwww/teaching/ram5/ram5_2018.pdf#page=27).

The elementary geometry is instructive. Two facing surface elements separated by distance $s$ exchange spectral [radiant flux](#radiant-flux)

$$
d^3\Phi=I_\nu\frac{\cos\theta_1\cos\theta_2}{s^2}\,dA_1\,dA_2\,d\nu.
$$

The receiver subtends $d\Omega_2=\cos\theta_2\,dA_2/s^2$ at the source. Describing that same traveling beam at the receiver instead uses $d\Omega_1=\cos\theta_1\,dA_1/s^2$. Both descriptions have identical geometric factors, so conservation of its [radiant flux](#radiant-flux) gives equal [specific intensities](#spectral-radiance) at the two ends. This compares the same propagation direction at both ends, not emission in the opposite direction.

A uniform source remains equally bright per resolved direction under these assumptions, but occupies a smaller apparent [solid angle](euclidean-geometry.md#solid-angle) farther away. For a small source of [projected area](#projected-area) $A_\perp$ at distance $d$ and a small receiver facing it, [irradiance](#irradiance) is approximately $E=L\Omega_{\rm source}\simeq LA_\perp/d^2$. The [radiant flux](#radiant-flux) intercepted by receiver [area](differential-geometry.md#surface-area) $A_d$ is approximately $EA_d$. With $L=10\,\mathrm{W\,m^{-2}\,sr^{-1}}$, $A_\perp=0.020\,\mathrm{m^2}$ and $A_d=10^{-4}\,\mathrm{m^2}$, distances $10$ and $20\,\mathrm m$ give $E\simeq0.002$ and $0.0005\,\mathrm{W\,m^{-2}}$, and received [radiant fluxes](#radiant-flux) of $0.20$ and $0.050\,\mu\mathrm W$. The [inverse-square law](physics.md#inverse-square-law) concerns collected radiation from the whole source; $L$ remains $10$ at either distance.

#### Limb darkening

↑ **Parent:** [Spectral radiance](#spectral-radiance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Limb_darkening)

Limb darkening is the decrease of emergent [specific intensity](#spectral-radiance) toward the apparent edge of a stellar disc. A transit depth then depends on the intensity sampled by the planet as well as its projected area; the uniform-disc area ratio is only an approximation.

For a spherical [star](stellar-astrophysics.md#star) of [radius](topology.md#radius) $R_\star$, let $r$ be distance from the centre of its projected disk and let $\theta$ be the [angle](geometry-and-topology.md#angle) between the outward [unit normal](differential-geometry.md#unit-normal) and the [line of sight](astrophysics.md#line-of-sight). The angular coordinate is

$$
\mu=\cos\theta=\sqrt{1-(r/R_\star)^2}.
$$

Disk centre has $\mu=1$; the apparent edge approaches $\mu=0$. A resolved image measures [specific intensity](#spectral-radiance) in each direction. [Limb darkening](#limb-darkening) means that this [specific intensity](#spectral-radiance) itself falls toward the edge; the [projected area](#projected-area) factor used when collecting [radiant flux](#radiant-flux) is a separate geometric effect.

A simple explanation assumes a horizontally uniform [plane-parallel atmosphere](astrophysics.md#plane-parallel-atmosphere), a sufficiently deep [optically thick medium](astrophysics.md#optically-thick-medium), negligible [scattering of light](optics.md#scattering-of-light), and thermal absorption and emission in [local thermodynamic equilibrium](astrophysics.md#local-thermodynamic-equilibrium). Let $\tau_\nu$ be inward vertical [optical depth](astrophysics.md#optical-depth) at fixed [frequency](wave.md#frequency) $\nu$. An oblique [light ray](geometrical-optics.md#light-ray) has [line of sight](astrophysics.md#line-of-sight) [optical depth](astrophysics.md#optical-depth) $\tau_\nu/\mu$, so it encounters the same attenuation at a smaller vertical [optical depth](astrophysics.md#optical-depth). The [formal solution of the radiative transfer equation](astrophysics.md#formal-solution-of-the-radiative-transfer-equation) gives

$$
I_\nu(0,\mu)=\int_0^\infty S_\nu(\tau_\nu)e^{-\tau_\nu/\mu}\frac{d\tau_\nu}{\mu},\qquad 0<\mu\le1.
$$

Here $S_\nu$ is the [source function](astrophysics.md#radiative-transfer-source-function); under these assumptions it is the [Planck function](astrophysics.md#planck-function) $B_\nu[T(\tau_\nu)]$. If [temperature](temperature.md) increases inward, an oblique view preferentially samples cooler layers and hence lower [specific intensity](#spectral-radiance). [§2.2.2, pp. 17–19, equations (2.37)–(2.44) and Figure 2.4](physics-bibliography.md#radiative-transfer-in-stellar-atmospheres-by-robert-j-rutten-8th-edition)

The weight $e^{-\tau_\nu/\mu}/\mu$ is an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) in vertical [optical depth](astrophysics.md#optical-depth), with [expected value](expected-value.md) $\mu$ and [standard deviation](variance.md#standard-deviation) $\mu$. Thus “seeing down to [optical depth](astrophysics.md#optical-depth) one” refers to the [line of sight](astrophysics.md#line-of-sight), and represents a broad sampling of layers rather than a sharp emitting surface. For a [source function](astrophysics.md#radiative-transfer-source-function) that is linear throughout the atmosphere, the [Eddington-Barbier relation](astrophysics.md#eddington-barbier-relation) is exact:

$$
S_\nu(\tau_\nu)=a_\nu+b_\nu\tau_\nu
\quad\Longrightarrow\quad
I_\nu(0,\mu)=a_\nu+b_\nu\mu=S_\nu(\mu).
$$

This follows by integrating the constant and linear terms separately. A constant [source function](astrophysics.md#radiative-transfer-source-function) instead gives constant [specific intensity](#spectral-radiance), as in the [blackbody limit of an isothermal atmosphere](astrophysics.md#blackbody-limit-of-an-isothermal-atmosphere). An outward-rising [temperature](temperature.md) or important [scattering of light](optics.md#scattering-of-light) changes the argument. Close enough to the actual edge, a [plane-parallel atmosphere](astrophysics.md#plane-parallel-atmosphere) also loses validity because of curvature. Neither one [limb-darkening coefficient](#limb-darkening-coefficient) nor a universal dependence on [wavelength](wave-equation.md#wavelength) follows from this simple model.

##### Linear limb-darkening law

↑ **Parent:** [Limb darkening](#limb-darkening)

The [linear limb-darkening law](#linear-limb-darkening-law) parametrizes angular [specific intensity](#spectral-radiance) by a stipulated [limb-darkening coefficient](#limb-darkening-coefficient) $u$:

$$
I(\mu)=I_c[1-u(1-\mu)],\qquad I_c=I(1),\qquad 0\le u\le1.
$$

Here $I$ denotes [specific intensity](#spectral-radiance) at one [frequency](wave.md#frequency), or [radiance](#radiance) integrated over a specified interval of [frequency](wave.md#frequency) or [wavelength](wave-equation.md#wavelength); it does not denote [radiant intensity](#radiant-intensity). Within this stipulated range, $u=0$ gives a uniform disk and $I(0)/I_c=1-u$. The [linear limb-darkening law](#linear-limb-darkening-law) is linear in $\mu$, while its radial profile $I(r)=I_c[1-u+u\sqrt{1-(r/R_\star)^2}]$ is curved. In the linear [source function](astrophysics.md#radiative-transfer-source-function) example above, $u=b_\nu/(a_\nu+b_\nu)$ when $a_\nu,b_\nu\ge0$ and $a_\nu+b_\nu>0$.

For the illustrative choice $u=0.6$, the [specific intensity](#spectral-radiance) at $r/R_\star=0$, $0.8$, and the limiting edge is respectively $I_c$, $0.76I_c$, and $0.4I_c$. These are synthetic values, not measurements of the [Sun](stellar-astrophysics.md#sun). Real [optical spectra](optics.md#optical-spectrum) and [stellar atmospheres](stellar-astrophysics.md#stellar-atmosphere) need not obey a [linear limb-darkening law](#linear-limb-darkening-law); more flexible profiles can be necessary for accurate [exoplanet transit photometry](exoplanet.md#exoplanet-transit-photometry). [§1, p. L171: the linear law is insufficient for the cited high-quality transit observations; §4 defines a quadratic law](physics-bibliography.md#analytic-light-curves-for-planetary-transit-searches-by-kaisey-mandel-and-eric-agol)

<a id="image-synthetic-stellar-disk-and-angular-and-radial-limb-darkening-profiles"></a>
![](stellar-limb-darkening-disk-profiles.png)

**[Figure 5](#image-synthetic-stellar-disk-and-angular-and-radial-limb-darkening-profiles). Synthetic stellar disk and angular and radial limb darkening profiles**. The disk uses the stipulated [linear limb-darkening law](#linear-limb-darkening-law) with $u=0.6$. The profiles compare four stipulated [limb-darkening coefficients](#limb-darkening-coefficient) at equal central [specific intensity](#spectral-radiance). Shading represents relative brightness, without prescribing a [wavelength](wave-equation.md#wavelength) or copying a solar measurement.

###### Limb-darkening coefficient

↑ **Parent:** [Linear limb-darkening law](#linear-limb-darkening-law)

The parameter $u$ in the [linear limb-darkening law](#linear-limb-darkening-law) specifies its contrast between disk centre and the limiting edge. Its interpretation requires the chosen law and interval of [frequency](wave.md#frequency) or [wavelength](wave-equation.md#wavelength). A [limb-darkening coefficient](#limb-darkening-coefficient) fitted to an [exoplanet transit](exoplanet.md#exoplanet-transit) may trade off against the [transit impact parameter](exoplanet.md#transit-impact-parameter) and [planet](planetary-science.md#planet) [radius](topology.md#radius); it is not a direct measurement of one layer's [temperature](temperature.md).

##### Limb-darkened disk flux

↑ **Parent:** [Limb darkening](#limb-darkening)

For a circular stellar disk whose [specific intensity](#spectral-radiance) is independent of [azimuth](astrophysics.md#azimuth), its mean [specific intensity](#spectral-radiance) over [projected area](#projected-area) is

$$
\overline I=\frac{1}{\pi R_\star^2}\int_{\rm disk} I\,dA_{\rm proj}
=2\int_0^1 I(\mu)\mu\,d\mu.
$$

The [polar coordinates](multivariable-calculus.md#polar-coordinates) element is $dA_{\rm proj}=2\pi r\,dr$ after angular integration, and $r\,dr=-R_\star^2\mu\,d\mu$. Substitution of the [linear limb-darkening law](#linear-limb-darkening-law) gives

$$
\overline I=2I_c\int_0^1(1-u+u\mu)\mu\,d\mu=I_c(1-u/3).
$$

For a distant observer at distance $D\gg R_\star$ receiving [light](optics.md#light) normally to the detecting plane, the [observed radiative flux](astrophysics.md#observed-radiative-flux) is

$$
f_\nu\simeq\frac{\pi R_\star^2}{D^2}\overline I_\nu
=\pi\left(\frac{R_\star}{D}\right)^2I_{\nu,c}(1-u_\nu/3).
$$

It is spectral [irradiance](#irradiance), with units $\mathrm{W\,m^{-2}\,Hz^{-1}}$ when $I_\nu$ is per hertz. The local outward [radiative flux](astrophysics.md#radiative-flux) per actual surface [area](differential-geometry.md#surface-area) is instead $F_\nu=2\pi\int_0^1 I_\nu(\mu)\mu\,d\mu=\pi\overline I_\nu$, a spectral [radiant exitance](#radiant-exitance). In a spherical model with the same [stellar atmosphere](stellar-astrophysics.md#stellar-atmosphere) everywhere, the [luminosity](astrophysics.md#luminosity) is $L_\nu=4\pi R_\star^2F_\nu$ and $f_\nu=L_\nu/(4\pi D^2)$, consistent with the [inverse-square law](physics.md#inverse-square-law). Compare disks at fixed $I_c$ or fixed total [observed radiative flux](astrophysics.md#observed-radiative-flux) explicitly: increasing $u$ lowers the total in the first comparison, while the second requires a larger $I_c$.

##### Small-planet transit weighting

↑ **Parent:** [Limb darkening](#limb-darkening)

A dark, opaque circular [planet](planetary-science.md#planet) of [radius](topology.md#radius) $R_p$ blocks [specific intensity](#spectral-radiance) over its overlap with the projected [star](stellar-astrophysics.md#star). With $k=R_p/R_\star$ and no [transit dilution](exoplanet.md#transit-dilution), the instantaneous [exoplanet transit depth](exoplanet.md#exoplanet-transit-depth) is exactly

$$
\delta=\frac{\displaystyle\int_{\rm overlap}I\,dA_{\rm proj}}{\pi R_\star^2\overline I}.
$$

When $k\ll1$, the entire planetary disk is inside the stellar disk, and [specific intensity](#spectral-radiance) varies little across that disk, [small-planet transit weighting](#small-planet-transit-weighting) reduces to

$$
\delta\simeq k^2\frac{I(\mu_p)}{\overline I}
=k^2\frac{1-u+u\mu_p}{1-u/3},\qquad
\mu_p=\sqrt{1-z^2},\qquad z<1-k.
$$

Here $z$ is the projected centre separation divided by $R_\star$. The numerator samples the local [specific intensity](#spectral-radiance); the denominator normalizes by the whole [star](stellar-astrophysics.md#star)'s mean [specific intensity](#spectral-radiance). The small-size argument and the distinction between full overlap and ingress are explicit in the original analytic treatment. [§2, p. L171, geometry; §5, p. L174, small-planet approximation restricted to the interior $z<1-p$](physics-bibliography.md#analytic-light-curves-for-planetary-transit-searches-by-kaisey-mandel-and-eric-agol)

For a short approximately straight crossing at constant transverse [velocity](classical-mechanics.md#velocity) $v_\perp$, write $x=v_\perp t/R_\star$ with $t=0$ at mid-transit, and let $b$ be the [transit impact parameter](exoplanet.md#transit-impact-parameter). Then $z^2=x^2+b^2$ and $\mu_p=\sqrt{1-b^2-x^2}$. With stipulated $u=0.6$ and $k=0.05$, a central crossing has mid-transit [exoplanet transit depth](exoplanet.md#exoplanet-transit-depth) approximately $0.003125$, whereas $b=0.8$ gives $0.002375$. A uniform disk would give $k^2=0.0025$ for either fully overlapping crossing. The brighter central chord produces a deeper dip and the off-centre chord a shorter crossing at the same $v_\perp$.

<a id="image-two-transit-chords-across-the-same-synthetic-limb-darkened-disk-flux-distribution"></a>
![](limb-darkened-transit-chord-weighting.png)

**[Figure 6](#image-two-transit-chords-across-the-same-synthetic-limb-darkened-disk-flux-distribution). Two transit chords across the same synthetic limb-darkened disk flux distribution**. Stipulated $u=0.6$ and $k=0.05$; the coloured curves integrate the occulted [specific intensity](#spectral-radiance) over the finite planetary disk, including ingress and egress. Dashed curves show [small-planet transit weighting](#small-planet-transit-weighting) only where the whole planetary disk is inside the [star](stellar-astrophysics.md#star). Horizontal dotted segments give the uniform-disk full-overlap depth $k^2$. The chord panel shows mid-transit positions; the horizontal coordinate in the [light curve](astrophysics.md#light-curve) is distance travelled divided by stellar [radius](topology.md#radius), equivalent to scaled [time](classical-mechanics.md#time-in-physics) at constant transverse [velocity](classical-mechanics.md#velocity).

At fixed $z<1$ away from the edge, a two-dimensional [Taylor's theorem](calculus.md#taylor-s-theorem) expansion over the symmetric planetary disk cancels the first [derivatives](calculus.md#derivative); the first correction to the blocked [radiant flux](#radiant-flux) is of order $k^4$ if the second [derivatives](calculus.md#derivative) remain bounded. This error estimate is not uniform at the edge, where the radial [derivative](calculus.md#derivative) of the [linear limb-darkening law](#linear-limb-darkening-law) diverges. Ingress, egress, a grazing [exoplanet transit](exoplanet.md#exoplanet-transit), and a crossing of a [starspot](exoplanet.md#starspot) require the overlap [integral](integral.md) or a suitable more complete model. Inferring $k=\sqrt\delta$ without the local-to-mean [specific intensity](#spectral-radiance) ratio can bias the estimated [planet](planetary-science.md#planet) [radius](topology.md#radius).

##### Solar limb-darkening drift-scan experiment

↑ **Parent:** [Limb darkening](#limb-darkening)

A motivating measurement used the McMath solar [optical telescope](optical-instrument.md#optical-telescope) at Kitt Peak. The [Sun](stellar-astrophysics.md#sun)'s image drifted across a $10\,\mathrm{mm}$-high, $0.2\,\mathrm{mm}$-wide [optical slit](optical-instrument.md#optical-slit); a double-pass [spectrograph](optical-instrument.md#spectrograph) selected [wavelength](wave-equation.md#wavelength) intervals from $0.0015\,\mathrm{nm}$ wide at $303\,\mathrm{nm}$ to $0.007\,\mathrm{nm}$ at $1099\,\mathrm{nm}$. An EMI 9750 QB [photodetector](optical-instrument.md#photodetector) or [silicon](chemical-substance.md#silicon) [photodiode](optical-instrument.md#photodiode) supplied a digitized signal: $1\,\mathrm{kHz}$ samples were summed into 4096 positions per crossing, including dark and off-limb sky readings. [§2, p. 93, instrumental compilation: slit dimensions, double pass, detectors, sampling and drift-curve layout; p. 113, acknowledgements identifying the telescope](physics-bibliography.md#solar-limb-darkening-1986-1990-lambda-lambda-303-to-1099-nm-by-heinz-neckel-and-dietrich-labs)

Controls included daily realignment of [optical telescope](optical-instrument.md#optical-telescope) mirrors, [wavelength](wave-equation.md#wavelength) settings between [spectral lines](stellar-astrophysics.md#spectral-line) insensitive to the rotational [Doppler shift](wave.md#doppler-effect), selection of detectors without detectable [hysteresis](critical-phenomenon.md#hysteresis), and measured electronic nonlinearity corrections below $0.1\%$ of maximum signal. Limb-position calibration combined centres of gravity of the edge [derivative](calculus.md#derivative) profiles with almanac semidiameters; the preliminary edge shifts were consistent with [astronomical seeing](optics.md#astronomical-seeing) of approximately $5$ [arcseconds](geometry-and-topology.md#arcsecond) [full width at half maximum](analysis.md#full-width-at-half-maximum). [§2, pp. 93–94, precautions (1), (6)–(8); §3.1, p. 94, two-step limb positions and seeing estimate](physics-bibliography.md#solar-limb-darkening-1986-1990-lambda-lambda-303-to-1099-nm-by-heinz-neckel-and-dietrich-labs)

The decreasing centre-to-limb readout gives a [specific intensity](#spectral-radiance) profile, constraining stratification of the [photosphere](stellar-structure.md#photosphere) under a [radiative transfer](astrophysics.md#radiative-transfer) model. [Astronomical seeing](optics.md#astronomical-seeing), instrumental [scattering of light](optics.md#scattering-of-light), and [solar granulation](stellar-astrophysics.md#solar-granulation) limit this inference; brightness alone does not uniquely determine [temperature](temperature.md) versus geometric height. These observations need not follow the stipulated [linear limb-darkening law](#linear-limb-darkening-law).

## Radiant exitance

↑ **Parent:** [Radiometry](radiometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiant_exitance)

[Radiant exitance](#radiant-exitance) is total outward emitted [radiant flux](#radiant-flux) per actual emitting [area](differential-geometry.md#surface-area), measured in $\mathrm{W\,m^{-2}}$. Integrate [radiance](#radiance) over the outward [hemisphere](euclidean-geometry.md#hemisphere), keeping the [projected area](#projected-area) factor:

$$
M=\int_{\Omega_{\rm outward}}L(\theta,\varphi)\cos\theta\,d\Omega.
$$

If the [radiance](#radiance) is direction-independent, the [spherical coordinates](multivariable-calculus.md#spherical-coordinate-system) element is $d\Omega=\sin\theta\,d\theta\,d\varphi$, so

$$
M=L\int_0^{2\pi}\!d\varphi\int_0^{\pi/2}\cos\theta\sin\theta\,d\theta=\pi L.
$$

The weighted [solid angle](euclidean-geometry.md#solid-angle) is $\pi\,\mathrm{sr}$, although the whole [hemisphere](euclidean-geometry.md#hemisphere) covers $2\pi\,\mathrm{sr}$. Directions near grazing contribute less because of the [projected area](#projected-area). This geometric factor is the bridge between [Lambert's cosine law](optics.md#lambert-s-cosine-law) and the total output of a diffuse patch. [Breinig, Radiometry: hemispherical integration of radiance](https://labs.phys.utk.edu/mbreinig/phys421/modules/m5/Radiometry.html).

For the uniform patch with $L=10\,\mathrm{W\,m^{-2}\,sr^{-1}}$, [radiant exitance](#radiant-exitance) is $M=10\pi\,\mathrm{W\,m^{-2}}$. Its [area](differential-geometry.md#surface-area) $0.020\,\mathrm{m^2}$ gives total [radiant flux](#radiant-flux) $\Phi=MA=0.20\pi\,\mathrm W\approx0.628319\,\mathrm W$ over the outward [hemisphere](euclidean-geometry.md#hemisphere). This total differs from its [radiant intensity](#radiant-intensity) $I(0)=0.20\,\mathrm{W\,sr^{-1}}$, which describes only one direction.

For an ideal [blackbody](astrophysics.md#blackbody), integrate [Planck's law](statistical-physics.md#planck-s-law) over [frequency](wave.md#frequency) as well: $M=M_e=j^*=\sigma T^4$ by the [Stefan–Boltzmann law](heat.md#stefan-boltzmann-law). An ideal $6000\,\mathrm K$ emitting patch of [area](differential-geometry.md#surface-area) $1\,\mathrm{mm^2}$ emits about $73.4881\,\mathrm W$ outward. [Irradiance](#irradiance) counts incoming radiation separately; for purely emitted output the net outward exchange per [area](differential-geometry.md#surface-area) is $M-E$. Reflected output must also be included if the surface reflects incident radiation.

## Irradiance

↑ **Parent:** [Radiometry](radiometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Irradiance)

[Irradiance](#irradiance) measures incident [radiant flux](#radiant-flux) per actual receiving [area](differential-geometry.md#surface-area). Its units $\mathrm{W\,m^{-2}}$ match [radiant exitance](#radiant-exitance), but it counts the incoming side of the radiation exchange. Measure incoming [angles](geometry-and-topology.md#angle) from the [unit normal](differential-geometry.md#unit-normal) pointing toward the incident hemisphere. Then

$$
E=\int_{\Omega_{\rm incident}}L_{\rm incoming}(\theta,\varphi)\cos\theta\,d\Omega.
$$

For $2\,\mathrm W$ distributed uniformly over $0.010\,\mathrm{m^2}$, $E=200\,\mathrm{W\,m^{-2}}$. If the receiving plane is tilted $60^\circ$ in the same broad uniform parallel beam, the incident [power](energy.md#power) per actual [area](differential-geometry.md#surface-area) is halved to $100\,\mathrm{W\,m^{-2}}$. This receiving-surface [cosine](geometry-and-topology.md#cosine) factor is geometric and does not assume [Lambertian reflectance](optics.md#lambertian-reflectance). Together, [irradiance](#irradiance) and [radiant exitance](#radiant-exitance) describe how radiation supplies and removes [energy](energy.md) at a surface, while [radiance](#radiance) preserves the directional information.

### Horizontal versus beam-normal solar irradiance

↑ **Parent:** [Irradiance](#irradiance)

A parallel beam incident at elevation $\alpha$ has horizontal irradiance $F_h=F_\perp\sin\alpha$. Its path optical depth in a plane-parallel atmosphere is $\tau_v/\sin\alpha$. Confusing these projections changes both attenuation and intercepted power.

## Radiometric absorptance

↑ **Parent:** [Radiometry](radiometry.md)

[Radiometric absorptance](#radiometric-absorptance) is the fraction of incident [radiant flux](#radiant-flux) converted to [heat](heat.md) in the specified receiver: $P_{\rm abs}=aP_{\rm in}$, with $0\leq a\leq1$ for a passive receiver. Specify the entrance boundary, [wavelength](wave-equation.md#wavelength), incidence [angle](geometry-and-topology.md#angle) and receiver [temperature](temperature.md). Radiation reflected or transmitted out of that receiver is not absorbed [power](energy.md#power). A cavity can improve [radiometric absorptance](#radiometric-absorptance) by giving [light](optics.md#light) repeated opportunities for [wave absorption](wave.md#wave-absorption); a dark coating alone does not establish $a=1$.

For broadband [light](optics.md#light), [spectral radiant flux](#spectral-radiant-flux) matters: $P_{\rm abs}=\int a(\lambda)\Phi_{e,\lambda}(\lambda)\,d\lambda$. A single effective [radiometric absorptance](#radiometric-absorptance) therefore depends on the incident [optical spectrum](optics.md#optical-spectrum) as well as on the receiver. If the stated incident boundary lies before a window of known power transmission $\tau_w$, the receiver absorbs $a\tau_wP_{\rm before}$ when other optical losses are absent. Window loss and receiver [radiometric absorptance](#radiometric-absorptance) are separate corrections.

## Electrical substitution radiometer

↑ **Parent:** [Radiometry](radiometry.md)

An [electrical substitution radiometer](#electrical-substitution-radiometer) measures [radiant flux](#radiant-flux) by replacing absorbed optical [power](energy.md#power) with calibrated [Joule heating](electric-charge.md#joule-heating). At fixed [temperature](temperature.md), [feedback control](control-theory.md#closed-loop-control) holds the receiver equally warm with the beam blocked or admitted: after corrections, absorbed optical [power](energy.md#power) equals the reduction in supplied electrical heating. Incident [radiant flux](#radiant-flux) additionally requires [radiometric absorptance](#radiometric-absorptance) and entrance-path corrections. This connects [radiometry](radiometry.md) to electrical standards.[§5.2, printed p. 30: electrical substitution and electrical standards](physics-bibliography.md#spectroradiometric-detector-measurements-ultraviolet-visible-and-near-infrared-detectors-for-spectral-power-by-thomas-c-larason-and-others)

Picture a small absorbing cavity connected to a colder reference block by a [radiometer thermal link](#radiometer-thermal-link). A heater supplies [Joule heating](electric-charge.md#joule-heating), a [thermometer](temperature.md#thermometer) senses the receiver, and [feedback control](control-theory.md#closed-loop-control) adjusts the heater. When [light](optics.md#light) supplies some of the heating, the controller supplies less. The readout is the change in heater [power](energy.md#power), rather than the beam's brightness or its number of [photons](quantum-mechanics.md#photon). NIST's institutional description gives a concrete receiver with a conical interior, absorbing coating and weak Kapton support, operated with a receiver heater and [thermometer](temperature.md#thermometer).[Description, Design Parameters for Improved ACR Sensitivity; Key Design Features: conical receiver, coating, constant-temperature loop and thin-walled Kapton link](physics-bibliography.md#pico-watt-acr-by-national-institute-of-standards-and-technology)

<a id="electrical-substitution-radiometer-cavity-control"></a>
![](electrical-substitution-radiometer-cavity-control.png)

**[Figure 7](#electrical-substitution-radiometer-cavity-control). Cavity, radiometer thermal link and heater readout in an electrical substitution radiometer**. Original functional schematic, not a drawing of a particular laboratory instrument. The shutter defines dark and illuminated states; incident [radiant flux](#radiant-flux) is specified at the receiver entrance. The cavity absorbs a fraction $a$, while the remainder escapes. The reference block and receiver have distinct controlled [temperatures](temperature.md). The [thermometer](temperature.md#thermometer) signal drives [feedback control](control-theory.md#closed-loop-control), and heater voltage and [electric current](electric-charge.md#electric-current) provide the electrical [power](energy.md#power) readout. Lead heating, stray radiation and spatial heating differences require separate checks.

### Electrical substitution heat balance

↑ **Parent:** [Electrical substitution radiometer](#electrical-substitution-radiometer)

An explicit lumped model makes the cancellation understandable. Treat the receiver as having uniform [temperature](temperature.md) $T$, [heat capacity](heat.md#heat-capacity) $C$, heater [power](energy.md#power) $P_h$ deposited in the receiver, net parasitic input $P_{\rm par}$, and outward [heat transfer](heat.md#heat-transfer) $Q_{\rm out}(T,T_b)$ to a reference at [temperature](temperature.md) $T_b$. With incident [radiant flux](#radiant-flux) $P_{\rm in}$ and [radiometric absorptance](#radiometric-absorptance) $a$, [conservation of energy](mathematical-physics.md#conservation-of-energy) gives

$$
C\frac{dT}{dt}=P_h+aP_{\rm in}+P_{\rm par}-Q_{\rm out}(T,T_b).
$$

The dark state has no admitted beam. Compare settled dark and light states, denoted $d$ and $l$; each has $dT/dt=0$. Subtracting their balances gives

$$
P_{\rm abs}=aP_{\rm in}=\Delta P_h+\Delta Q_{\rm out}-\Delta P_{\rm par},\qquad
\Delta P_h=P_{h,d}-P_{h,l},
$$

where $\Delta Q_{\rm out}=Q_{{\rm out},l}-Q_{{\rm out},d}$ and $\Delta P_{\rm par}=P_{{\rm par},l}-P_{{\rm par},d}$. At identical $T$ and $T_b$, with unchanged surroundings and parasitic heating, both correction differences vanish. Thus $P_{\rm abs}=\Delta P_h$, and $P_{\rm in}=\Delta P_h/a$. Notice the signs: extra stray [thermal radiation](electromagnetic-radiation.md#thermal-radiation) admitted with the beam also reduces heater [power](energy.md#power), so it must be subtracted from that reduction before attributing the result to the intended beam.

Measure the heater's own terminal voltage $V_h$ and [electric current](electric-charge.md#electric-current) $I_h$: for steady electrical heating, $P_h=V_hI_h=I_h^2R_h$, where $R_h$ is its [electrical resistance](electric-charge.md#electrical-resistance). A supply voltage that includes wire voltage drops counts [Joule heating](electric-charge.md#joule-heating) in the leads too; only the portion deposited in the receiver belongs in this balance. Changes in that deposited lead [heat](heat.md) belong in $\Delta P_{\rm par}$. [Optical-electrical heating non-equivalence](#optical-electrical-heating-non-equivalence) adds a further instrument-specific correction when the uniform-[temperature](temperature.md) model is insufficient.[§5.2, printed p. 30: heater wires, window transmission and optical/electrical non-equivalence](physics-bibliography.md#spectroradiometric-detector-measurements-ultraviolet-visible-and-near-infrared-detectors-for-spectral-power-by-thomas-c-larason-and-others)

#### Radiometer thermal link

↑ **Parent:** [Electrical substitution heat balance](#electrical-substitution-heat-balance)

A [radiometer thermal link](#radiometer-thermal-link) is the intentional path for [thermal conduction](heat.md#thermal-conduction) from receiver to reference block. Near a chosen operating point, write $Q_{\rm link}\simeq G(T-T_b)$ with local conductance $G$ in $\mathrm{W\,K^{-1}}$. A weaker link increases the steady [temperature](temperature.md) rise per added [power](energy.md#power), $\delta T\simeq\delta P/G$, but also increases the uncontrolled relaxation [time](classical-mechanics.md#time-in-physics) $\tau=C/G$ when the link dominates other [heat transfer](heat.md#heat-transfer). These are local linear approximations: actual [thermal conductivity](heat.md#thermal-conductivity) depends on [temperature](temperature.md), and active [feedback control](control-theory.md#closed-loop-control) introduces its own response. NIST explicitly describes the tradeoff between weaker links and smaller receiver [heat capacity](heat.md#heat-capacity).[Key Design Features, final paragraph: response time proportional to receiver heat capacity and inverse thermal conductance](physics-bibliography.md#pico-watt-acr-by-national-institute-of-standards-and-technology)

#### Fixed-temperature electrical substitution example

↑ **Parent:** [Electrical substitution heat balance](#electrical-substitution-heat-balance)

Stipulate a model receiver held at $T=5.4\,\mathrm K$ with a reference at $T_b=5.0\,\mathrm K$. Choose $G=5\,\mathrm{mW\,K^{-1}}$, so outward [thermal conduction](heat.md#thermal-conduction) is $G(T-T_b)=2\,\mathrm{mW}$. Ignore other [heat transfer](heat.md#heat-transfer), take $P_{\rm par}=0$ in both states, and stipulate perfect optical/electrical thermal equivalence. These values specify an original example; they are not measurements or claimed performance of a NIST instrument.

With the beam blocked, supply $P_{h,d}=2\,\mathrm{mW}$. With [light](optics.md#light) admitted, the required heater [power](energy.md#power) is $P_{h,l}=1.005\,\mathrm{mW}$. For stipulated [radiometric absorptance](#radiometric-absorptance) $a=0.995$ at the chosen single [wavelength](wave-equation.md#wavelength),

$$
P_{\rm abs}=2-1.005=0.995\,\mathrm{mW},\qquad
P_{\rm in}=\frac{0.995\,\mathrm{mW}}{0.995}=1.000\,\mathrm{mW}.
$$

The illuminated receiver still gets $1.005+0.995=2\,\mathrm{mW}$ of heating. The remaining $0.005\,\mathrm{mW}$ of incident [radiant flux](#radiant-flux) escapes without heating it. Calling the measured heater reduction “incident [power](energy.md#power)” would underestimate the stipulated incident [radiant flux](#radiant-flux) by $0.5\%$.

<a id="electrical-substitution-dark-light-heater-balance"></a>
![](electrical-substitution-dark-light-heater-balance.png)

**[Figure 8](#electrical-substitution-dark-light-heater-balance). The same receiver temperature with different electrical and optical heating**. Original stipulated steady-state example, not experimental data. Both columns total $2\,\mathrm{mW}$ of deposited heating and balance the same outward [thermal conduction](heat.md#thermal-conduction). Incident [radiant flux](#radiant-flux) is $1\,\mathrm{mW}$, of which $0.995\,\mathrm{mW}$ is absorbed; the $0.005\,\mathrm{mW}$ that escapes is outside the heating column. No response time or measured uncertainty is implied.

Two variations expose different pitfalls. First, if admitting the beam also adds $0.010\,\mathrm{mW}$ of stray heating while the same $0.995\,\mathrm{mW}$ is absorbed from the intended beam, the heater falls to $0.995\,\mathrm{mW}$. The apparent reduction is now $1.005\,\mathrm{mW}$; subtracting $\Delta P_{\rm par}=0.010\,\mathrm{mW}$ recovers the beam's absorbed [power](energy.md#power). Second, keep the original heater readings but stipulate a light-state receiver offset $\delta T=+1\,\mathrm{mK}$ at fixed reference [temperature](temperature.md). The link carries an extra $G\delta T=0.005\,\mathrm{mW}$; the inferred absorbed [power](energy.md#power) becomes $1.000\,\mathrm{mW}$, and incident [radiant flux](#radiant-flux) becomes $1.000/0.995\simeq1.005025\,\mathrm{mW}$. This second variation deliberately violates exact fixed-[temperature](temperature.md) substitution.

The heater can supply only nonnegative [power](energy.md#power) in this model. Consequently an absorbed beam above the available dark heater [power](energy.md#power) cannot be compensated at the chosen setpoint merely by reducing the heater. The operating point, link, or admitted [radiant flux](#radiant-flux) must change; zero heater demand is a range boundary, not evidence of greater [radiant flux](#radiant-flux) sensitivity.

### Optical-electrical heating non-equivalence

↑ **Parent:** [Electrical substitution radiometer](#electrical-substitution-radiometer)

[Optical-electrical heating non-equivalence](#optical-electrical-heating-non-equivalence) means that equal absorbed optical and electrical [powers](energy.md#power) do not necessarily give identical [thermometer](temperature.md#thermometer) responses. [Light](optics.md#light) and the heater may deposit [heat](heat.md) in different places, producing different [temperature gradients](heat.md#temperature-gradient) and different routes of [thermal conduction](heat.md#thermal-conduction) to the support. Holding one [thermometer](temperature.md#thermometer) reading fixed need not hold every part of the cavity at the same [temperature](temperature.md). This differs from incomplete [radiometric absorptance](#radiometric-absorptance): one concerns where absorbed [heat](heat.md) goes, the other how much incident [light](optics.md#light) becomes absorbed [heat](heat.md).

A useful accounting convention is

$$
P_{\rm in}=\frac{\Delta P_h+\Delta Q_{\rm out}-\Delta P_{\rm par}+\delta_{\rm ne}}{a},
$$

where the signed correction $\delta_{\rm ne}$ is determined by characterization of the instrument and represents the residual departure from the lumped [electrical substitution heat balance](#electrical-substitution-heat-balance). It is not a universal extra source of [energy](energy.md). Varying the beam location or heater location, comparing equivalent temperature excursions, and checking repeatable dark returns can test the assumptions; no single small correction proves that every other correction vanishes.

### Cryogenic radiometer

↑ **Parent:** [Electrical substitution radiometer](#electrical-substitution-radiometer)

A [cryogenic radiometer](#cryogenic-radiometer) uses low-[temperature](temperature.md) operation to improve [electrical substitution radiometry](#electrical-substitution-radiometer) through particular material and thermal properties. Lower [heat capacity](heat.md#heat-capacity) of a copper receiver permits a substantial cavity without proportionately slow relaxation; cold shields reduce unwanted [thermal radiation](electromagnetic-radiation.md#thermal-radiation), and heater leads with [superconductivity](superconductivity.md) can suppress resistive lead heating. These features do not make [radiometric absorptance](#radiometric-absorptance) exactly one or abolish [optical-electrical heating non-equivalence](#optical-electrical-heating-non-equivalence).[§5.2, printed pp. 30–32: cryogenic advantages and remaining window/non-equivalence corrections](physics-bibliography.md#spectroradiometric-detector-measurements-ultraviolet-visible-and-near-infrared-detectors-for-spectral-power-by-thomas-c-larason-and-others)

Cold surroundings matter as much as a cold receiver. In a simplified gray-surface model, net outward [thermal radiation](electromagnetic-radiation.md#thermal-radiation) is $\epsilon\sigma A(T^4-T_s^4)$, using [emissivity](heat.md#emissivity) $\epsilon$, [area](differential-geometry.md#surface-area) $A$, shield [temperature](temperature.md) $T_s$ and the [Stefan-Boltzmann constant](heat.md#stefan-boltzmann-constant) $\sigma$. Cold shields reduce the incoming term as well as the receiver's emission; cooling the receiver alone while leaving it exposed to warm surroundings does not remove incoming radiation. An entrance window still provides an optical and thermal path. [Vacuum](physics.md#vacuum) reduces gas-mediated [heat transfer](heat.md#heat-transfer), while an intentional [radiometer thermal link](#radiometer-thermal-link) remains necessary. This model explains specific losses, rather than promising a universal improvement factor or perfect accuracy.

#### Cryogenic laser-power substitution experiment

↑ **Parent:** [Cryogenic radiometer](#cryogenic-radiometer)

In NIST's 2001 comparison, the Laser-Optimized Cryogenic Radiometer held its cavity near $5.4\,\mathrm K$ and controlled the heat sink separately. Opening the beam reduced heater [power](energy.md#power) at fixed cavity [temperature](temperature.md); an AC bridge read the [temperature](temperature.md). Tests used stabilized, spatially filtered [lasers](laser.md) at $488$, $514$ and $633\,\mathrm{nm}$, with horizontal input and a movable [photodiode](optical-instrument.md#photodiode) transfer detector in the cavity's optical plane. The paper contrasts this with the High Accuracy Cryogenic Radiometer's optical heating followed by two electrical heating cycles and interpolation.[§§2–3, printed pp. 642–643: apparatus, wavelengths, readout and the two substitution protocols](physics-bibliography.md#comparison-of-two-cryogenic-radiometers-at-nist-by-jeanne-m-houston-and-others)

The two laboratories compared calibrations of the same transfer detectors, and checked their spatial response. Alignment differences and transported dust limited that comparison; its agreement did not prove universal equivalence. Its correction tables retain window transmission, cavity [radiometric absorptance](#radiometric-absorptance), alignment, electrical readout and [optical-electrical heating non-equivalence](#optical-electrical-heating-non-equivalence). The heat sink was controlled, but §3 does not specify its numerical setpoint: the $5.0\,\mathrm K$ reference in the preceding example is stipulated.[§§3–5, printed pp. 643–646, especially Tables 2–3 and spatial-uniformity checks](physics-bibliography.md#comparison-of-two-cryogenic-radiometers-at-nist-by-jeanne-m-houston-and-others)

For a reproducible substitution measurement, record the beam's [wavelength](wave-equation.md#wavelength) and entrance boundary, receiver and reference [temperatures](temperature.md), heater terminal voltage and [electric current](electric-charge.md#electric-current), dark readings before and after illumination, and the settling rule. Check beam collection at the [aperture](optics.md#aperture), window transmission, [radiometric absorptance](#radiometric-absorptance), deposited lead heating, and sensitivity to beam position. Repeatability alone misses a stable correction error. [Photometric calibration](optics.md#photometric-calibration) can subsequently use this [radiant flux](#radiant-flux) scale, but [photometry](optics.md#photometry-optics) still needs the appropriate spectral visual weighting; the cold receiver does not itself measure [luminous flux](optics.md#luminous-flux).

## Transmittance

↑ **Parent:** [Radiometry](radiometry.md)

[Transmittance](#transmittance) is the fraction of incident [radiant flux](#radiant-flux) transmitted through a specified object or boundary. Specify [wavelength](wave-equation.md#wavelength), [angle of incidence](optics.md#angle-of-incidence), [electromagnetic polarization](electromagnetic-wave.md#polarization-of-an-electromagnetic-wave) and which outgoing [light](optics.md#light) is collected.

## ↑ Ancestors (4)

1. [Optics](optics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Electrical substitution radiometer](#electrical-substitution-radiometer)
- [Photometry (optics)](optics.md#photometry-optics)
- [Radiometry](radiometry.md)
- [Spectral radiance](#spectral-radiance)
