<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After integrating out the [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) $\beta$, the [marginal distribution](../../../../../../marginal-distribution.md) is

$$
Y\sim N\!\left(0,\sigma^2A\right),
\qquad A=XX^T+\alpha I_n.
$$

Up to terms independent of $\sigma^2$, the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\sigma^2)=-\frac n2\log\sigma^2
-\frac1{2\sigma^2}Y^TA^{-1}Y.
$$

Differentiating and setting the result to zero gives the [maximum marginal likelihood estimator](../../../../../../maximum-marginal-likelihood-estimator.md)

$$
\widehat{\sigma}^2=\frac1nY^T(XX^T+\alpha I_n)^{-1}Y.
$$

This is an [Empirical Bayes method](../../../../../../empirical-bayes-method.md) because the estimated [hyperparameter](../../../../../../hyperparameter.md) is then inserted into the prior and posterior distributions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
