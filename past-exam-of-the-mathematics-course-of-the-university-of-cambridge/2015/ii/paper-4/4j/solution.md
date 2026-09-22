<h1 id="4j/solution">Solution</h1>

↑ **Parent:** [4J](../4j.md)

This is a [generalized linear model](../../../../../generalized-linear-model.md) with independent [Bernoulli distributions](../../../../../bernoulli-distribution.md) for the responses and the [logit link](../../../../../logit.md). Under treatment coding with colour one as the reference level, the [linear predictor](../../../../../linear-predictor.md) is

$$
\log\frac{p_i}{1-p_i}=\beta_0+\beta_2\mathbf1_{\{c_i=2\}}+\beta_3\mathbf1_{\{c_i=3\}}+\beta_4\mathbf1_{\{c_i=4\}}+\beta_w w_i.
$$

Colour is a [categorical variable](../../../../../categorical-variable.md), not a numerical trend. Width has the same slope for every colour, since no [interaction term](../../../../../interaction-term.md) is fitted. The parameters are estimated by [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md).

The approximate [Wald confidence interval](../../../../../wald-confidence-interval.md) for the width coefficient is $\boxed{0.46\pm1.96(0.106)}$, or approximately $(0.2522,0.6678)$. This uses the approximate [normal distribution](../../../../../normal-distribution.md) of the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md), rather than a confidence interval for an individual binary response.

For the requested crab, the fitted [linear predictor](../../../../../linear-predictor.md) is $\widehat\eta=-11.38-0.22+0.46(20)=-2.40$. Applying the inverse [logit link](../../../../../logit.md) gives $\boxed{\widehat p=(1+e^{2.40})^{-1}\simeq0.0832}$. The rounded displayed coefficients need not reproduce the reported test statistics exactly.

## ↑ Ancestors (10)

1. [4J](../4j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
