# Poisson-sampled continuous-time Markov chain

↑ **Parent:** [Transition semigroup of a continuous-time Markov chain](transition-semigroup-of-a-continuous-time-markov-chain.md)

Sample a finite-state [continuous-time Markov chain](continuous-time-markov-chain.md) with generator $Q$ at the independent arrival times of a rate-$\lambda$ [Poisson process](poisson-process.md). The sampled states form a discrete-time Markov chain with transition matrix

$$
P_\lambda
=\int_0^\infty\lambda e^{-\lambda t}e^{tQ}\,dt
=\lambda(\lambda I-Q)^{-1}.
$$

Its invariant distributions are exactly those of the continuous-time chain.

## ↑ Ancestors (9)

1. [Transition semigroup of a continuous-time Markov chain](transition-semigroup-of-a-continuous-time-markov-chain.md)
2. [Continuous-time Markov chain](continuous-time-markov-chain.md)
3. [Markov chain](markov-chain.md)
4. [Markov process](markov-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/27j/solution.md)
