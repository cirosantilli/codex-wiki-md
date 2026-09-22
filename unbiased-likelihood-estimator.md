# Unbiased likelihood estimator

↑ **Parent:** [Pseudo-marginal Metropolis–Hastings algorithm](pseudo-marginal-metropolis-hastings-algorithm.md)

An [unbiased likelihood estimator](unbiased-likelihood-estimator.md) has expectation equal to the [likelihood function](likelihood-function.md) at each parameter. A [pseudo-marginal algorithm](pseudo-marginal-metropolis-hastings-algorithm.md) requires this estimator to be nonnegative. [Importance sampling](importance-sampling.md) provides $\widehat L=M^{-1}\sum_j\ell(F_j)p_\theta(F_j)/g_\theta(F_j)$ for [independent random variables](independent-random-variables.md) $F_j\sim g_\theta$, provided the proposal covers the target support. Relative [variance](variance-split.md) affects the [mixing time](mixing-time-of-a-markov-chain.md) even though unbiasedness guarantees the correct marginal target.

## ↑ Ancestors (9)

1. [Pseudo-marginal Metropolis–Hastings algorithm](pseudo-marginal-metropolis-hastings-algorithm.md)
2. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
3. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
4. [Bayesian statistics](bayesian-statistics.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/5/b/solution.md)
- [Pseudo-marginal Metropolis–Hastings algorithm](pseudo-marginal-metropolis-hastings-algorithm.md)
- [Unbiased likelihood estimator](unbiased-likelihood-estimator.md)
