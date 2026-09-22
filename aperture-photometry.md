# Aperture photometry

↑ **Parent:** [Light curve](light-curve.md)

[Aperture photometry](aperture-photometry.md) estimates brightness by summing calibrated detector pixels in an extraction region and subtracting the estimated background in that region. For $n$ equally weighted pixels, let $S$ be their total accumulated signal in [electrons](electron.md), $b$ the estimated background [electrons](electron.md) per pixel over the same exposure, and $\Delta t$ the exposure duration. Then $\widehat r=(S-nb)/\Delta t$ is a background-subtracted electron rate. Kepler applied [aperture photometry](aperture-photometry.md) to calibrated pixels with a fitted sky background. [Jenkins et al. (2010), photometric analysis, section 3](https://arxiv.org/pdf/1001.0258).

This measurement trades source collection against background: enlarging the extraction region can retain more starlight but includes more [sky brightness](sky-brightness.md) and neighbouring sources. [Photon shot noise](photon-shot-noise.md), [read noise](read-noise.md), and uncertainty in [background subtraction](background-subtraction.md) contribute to its uncertainty. Dividing $\widehat r$ by a consistently measured reference rate gives a dimensionless [light curve](light-curve.md); it does not supply an absolute [observed radiative flux](observed-radiative-flux.md). If contaminating light remains, the reference includes it and the inferred [exoplanet transit depth](exoplanet-transit-depth.md) suffers [transit dilution](transit-dilution.md).

In the first toy figure, the source's reference rate is $100{,}000$ electrons per second, the summed sky contribution is $4{,}000$ electrons per second, and a known multiplicative response is $g(t)=1+0.0003t$ with $t$ in hours from mid-transit. The artificial [exoplanet transit depth](exoplanet-transit-depth.md) is $0.010$, its total duration four hours, and its flat-bottom duration $2.8$ hours; the straight ingress and egress are a toy approximation, not an exact [exoplanet transit photometry](exoplanet-transit-photometry.md) model. Each synthetic sample averages a $0.5$-hour exposure and adds seeded [normal distribution](normal-distribution.md) noise with relative [standard deviation](standard-deviation.md) $0.0006$. Subtracting the known sky rate and dividing by the known response and reference rate recovers the dip. Real observations require estimating those corrections and carrying their uncertainty.

## ↑ Ancestors (5)

1. [Light curve](light-curve.md)
2. [Astrophysics](astrophysics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Aperture photometry](aperture-photometry.md)
- [Light curve](light-curve.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2013/paper-1/3/c/solution.md)
