<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Measure counts in electrons so that [photon](../../../../../photon.md) and detector [noise](../../../../../noise-signal-processing.md) can be combined directly. For source electrons $S$, $n$ aperture pixels, total time $t$, sky rate $b$ per pixel, dark-current rate $d$ per pixel, $M$ reads with rms [read noise](../../../../../read-noise.md) $r$ per pixel, and an independently estimated mean background per pixel of [variance](../../../../../variance-split.md) $\sigma_{\widehat B}^2$, an ideal aperture-sum budget is

$$
\boxed{\operatorname{Var}(\widehat S)
\simeq S+n(b+d)t+nMr^2+n^2\sigma_{\widehat B}^2
+\sigma_{\rm cal}^2,\qquad
{\rm SNR}=\frac{S}{\sqrt{\operatorname{Var}(\widehat S)}}.}
$$

The last term represents the propagated [calibration](../../../../../calibration-differential-geometry.md) uncertainty if it can be treated as a random [variance](../../../../../variance-split.md); systematic residuals can instead bias the measurement and need an explicit error model. For a background estimated from $n_b$ independent, equally exposed sky pixels, one approximation is $\sigma_{\widehat B}^2=[(b+d)t+Mr^2]/n_b$. Correlated resampling, detector cross-talk or a spatially structured sky invalidates the independent-pixel simplification.

**[Photon](../../../../../photon.md) counting and sky.** Source [photon shot noise](../../../../../photon-shot-noise.md) has [variance](../../../../../variance-split.md) $S$ and cannot be calibrated away. Longer integration or greater throughput improves its fractional error as $S^{-1/2}$. Sky [photons](../../../../../photon.md), including moonlight, airglow and scattered light, add their own Poisson fluctuations. A dark site, appropriate observing time and filter, good baffling and a smaller or optimally weighted source aperture reduce sky contributions. Better [seeing](../../../../../astronomical-seeing.md) or [adaptive optics](../../../../../adaptive-optics.md) can concentrate a point source into fewer noise-bearing pixels. Sky subtraction removes the mean background but not the random sky [photons](../../../../../photon.md) already recorded, and the sky estimate adds uncertainty of its own.

**Dark and [read noise](../../../../../read-noise.md).** Thermal [dark current](../../../../../dark-current-physics.md) contributes a mean and shot [noise](../../../../../noise-signal-processing.md). Cooling reduces its rate; well-matched dark frames remove a reproducible mean and map hot pixels, but do not undo the science exposure's random dark-current fluctuations. Each read adds electronic [noise](../../../../../noise-signal-processing.md). At fixed total integration, many short exposures add more read [variance](../../../../../variance-split.md) than fewer long exposures, so use exposures long enough to become sky limited when saturation, [cosmic rays](../../../../../cosmic-ray.md) and temporal changes permit. Multiple non-destructive reads can help on detectors that support them. Subtracting a bias frame corrects an electronic offset, not the stochastic [read noise](../../../../../read-noise.md).

**[Calibration](../../../../../calibration-differential-geometry.md) and non-Poisson effects.** Pixel sensitivity differences, illumination gradients, fringes, nonlinearity, imperfect charge transfer and electronic pattern [noise](../../../../../noise-signal-processing.md) leave [calibration](../../../../../calibration-differential-geometry.md) errors. High-count flat fields, stable operating conditions, linearity [calibration](../../../../../calibration-differential-geometry.md), dithering and appropriate detector models help, while the finite signal-to-noise of [calibration](../../../../../calibration-differential-geometry.md) frames propagates into the result. Cosmic-ray hits, hot pixels, satellite trails and scattered-light artefacts are not ordinary stationary Gaussian [noise](../../../../../noise-signal-processing.md): identify or mask them, often using several exposures. Overaggressive clipping can remove real transient or compact-source signal.

[Atmospheric scintillation](../../../../../scintillation-astronomy.md) adds correlated intensity fluctuations, especially in short bright-star measurements; [seeing](../../../../../astronomical-seeing.md) changes and guiding errors move [flux](../../../../../flux.md) between pixels or apertures. Differential photometry using appropriate reference [stars](../../../../../star.md) and stable apertures reduces common variations but does not guarantee removal of chromatic or position-dependent effects. For a constant flux-limited source in independent stationary [noise](../../../../../noise-signal-processing.md) the final signal-to-noise usually grows as $\sqrt t$ once background limited; a systematic floor or correlated sky can stop that improvement. Distinguish improvement of [calibration](../../../../../calibration-differential-geometry.md), which removes reproducible bias, from elimination of intrinsically random [photon](../../../../../photon.md) arrivals, which is impossible.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the frontiers of Observational Astrophysics course of the University of Cambridge](../../../../split.md)
6. [Frontiers of Observational Astrophysics course of the University of Cambridge](../../../../../frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
