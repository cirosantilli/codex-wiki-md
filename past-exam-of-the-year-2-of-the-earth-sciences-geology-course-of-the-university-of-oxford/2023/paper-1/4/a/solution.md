<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use repeat-pass [interferometric synthetic-aperture radar](../../../../../interferometric-synthetic-aperture-radar.md). An orbiting radar transmits coherent microwave pulses and records the amplitude and phase of the returning field. Form an [interferogram](../../../../../interferogram.md) from registered complex images acquired before and after the [earthquake](../../../../../earthquake.md), remove the orbital contribution and the topographic phase predicted by a [digital elevation model](../../../../../digital-elevation-model.md), and correct atmospheric and other long-wavelength phase delays. Where [interferometric coherence](../../../../../interferometric-coherence.md) is adequate, unwrap the residual phase to estimate [line-of-sight displacement](../../../../../line-of-sight-displacement.md):

$$
\Delta d_{\rm LOS}=-\frac{\lambda}{4\pi}\Delta\phi,
$$

with sign set by the instrument's displacement convention. Each $2\pi$ phase cycle represents $\lambda/2$ of range change.

This maps a distributed [earthquake](../../../../../earthquake.md) displacement field day or night and through cloud, including areas inaccessible on foot. Roughly $10$–$30\ \mathrm m$ ground sampling and a scene spanning many kilometres on both sides of the [fault](../../../../../geological-fault.md) can resolve regional deformation; a narrow surface break benefits from finer pixels or complementary sub-metre optical surveys. Sensitivity to displacement can be millimetres to centimetres in coherent areas, but that does not equal [spatial resolution](../../../../../spatial-resolution.md). A single viewing direction measures one component; ascending and descending tracks and [GNSS](../../../../../gnss.md) constrain more components. At the rupture itself, large gradients and changed ground cover can destroy [interferometric coherence](../../../../../interferometric-coherence.md); radar pixel-offset tracking or before/after optical correlation can then recover metre-scale [fault offsets](../../../../../fault-offset.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
