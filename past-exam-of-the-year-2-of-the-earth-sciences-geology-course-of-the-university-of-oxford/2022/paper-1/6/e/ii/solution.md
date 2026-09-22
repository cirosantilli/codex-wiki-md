<h1 id="6/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At each source position, couple the vibrator to the ground, transmit a known [frequency](../../../../../../frequency.md) sweep $s(t)$ and record the ground response on synchronized [geophones](../../../../../../geophone.md). Record a pilot or measured source-force reference and sufficient listening time for delayed arrivals. Repeat sweeps where beneficial and retain geometry and timing information.

If the Earth’s impulse response is $h(t)$, a linear model is $d=s*h+n$. [Vibroseis correlation](../../../../../../vibroseis-correlation.md) cross-correlates the record with the known sweep:

$$
c(\tau)=\int d(t)s(t-\tau)\,dt=(h*R_{ss})(\tau)+R_{ns}(\tau).
$$

The sweep’s [autocorrelation](../../../../../../autocorrelation.md) $R_{ss}$ is a compact, approximately zero-phase wavelet, so the long chirp is compressed into identifiable delayed events. In the [frequency](../../../../../../frequency.md) domain this multiplies $D(\omega)$ by $\overline{S(\omega)}$, yielding $H(\omega)|S(\omega)|^2$ plus noise. It is **pulse compression, not an exact recovery of $h$ at [frequencies](../../../../../../frequency.md) never transmitted**. Spectral shaping or stabilized deconvolution can further compensate the finite source bandwidth and sidelobes.[Vibratory sources: known input sweep correlated with geophone records](../../../../../../geophysical-survey-summary-report-section-3-geophysical-testing-methodology.md)

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [6](../../../6.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../split.md)
7. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Earth sciences (geology) course of the University of Oxford](../../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
