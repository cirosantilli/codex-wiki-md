<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The [number needed to treat](../../../../../../number-needed-to-treat.md) is the reciprocal of the absolute reduction in the 12-week adverse-outcome risk. Using the counts rather than rounding the percentages first gives

$$
\widehat\Delta=\frac{78}{316}-\frac{40}{297}\simeq0.11216,
\qquad\boxed{\mathrm{NNT}=\frac1{\widehat\Delta}\simeq8.92,\ \text{reported as }9.}
$$

This means about nine high-risk women would need to be offered the intervention to prevent one additional screen-defined case over that follow-up, under the trial's comparison. It is not a lifetime quantity or automatically an estimate for clinical-interview diagnoses. Calculating from the rounded difference $25\%-14\%$ gives approximately nine but need not give the same integer rounding; the exact counts explain the reported value.

For a [confidence interval](../../../../../../confidence-interval.md), first construct an interval for the difference between the two [independent](../../../../../../independent-random-variables.md) event proportions, allowing for [binomial distribution](../../../../../../binomial-distribution.md) sampling uncertainty. If both risk-reduction endpoints are positive, take their reciprocals and reverse their order to obtain an NNT interval. A [bootstrap](../../../../../../bootstrapping-statistics.md) can instead resample women within their [randomized controlled trial](../../../../../../randomized-controlled-trial.md) arms and transform the resulting risk-difference distribution. If the difference interval includes zero, the NNT confidence set extends through infinity and can include harm as well as benefit; it is not an ordinary bounded interval. The raw-outcome interval also relies on the missing-outcome assumptions discussed above.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
