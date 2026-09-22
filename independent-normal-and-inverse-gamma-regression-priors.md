# Independent normal and inverse-gamma regression priors

↑ **Parent:** [Polynomial regression](polynomial-regression.md)

With independent [prior distributions](prior-probability.md) $\beta\sim N(\mu,\Sigma)$ and $s\sim\operatorname{IG}(a,b)$ in a [normal distribution](normal-distribution.md) regression model, the conditional [posterior distribution](bayesian-posterior.md) of $\beta$ has [covariance matrix](covariance-matrix.md) $V=(X^TX/s+\Sigma^{-1})^{-1}$ and [mean](expected-value.md) $V(X^Ty/s+\Sigma^{-1}\mu)$. The conditional [posterior distribution](bayesian-posterior.md) of $s$ is [inverse-gamma distribution](inverse-gamma-distribution.md) $\operatorname{IG}(a+n/2,b+\|y-X\beta\|^2/2)$. The shape contains no half-dimension contribution from $\beta$, since its [prior distribution](prior-probability.md) is independent of $s$. These conditionals give a two-block [Gibbs sampler](gibbs-sampler.md).

## ↑ Ancestors (9)

1. [Polynomial regression](polynomial-regression.md)
2. [Linear regression](linear-regression-split.md)
3. [Normal linear model](normal-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/3/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/5/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/5/a/iii/solution.md)
