<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

The command fits independent grouped [binomial distributions](../../../../../binomial-distribution.md) $Y_j\sim\operatorname{Bin}(N_j,p_j)$, using the supplied totals as trial counts. The [logistic regression](../../../../../logistic-regression.md) has the additive [linear predictor](../../../../../linear-predictor.md)

$$
\widehat\eta=-3.06073-1.27079\,\mathbf1_{\{\mathrm{Kid}\}}-0.37211\,\mathbf1_{\{\mathrm M\}},\qquad
\boxed{\widehat p=\frac{e^{\widehat\eta}}{1+e^{\widehat\eta}}.}
$$

The reference category is adult females. The age and gender coefficients are conditional [log odds ratios](../../../../../log-odds-ratio.md): the fitted odds for a child are multiplied by $e^{-1.27079}\approx0.281$, and those for a male by $e^{-0.37211}\approx0.689$.

The coefficients are [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md), found by [Newton's method](../../../../../newton-s-method-in-optimization.md) or [iteratively reweighted least squares](../../../../../iteratively-reweighted-least-squares.md). With [design matrix](../../../../../design-matrix.md) $X$ and $W_{jj}=N_j\widehat p_j(1-\widehat p_j)$, the estimated [covariance matrix](../../../../../covariance-matrix.md) is $(X^TWX)^{-1}$; the printed [standard errors](../../../../../standard-error.md) are square roots of its diagonal entries. Each [Wald test](../../../../../wald-test.md) compares a coefficient with zero using its estimate divided by its [standard error](../../../../../standard-error.md), approximately a standard [normal distribution](../../../../../normal-distribution.md) under the null. The age and gender effects are strongly significant. The intercept test instead tests whether the reference probability is $1/2$.

The fitted probabilities are about $0.04476$ for adult females, $0.03128$ for adult males, $0.01298$ for female children, and $0.008981$ for male children. **Adult females have the largest fitted probability**, about **4.48%**. The residual [deviance](../../../../../exponential-family-deviance.md) is $0.06514$ on $4-3=1$ [degree of freedom](../../../../../degree-of-freedom.md); comparison with a [chi-squared distribution](../../../../../chi-squared-distribution.md) gives $p\approx0.799$. There is no evidence here that an age–gender [interaction](../../../../../interaction-statistics.md) is needed, under the assumed independent [binomial distribution](../../../../../binomial-distribution.md) model.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
