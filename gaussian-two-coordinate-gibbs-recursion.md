# Gaussian two-coordinate Gibbs recursion

↑ **Parent:** [Gibbs sampler](gibbs-sampler.md)

For a standard bivariate [normal distribution](normal-distribution.md) with correlation $\rho$, each conditional has variance $1-\rho^2$ and mean $\rho$ times the other coordinate. A sweep draws $X_{n+1}=\rho Y_n+\sqrt{1-\rho^2}Z_1$, then $Y_{n+1}=\rho X_{n+1}+\sqrt{1-\rho^2}Z_2$. The resulting coordinate chain is an [AR(1)](autoregressive-process-of-order-one.md) process with coefficient $\rho^2$ and innovation variance $1-\rho^4$. It shows explicitly why near-unit correlation slows successive Gibbs sweeps.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/5/b/solution.md)
