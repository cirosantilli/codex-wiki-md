# Aperture photometry with an estimated background

↑ **Parent:** [CCD noise budget](ccd-noise-budget.md)

For total source electrons $S$, $n$ aperture pixels, sky-plus-dark rate $b+d$, time $t$, $M$ reads with rms $r$, and an independent mean-background estimate of [variance](variance-split.md) $\sigma_{\widehat B}^2$ per pixel, the aperture [variance](variance-split.md) is $S+n(b+d)t+nMr^2+n^2\sigma_{\widehat B}^2$ before additional [calibration](calibration-differential-geometry.md) terms. The last factor is $n^2$ because one uncertain background mean is subtracted from all aperture pixels. Pixel correlations require [covariance](covariance.md) terms.

## ↑ Ancestors (8)

1. [CCD noise budget](ccd-noise-budget.md)
2. [Charge-coupled device](charge-coupled-device.md)
3. [Photodetector](photodetector.md)
4. [Optical instrument](optical-instrument-split.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2013/paper-1/3/c/solution.md)
