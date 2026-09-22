<h1 id="pseudo-marginal-metropolis-hastings-algorithm">Pseudo-marginal Metropolis–Hastings algorithm</h1>

↑ **Parent:** [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)

A [pseudo-marginal Metropolis–Hastings algorithm](pseudo-marginal-metropolis-hastings-algorithm.md) replaces an intractable [likelihood function](likelihood-function.md) by a nonnegative [unbiased likelihood estimator](unbiased-likelihood-estimator.md) and includes its auxiliary randomness in the state. If $\mathbb E[\widehat L(\theta,U)]=L(\theta)$ for $U\sim m_\theta$, the extended target is proportional to $p(\theta)\widehat L(\theta,u)m_\theta(u)$. An [independence](independent-random-variables.md) proposal for new auxiliary randomness cancels the $m_\theta$ factors in the [Metropolis–Hastings acceptance probability](metropolis-hastings-acceptance-probability.md). On rejection the old estimate must be retained. Integrating the extended target gives the desired marginal [posterior distribution](bayesian-posterior.md) exactly.

**Table of contents**

- [Unbiased likelihood estimator](unbiased-likelihood-estimator.md)

## ↑ Ancestors (8)

1. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
2. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
3. [Bayesian statistics](bayesian-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/5/b/solution.md)
- [Pseudo-marginal Metropolis–Hastings algorithm](pseudo-marginal-metropolis-hastings-algorithm.md)
