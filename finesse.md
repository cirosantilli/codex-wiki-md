# Finesse

↑ **Parent:** [Fabry–Pérot interferometer](fabry-perot-interferometer.md)

The [finesse](finesse.md) of a [Fabry–Pérot interferometer](fabry-perot-interferometer.md) is its [free spectral range](free-spectral-range.md) divided by a transmission peak's [full width at half maximum](full-width-at-half-maximum.md). Large [finesse](finesse.md) means a narrow accepted [frequency](frequency.md) interval compared with the spacing between repeated orders. Here half maximum means $T=1/2$ of the ideal unit peak, with zero detector background subtracted; it does not mean halfway between the transmission minimum and maximum.

Write $A=4R/(1-R)^2$ for the coefficient multiplying $\sin^2(\delta/2)$ in [Fabry–Pérot transmission from multiple reflections](fabry-perot-transmission-from-multiple-reflections.md). This coefficient is sometimes called the coefficient of finesse; it is not the [finesse](finesse.md) $\mathcal F$. About a resonance $\delta=2\pi m$, put $\epsilon=\delta-2\pi m$. Solving $T=1/2$ gives

$$
\sin^2(\epsilon/2)=\frac1A,\qquad
\Delta\delta_{\rm FWHM}=4\arcsin\!\left(\frac{1-R}{2\sqrt R}\right),
$$

and, since one [free spectral range](free-spectral-range.md) advances the [wave phase](phase-waves.md) by $2\pi$,

$$
\frac{\Delta\nu_{\rm FWHM}}{\Delta\nu_{\rm FSR}}
=\frac2\pi\arcsin\!\left(\frac{1-R}{2\sqrt R}\right),\qquad
\mathcal F=\frac{\pi}{2\arcsin[(1-R)/(2\sqrt R)]}.
$$

These are exact for the ideal nondispersive model with constant $R$ and linear [frequency](frequency.md) dependence of $\delta$. The [inverse sine](inverse-sine.md) requires $(1-R)/(2\sqrt R)\leq1$, or $R\geq3-2\sqrt2\simeq0.171573$. At equality, neighbouring peaks merely touch half maximum at their shared minima: the nominal width is one full [free spectral range](free-spectral-range.md) and $\mathcal F=1$. Isolated half-maximum peaks require the strict inequality. Below this threshold the transmission never falls to $1/2$, so this peak-width definition supplies no [finesse](finesse.md); at $R=0$ the transmission is flat.

For large reflectivity, the [small-angle approximation](small-angle-approximation.md) $\arcsin x\simeq x$ gives

$$
\mathcal F\simeq\frac{\pi\sqrt R}{1-R},\qquad
\frac{\Delta\nu_{\rm FWHM}}{\Delta\nu_{\rm FSR}}\simeq\frac{1-R}{\pi\sqrt R}.
$$

This is a high-reflectivity approximation, not an identity for every $R$. The original dimensionless examples below have exact [full width at half maximum](full-width-at-half-maximum.md) values obtained from the [inverse sine](inverse-sine.md) formula.

| Mirror intensity reflectivity $R$ | Exact $\Delta\nu_{\rm FWHM}/\Delta\nu_{\rm FSR}$ | Exact [finesse](finesse.md) | Approximate [finesse](finesse.md) $\pi\sqrt R/(1-R)$ |
| --- | --- | --- | --- |
| $0.25$ | $0.53989$ | $1.85222$ | $2.09440$ |
| $0.75$ | $0.09221$ | $10.84478$ | $10.88280$ |
| $0.95$ | $0.01633$ | $61.23420$ | $61.24092$ |

<a id="image-increasing-mirror-reflectivity-narrows-fabry-perot-interferometer-transmission-peaks"></a>
![](fabry-perot-normalized-transmission-peaks.png)

**[Figure 3](#image-increasing-mirror-reflectivity-narrows-fabry-perot-interferometer-transmission-peaks). Increasing mirror reflectivity narrows Fabry–Pérot interferometer transmission peaks**. Original stipulated dimensionless model for $R=0.25,0.75,0.95$, with $x=(\nu-\nu_m)/\Delta\nu_{\rm FSR}$ and $\delta=2\pi x$ modulo $2\pi$. All curves peak at unity and repeat after $\Delta x=1$. The second panel enlarges the central resonance; coloured segments at $T=1/2$ mark each exact [full width at half maximum](full-width-at-half-maximum.md). The inset compares exact [finesse](finesse.md) with the high-reflectivity approximation. These are calculations, not measured scans.

The beauty of the narrowing is visible directly in the [geometric series](geometric-series.md): large $R$ preserves contributions from many round trips, so a small [phase difference](phase-difference.md) accumulates across many terms and spoils their addition. For the stipulated $10\,\mathrm{mm}$ vacuum gap, $R=0.95$ gives an ideal [full width at half maximum](full-width-at-half-maximum.md) of about $244.792\,\mathrm{MHz}$. This instrumental width is not a measured [spectral line](spectral-line.md) width. A real scan also depends on the source profile, accepted [angles](angle.md), mirror shape, alignment, and scan stability. The University of Washington handout separately discusses mirror-reflectivity, mirror-flatness, and detector-pinhole contributions; increasing $R$ alone cannot remove the others.[Finesse discussion, equations (5)–(8), and §2.3 Determine the Finesse](fabry-perot-interferometer-university-of-washington-physics-331.md)

**Table of contents**

- [Etalon resolving power and order overlap](etalon-resolving-power-and-order-overlap.md)

## ↑ Ancestors (6)

1. [Fabry–Pérot interferometer](fabry-perot-interferometer.md)
2. [Optical instrument](optical-instrument-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Fabry–Pérot interferometer](fabry-perot-interferometer.md)
- [Finesse](finesse.md)
- [Order-safe angular scanning of a Fabry–Pérot spectrum](order-safe-angular-scanning-of-a-fabry-perot-spectrum.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2011/paper-1/section-b/b9/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2012/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2/section-d/d13/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2/section-b/b9/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2/section-b/b6/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2/section-b/b6/d/solution.md)
- [Scanning Fabry–Pérot measurement](scanning-fabry-perot-measurement.md)
