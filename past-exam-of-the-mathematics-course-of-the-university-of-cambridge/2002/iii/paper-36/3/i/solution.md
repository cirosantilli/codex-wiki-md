<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $e_{ij}$ for the expected accident count, not for the accident rate. With a design row $z_{ij}$ consisting of an intercept, seven non-reference site indicators and the after-treatment indicator,

$$
e_{ij}=p_{ij}\exp(\mu+\alpha_i+\beta_j),\qquad
\ell=\sum_{ij}\{y_{ij}(\log p_{ij}+z_{ij}^{\mathsf T}\gamma)-e_{ij}-\log(y_{ij}!)\}.
$$

Here $\log p_{ij}$ is a known [generalized linear model offset](../../../../../../generalized-linear-model-offset.md), with coefficient fixed at one. Differentiating the [Poisson regression](../../../../../../poisson-regression.md) [log-likelihood](../../../../../../log-likelihood.md) gives the [score function](../../../../../../informant-function.md) equations

$$
\boxed{\sum_{ij}(y_{ij}-e_{ij})=0,\qquad
\sum_{j=1}^2(y_{ij}-e_{ij})=0\ (i=2,\ldots,8),\qquad
\sum_{i=1}^8(y_{i2}-e_{i2})=0}.
$$

These nine equations estimate the intercept, seven site contrasts and one treatment contrast, with the stated reference-level constraints.

The [Fisher information](../../../../../../fisher-information-matrix.md) is $Z^{\mathsf T}WZ$, where $W=\operatorname{diag}(e_{ij})$. A [Fisher scoring](../../../../../../scoring-algorithm.md) update adds $(Z^{\mathsf T}WZ)^{-1}Z^{\mathsf T}(y-e)$ to the current coefficient vector. In [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md), the working response is $z^*_{ij}=\log e_{ij}+(y_{ij}-e_{ij})/e_{ij}$; regress $z^*_{ij}-\log p_{ij}$ on the design with weights $e_{ij}$. Thus the reported four iterations solve the [likelihood](../../../../../../likelihood-function.md) equations while accounting for unequal exposure periods.

The common adjusted [rate ratio](../../../../../../rate-ratio.md) is obtained by exponentiating the after coefficient:

$$
\boxed{\widehat r=e^{-0.7806616}\simeq0.4581}.
$$

This estimates a $54.2\%$ lower accident rate after the intervention, conditional on the additive site model. The [standard error](../../../../../../standard-error.md) $0.2751810$ gives normal [Wald statistic](../../../../../../wald-test.md) $-2.8369$, two-sided $p\simeq0.0046$, and an approximate $95\%$ [confidence interval](../../../../../../confidence-interval.md) for the [rate ratio](../../../../../../rate-ratio.md)

$$
\boxed{\exp[-0.7806616\pm1.96(0.2751810)]\simeq[0.267,0.786]}.
$$

The label t value is again a normal-reference Wald ratio under fixed Poisson dispersion, rather than an exact Student statistic.

The intercept gives the before rate at reference site one: $e^{0.2707792}\simeq1.311$ accidents per year. The seven site coefficients are log baseline-[rate ratios](../../../../../../rate-ratio.md) relative to that site. In site order two through eight, their exponentials are about $0.615,2.767,1.711,0.769,1.797,0.615,1.221$. The third site has the largest estimated rate and a nominal Wald ratio about $3.118$ against the reference. These are adjusted baseline comparisons, not differences in absolute accident counts. The overall unadjusted before/after [rate ratio](../../../../../../rate-ratio.md) is $(15/18)/(114/68)\simeq0.497$, and it differs from $0.458$ because site risks and their relative exposure weights differ.

An [independent](../../../../../../independent-random-variables.md) way to solve the fit is the [profile likelihood for a common Poisson rate ratio with unequal exposures](../../../../../../profile-likelihood-for-a-common-poisson-rate-ratio-with-unequal-exposures.md). Put $t_i=y_{i1}+y_{i2}$ and $\lambda_i=\exp(\mu+\alpha_i)$. For fixed $r$, the site score gives $\widehat\lambda_i=t_i/(p_{i1}+rp_{i2})$. The remaining equation is

$$
\sum_i\frac{t_i r p_{i2}}{p_{i1}+rp_{i2}}=15.
$$

Its positive root reproduces the reported treatment estimate. Comparing the same site model with $r=1$ to the fitted model gives a [deviance](../../../../../../exponential-family-deviance.md) improvement about $9.750$ on one degree of freedom, with nominal likelihood-ratio $p\simeq0.0018$.

There are $16$ count observations and $9$ fitted mean parameters, leaving $7$ residual degrees of freedom. The [null deviance](../../../../../../null-deviance.md) $132.9485$ on $15$ degrees of freedom is for the intercept-only rate model, still including the exposure offset. The residual [Poisson deviance](../../../../../../poisson-deviance.md) is $16.27524$ on $7$ degrees of freedom. A chi-squared comparison gives approximately $p=0.023$, suggesting potential lack of fit of a single common treatment ratio; the extreme [deviance residuals](../../../../../../deviance-residual.md) near $-2.03$ and $2.14$ also deserve inspection. Several after-cell expected counts are below one or near two, so this absolute-fit calibration is only approximate. Site-specific treatment effects, [overdispersion](../../../../../../overdispersion.md) or temporal dependence are possible explanations to investigate, with a [parametric bootstrap](../../../../../../parametric-bootstrap.md) available to calibrate the sparse-count fit statistic. A before/after association alone does not isolate a causal effect from secular changes or [regression to the mean](../../../../../../regression-to-the-mean.md) at selected sites.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
