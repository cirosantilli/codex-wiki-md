<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Independence in the [Bernoulli logistic-regression model](../../../../../bernoulli-logistic-regression-model.md) gives the [log-likelihood](../../../../../log-likelihood.md)

$$
\ell(\beta)=\sum_{i=1}^n\left[y_i\beta x_i-\log(1+e^{\beta x_i})\right].
$$

Writing $\mu_i=(1+e^{-\beta x_i})^{-1}$, the [score function](../../../../../informant-function.md) and curvature are

$$
\boxed{\ell'(\beta)=\sum_i x_i(y_i-\mu_i),\qquad
\ell''(\beta)=-\sum_i x_i^2\mu_i(1-\mu_i).}
$$

Thus a finite [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) solves $\sum_i x_i(y_i-\widehat\mu_i)=0$. If at least one $x_i\ne0$, the curvature is strictly negative for finite $\beta$, so any such solution is the unique maximizer.

Use the [Newton method](../../../../../newton-s-method-in-optimization.md), which here coincides with [Fisher scoring](../../../../../scoring-algorithm.md) because the second derivative does not depend on the observed responses:

$$
\beta_{k+1}=\beta_k+
\frac{\sum_i x_i(y_i-\mu_i(\beta_k))}{\sum_i x_i^2\mu_i(\beta_k)(1-\mu_i(\beta_k))}.
$$

Step damping or a bracket for the monotone score provides reliable numerical convergence. If all covariates are zero the parameter is unidentifiable; if the outcomes are separated in the direction of the covariates, the likelihood supremum may occur at $\beta=+\infty$ or $-\infty$ rather than at a finite estimate.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
