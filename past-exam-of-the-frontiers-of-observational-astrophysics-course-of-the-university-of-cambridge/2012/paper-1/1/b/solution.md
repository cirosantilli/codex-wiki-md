<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the projected baseline along the source offset, $b_p$, and $\alpha=10'=2.909\times10^{-3}\,\mathrm{rad}$. The first [bandwidth](../../../../../bandwidth-signal-processing.md) null occurs at $\Delta\nu=c/(b_p\alpha)$. A worst-case $b_p=25.46\,\mathrm m$ gives $4.05\,\mathrm{GHz}$. **That is a zero of the response, not a good usable [bandwidth](../../../../../bandwidth-signal-processing.md).** A quantitative maximum needs an allowed attenuation.

For example, requiring a response of at least $0.9$ gives $\operatorname{sinc}x=0.9$ at $x\simeq0.787$. Hence

$$
\boxed{\Delta\nu_{10\%}\simeq0.250\frac c{b_p\alpha}\simeq1.01\,\mathrm{GHz}}
$$

for that worst projection. A strictly east-west offset in a sides-aligned square instead samples at most $18\,\mathrm m$, giving a $5.73\,\mathrm{GHz}$ first null and a $1.43\,\mathrm{GHz}$ ten-percent-loss [bandwidth](../../../../../bandwidth-signal-processing.md). The original two-antenna geometry supplies an additional $\cos\theta$ projection; these examples use its maximum magnitude. Thus **a [bandwidth](../../../../../bandwidth-signal-processing.md) of order $1\,\mathrm{GHz}$** is a reasonable conservative estimate with a stated small-loss criterion, rather than a unique geometry-free limit.

<a id="1/b/image-array-baselines-and-bandwidth-decorrelation-away-from-the-tracking-center"></a>
![](../../../../../past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2012/paper-1-array-and-bandwidth.png)

**[Figure 2](#1/b/image-array-baselines-and-bandwidth-decorrelation-away-from-the-tracking-center). Array baselines and bandwidth decorrelation away from the tracking center**. Original array geometry and rectangular-band sinc calculations for a ten-arcminute offset. The marked ten-percent-loss bandwidth is an illustrative response criterion; the first null is not a usable-bandwidth recommendation.

To use a much wider total band, channelize the signals before correlation or before irreversible [frequency](../../../../../frequency.md) averaging. Correlate sufficiently narrow channels, track the reference delay and phase at each [frequency](../../../../../frequency.md), and combine frequency-aware visibilities or images. This preserves sensitivity while avoiding [field-dependent averaging losses in radio interferometry](../../../../../field-dependent-averaging-losses-in-radio-interferometry.md). Merely adding a phase correction after a broad channel has decorrelated cannot recover the lost signal; nor can one tracking delay cancel every sky direction simultaneously.[VLA Observational Status Summary 2018A, bandwidth and time-averaging limitations](../../../../../field-of-view-by-national-radio-astronomy-observatory.md)

## ↑ Ancestors (14)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
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
