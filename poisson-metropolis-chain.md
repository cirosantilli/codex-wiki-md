# Poisson Metropolis chain

↑ **Parent:** [Random-walk Metropolis algorithm](random-walk-metropolis-algorithm.md)

A [Poisson Metropolis chain](poisson-metropolis-chain.md) samples a [Poisson distribution](poisson-distribution.md) by proposing an upward or downward unit step with equal [probability](probability.md) and reflecting a downward proposal at zero into a self-proposal. Its upward and downward [transition probabilities](transition-probability.md) are the displayed $u_n,d_n$, with $d_0=0$, and the diagonal entry is $1-u_n-d_n$. For $\pi_n=e^{-\lambda}\lambda^n/n!$, adjacent stationary fluxes equal $\tfrac12\min(\pi_n,\pi_{n+1})$. Hence [detailed balance](detailed-balance.md) holds. Positive adjacent [probabilities](probability.md) imply an [irreducible Markov chain](irreducible-markov-chain.md); $P(0,0)\geq1/2$ implies [aperiodicity](aperiodic-markov-chain.md). The normalized invariant [Poisson distribution](poisson-distribution.md) implies [positive recurrence](positive-recurrent-markov-chain.md), so the [countable-state Markov chain convergence theorem](countable-state-markov-chain-convergence-theorem.md) applies. The boundary proposal [probability](probability.md) is essential: forcing every proposal at zero to go upward would require a different acceptance ratio.

## ↑ Ancestors (9)

1. [Random-walk Metropolis algorithm](random-walk-metropolis-algorithm.md)
2. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
3. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
4. [Bayesian statistics](bayesian-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/1/e/solution.md)
- [Poisson Metropolis chain](poisson-metropolis-chain.md)
