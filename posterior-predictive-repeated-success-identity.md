# Posterior predictive repeated-success identity

↑ **Parent:** [Posterior predictive distribution](posterior-predictive-distribution.md)

If future [Bernoulli random variables](bernoulli-distribution.md) are conditionally independent given a shared parameter $\Theta$, with success [probability](probability.md) $\pi(\Theta)$, their all-success [conditional probability](conditional-probability.md) is $\pi(\Theta)^k$. Taking a posterior [expectation](expected-value-split.md) proves the identity. For $k\geq1$, [Jensen's inequality](jensen-s-inequality.md) and $0\leq\pi\leq1$ give $(\mathbb E[\pi\mid D])^k\leq\mathbb E[\pi^k\mid D]\leq\mathbb E[\pi\mid D]$. For two distinct future trials the posterior [covariance](covariance.md) is $\mathbb E[\pi^2\mid D]-(\mathbb E[\pi\mid D])^2=\operatorname{Var}(\pi\mid D)$. Thus shared parameter uncertainty can induce positive dependence even when trials are conditionally independent.

## ↑ Ancestors (8)

1. [Posterior predictive distribution](posterior-predictive-distribution.md)
2. [Bayesian posterior](bayesian-posterior.md)
3. [Bayesian statistics](bayesian-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/3/d/solution.md)
