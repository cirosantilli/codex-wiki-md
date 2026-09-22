<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [cumulative-response logistic model](../../../../../../../cumulative-response-logistic-model.md) uses $C_{it}=\sum_{s<t}Y_{is}$ instead of the two individual lag predictors. It and the two-lag [history-dependent logistic regression](../../../../../../../conditional-logistic-model-for-longitudinal-binary-data.md) are nonnested: the entire accumulated history generally cannot be represented using only the two recent outcomes. Their [binomial deviance](../../../../../../../binomial-deviance.md) difference therefore has no ordinary nested [chi-squared distribution](../../../../../../../chi-squared-distribution.md) calibration.

Use the [Akaike information criterion](../../../../../../../akaike-information-criterion.md), which up to the same saturated-model constant equals $D+2k$ for these [Bernoulli distribution](../../../../../../../bernoulli-distribution.md) conditional [likelihoods](../../../../../../../likelihood-function.md). The two-lag fit has six coefficients, while the cumulative fit has five:

$$
\operatorname{AIC}_2\doteq1155+2(6)=1167,\qquad
\operatorname{AIC}_3\doteq1122+2(5)=1132.
$$

Thus **prefer the cumulative-history model**, whose [Akaike information criterion](../../../../../../../akaike-information-criterion.md) is lower by 35 despite its smaller number of [statistical parameters](../../../../../../../statistical-parameter.md). This is a model-selection comparison of conditional histories, not a nested [likelihood-ratio test](../../../../../../../likelihood-ratio-test.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 30](../../../../paper-30-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
