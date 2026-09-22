# Transmission electron microscopy specimen dose and calibration

↑ **Parent:** [Transmission electron microscopy](transmission-electron-microscopy.md)

JEOL's minimum-dose method focuses and corrects [astigmatism](astigmatism-optical-systems.md) away from the recording position before exposing it, reducing irradiation of the chosen field.[Definition: adjustments away from the photographed position](minimum-dose-system-mds-by-jeol.md) A downstream [objective aperture](objective-aperture.md) cannot undo irradiation that has already reached the specimen: rejecting more outgoing [electrons](electron.md) does not itself reduce specimen exposure.

For an original dose budget, define $D$ as incident [electron](electron.md) count per specimen area, rather than absorbed [energy](energy-split.md) per [mass](mass.md). A uniform beam of [electric current](electric-current.md) magnitude $I$, illuminating area $A$ for time $T$, gives

$$
N=\frac{IT}{e},\qquad D=\frac{IT}{eA},
$$

where $e$ is the [elementary charge](elementary-charge.md). Choosing $I=1\,\mathrm{pA}$, $T=1\,\mathrm{s}$ and $A=1\,\mathrm{\mu m^2}$ gives approximately $6.24\times10^6$ incident [electrons](electron.md), or $6.24\,\mathrm{electrons\,nm^{-2}}$. This is an invented exposure calculation, not a safe-dose recommendation. Focusing and searching exposures must also enter the accumulated budget.

If detected counts follow a [Poisson distribution](poisson-distribution.md), a mean count $\mu$ has [standard deviation](standard-deviation.md) $\sqrt{\mu}$. Ignoring background, $100$ accepted counts therefore have $10\%$ relative counting uncertainty, while $25$ have $20\%$. Reducing accepted counts can reveal useful [diffraction contrast](diffraction-contrast.md) while increasing counting uncertainty. It is useful to specify both contrast and count budget when discussing [electron microscope resolution](electron-microscope-resolution.md).

A proposed [measurement calibration](measurement-calibration.md) sequence records a beam-blocked detector background, an illuminated empty support region, and a specimen image with fixed [voltage](voltage.md), exposure and detector gain. Test detector linearity with exposure time before comparing corrected intensities. Calibrate the image scale against a known spacing, as in [microscope scale calibration](microscope-scale-calibration.md), and independently calibrate [electron diffraction](electron-diffraction.md) spacing at its own lens settings; one calibration does not supply the other. Register compared regions, record [objective aperture](objective-aperture.md) selection, specimen tilt and accumulated exposure, then repeat the first setting to test drift and irradiation changes. These are proposed controls, not undocumented steps attributed to JEOL's [silicon](silicon.md) example.

## ↑ Ancestors (8)

1. [Transmission electron microscopy](transmission-electron-microscopy.md)
2. [Electron microscopy](electron-microscopy.md)
3. [Electron microscope](electron-microscope.md)
4. [Electron optics](electron-optics.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
