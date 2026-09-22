# Non-centered Gaussian random-effect parameterization

↑ **Parent:** [Hierarchical Bayesian model](hierarchical-bayesian-model.md)

A normal local effect $\alpha_i\mid\delta,\tau\sim N(\delta,\tau^2)$ can be represented by a standardized [latent variable](latent-variable.md) $z_i\sim N(0,1)$ independent of the hyperparameters, with $\alpha_i=\delta+\tau z_i$. This preserves the hierarchical model while changing the coordinates explored by [Markov chain Monte Carlo](markov-chain-monte-carlo.md). It often improves mixing when individual effects are weakly informed, reducing strong scale-effect dependence. Centered coordinates can be better with very informative individual data. The stochastic prior on $z_i$ implements the transformation correctly; re-expressing an existing density directly instead requires the appropriate [Jacobian determinant](jacobian-determinant.md).

## ↑ Ancestors (7)

1. [Hierarchical Bayesian model](hierarchical-bayesian-model.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/4/b/solution.md)
