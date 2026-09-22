<h1 id="5k/solution">Solution</h1>

↑ **Parent:** [5K](../5k.md)

[Logistic regression](../../../../../logistic-regression.md) assumes independent $Y_i\mid X_i\sim\operatorname{Bernoulli}(\pi_i)$ with

$$
\log\frac{\pi_i}{1-\pi_i}=\beta_0+X_i^T\beta.
$$

For the binomial exponential family, $\ell=y\theta-m\log(1+e^\theta)+\text{constant}$, so the mean is $m e^\theta/(1+e^\theta)$ and the canonical parameter is its logit. It may be fitted by [iteratively reweighted least squares](../../../../../iteratively-reweighted-least-squares.md).

Under LDA, Bayes' rule gives

$$
\log\frac{P(Y=1\mid x)}{P(Y=0\mid x)}=log\frac{\pi_1}{\pi_0}+(\mu_1-\mu_0)^T\Sigma^{-1}x-	frac12(\mu_1^T\Sigma^{-1}\mu_1-\mu_0^T\Sigma^{-1}\mu_0),
$$

which is a logistic model with an intercept.

## ↑ Ancestors (10)

1. [5K](../5k.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
