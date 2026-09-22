<h1 id="section-a/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A small constant input can repeatedly produce the same [analogue-to-digital converter](../../../../../analog-to-digital-converter.md) code, so averaging those codes cannot reveal its position within a conversion interval. [dither](../../../../../dither.md) makes adjacent codes toggle; their relative [frequencies](../../../../../frequency.md) then encode changes smaller than one conversion step. With adequate [oversampling](../../../../../oversampling.md), low-pass filtering and averaging reduce the added, sufficiently uncorrelated [noise](../../../../../noise-signal-processing.md) while retaining the slow [signal](../../../../../signal.md).

For independent sample errors, the averaged [standard deviation](../../../../../standard-deviation.md) scales as $N^{-1/2}$; ideally four times as many samples gain about one effective bit. For example a constant input $0.2\Delta$ rounded to levels separated by $\Delta$ would always return zero. Adding uniform [dither](../../../../../dither.md) on $[-\Delta/2,\Delta/2]$ gives output $\Delta$ with [probability](../../../../../probability.md) $0.2$ and zero otherwise: the expected average is $0.2\Delta$, with error $0.4\Delta/\sqrt N$. The benefit concerns the filtered estimate, not a more accurate individual conversion. Excessive [dither](../../../../../dither.md) wastes range, and averaging does not correct calibration bias, correlated drift or arbitrary converter nonlinearity.[Oversampling and Averaging, especially the dither and uncorrelated-noise discussion; Table 1](../../../../../an-1549-performance-optimization-of-the-integrated-adc-on-the-aducm4050-by-analog-devices.md)

## ↑ Ancestors (14)

1. [5](../5.md)
2. [Section A](../../section-a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
