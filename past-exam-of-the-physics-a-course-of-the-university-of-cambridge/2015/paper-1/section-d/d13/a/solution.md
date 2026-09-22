<h1 id="section-d/d13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [systematic error](../../../../../../systematic-error.md) is a reproducible displacement caused by the apparatus, procedure or measurement model. Repeating the same experiment can determine its mean very precisely while retaining that displacement. Reducing random [measurement error](../../../../../../measurement-error.md) therefore does not establish accuracy.

Start with a measurement model listing the response, zero offset, [calibration](../../../../../../calibration-differential-geometry.md) scale and relevant environmental corrections. Compare the instrument with traceable standards at several points across its working range; a single zero check cannot reveal a gain error or nonlinearity. Measure blanks and backgrounds using the same acquisition chain as the signal. Repeat [calibration](../../../../../../calibration-differential-geometry.md) before and after the run to detect drift, and retain the uncertainty of every applied correction.

[systematic-error cancellation by reversal](../../../../../../systematic-error-cancellation-by-reversal.md) separates a wanted effect from an offset with a different symmetry. For example, a resistance measurement with thermoelectric offset $V_0$ gives $V_+=RI+V_0$ and $V_-=-RI+V_0$. The difference gives

$$
\boxed{R=\frac{V_+-V_-}{2I}},
$$

cancelling a stable offset, while $(V_++V_-)/2$ diagnoses it. Alternate the current direction quickly enough that the offset is approximately unchanged. This does not cancel a current-scale [calibration](../../../../../../calibration-differential-geometry.md) error or resistance changes from [Joule heating](../../../../../../joule-heating.md); vary the current magnitude and monitor temperature to test those effects. Control measurements must target the actual proposed bias.

Randomizing the order of settings prevents slow drift from consistently imitating a physical trend. Interleaving a reference measurement helps track that drift. Reversing geometry, exchanging matched detectors and changing alignment can expose effects tied to one part of the apparatus. Repeating the measurement with an independent method is particularly valuable when its dominant biases differ; agreement between two instruments sharing the same [calibration](../../../../../../calibration-differential-geometry.md) does not test a common [calibration](../../../../../../calibration-differential-geometry.md) error.

Apply justified corrections, propagate their uncertainties and include [correlations](../../../../../../pearson-correlation-coefficient.md) when the same [calibration](../../../../../../calibration-differential-geometry.md) enters several observations. A systematic component shared by all observations does not shrink as $1/\sqrt N$. A [measurement uncertainty budget](../../../../../../measurement-uncertainty-budget.md) should distinguish the physical origin of each effect from the method used to evaluate its uncertainty: statistical Type A and other Type B evaluations do not simply mean random and systematic, respectively.[sections 2–5 and Appendix D.1.1.6: systematic error and correction](../../../../../../guidelines-for-evaluating-and-expressing-the-uncertainty-of-nist-measurement-results-by-barry-n-taylor-and-chris-e-kuyatt.md)

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2015](../../../../split.md)
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
