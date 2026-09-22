<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

A [generalized linear model](../../../../../generalized-linear-model.md) assumes that the independent responses $Y_i$ have distributions in an [exponential family](../../../../../exponential-family-split.md), with means $\mu_i$, and that

$$
g(\mu_i)=\eta_i=x_i^T\beta.
$$

The invertible function $g$ is the [link function](../../../../../link-function.md); it connects the mean to the [linear predictor](../../../../../linear-predictor.md).

For [binomial regression](../../../../../binomial-regression.md), write $Y_i\sim\operatorname{Bin}(m_i,p_i)$ independently, so $\mu_i=m_ip_i$. The [logistic regression](../../../../../logistic-regression.md) link is

$$
\log\frac{p_i}{1-p_i}=x_i^T\beta,
\qquad
p_i=\frac{e^{x_i^T\beta}}{1+e^{x_i^T\beta}},
$$

while [probit regression](../../../../../probit-model.md) uses

$$
\Phi^{-1}(p_i)=x_i^T\beta,
\qquad
p_i=\Phi(x_i^T\beta),
$$

where $\Phi$ is the standard-normal distribution function. The logit is the [canonical link function](../../../../../canonical-link-function.md) for the binomial family.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
