<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [charge-coupled device](../../../../../charge-coupled-device.md) converts incident optical [photons](../../../../../photon.md) into collected [electrons](../../../../../electron.md) in pixel potential wells. Exposure accumulates charge; clocked transfers move it to readout amplifiers. Quantum efficiency, gain, read noise, dark current, saturation and charge-transfer behavior determine the usable signal. Bias or overscan estimates remove electronic offsets, dark frames characterize dark signal where needed, and flat fields correct relative response and illumination. Multiple exposures help identify cosmic rays and defective pixels, while astrometric alignment permits stacking.

For [aperture photometry](../../../../../aperture-photometry.md), sum the source aperture and subtract an estimated local sky contribution. A point-spread-function fit can instead use the expected spatial shape, particularly in crowded fields. Detector gain converts recorded units to [electrons](../../../../../electron.md) before applying a Poisson noise calculation. Let the aperture contain $n$ pixels, total expected source charge $S$, sky charge $B$ per pixel, dark charge $D$ per pixel and rms read noise $r$ per pixel. With a perfectly known background mean,

$$
\mathrm{Var}(\widehat S)\simeq S+n(B+D+r^2).
$$

If the background is estimated from $M$ independent comparable blank pixels, its subtraction adds approximately $n^2(B+D+r^2)/M$, giving

$$
\boxed{\mathrm{SNR}\simeq\frac{S}{\sqrt{S+n(B+D+r^2)+n^2(B+D+r^2)/M}}.}
$$

The extra term is uncertainty in the estimated mean; it does not replace the sky shot noise already present in the source aperture. A more exact budget propagates the actual bias, dark and flat calibrations and any pixel correlations. The existing [aperture photometry with an estimated background](../../../../../aperture-photometry-with-an-estimated-background.md) derives this distinction.

For one exposure in the photon-limited regime, signal grows as $t$ and its counting noise as $\sqrt t$, so SNR grows as $\sqrt t$. Read-noise domination can favor longer individual exposures, but full-well saturation, cosmic rays, tracking and changing sky constrain them. Extraction uses an aperture correction or a calibrated PSF model to recover light outside the measured region. Flat-field errors, nonlinearity, imperfect sky gradients, blending and atmospheric transparency can dominate bright-source accuracy even when the formal [photon](../../../../../photon.md) error is tiny.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
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
