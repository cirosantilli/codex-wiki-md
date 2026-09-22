# Logistic-normal regression with autoregressive random effects

↑ **Parent:** [Logistic regression](logistic-regression.md)

A logistic-normal count model takes $Y_i\mid\theta_i\sim\operatorname{Bin}(n_i,\operatorname{logit}^{-1}\theta_i)$ and $\theta_i=x_i^T\beta+\lambda Z_i+\eta_i$, where $Z$ is a stationary unit-variance [autoregressive process of order one](autoregressive-process-of-order-one.md) with coefficient $a$ and the independent $\eta_i$ have [normal distribution](normal-distribution.md) with variance $v$. The marginal latent variance is $\lambda^2+v$, and its off-diagonal [covariance](covariance.md) is $\lambda^2 a^{|i-j|}$. Random success probabilities produce [overdispersion](overdispersion.md) relative to the [binomial distribution](binomial-distribution.md).

## ↑ Ancestors (8)

1. [Logistic regression](logistic-regression.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/3/a/solution.md)
