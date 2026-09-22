<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

The commands choose $n=100$ observations and $p=2$ predictors; generate a $100\times2$ matrix $X$ of [independent](../../../../../independent-random-variables.md) [standard-normal](../../../../../standard-normal-distribution.md) values; generate [independent binary random variables](../../../../../independent-random-variables.md) $Y_i$ with success probability $1/2$; and report the observed number of successes, $\sum_iY_i=48$. The first `glm` call then fits the [Bernoulli logistic-regression model](../../../../../bernoulli-logistic-regression-model.md)

$$
Y_i\sim\operatorname{Bernoulli}(p_i),
\qquad
\log\frac{p_i}{1-p_i}
=\beta_0+\beta_1X_{i1}+\beta_2X_{i2}.
$$

The prediction command returns the fitted response probabilities $\widehat p_i$ and sums them.

The likelihood is

$$
L(\beta)=\prod_{i=1}^{100}
 p_i^{Y_i}(1-p_i)^{1-Y_i},
\qquad
p_i=\frac{e^{\eta_i}}{1+e^{\eta_i}},
\quad
\eta_i=\beta_0+\beta_1X_{i1}+\beta_2X_{i2}.
$$

At the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md), the intercept component of the [score function](../../../../../informant-function.md) is

$$
0=\frac{\partial\log L}{\partial\beta_0}
 =\sum_{i=1}^{100}(Y_i-\widehat p_i).
$$

Therefore

$$
\sum_i\widehat p_i=\sum_iY_i=48
$$

exactly, by the [fitted-mean balance for logistic regression with an intercept](../../../../../fitted-mean-balance-for-logistic-regression-with-an-intercept.md).

The second fit uses [probit regression](../../../../../probit-model.md),

$$
p_i=\Phi(\eta_i),
$$

where $\Phi$ is the [standard normal distribution](../../../../../standard-normal-distribution.md) function. Its intercept score is

$$
\sum_i
\frac{\phi(\eta_i)}{p_i(1-p_i)}(Y_i-p_i)=0,
$$

a weighted residual equation. It does not imply $\sum_i\widehat p_i=48$, so exact equality is not expected. The output should nevertheless be close to $48$: the data were generated with constant success probability $1/2$ independently of $X$, so the fitted slopes should be small, the linear predictors should cluster near a common intercept, and the score weights should be nearly constant.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
