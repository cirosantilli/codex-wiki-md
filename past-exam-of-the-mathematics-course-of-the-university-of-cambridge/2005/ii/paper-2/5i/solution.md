<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

Each `scan()` command reads a numeric vector from the entered data: the first creates the nine counts, and the second their nine predictor values. The last command fits a [generalized linear model](../../../../../generalized-linear-model.md) with the [Poisson distribution](../../../../../poisson-distribution.md) and its default [log link](../../../../../logarithmic-link-function.md), including an intercept, then prints a summary. Thus the model is [independent](../../../../../independent-random-variables.md) counts with means $\mu_j$ satisfying

$$
\log\mu_j=b_0+b_1i_j,
\qquad \widehat\mu_j=\exp(1.363+0.3106i_j).
$$

The coefficients are [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md), and the reported standard errors come from the inverse fitted [Fisher information matrix](../../../../../fisher-information-matrix.md). Increasing the predictor by one multiplies the fitted mean by $e^{0.3106}\simeq1.364$, about a $36.4\%$ increase. The intercept corresponds to a mean $e^{1.363}\simeq3.91$ at predictor zero, outside the observed range. Approximate coefficient-to-standard-error ratios are $6.17$ and $8.13$; the slope is strongly different from zero under the assumed model. A $95\%$ [Wald confidence interval](../../../../../wald-confidence-interval.md) for the slope is about $[0.236,0.385]$, or $[1.266,1.470]$ for the multiplicative change.

The [deviance](../../../../../exponential-family-deviance.md) is twice the log-likelihood advantage of the [saturated model](../../../../../saturated-model.md) over the fitted model. For these counts it is

$$
D=2\sum_{j=1}^9\left[n_j\log\frac{n_j}{\widehat\mu_j}-(n_j-\widehat\mu_j)\right],
$$

with the logarithmic term interpreted as zero when a count is zero. The [saturated model](../../../../../saturated-model.md) has nine freely fitted means; the fitted model has two [independent](../../../../../independent-random-variables.md) regression coefficients, so the residual [degrees of freedom](../../../../../degree-of-freedom.md) are **$9-2=7$**.

Under an adequate Poisson model and the usual large-sample approximation, $D$ is compared with $\chi^2_7$. The reported $13.218$ is rather large relative to seven, but below the $5\%$ upper critical value about $14.07$; its approximate upper-tail [probability](../../../../../probability.md) is $0.067$. Thus there is some indication of lack of fit or [overdispersion](../../../../../overdispersion.md), but not a rejection at the $5\%$ level on this diagnostic. The deviance-to-d.f. ratio is about $1.89$; it does not by itself prove an overdispersed model, and the chi-square approximation is imperfect for small counts.

There is one inconsistency in the supplied numerical output. Independently solving the Poisson score equations for the displayed nine counts gives $\widehat b_0=1.363454$, $\widehat b_1=0.310563$ and deviance $13.217971$, agreeing with the printed estimates and deviance. But $[X^{\mathsf T}\operatorname{diag}(\widehat\mu)X]^{-1}$ gives standard errors approximately $0.221295$ and $0.030850$. In particular the printed slope standard error $0.0382$ is not the standard Poisson-model value for these data. The interpretations above describe the supplied numbers; the directly recomputed slope ratio is $10.07$ and its normal-approximation $95\%$ interval is about $[0.2501,0.3710]$. The conclusion of a strong increasing trend is unchanged.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
