# Product-Poisson stationary distribution

↑ **Parent:** [Invariant distribution of a continuous-time Markov chain](invariant-distribution-of-a-continuous-time-markov-chain.md)

An [invariant distribution of a continuous-time Markov chain](invariant-distribution-of-a-continuous-time-markov-chain.md) whose coordinates are independent [Poisson distributions](poisson-distribution.md). This property needs verification from the [reaction propensity functions](reaction-propensity-function.md); it does not follow merely from having an equilibrium for the deterministic [reaction-rate equations](rate-equation.md).

For example, consider the cyclic [chemical reaction network](chemical-reaction-network.md) with [stoichiometric vectors](stoichiometric-vector.md) $(1,0)$, $(0,1)$ and $(-1,-1)$ and respective [reaction propensity functions](reaction-propensity-function.md) $\lambda$, $\beta n$, $\gamma nm$, where all three constants are positive. Put $a=\lambda/\beta$ and $b=\beta/\gamma$. For $\pi(n,m)=e^{-a-b}a^nb^m/(n!m!)$, the three incoming terms in the [chemical master equation](chemical-master-equation.md) are respectively $\beta n\pi(n,m)$, $\gamma nm\pi(n,m)$ and $\lambda\pi(n,m)$. They exactly cancel the outgoing terms. Boundary terms vanish by the zero negative-index convention, and normalization follows from the two [Poisson distributions](poisson-distribution.md). Establishing a limiting [probability distribution](probability-distribution-split.md) additionally requires [nonexplosion](nonexplosion-of-a-continuous-time-markov-chain.md), an [irreducible Markov chain](irreducible-markov-chain.md) and [positive recurrence](positive-recurrent-markov-chain.md).

## ↑ Ancestors (9)

1. [Invariant distribution of a continuous-time Markov chain](invariant-distribution-of-a-continuous-time-markov-chain.md)
2. [Continuous-time Markov chain](continuous-time-markov-chain-split.md)
3. [Markov chain](markov-chain-split.md)
4. [Markov process](markov-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford/2023/1/d/solution.md)
