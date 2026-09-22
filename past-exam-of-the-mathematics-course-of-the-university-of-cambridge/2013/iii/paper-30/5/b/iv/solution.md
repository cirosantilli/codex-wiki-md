<h1 id="5/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The preferred [cumulative-response logistic model](../../../../../../../cumulative-response-logistic-model.md) estimates

$$
\operatorname{logit}(p_{it})=-1.417630-0.364092S_i+0.001224A_i
+0.327118T_i+0.399296C_{it},\qquad C_{it}=\sum_{s<t}Y_{is}.
$$

Its [logit link](../../../../../../../logit.md) describes conditional smoking-free [probability](../../../../../../../probability.md) given baseline predictors and prior successful weeks. Holding the other predictors fixed, males have $e^{-0.364092}=0.695$ times the female success [odds](../../../../../../../odds.md); the reported [p-value](../../../../../../../p-value.md) is $0.0152$, and the approximate 95% [odds ratio](../../../../../../../odds-ratio.md) [confidence interval](../../../../../../../confidence-interval.md) is $(0.518,0.932)$. Age has estimated [odds ratio](../../../../../../../odds-ratio.md) $e^{0.001224}=1.0012$ per additional year, with [p-value](../../../../../../../p-value.md) $0.918$, giving little evidence for an age association in this fit.

The combined treatment has conditional success [odds ratio](../../../../../../../odds-ratio.md) $e^{0.327118}=1.387$ versus the reference treatment, with approximate 95% [confidence interval](../../../../../../../confidence-interval.md) $(1.035,1.859)$ and [p-value](../../../../../../../p-value.md) $0.0285$. **The fitted conditional odds are about 39% higher for the combined treatment.** The trial randomization supports treatment comparisons, but conditioning on accumulated post-treatment outcomes means this coefficient is not directly the marginal total treatment effect.

Each previous successful week multiplies current success [odds](../../../../../../../odds.md) by $e^{0.399296}=1.491$, with approximate 95% [confidence interval](../../../../../../../confidence-interval.md) $(1.329,1.673)$ and very small [p-value](../../../../../../../p-value.md) $1.06\times10^{-11}$. This is strong fitted persistence. It can reflect [true state dependence](../../../../../../../true-state-dependence.md), [unobserved heterogeneity](../../../../../../../unobserved-heterogeneity.md), or an omitted calendar-time trend; this fit alone cannot distinguish them. The baseline intercept implies success [probability](../../../../../../../probability.md) $\operatorname{logit}^{-1}(-1.417630)\simeq0.195$ for a reference-treatment female aged zero with no previous success. That age is outside the study's useful interpretation range, so the intercept chiefly anchors the regression. The [Bernoulli distribution](../../../../../../../bernoulli-distribution.md) [dispersion parameter](../../../../../../../dispersion-parameter.md) is fixed at one, and the residual [binomial deviance](../../../../../../../binomial-deviance.md) is 1122 on 995 [statistical degrees of freedom](../../../../../../../statistical-degrees-of-freedom.md). With individual binary outcomes, comparing that [binomial deviance](../../../../../../../binomial-deviance.md) mechanically to a [chi-squared distribution](../../../../../../../chi-squared-distribution.md) is not a reliable general goodness-of-fit test.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
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
