# Radiometry

↑ **Parent:** [Optics](optics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiometry)

[Radiometry](radiometry-split.md) measures the [energy](energy-split.md) and [power](power.md) carried by [electromagnetic radiation](electromagnetic-radiation-split.md), including [light](light.md). It asks how much radiation a source supplies, where it travels, and how much reaches a receiving surface. The measurements are physical rather than weighted by the sensitivity of the human eye: equal [radiant fluxes](radiant-flux.md) at different [wavelengths](wavelength.md) need not look equally bright. [Yoshihiro Ohno, Radiometry and Photometry: Review for Vision Optics, 2000](https://www.nist.gov/publications/radiometry-and-photometry-review-vision-optics).

The five quantities below answer different questions about the same radiation. The [International System of Units](international-system-of-units.md) makes the distinctions visible: a watt is a joule per second, while a steradian measures [solid angle](solid-angle.md). [NIST Guide to the SI, Chapter 4: derived units](https://www.nist.gov/pml/special-publication-811/nist-guide-si-chapter-4-two-classes-si-units-and-si-prefixes).

| Quantity | What is resolved? | Units |
| --- | --- | --- |
| [Radiant flux](radiant-flux.md) $\Phi$ | Total radiation [power](power.md) in the specified beam or collection | $\mathrm W$ |
| [Radiant intensity](radiant-intensity.md) $I$ | [Power](power.md) per outgoing [solid angle](solid-angle.md) | $\mathrm{W\,sr^{-1}}$ |
| [Radiance](radiance.md) $L$ | [Power](power.md) per [projected area](projected-area.md) and per [solid angle](solid-angle.md) | $\mathrm{W\,m^{-2}\,sr^{-1}}$ |
| [Irradiance](irradiance.md) $E$ | Incident [power](power.md) per receiving [area](surface-area.md) | $\mathrm{W\,m^{-2}}$ |
| [Radiant exitance](radiant-exitance.md) $M$ | Outward emitted [power](power.md) per emitting [area](surface-area.md) | $\mathrm{W\,m^{-2}}$ |

Resolving [wavelength](wavelength.md) or [frequency](frequency.md) adds a further “per unit interval”, as in [spectral radiance](spectral-radiance.md). The notation is consistent with NIST's table of spectral quantities. In particular, [radiant flux](radiant-flux.md) is [power](power.md), whereas the existing astronomical [radiative flux](radiative-flux.md) is [power](power.md) per [area](surface-area.md). [NISTIR 6657, A Rational Methodology for Estimating the Luminous Flux Based upon Color Primaries from Digital Projection Displays, 2009, Table 1](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=901354).

This bookkeeping makes an [optical camera](optical-camera.md)'s collected signal calculable from a source's [radiance](radiance.md) and the geometry of the receiving aperture. It also lets radiation measurements from different instruments be compared. For example, NIST describes separate calibrations of [spectral radiance](spectral-radiance.md) and spectral [irradiance](irradiance.md) for instruments used to observe Earth. [Johnson, Brown and Rice, Metrology for remote sensing radiometry, §§3.4.1–3.4.2](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=104550).

**Table of contents**

- [Ocean optics](ocean-optics.md)
  - [Photic zone](photic-zone.md)
    - [Euphotic zone](euphotic-zone.md)
      - [Euphotic depth](euphotic-depth.md)
  - [Ocean colour](ocean-colour.md)
    - [Diffuse attenuation coefficient](diffuse-attenuation-coefficient.md)
    - [Chlorophyll retrieval](chlorophyll-retrieval.md)
    - [Backscattering coefficient](backscattering-coefficient.md)
    - [Remote-sensing reflectance](remote-sensing-reflectance.md)
    - [Non-algal particle](non-algal-particle.md)
    - [Coloured dissolved organic matter](coloured-dissolved-organic-matter.md)
- [Solar irradiance](solar-irradiance.md)
- [Remote sensing](remote-sensing.md)
  - [Lidar](lidar.md)
    - [Airborne lidar](airborne-lidar.md)
  - [Photogrammetry](photogrammetry.md)
    - [Ground control point](ground-control-point.md)
    - [Structure-from-motion photogrammetry](structure-from-motion-photogrammetry.md)
    - [Stereo photogrammetry](stereo-photogrammetry.md)
  - [Hyperspectral imaging](hyperspectral-imaging.md)
  - [Atmospheric correction](atmospheric-correction.md)
  - [GOES](goes.md)
  - [Meteosat](meteosat.md)
  - [Sentinel-1](sentinel-1.md)
  - [Sentinel-2](sentinel-2.md)
  - [Landsat](landsat.md)
  - [Multispectral imaging](multispectral-imaging.md)
    - [Band ratio image](band-ratio-image.md)
    - [Normalized difference vegetation index](normalized-difference-vegetation-index.md)
    - [False-colour composite](false-colour-composite.md)
    - [Red edge](red-edge.md)
  - [Interferometric synthetic-aperture radar](interferometric-synthetic-aperture-radar.md)
    - [Radar interferogram](radar-interferogram.md)
    - [Interferometric coherence](interferometric-coherence.md)
    - [Line-of-sight displacement](line-of-sight-displacement.md)
    - [Interferometric phase](interferometric-phase.md)
- [Optical haze](optical-haze.md)
- [Actinic flux](actinic-flux.md)
- [Fluence](fluence.md)
  - [Photon energy fluence](photon-energy-fluence.md)
  - [Photon fluence](photon-fluence.md)
- [Radiometer](radiometer.md)
  - [Radiometer two-point calibration](radiometer-two-point-calibration.md)
  - [Noise temperature](noise-temperature.md)
    - [System noise temperature](system-noise-temperature.md)
    - [Receiver noise temperature](receiver-noise-temperature.md)
  - [Two-load radiometer calibration](two-load-radiometer-calibration.md)
- [Reflectance](reflectance.md)
  - [Bidirectional reflectance distribution function](bidirectional-reflectance-distribution-function.md)
  - [Spectral reflectance](spectral-reflectance.md)
- [Absorption (electromagnetic radiation)](absorption-electromagnetic-radiation.md)
- [Radiant flux](radiant-flux.md)
  - [Radiant flux through an oriented surface](radiant-flux-through-an-oriented-surface.md)
  - [Beam collection at fixed radiant flux](beam-collection-at-fixed-radiant-flux.md)
  - [Spectral radiant flux](spectral-radiant-flux.md)
  - [Calibrated radiant-flux measurement](calibrated-radiant-flux-measurement.md)
- [Radiant intensity](radiant-intensity.md)
  - [Point emitter](point-emitter.md)
- [Radiance](radiance.md)
  - [Projected area](projected-area.md)
  - [Spectral radiance](spectral-radiance.md)
    - [Frequency and wavelength spectral radiance conversion](frequency-and-wavelength-spectral-radiance-conversion.md)
    - [Vacuum conservation of specific intensity](vacuum-conservation-of-specific-intensity.md)
    - [Limb darkening](limb-darkening.md)
      - [Linear limb-darkening law](linear-limb-darkening-law.md)
        - [Limb-darkening coefficient](limb-darkening-coefficient.md)
      - [Limb-darkened disk flux](limb-darkened-disk-flux.md)
      - [Small-planet transit weighting](small-planet-transit-weighting.md)
      - [Solar limb-darkening drift-scan experiment](solar-limb-darkening-drift-scan-experiment.md)
- [Radiant exitance](radiant-exitance.md)
  - [Spectral radiant exitance](spectral-radiant-exitance.md)
- [Irradiance](irradiance.md)
  - [Spectral irradiance](spectral-irradiance.md)
  - [Horizontal versus beam-normal solar irradiance](horizontal-versus-beam-normal-solar-irradiance.md)
- [Radiometric absorptance](radiometric-absorptance.md)
- [Electrical substitution radiometer](electrical-substitution-radiometer.md)
  - [Electrical substitution heat balance](electrical-substitution-heat-balance.md)
    - [Radiometer thermal link](radiometer-thermal-link.md)
    - [Fixed-temperature electrical substitution example](fixed-temperature-electrical-substitution-example.md)
  - [Optical-electrical heating non-equivalence](optical-electrical-heating-non-equivalence.md)
  - [Cryogenic radiometer](cryogenic-radiometer.md)
    - [Cryogenic laser-power substitution experiment](cryogenic-laser-power-substitution-experiment.md)
- [Transmittance](transmittance.md)

## ↑ Ancestors (4)

1. [Optics](optics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Electrical substitution radiometer](electrical-substitution-radiometer.md)
- [Photometry (optics)](photometry-optics.md)
- [Radiometry](radiometry-split.md)
- [Spectral radiance](spectral-radiance.md)
