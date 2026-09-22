# Quadratic posterior deviance moments

↑ **Parent:** [Effective parameter count in DIC](effective-parameter-count-in-dic.md)

Suppose the [Bayesian deviance](bayesian-deviance.md) is locally $D(\theta)=D(\widehat\theta)+(\theta-\widehat\theta)^TJ(\theta-\widehat\theta)$ with positive-definite $J$, and the posterior is normal with mean $m$ and covariance $\Sigma$. Writing $b=m-\widehat\theta$, expectation and variance of the [quadratic form](quadratic-form.md) give

$$
\mathbb E[D(\theta)\mid y]=D(\widehat\theta)+b^TJb+\operatorname{tr}(J\Sigma),
$$



$$
\operatorname{Var}[D(\theta)\mid y]=2\operatorname{tr}\{(J\Sigma)^2\}+4b^TJ\Sigma Jb.
$$

Consequently the usual [effective parameter count in DIC](effective-parameter-count-in-dic.md) is $p_D=\operatorname{tr}(J\Sigma)$, whereas half the deviance variance is $\operatorname{tr}\{(J\Sigma)^2\}+2b^TJ\Sigma Jb$. A locally flat prior gives $m=\widehat\theta$ and $\Sigma=J^{-1}$, so both counts equal the parameter dimension. Informative priors generally destroy their equality. The expectation formula requires only the first two moments; normality is used for the variance formula.

## ↑ Ancestors (9)

1. [Effective parameter count in DIC](effective-parameter-count-in-dic.md)
2. [Deviance information criterion](deviance-information-criterion.md)
3. [Model selection](model-selection.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/3/d/solution.md)
