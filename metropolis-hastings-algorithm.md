<h1 id="metropolis-hastings-algorithm">Metropolis–Hastings algorithm</h1>

↑ **Parent:** [Markov chain Monte Carlo](markov-chain-monte-carlo.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metropolis–Hastings_algorithm)

The Metropolis–Hastings algorithm proposes $y$ from $q(x,\mathord\cdot)$ at state $x$ and accepts it with probability

$$
1\wedge\frac{\pi(y)q(y,x)}{\pi(x)q(x,y)}.
$$

This acceptance rule enforces [detailed balance](detailed-balance.md) with the target density $\pi$.

**Table of contents**

- [Metropolis-within-Gibbs algorithm](metropolis-within-gibbs-algorithm.md)
- [Pseudo-marginal Metropolis–Hastings algorithm](pseudo-marginal-metropolis-hastings-algorithm.md)
  - [Unbiased likelihood estimator](unbiased-likelihood-estimator.md)
- [Metropolis–Hastings acceptance probability](metropolis-hastings-acceptance-probability.md)
- [Proposal distribution](proposal-distribution.md)
  - [Involutive Metropolis proposal](involutive-metropolis-proposal.md)
  - [Orthogonal-mixture Metropolis proposal](orthogonal-mixture-metropolis-proposal.md)
  - [Gaussian autoregressive proposal reversible with respect to a standard normal distribution](gaussian-autoregressive-proposal-reversible-with-respect-to-a-standard-normal-distribution.md)
    - [Preconditioned Crank–Nicolson algorithm](preconditioned-crank-nicolson-algorithm.md)
- [Random-walk Metropolis algorithm](random-walk-metropolis-algorithm.md)
  - [Positive-parameter random walk with boundary rejection](positive-parameter-random-walk-with-boundary-rejection.md)
  - [Proposal scale and random-walk Metropolis efficiency](proposal-scale-and-random-walk-metropolis-efficiency.md)
- [Independence Metropolis–Hastings algorithm](independence-metropolis-hastings-algorithm.md)

## ↑ Ancestors (7)

1. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (28)

- [Metropolis-within-Gibbs algorithm](metropolis-within-gibbs-algorithm.md)
- [Orthogonal-mixture Metropolis proposal](orthogonal-mixture-metropolis-proposal.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/4/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/26j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/6/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/2/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-219/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/28j/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-219/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-219/2/c/solution.md)
- [Preconditioned Crank–Nicolson algorithm](preconditioned-crank-nicolson-algorithm.md)
- [Proposal distribution](proposal-distribution.md)
- [Spatial Bernoulli infection model](spatial-bernoulli-infection-model.md)
