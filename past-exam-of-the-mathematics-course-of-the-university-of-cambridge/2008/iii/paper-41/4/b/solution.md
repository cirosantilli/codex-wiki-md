<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Index city by $g\in\{0,1\}$ and age group by $j$, with the youngest group the [reference level](../../../../../../reference-level-in-a-regression-factor.md). For each of the 15 observed cells, the [grouped-binomial logistic regression](../../../../../../grouped-binomial-logistic-regression.md) assumes

$$
C_{gj}\sim\operatorname{Binomial}(N_{gj},\pi_{gj}),\qquad \log\frac{\pi_{gj}}{1-\pi_{gj}}=\alpha+a_j+\gamma g,\qquad a_{15\text{–}24}=0,
$$

with independent cell counts. The response supplied to R is $C_{gj}/N_{gj}$, and the weights specify the binomial numbers of trials $N_{gj}$. They are not 15 arbitrary precision weights: the conditional [variance](../../../../../../variance-split.md) of the proportion is $\pi_{gj}(1-\pi_{gj})/N_{gj}$. The [logit link](../../../../../../logit.md) models log odds, and the two sets of factor coefficients use corner-point constraints.

There are nine parameters: one [intercept](../../../../../../regression-intercept.md), seven age contrasts and one city contrast. Hence the residual [degrees of freedom](../../../../../../degree-of-freedom.md) are $15-9=6$, not the total population minus nine. The null model has only an [intercept](../../../../../../regression-intercept.md) and $14$ residual [degrees of freedom](../../../../../../degree-of-freedom.md). Adding age uses seven more parameters and reduces the [binomial deviance](../../../../../../binomial-deviance.md) from $2330.46$ to $232.28$, a drop of $2098.19$. Adding city then uses one parameter and reduces it by $227.12$ to $5.15$. These are sequential [likelihood-ratio tests](../../../../../../likelihood-ratio-test.md), asymptotically compared with [chi-squared distributions](../../../../../../chi-squared-distribution.md) on seven and one [degrees of freedom](../../../../../../degree-of-freedom.md). Both provide extremely strong evidence of an effect; the printed age [p-value](../../../../../../p-value.md) $0.00$ is rounding, not an exactly zero probability. Because the table is incomplete, sequential main-effect sums need not be invariant to the order of fitting.

The [intercept](../../../../../../regression-intercept.md) estimate $-11.69364$ is the log odds for the youngest Minneapolis–Saint Paul group. It implies baseline odds $e^{-11.69364}$ and a fitted probability about $8.35\times10^{-6}$. Its [standard error](../../../../../../standard-error.md) is $0.44923$; its reported [Wald test](../../../../../../wald-test.md) tests log odds zero, or probability $1/2$, rather than a scientifically interesting comparison of groups.

The age coefficients are log [odds ratios](../../../../../../odds-ratio.md) relative to the youngest group within the same city. Their exponentials are approximately $13.86$, $46.82$, $99.03$, $162.23$, $284.38$, $497.07$ and $484.57$ as age increases through the seven other groups. All these comparisons have large positive [Wald statistics](../../../../../../wald-test.md) and small [p-values](../../../../../../p-value.md). Thus the fitted probabilities are much higher in the older groups than in the youngest group. The slightly smaller coefficient in the oldest group than in the preceding group does not itself prove a real decline: that claim needs a contrast and its [standard error](../../../../../../standard-error.md), including the [covariance](../../../../../../covariance.md) of the two estimates.

The city coefficient $0.85492$ is the log [odds ratio](../../../../../../odds-ratio.md) for Fort Worth relative to Minneapolis–Saint Paul, adjusted for age. Its [standard error](../../../../../../standard-error.md) $0.05969$ gives $z=14.322$, so the null city effect is strongly rejected by the [Wald test](../../../../../../wald-test.md), consistent with the sequential [likelihood-ratio test](../../../../../../likelihood-ratio-test.md). The fitted constant-over-age city [odds ratio](../../../../../../odds-ratio.md) and an approximate 95% [confidence interval](../../../../../../confidence-interval.md) are

$$
\boxed{\operatorname{OR}=e^{0.85492}=2.351,\qquad \operatorname{CI}_{95\%}=e^{0.85492\pm1.96(0.05969)}\approx(2.09,2.64).}
$$

This is an odds ratio, not generally a probability ratio. The probabilities here are sufficiently small that the two ratios are close. The absence of an age-by-city [interaction](../../../../../../interaction-statistics.md) is an assumption of the fitted additive log-odds model.

The final [binomial deviance](../../../../../../binomial-deviance.md) is $5.1509$ on six [degrees of freedom](../../../../../../degree-of-freedom.md); its approximate upper-tail [p-value](../../../../../../p-value.md) is $0.525$. It gives no indication of substantial lack of fit against the saturated observed-cell model. The [deviance residuals](../../../../../../deviance-residual.md) range from $-1.2830$ to $1.0820$, with median zero and no conspicuously large value in the five-number summary. Neither statement proves that every model assumption holds. In particular, the small case counts motivate checking the accuracy of the [chi-squared asymptotic approximation](../../../../../../chi-squared-asymptotic-approximation.md), for example by a fitted-model [parametric bootstrap](../../../../../../parametric-bootstrap.md).

The dispersion is fixed at one by the [binomial distribution](../../../../../../binomial-distribution.md); it was not estimated as a free scale parameter. Four [Fisher scoring](../../../../../../scoring-algorithm.md) iterations describe the numerical optimization, not four additional parameters. Residual and cellwise observed-versus-fitted comparisons would help assess adequacy and potential [overdispersion](../../../../../../overdispersion.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
