# Metropolis-within-Gibbs algorithm

↑ **Parent:** [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)

A [Metropolis-within-Gibbs](metropolis-within-gibbs-algorithm.md) sweep updates one coordinate or block at a time by a [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md) transition whose invariant law is that block's [full conditional distribution](full-conditional-distribution.md). For a proposal changing only block $j$, the acceptance ratio uses the full joint target with the other coordinates fixed, together with the reverse/forward proposal ratio. Each block kernel preserves the joint [posterior](bayesian-posterior.md), so their composition does as well. Conjugate blocks can instead use exact [Gibbs sampling](gibbs-sampler.md) draws. Systematic composition need not be reversible, even when every block kernel is reversible.

## ↑ Ancestors (8)

1. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
2. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
3. [Bayesian statistics](bayesian-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/5/iv/solution.md)
