# Photometric calibration

↑ **Parent:** [Photometer](photometer.md)

[NIST Measurement Services: Photometric Calibrations by Yuqin Zong and others](nist-measurement-services-photometric-calibrations-by-yuqin-zong-and-others.md) describes a concrete experiment (§§3.2–3.3.2): a [silicon](silicon.md) [photodiode](photodiode.md), multilayer [photometric matching filter](photometric-matching-filter.md), precision aperture, [temperature](temperature-split.md) sensor and current-to-voltage converter. A [monochromator](monochromator.md) supplies a small beam; scanning [wavelength](wavelength.md) yields [spectral responsivity](spectral-responsivity.md), and scanning position checks response across the aperture. Finite spectral bandwidth requires correction. The average aperture response converts uniform illumination to [illuminance](illuminance.md).

On the photometric bench (§§3.4.1, 3.5.3, 3.5.6), align lamp and aperture reference planes, set the lamp's [electric current](electric-current.md), stabilize, and compare a check lamp with standard [photometers](photometer.md). The readout is a [voltmeter](voltmeter.md) signal. Subtract the shutter-closed reading (§3.4.4), divide by converter gain to infer [electric current](electric-current.md), and use calibrated [illuminance](illuminance.md) responsivity $S_A$ to obtain $E_v=i/S_A$. For a distant source, [luminous intensity](luminous-intensity.md) follows from $I_v=E_vd^2$, with $d$ between reference planes.

Controls include repeat lamp operations, distance changes to test the [inverse-square law](inverse-square-law.md), [temperature](temperature-split.md) corrections and gain [linearity](linearity.md) checks. [Spectral mismatch correction](spectral-mismatch-correction.md) is source dependent (§3.4.3). Unknown [optical spectra](optical-spectrum.md), spatial nonuniformity and incorrect reference planes remain limitations.[§§3.2–3.5.6, printed pp. 16–19, 22–28, 33–37: apparatus, dark subtraction, readout, corrections and check-lamp procedure](nist-measurement-services-photometric-calibrations-by-yuqin-zong-and-others.md)

**Table of contents**

- [Spectral mismatch correction](spectral-mismatch-correction.md)
  - [Calibrated photometer model](calibrated-photometer-model.md)

## ↑ Ancestors (6)

1. [Photometer](photometer.md)
2. [Photometry (optics)](photometry-optics.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Cryogenic laser-power substitution experiment](cryogenic-laser-power-substitution-experiment.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1/2/d/solution.md)
- [Solution](past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2012/paper-1/3/b/solution.md)
- [Photometric matching filter](photometric-matching-filter.md)
