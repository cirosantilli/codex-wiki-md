<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Allow each subject to have a separate baseline and slope through a [correlated random-intercept and random-slope model](../../../../../../correlated-random-intercept-and-random-slope-model.md):

$$
Y_{ij}=\beta_0+\beta_1t_j+b_{0i}+b_{1i}t_j+\varepsilon_{ij},\qquad
\begin{pmatrix}b_{0i}\\b_{1i}\end{pmatrix}\overset{\mathrm{iid}}\sim
N_2\left(0,
\begin{pmatrix}\tau_0^2&\rho\tau_0\tau_1\\\rho\tau_0\tau_1&\tau_1^2\end{pmatrix}\right),
\qquad \varepsilon_{ij}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

The subject [random effects](../../../../../../random-effect.md) are independent of all measurement errors, and subjects are independent. The within-person [covariance](../../../../../../covariance.md) between times $s,t$ is $\tau_0^2+(s+t)\rho\tau_0\tau_1+st\tau_1^2$, with an additional $\sigma^2$ when the same reading is used twice.

**Prefer the model with a [random slope](../../../../../../random-slope.md).** The [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) refits improve twice the [log-likelihood](../../../../../../log-likelihood.md) by $227.9604$ while adding two [covariance](../../../../../../covariance.md) [statistical parameters](../../../../../../statistical-parameter.md). Both the [Akaike information criterion](../../../../../../akaike-information-criterion.md) ($5165.779$ to $4941.819$) and [Bayesian information criterion](../../../../../../bayesian-information-criterion.md) ($5183.367$ to $4968.200$) strongly favour it. The printed nominal [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) is overwhelming. The usual reference [chi-squared distribution](../../../../../../chi-squared-distribution.md) with two [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md) is not an exact regular calibration, since zero slope [variance](../../../../../../variance-split.md) is a boundary and the intercept–slope [correlation](../../../../../../pearson-correlation-coefficient.md) is then unidentified; a design-specific [parametric bootstrap](../../../../../../parametric-bootstrap.md) could calibrate it. This qualification does not undermine the substantial descriptive improvement shown by both information criteria.

The preferred fit estimates population mean baseline strength $\widehat\beta_0=61.09286$ kg and weekly gain $\widehat\beta_1=2.83143$ kg/week. The between-person baseline [standard deviation](../../../../../../standard-deviation.md) is $\widehat\tau_0=15.785582$ kg, and the between-person slope [standard deviation](../../../../../../standard-deviation.md) is $\widehat\tau_1=2.738666$ kg/week. Their estimated [correlation](../../../../../../pearson-correlation-coefficient.md) $\widehat\rho=0.117$ is weakly positive, giving random-effect [covariance](../../../../../../covariance.md) about $5.058$ kg$^2$/week; its uncertainty is not supplied. The measurement-error [standard deviation](../../../../../../standard-deviation.md) is $\widehat\sigma=9.923280$ kg. The printed $-0.038$ instead describes the [correlation](../../../../../../pearson-correlation-coefficient.md) between the estimated [fixed effects](../../../../../../fixed-effect.md), not between the subject [random effects](../../../../../../random-effect.md). These [statistical parameter](../../../../../../statistical-parameter.md) estimates come from [restricted maximum likelihood](../../../../../../restricted-maximum-likelihood.md); the model comparison uses the separate [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) fits.

The population mean fitted trajectory is $61.09286+2.83143t$ kg. Hence

$$
\boxed{\text{mean ten-week gain}=10\widehat\beta_1=28.3143\ \mathrm{kg},
\qquad \text{mean at week ten}=89.40716\ \mathrm{kg}.}
$$

Using the reported slope [standard error](../../../../../../standard-error.md), an approximate 95% [confidence interval](../../../../../../confidence-interval.md) for the population mean gain is $28.3143\pm1.96(2.984464)=(22.46,34.16)$ kg; a [Student t confidence interval](../../../../../../student-t-confidence-interval.md) with 499 [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md) is almost identical.

Successful individuals can improve far more than the average. Their latent ten-week gains have fitted [normal distribution](../../../../../../normal-distribution.md)

$$
G_i=10(\beta_1+b_{1i})\sim N(28.3143,27.38666^2).
$$

A clear estimate for an upper-performing group uses a [between-person slope quantile](../../../../../../between-person-slope-quantile.md): the 95th percentile is $28.3143+1.645(27.38666)\simeq73.4$ kg, and the 97.5th percentile is about $82.0$ kg. **The upper 5% of fitted underlying gains begin around 73 kg.** These are person-to-person performance [quantiles](../../../../../../quantile-function.md), not [confidence intervals](../../../../../../confidence-interval.md) for the population mean. Identifying the best observed trainee would require that person's data or fitted subject [random effects](../../../../../../random-effect.md); the aggregate output cannot identify a literal maximum. If performance means the observed difference of endpoint readings, add the measurement-error [variance](../../../../../../variance-split.md) $2\sigma^2$ to the latent gain [variance](../../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
