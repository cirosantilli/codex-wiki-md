# Photopic luminous efficiency function

↑ **Parent:** [Photometry (optics)](photometry-optics.md)

The [photopic luminous efficiency function](photopic-luminous-efficiency-function.md) $V(\lambda)$ is dimensionless and describes standardized relative sensitivity for [photopic vision](photopic-vision.md). It is normalized to $V(555\,\mathrm{nm})=1$ and tabulated over $360$–$830\,\mathrm{nm}$. The [wavelength](wavelength.md) coordinate is in standard air, rather than [vacuum](vacuum.md); changing coordinates requires converting the [spectral radiant flux](spectral-radiant-flux.md) density as well. The official prescription uses linear [interpolation](interpolation.md) between the specified 1 nm entries.[§3.1, printed pp. 2–3: wavelength convention, normalized functions and interpolation](the-international-system-of-units-si-ninth-edition-si-brochure/mise-en-pratique-for-the-definition-of-the-candela-and-associated-derived-units-for-photometric-and-radiometric-quantities-in-the-si.md)

Write $\lambda_a$ for the standard-air [wavelength](wavelength.md) at $540\,\mathrm{THz}$. With [spectral radiant flux](spectral-radiant-flux.md) $\Phi_{e,\lambda}$ in $\mathrm{W\,nm^{-1}}$ and $d\lambda$ in nanometres, the [luminous flux](luminous-flux.md) is

$$
\Phi_v=K_m\int_{360\,\mathrm{nm}}^{830\,\mathrm{nm}}V(\lambda)\Phi_{e,\lambda}(\lambda)\,d\lambda,
\qquad K_m=\frac{K_{\mathrm{cd}}}{V(\lambda_a)},\qquad K_{\mathrm{cd}}=683\,\mathrm{lm\,W^{-1}}.
$$

The [integral](integral.md) has units of [watts](watt.md), and $K_m$ converts them to [lumens](lumen-unit.md). For radiation at a single [wavelength](wavelength.md) $\lambda_0$ with total [radiant flux](radiant-flux.md) $P$, this reduces to $\Phi_v=K_mV(\lambda_0)P$. For a sufficiently narrow finite band, this is an approximation requiring nearly constant $V$ across the band.[§3.1, equation (2), printed p. 3: spectral weighting normalized at the defining frequency](the-international-system-of-units-si-ninth-edition-si-brochure/mise-en-pratique-for-the-definition-of-the-candela-and-associated-derived-units-for-photometric-and-radiometric-quantities-in-the-si.md)

## ↑ Ancestors (5)

1. [Photometry (optics)](photometry-optics.md)
2. [Optics](optics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Equal radiant power under visual weighting](equal-radiant-power-under-visual-weighting.md)
- [Photometer](photometer.md)
- [Photometric matching filter](photometric-matching-filter.md)
- [Photopic luminous efficiency function](photopic-luminous-efficiency-function.md)
- [Photopic vision](photopic-vision.md)
- [Spectral luminous efficacy](spectral-luminous-efficacy.md)
