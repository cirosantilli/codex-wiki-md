# Concavity of the Poisson regression likelihood

↑ **Parent:** [Poisson regression](poisson-regression.md)

For a full-column-rank design $X$ and positive fitted means $\mu_i=\exp(x_i^T\beta)$, the [log-likelihood](log-likelihood.md) has Hessian $-X^T\operatorname{diag}(\mu_i)X$, which is negative definite. Thus any finite stationary point is the unique [maximum-likelihood estimator](maximum-likelihood-estimator.md). Full rank does not guarantee existence: with an intercept and all counts zero, the supremum is approached as the intercept tends to $-\infty$. If every observed count is positive, a full-rank design does give a finite maximum: each function $y_i\eta_i-e^{\eta_i}$ tends to $-\infty$ in either tail and is bounded above, and $\|X\beta\|\to\infty$ as $\|\beta\|\to\infty$, so the negative [log-likelihood](log-likelihood.md) is coercive.

## ↑ Ancestors (8)

1. [Poisson regression](poisson-regression.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37/1/i/solution.md)
