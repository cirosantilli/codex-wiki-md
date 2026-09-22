# Spectral mismatch correction

↑ **Parent:** [Photometric calibration](photometric-calibration.md)

For collected [spectral radiant flux](spectral-radiant-flux.md) $f(\lambda)$ and a linear [photodiode](photodiode.md) with [spectral responsivity](spectral-responsivity.md) $r(\lambda)$, the dark-subtracted [electric current](electric-current.md) is $i=\int r f\,d\lambda$. A reference [optical spectrum](optical-spectrum.md) $f_A$ sets the conversion $C_A$ from [electric current](electric-current.md) to collected [luminous flux](luminous-flux.md). Applying it to another [optical spectrum](optical-spectrum.md) $f_T$ gives

$$
C_A=\frac{K_m\int V f_A\,d\lambda}{\int r f_A\,d\lambda},\qquad
\Phi_{v,\mathrm{indicated}}=C_A\int r f_T\,d\lambda,
\qquad
F=\frac{\int V f_T\,d\lambda}{\int r f_T\,d\lambda}
\frac{\int r f_A\,d\lambda}{\int V f_A\,d\lambda}.
$$

Assume nonzero calibration and test signals. Then $F\Phi_{v,\mathrm{indicated}}$ is the corrected [luminous flux](luminous-flux.md). Multiplying either [optical spectrum](optical-spectrum.md) by an overall positive scale leaves $F$ unchanged. If $r$ is proportional to $V$, $F=1$ for every [optical spectrum](optical-spectrum.md). Uniformly overfilled aperture measurements use [wavelength](wavelength.md)-resolved [irradiance](irradiance.md) instead, multiplying the [electric current](electric-current.md) expression by aperture [area](surface-area.md); the same ratio cancellation gives the [illuminance](illuminance.md) correction. This is the algebra behind source-dependent calibration, rather than a new measured correction curve. [Realization of the candela](realization-of-the-candela.md)

**Table of contents**

- [Calibrated photometer model](calibrated-photometer-model.md)

## ↑ Ancestors (7)

1. [Photometric calibration](photometric-calibration.md)
2. [Photometer](photometer.md)
3. [Photometry (optics)](photometry-optics.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Calibrated photometer model](calibrated-photometer-model.md)
- [Photometric calibration](photometric-calibration.md)
