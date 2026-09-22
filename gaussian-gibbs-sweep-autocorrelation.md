# Gaussian Gibbs sweep autocorrelation

↑ **Parent:** [Gibbs sampler](gibbs-sampler.md)

In a systematic [Gibbs sampler](gibbs-sampler.md) for a standardized [bivariate normal distribution](bivariate-normal-distribution.md) with [correlation](pearson-correlation-coefficient.md) $\rho$, update $Z_1$ conditionally on the old $Z_2$, then update $Z_2$ using the new $Z_1$. Substitution gives the displayed [autoregressive process of order one](autoregressive-process-of-order-one.md), with [independent](independent-random-variables.md) noises with the [standard normal distribution](standard-normal-distribution.md) $\eta_{1,r},\eta_{2,r}$. The sweep-to-sweep [autocorrelation](autocorrelation.md) of $Z_2$ at lag $h$ is $\rho^{2h}$, so the chain mixes slowly as $|\rho|$ approaches one.

## ↑ Ancestors (8)

1. [Gibbs sampler](gibbs-sampler.md)
2. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
3. [Bayesian statistics](bayesian-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/2/ii/solution.md)
