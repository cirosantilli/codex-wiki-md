# Calibrated radiant-flux measurement

↑ **Parent:** [Radiant flux](radiant-flux.md)

An [optical power meter](optical-power-meter.md) makes the definition operational: collect a specified beam on a calibrated [photodiode](photodiode.md), measure its [electric current](electric-current.md), and infer incident [radiant flux](radiant-flux.md) using [spectral responsivity](spectral-responsivity.md). In the manufacturer-authored [Model 1830-R Series Optical Power Meters User's Manual by Newport Corporation](model-1830-r-series-optical-power-meters-user-s-manual-by-newport-corporation.md), §5.5.1 specifies a concrete sequence: connect the detector and its calibration module, select watt mode and the source [wavelength](wavelength.md), block the beam and press ZERO, then unblock it and read the display. The stored background includes [dark current](dark-current-physics.md) and ambient [light](light.md) present during zeroing. For narrowband radiation,

$$
\Phi_{\rm indicated}=\frac{i_{\rm illuminated}-i_{\rm zero}}{R(\lambda)}.
$$

The [electric current](electric-current.md) difference divided by [spectral responsivity](spectral-responsivity.md) has units $\mathrm A/(\mathrm{A\,W^{-1}})=\mathrm W$. For a stipulated $R=0.40\,\mathrm{A\,W^{-1}}$ and difference $0.20\,\mathrm{mA}$, the inferred [radiant flux](radiant-flux.md) is $0.50\,\mathrm{mW}$; these numbers illustrate the inference and are not reported measurements. The entire beam must hit the active [area](surface-area.md), and §5.6 calls for correct [wavelength](wavelength.md), background subtraction, and operation below detector saturation. If an [optical attenuator](optical-attenuator.md) is fitted, §5.4 requires the calibrated detector–attenuator pair and the matching meter setting.

The calibration itself must connect [electric current](electric-current.md) to independently known incident [power](power.md). NIST's [Spectroradiometric Detector Measurements: Ultraviolet, Visible, and Near-Infrared Detectors for Spectral Power by Thomas C. Larason and others](spectroradiometric-detector-measurements-ultraviolet-visible-and-near-infrared-detectors-for-spectral-power-by-thomas-c-larason-and-others.md) describes this chain. A [cryogenic radiometer](cryogenic-radiometer.md), an [electrical substitution radiometer](electrical-substitution-radiometer.md), compares [temperature](temperature.md) changes from absorbed [light](light.md) with those from known [Joule heating](joule-heating.md) (§5.2). Transfer and working detectors carry that [watt](watt.md) scale to a spectral comparator (§5.1). A source, [monochromator](monochromator.md), focusing optics, shutter, [beam splitter](beam-splitter.md), and monitor [photodiode](photodiode.md) illuminate a standard and test detector in turn; calibrated current-to-voltage electronics and voltmeters provide the readout (§§3.2.2–3.2.4, 4.3.1). At each [wavelength](wavelength.md), subtract blocked-beam signals and normalize each detector signal by the simultaneously sampled monitor signal. Comparison with the standard yields the test detector's [spectral responsivity](spectral-responsivity.md). NIST uses two working standards and alignment normal to the beam (§6.1.1).

Controls distinguish a smaller collected [radiant flux](radiant-flux.md) from a faulty conversion: block and unblock the beam to check the baseline; check that its footprint fits the active [area](surface-area.md); verify the calibrated [optical attenuator](optical-attenuator.md) configuration; and test proportional response within the specified operating range. Source drift faster than monitor sampling is not removed. NIST discusses finite spectral bandwidth, stray [light](light.md), [temperature](temperature.md), and spatial response variations (§§3.1.1, 6.2, 7.2). A broadband [optical spectrum](optical-spectrum.md) requires the weighted [integral](integral.md) in [spectral radiant flux](spectral-radiant-flux.md), rather than dividing by an arbitrary single [spectral responsivity](spectral-responsivity.md). These limitations explain why the meter's displayed [watts](watt.md) need a stated collection boundary, spectral assumptions, and calibration conditions.

## ↑ Ancestors (6)

1. [Radiant flux](radiant-flux.md)
2. [Radiometry](radiometry.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Monochromator](monochromator.md)
- [Optical power meter](optical-power-meter.md)
