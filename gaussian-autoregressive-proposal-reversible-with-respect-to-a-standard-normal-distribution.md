# Gaussian autoregressive proposal reversible with respect to a standard normal distribution

↑ **Parent:** [Proposal distribution](proposal-distribution.md)

Let $0<\beta\leq1$, let $X\in\mathbb R^p$, and propose

$$
Y=\sqrt{1-\beta^2}\,X+\beta Z,
\qquad Z\sim N(0,I_p).
$$

The [proposal distribution](proposal-distribution.md) is $N(\sqrt{1-\beta^2}\,X,\beta^2I_p)$. If $X\sim N(0,I_p)$ independently of $Z$, then $(X,Y)$ is a jointly [multivariate normal distribution](multivariate-normal-distribution.md) invariant under exchanging $X$ and $Y$, because both [random vectors](random-vector.md) have [covariance matrix](covariance-matrix.md) $I_p$ and their cross-covariance matrices are both $\sqrt{1-\beta^2}I_p$. Consequently its density $q$ satisfies

$$
\phi(x)q(y\mid x)=\phi(y)q(x\mid y),
$$

where $\phi$ is the standard-normal density. Thus the proposal is [reversible](reversible-markov-chain.md) with respect to the standard normal distribution.

**Table of contents**

- [Preconditioned Crank–Nicolson algorithm](preconditioned-crank-nicolson-algorithm.md)

## ↑ Ancestors (9)

1. [Proposal distribution](proposal-distribution.md)
2. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
3. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
4. [Bayesian statistics](bayesian-statistics.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/28j/ii/solution.md)
- [Preconditioned Crank–Nicolson algorithm](preconditioned-crank-nicolson-algorithm.md)
