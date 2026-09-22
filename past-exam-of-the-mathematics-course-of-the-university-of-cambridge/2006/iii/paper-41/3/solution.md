<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Poisson distribution](../../../../../poisson-distribution.md) mass function is

$$
P(Y=y)=\frac{e^{-\mu}\mu^y}{y!}
=\exp\{y\log\mu-\mu-\log(y!)\},\qquad y=0,1,\ldots.
$$

It is an [exponential dispersion family of order one](../../../../../exponential-dispersion-family-of-order-one.md) with

$$
\boxed{\theta=\log\mu,\qquad b(\theta)=e^\theta,\qquad\phi=1,\qquad c(y,\phi)=-\log(y!).}
$$

Indeed, $b'(\theta)=e^\theta=E(Y)$ and $\phi b''(\theta)=e^\theta=\operatorname{Var}(Y)$. A [generalized linear model](../../../../../generalized-linear-model.md) specifies [independent random variables](../../../../../independent-random-variables.md) from a response [exponential family](../../../../../exponential-family-split.md), together with a [linear predictor](../../../../../linear-predictor.md) and a [link function](../../../../../link-function.md) relating it to the response mean. The [Poisson canonical link](../../../../../poisson-canonical-link.md) is $g(\mu)=\log\mu$.

For the insurance counts, let class $1$ and merit $0$ be the [reference levels in a regression factor](../../../../../reference-level-in-a-regression-factor.md). The fitted [Poisson regression](../../../../../poisson-regression.md) assumes

$$
Y_{ij}\overset{\mathrm{ind}}\sim\operatorname{Pois}(\mu_{ij}),\qquad
\mu_{ij}=n_{ij}\lambda_{ij},\qquad
\log\lambda_{ij}=\alpha+c_i+m_j,\qquad c_1=m_0=0.
$$

The insured exposure $n_{ij}$ is known; its [logarithm](../../../../../logarithm.md) is an [offset](../../../../../generalized-linear-model-offset.md), not a coefficient to estimate. The model has eight free mean parameters and fixes the [dispersion parameter](../../../../../dispersion-parameter.md) at one. It assumes additive class and merit effects on the log-rate scale, hence multiplicative effects on the rate scale without a class-by-merit [interaction](../../../../../interaction-statistics.md).

Apart from constants independent of the parameters, the [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell=\sum_{i,j}\left[Y_{ij}(\alpha+c_i+m_j)-n_{ij}e^{\alpha+c_i+m_j}\right].
$$

Differentiating gives the [Poisson regression margin-matching score equations](../../../../../poisson-regression-margin-matching-score-equations.md)

$$
\sum_{i,j}(Y_{ij}-\widehat\mu_{ij})=0,\qquad
\sum_i(Y_{ij}-\widehat\mu_{ij})=0\quad(j=1,2,3),\qquad
\sum_j(Y_{ij}-\widehat\mu_{ij})=0\quad(i=2,3,4,5).
$$

Thus the fitted totals equal the observed totals in each class and merit category, including the reference categories by subtraction. In [design matrix](../../../../../design-matrix.md) notation these equations are $Z^T(Y-\widehat\mu)=0$. [Fisher scoring](../../../../../scoring-algorithm.md) solves them iteratively; the reported three iterations describe the numerical fit, not an additional statistical result.

The [regression intercept](../../../../../regression-intercept.md) gives the baseline fitted claim rate $e^{-2.0357359}=0.130584$ per insured car year. The merit [rate ratios](../../../../../rate-ratio.md), relative to merit $0$ at the same class, are

$$
\boxed{e^{\widehat m_1}=0.87131,\qquad e^{\widehat m_2}=0.80197,\qquad e^{\widehat m_3}=0.61082.}
$$

The class [rate ratios](../../../../../rate-ratio.md), relative to class $1$ at the same merit, are

$$
\boxed{e^{\widehat c_2}=1.34963,\quad e^{\widehat c_3}=1.59848,\quad
 e^{\widehat c_4}=1.69190,\quad e^{\widehat c_5}=1.24054.}
$$

Each predicted cell rate is the baseline rate times its class and merit multipliers. The output's coefficient-to-[standard error](../../../../../standard-error.md) ratios are asymptotic normal [Wald test](../../../../../wald-test.md) statistics under the fitted [Poisson regression](../../../../../poisson-regression.md), despite the software label “t value”; there is no estimated Gaussian residual scale in this model. All nonreference effects have very large absolute ratios.

The null [Poisson deviance](../../../../../poisson-deviance.md) is $33854.16$ on nineteen [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md); adding the seven factor coefficients reduces it by $33274.6437$. But the final [Poisson deviance](../../../../../poisson-deviance.md) is still $579.5163$ on twelve [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md), and the [deviance residuals](../../../../../deviance-residual.md) include values near $-10.79$ and $11.63$. These are far beyond what a well-fitting unit-dispersion model would normally produce. **The additive Poisson model fits substantially better than a common rate, but remains grossly inadequate.** A class-by-merit [interaction](../../../../../interaction-statistics.md), [overdispersion](../../../../../overdispersion.md), or [statistical dependence](../../../../../statistical-dependence.md) between claims could contribute; the summary alone does not distinguish these explanations. Its very small nominal [standard errors](../../../../../standard-error.md) and formal [Wald tests](../../../../../wald-test.md) rely on the rejected model, so improved mean structure and error assumptions are needed before treating them as reliable uncertainty assessments.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
