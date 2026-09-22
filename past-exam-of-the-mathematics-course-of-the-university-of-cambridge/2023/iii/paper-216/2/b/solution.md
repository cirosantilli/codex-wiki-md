<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiplying the [exponential family](../../../../../../exponential-family-split.md) likelihood by its [natural conjugate prior](../../../../../../natural-conjugate-prior.md) gives

$$
\pi(\theta\mid x)
=\exp\left\{
\theta^T(\lambda_1+T(x))
-Z(\theta)(\lambda_2+1)
-\widetilde Z(\lambda_1+T(x),\lambda_2+1)
\right\}.
$$

Thus the posterior remains in the same family, with updated [hyperparameters](../../../../../../hyperparameter.md)

$$
\lambda_1'=\lambda_1+T(x),
\qquad \lambda_2'=\lambda_2+1.
$$

Under [quadratic loss](../../../../../../squared-error-loss.md), the [Bayes estimator under squared error loss](../../../../../../bayes-estimator-under-squared-error-loss.md) is the [posterior mean](../../../../../../posterior-mean.md). Differentiating the [log-partition function](../../../../../../cumulant-function-of-an-exponential-family.md) that normalizes the conjugate prior gives

$$
\boxed{\widehat\theta
=\mathbb E[\theta\mid x]
=\nabla_{\lambda_1}\widetilde Z
(\lambda_1+T(x),\lambda_2+1).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
