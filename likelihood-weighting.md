# Likelihood weighting

↑ **Parent:** [Importance sampling](importance-sampling.md)

[Likelihood weighting](likelihood-weighting.md) uses observation [likelihoods](likelihood-function.md) as [importance weights](importance-weight.md). If parameters are drawn independently from their [prior distribution](prior-probability.md) $\rho$, weight a draw by $L(\theta)$ and estimate a posterior [expectation](expected-value-split.md) of $h$ by $\sum_jL(\theta_j)h(\theta_j)/\sum_jL(\theta_j)$. With positive finite evidence and integrable weighted quantities, the [strong law of large numbers](strong-law-of-large-numbers.md) proves consistency of this [self-normalized importance sampling](self-normalized-importance-sampling.md) ratio. Finite-sample [bias](bias-of-an-estimator.md) and concentration of the weights remain possible. A different proposal requires the additional [prior density](prior-density.md)-to-proposal density ratio.

## ↑ Ancestors (6)

1. [Importance sampling](importance-sampling.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Likelihood weighting](likelihood-weighting.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/3/e/solution.md)
