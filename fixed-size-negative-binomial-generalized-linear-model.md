# Fixed-size negative binomial generalized linear model

↑ **Parent:** [Negative binomial regression](negative-binomial-regression.md)

For known size $\theta>0$, the [negative binomial distribution](negative-binomial-distribution.md) is an [exponential family](exponential-family-split.md) with natural parameter $\eta=\log[\mu/(\theta+\mu)]<0$ and cumulant $b_\theta(\eta)=-\theta\log(1-e^\eta)$. A [generalized linear model](generalized-linear-model.md) can use a [logarithmic link function](logarithmic-link-function.md) for its mean, even though that link is not canonical. Jointly estimating the size changes the family and [variance function](variance-function.md), requiring additional updates beyond a single fixed-family GLM fit; this is what `MASS::glm.nb` does.

**Table of contents**

- [Negative binomial deviance](negative-binomial-deviance.md)

## ↑ Ancestors (8)

1. [Negative binomial regression](negative-binomial-regression.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/3/d/solution.md)
