# Independent stationary proposal lemma

↑ **Parent:** [Independence Metropolis–Hastings algorithm](independence-metropolis-hastings-algorithm.md)

If a [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md) proposes fresh draws from its target [stationary distribution](stationary-distribution.md) $\pi$, its acceptance ratio on the positive support is $\pi(y)\pi(x)/(\pi(x)\pi(y))=1$. Therefore every proposal is accepted, and $P(x,y)=\pi(y)$. From the first update onward the recorded states are [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with law $\pi$, regardless of the initial state in the support. An arbitrary initial state is excluded when claiming an unbiased finite-sample average.

## ↑ Ancestors (9)

1. [Independence Metropolis–Hastings algorithm](independence-metropolis-hastings-algorithm.md)
2. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
3. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
4. [Bayesian statistics](bayesian-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/1/b/solution.md)
