<h1 id="13j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The code fits a [Bernoulli logistic-regression model](../../../../../../bernoulli-logistic-regression-model.md). Conditionally on the covariates, the responses are independent with

$$
Y_i\sim\operatorname{Bernoulli}(p_i),
\qquad
\log\frac{p_i}{1-p_i}=x_i^T\beta,
$$

where the design includes the displayed numerical predictors and indicator columns for factor levels. It maximizes

$$
L(\beta)=\prod_{i=1}^{889}p_i^{Y_i}(1-p_i)^{1-Y_i}.
$$

[Akaike information criterion](../../../../../../akaike-information-criterion.md) is

$$
\operatorname{AIC}=2k-2\ell(\widehat\beta),
$$

where $k$ is the number of fitted parameters. Backward stepwise selection starts from the full model, tentatively removes each eligible term, chooses the removal producing the lowest AIC, and repeats while AIC decreases. It balances fit against model size rather than testing every coefficient at a fixed significance threshold.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
