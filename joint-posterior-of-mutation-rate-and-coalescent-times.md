# Joint posterior of mutation rate and coalescent times

↑ **Parent:** [Bayesian rejection sampling for a segregating-site count](bayesian-rejection-sampling-for-a-segregating-site-count.md)

For a proper [prior distribution](prior-probability.md) $\pi(\theta)$ independent of coalescent times $T$, let $q(T)=\prod_{j=2}^n\lambda_j e^{-\lambda_jT_j}$ with $\lambda_j=\binom j2$ and $L=\sum jT_j$. Observing $S=k$ under an [infinite sites mutation model](infinite-sites-mutation-model.md) gives [posterior density](posterior-density.md) $\pi(\theta)q(T)e^{-\theta L/2}(\theta L/2)^k/(k!m_k)$, where $m_k$ is the prior predictive [probability](probability.md) of $S=k$. Multiplication by the conditional Poisson mass and normalization is an application of [Bayes' theorem](bayes-theorem.md).

// Target: statistical-inference.bigb

## ↑ Ancestors (7)

1. [Bayesian rejection sampling for a segregating-site count](bayesian-rejection-sampling-for-a-segregating-site-count.md)
2. [Rejection sampling](rejection-sampling.md)
3. [Monte Carlo method](monte-carlo-method.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/3/iii/solution.md)
