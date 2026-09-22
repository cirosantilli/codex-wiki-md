<h1 id="section-d/d13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [systematic error](../../../../../../systematic-error.md) shifts results in a reproducible or correlated way relative to the [measurand](../../../../../../measurand.md). Examples include zero offsets, gain miscalibration, nonlinearity, drift, geometrical misalignment, loading, background contamination and an inadequate response model. Repeated measurements under unchanged conditions can reduce independent [noise](../../../../../../noise-signal-processing.md) without exposing such a shift; a small [standard error](../../../../../../standard-error.md) is not proof of [measurement accuracy](../../../../../../measurement-accuracy.md).

Use traceable standards and independent measurement methods, test zero and span, reverse the physical [signal](../../../../../../signal.md) where possible, and vary the conditions that could cause the bias. For [common-offset cancellation by signal reversal](../../../../../../common-offset-cancellation-by-signal-reversal.md), take measurements $y_+=S+b$ and $y_-=-S+b$. The half-difference estimates $S$ while the half-sum diagnoses an unchanged offset $b$. Drift between the two readings would violate that cancellation, so alternate or interleave measurements. Randomizing acquisition order separates slow drift from controlled parameter changes; blanks and [calibration](../../../../../../calibration-differential-geometry.md) samples test backgrounds and instrument gain. Blinding helps reduce analysis choices that follow an expected answer.

Corrections have uncertainties and may be correlated across data. Include residual offsets and gains as [nuisance parameters](../../../../../../nuisance-parameter.md) or propagate their [calibration](../../../../../../calibration-differential-geometry.md) [covariance](../../../../../../covariance.md), rather than treating a common [calibration](../../../../../../calibration-differential-geometry.md) error as fresh independent [noise](../../../../../../noise-signal-processing.md) for each datum. Document assumptions and check stability with controlled perturbations. These methods suppress or quantify specified systematic effects; they cannot guarantee elimination of every unknown bias.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
