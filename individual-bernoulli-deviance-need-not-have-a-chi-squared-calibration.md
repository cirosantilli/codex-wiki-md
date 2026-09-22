# Individual Bernoulli deviance need not have a chi-squared calibration

↑ **Parent:** [Deviance goodness-of-fit test](deviance-goodness-of-fit-test.md)

A [logistic regression](logistic-regression.md) fitted to ungrouped [Bernoulli](bernoulli-distribution.md) observations has [residual deviance](residual-deviance.md) $D=-2\ell(\widehat\beta)$. Comparing it automatically with $\chi^2_{n-p}$ is generally invalid: the saturated dimension grows with $n$, with one observation per fitted probability. If the true model has only an intercept and success probability $1/2$, then $D/n\to2\log2$, whereas $\chi^2_{n-1}/n\to1$. Fixed-dimensional nested-model [likelihood-ratio tests](likelihood-ratio-test.md) can still use [Wilks theorem](wilks-theorem.md) under regularity. For absolute fit, use meaningful grouping, residual diagnostics, or a fitted-model [parametric bootstrap](parametric-bootstrap.md).

## ↑ Ancestors (8)

1. [Deviance goodness-of-fit test](deviance-goodness-of-fit-test.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38/3/b/solution.md)
