<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Conditional on the observed data, the preceding [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) approximation implies that

$$
Z=J^{1/2}(\theta-\widehat\theta)\ \dot\sim\ N_p(0,I).
$$

The deviance expansion consequently gives

$$
D(\theta)-D(\widehat\theta)\approx(\theta-\widehat\theta)^TJ(\theta-\widehat\theta)=Z^TZ.
$$

The sum of squares of $p$ independent standard [normal distribution](../../../../../../normal-distribution.md) variables has [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $p$ degrees of freedom. Hence, as a statement about the [posterior distribution](../../../../../../bayesian-posterior.md) of the [Bayesian deviance](../../../../../../bayesian-deviance.md),

$$
\boxed{D(\theta)\mid y\ \dot\sim\ D(\widehat\theta)+\chi_p^2.}
$$

The data are fixed here and the parameter varies according to its posterior; this is not a claim about resampling the data.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
