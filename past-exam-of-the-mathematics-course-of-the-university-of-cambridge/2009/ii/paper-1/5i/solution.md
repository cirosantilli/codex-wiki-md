<h1 id="5i/solution">Solution</h1>

↑ **Parent:** [5I](../5i.md)

The [logit link](../../../../../logit.md) gives $\mu_i=e^{\beta x_i}/(1+e^{\beta x_i})$. Independence in the [Bernoulli logistic-regression model](../../../../../bernoulli-logistic-regression-model.md) therefore gives the [log-likelihood](../../../../../log-likelihood.md)

$$
\boxed{\ell(\beta)=\sum_{i=1}^n\left[y_i\beta x_i-\log(1+e^{\beta x_i})\right].}
$$

Differentiate using $d\mu_i/d\beta=x_i\mu_i(1-\mu_i)$:

$$
\boxed{\ell'(\beta)=\sum_i x_i(y_i-\mu_i),\qquad \ell''(\beta)=-\sum_i x_i^2\mu_i(1-\mu_i).}
$$

The [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md), if finite, solves the single [score equation](../../../../../score-equation.md) $\sum_i x_i(y_i-\widehat\mu_i)=0$. If at least one $x_i$ is nonzero, the log likelihood is strictly concave at finite $\beta$, so any root is the unique maximizer.

Use [Newton method](../../../../../newton-s-method-in-optimization.md), equivalently one-parameter iteratively reweighted fitting:

$$
\beta_{j+1}=\beta_j+\frac{\sum_i x_i[y_i-\mu_i(\beta_j)]}{\sum_i x_i^2\mu_i(\beta_j)[1-\mu_i(\beta_j)]}.
$$

A damped step or a bracketed score solver is useful if a full step overshoots. The [finite maximum-likelihood estimate in a one-parameter logistic model](../../../../../finite-maximum-likelihood-estimate-in-a-one-parameter-logistic-model.md) requires the score limit at minus infinity to be positive and its limit at plus infinity to be negative. Perfect sign separation of the observations can instead send the estimate to an infinite coefficient; if every $x_i=0$, the coefficient is unidentifiable. These possibilities should be checked before claiming convergence to a finite estimate.

## ↑ Ancestors (10)

1. [5I](../5i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
