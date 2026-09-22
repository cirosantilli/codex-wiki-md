<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $a_i$ be age in years, $g_i$ the male indicator and $m_i$ the indicator for the Messiah group. The fitted [Cox proportional-hazards model](../../../../../../../cox-proportional-hazards-model.md) is

$$
h_i(t)=h_0(t)\exp\{0.006536a_i-0.603547g_i+0.755308m_i\},
$$

with an unspecified common [baseline hazard](../../../../../../../baseline-hazard.md). Its coefficients were estimated by [Cox partial likelihood](../../../../../../../cox-partial-likelihood.md), using the [Breslow approximation for tied event times](../../../../../../../breslow-approximation-for-tied-event-times.md). There are $100$ participants, $96$ recorded completions and four censored observations.

A higher [hazard function](../../../../../../../hazard-function.md) means a greater instantaneous chance of completion among those not yet completing, so it describes faster completion rather than greater mortality. Holding gender and group fixed, an extra year of age multiplies the completion hazard by **$1.0066$**, about a $0.66\%$ increase. The 95% [confidence interval](../../../../../../../confidence-interval.md) is $(0.9865,1.0270)$ and the [Wald test](../../../../../../../wald-test.md) has $p=0.5241$, so there is little evidence of an age association.

Holding age and group fixed, male participants have a [hazard ratio](../../../../../../../hazard-ratio.md) **$0.5469$** relative to female participants, about a $45.3\%$ lower completion hazard. Its 95% [confidence interval](../../../../../../../confidence-interval.md) is $(0.3560,0.8401)$ and $p=0.00586$. Under the fitted model this corresponds to slower completion for males. It is not a ratio of mean or median completion times.

Holding age and gender fixed, participants assigned to Messiah have a [hazard ratio](../../../../../../../hazard-ratio.md) **$2.1283$** relative to The Kingdom, with 95% [confidence interval](../../../../../../../confidence-interval.md) $(1.3653,3.3176)$ and $p=0.000854$. This is strong evidence of a group difference, with faster completion in the Messiah group under the fitted model. Random assignment supports interpreting a group contrast as an effect of the assigned condition, subject to the assumptions about follow-up and censoring; age and gender contrasts remain observational associations.

Each printed $z$ statistic is the coefficient divided by its [standard error](../../../../../../../standard-error.md), using an asymptotic standard normal [sampling distribution](../../../../../../../sampling-distribution.md) under a zero-coefficient [null hypothesis](../../../../../../../null-hypothesis.md). The [hazard ratio](../../../../../../../hazard-ratio.md) is $e^\beta$, and its confidence limits exponentiate the coefficient limits. Proportional hazards assumes these covariate-specific hazard multipliers stay constant over follow-up, together with the specified linear age effect and [independent censoring](../../../../../../../independent-censoring.md) conditional on covariates.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
