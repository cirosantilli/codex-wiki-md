<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For separate binary observations, the [saturated model](../../../../../../saturated-model.md) fits each outcome exactly and has maximized log-likelihood zero. With $\hat p_i=p_i(\hat\beta)$, the [residual deviance](../../../../../../residual-deviance.md) is therefore

$$
D=-2\ell(\hat\beta)=-2\sum_i\left[y_i\operatorname{logit}\hat p_i+\log(1-\hat p_i)\right].
$$

Use the identity in part (b) to replace $y_i$ by $\hat p_i$ in its first term:

$$
\boxed{D=-2\sum_i\left[\hat p_i\operatorname{logit}\hat p_i+\log(1-\hat p_i)\right]=-2\sum_i\left[\hat p_i\log\hat p_i+(1-\hat p_i)\log(1-\hat p_i)\right].}
$$

Thus the deviance is twice the sum of the fitted binary [information entropies](../../../../../../information-entropy.md). A [deviance goodness-of-fit test](../../../../../../deviance-goodness-of-fit-test.md) against $\chi^2_{n-p}$ is unreliable for individual ungrouped binary observations: there is only one trial per saturated-model parameter, so the usual large-cell-count approximation fails. Deviance differences between fixed-dimensional nested [logistic regression](../../../../../../logistic-regression.md) models can still support a [likelihood-ratio test](../../../../../../likelihood-ratio-test.md), subject to its usual regularity assumptions.

The three tree models are respectively $\operatorname{logit}p_i=\beta_0$, $\operatorname{logit}p_i=\beta_0+\beta_1\log_2T_i$, and $\operatorname{logit}p_i=\beta_0+\beta_1\log_2T_i+\beta_2S_i$, with independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md) conditional on the covariates. Testing the additional severity effect gives

$$
\boxed{2\{\ell(\widehat\beta_{\rm full})-\ell(\widehat\beta_{\rm reduced})\}=655.24-563.90=91.34.}
$$

Under $H_0:\beta_2=0$, its reference distribution is asymptotically $\chi^2_1$. The $p$-value is approximately $1.21\times10^{-21}$, giving overwhelming evidence that severity improves the fitted model. Holding severity fixed, doubling $T$ increases $\log_2T$ by one and multiplies the odds by

$$
\boxed{e^{2.2164}\simeq9.17.}
$$

This is an [odds ratio](../../../../../../odds-ratio.md), not a multiplication of the event probability itself.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
