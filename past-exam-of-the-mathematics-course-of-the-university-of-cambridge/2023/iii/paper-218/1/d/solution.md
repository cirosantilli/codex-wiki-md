<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The Quasi-Poisson standard errors are trustworthy only if observations are independent, the log-linear mean is correct, and the variance is proportional to the mean with one common dispersion. Dependence, zero inflation, or covariate-dependent dispersion can invalidate this covariance formula.

A [parametric bootstrap](../../../../../../parametric-bootstrap.md) under model 1 proceeds as follows. Fit the Poisson model once and retain $X$ and the fitted means $\widehat\mu_i$. For bootstrap repetition $b$, independently draw

$$
Y_i^{*(b)}\sim\operatorname{Poisson}(\widehat\mu_i),
$$

refit the same Poisson regression to $(X,Y^{*(b)})$, and save its gender estimate $\widehat\beta_1^{*(b)}$. The sample standard deviation of these estimates over many repetitions estimates the model-1 standard error. This bootstrap deliberately measures uncertainty under the fitted Poisson model; it does not repair real overdispersion unless the resampling model is enlarged to represent its cause.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
