<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Use a [longitudinal study](../../../../../../longitudinal-study.md) with repeated measurements of the same individuals.** Recruit people across several starting ages and measure the same ear, with a standardized anatomical definition and instrument, at baseline and subsequent visits over several years. Repeat measurements at each visit to estimate [measurement error](../../../../../../measurement-error.md); where practical, conceal previous measurements from the observer. Record sex, body size, birth cohort and observer, and document reasons for loss to follow-up.

A simple [random-intercept linear mixed model](../../../../../../random-intercept-linear-mixed-model.md) for ear length $Y_{ij}$ at elapsed follow-up time $t_{ij}$ is

$$
Y_{ij}=\alpha_i+\beta t_{ij}+\gamma^Tz_{ij}+\varepsilon_{ij}.
$$

The individual intercept $\alpha_i$ absorbs persistent differences between people. Alternatively, differences $Y_{ij}-Y_{i0}$ remove that intercept directly. Estimate the within-person [regression coefficient](../../../../../../regression-coefficient.md) $\beta$ and its [confidence interval](../../../../../../confidence-interval.md), accounting for the [correlation](../../../../../../pearson-correlation-coefficient.md) of repeated measurements. Compare it with the cross-sectional slope rather than treating the two slopes as automatically identical.

This [longitudinal study](../../../../../../longitudinal-study.md) directly checks whether an individual's ears tend to lengthen as time passes. Several entry-age cohorts help assess whether the change varies with starting age. Calendar-period changes and selective dropout can still affect interpretation, so repeated observation alone does not eliminate every possible source of [confounding](../../../../../../confounding.md) or [selection bias](../../../../../../selection-bias.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
