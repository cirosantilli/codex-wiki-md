<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The **[normality assumption](../../../../normality-assumption.md) concerns the model's error distribution, not necessarily the pooled raw observations**. In an independent-groups [analysis of variance](../../../../analysis-of-variance.md), errors around each group [mean](../../../../expected-value-split.md) are modeled as following a [normal distribution](../../../../normal-distribution.md); combining groups with genuinely different [means](../../../../expected-value-split.md) can produce a nonnormal pooled distribution even when this assumption holds. In a [paired t-test](../../../../paired-t-test.md), the relevant distribution is that of within-pair differences. [Linear regression](../../../../linear-regression-split.md) conventionally assumes normal errors conditional on the predictors for exact small-sample [Student t-tests](../../../../student-s-t-test.md) and [F-tests](../../../../f-test.md).[Handbook Section 7.4.3.2, fixed-effects errors](../../../../the-one-way-anova-model-and-assumptions-by-national-institute-of-standards-and-technology.md)

Inspect suitable within-group or fitted-model [regression residuals](../../../../regression-residual.md) using a [quantile-quantile plot](../../../../q-q-plot.md) and examine outliers and asymmetry. A formal normality test is not a decisive automatic gatekeeper: with small samples it may miss important departures, while large samples can detect minor departures. Approximate robustness depends on the [sample size](../../../../sample-size.md), balance, tail behavior and intended inference. The [central limit theorem](../../../../central-limit-theorem.md) concerns sampling distributions and does not make every raw observation normal or repair dependence. Depending on the question, a justified transformation, a better-fitting probability model, robust inference or an appropriate [bootstrap](../../../../bootstrapping-statistics.md) may be preferable. The [normality assumption](../../../../normality-assumption.md), independence and equal [variance](../../../../variance-split.md) are distinct assumptions.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Section A](../../section-a.md)
4. [2022](../../../2022-split.md)
5. [Past exam of the experimental design and methods course of the year 2 of the psychology (experimental) course of the University of Oxford](../../../split.md)
6. [Experimental design and methods course of the year 2 of the psychology (experimental) course of the University of Oxford](../../../../experimental-design-and-methods-course-of-the-year-2-of-the-psychology-experimental-course-of-the-university-of-oxford.md)
7. [Year 2 of the psychology (experimental) course of the University of Oxford](../../../../year-2-of-the-psychology-experimental-course-of-the-university-of-oxford.md)
8. [Psychology (experimental) course of the University of Oxford](../../../../psychology-experimental-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../university-of-oxford-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
