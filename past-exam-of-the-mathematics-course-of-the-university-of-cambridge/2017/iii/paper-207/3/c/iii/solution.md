<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use one [joint hypothesis test](../../../../../../../joint-hypothesis-test.md) for $H_0:\beta_\lambda=\beta_\mu=0$. Fit the unrestricted model with [statistical parameters](../../../../../../../statistical-parameter.md) $(\lambda_0,\mu_0,\beta_\lambda,\beta_\mu)$, where $\lambda_i=\lambda_0e^{\beta_\lambda z_i}$ and $\mu_i=\mu_0e^{\beta_\mu z_i}$ for treatment indicator $z_i$. Refit under $H_0$, estimating the two common baseline intensities; do not fix them at their unrestricted estimates. The [likelihood-ratio test statistic](../../../../../../../likelihood-ratio-test-statistic.md) is

$$
\boxed{D=2\{\ell(\widehat\lambda_0,\widehat\mu_0,\widehat\beta_\lambda,\widehat\beta_\mu)-\ell(\widetilde\lambda_0,\widetilde\mu_0,0,0)\}\ \dot\sim\ \chi^2_2.}
$$

Under regular identifiable positive-rate models, sufficient [independent](../../../../../../../independent-random-variables.md) patient trajectories, and the [null hypothesis](../../../../../../../null-hypothesis.md), [Wilks theorem](../../../../../../../wilks-theorem.md) gives two degrees of freedom because two coefficients are constrained. Reject if $D$ exceeds the chosen upper [chi-squared distribution](../../../../../../../chi-squared-distribution.md) [quantile](../../../../../../../quantile-function.md). Alternatively a two-dimensional [Wald test](../../../../../../../wald-test.md) uses $\widehat\beta^T\widehat{\operatorname{Cov}}(\widehat\beta)^{-1}\widehat\beta$, including the off-diagonal [covariance](../../../../../../../covariance.md). Two separate tests do not provide this single calibrated assessment. The point estimates alone cannot produce a numerical [p-value](../../../../../../../p-value.md) without fitted likelihoods or a coefficient [covariance matrix](../../../../../../../covariance-matrix.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
