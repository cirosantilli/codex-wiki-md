# Continuous-time Markov chain convergence theorem

↑ **Parent:** [Invariant distribution of a continuous-time Markov chain](invariant-distribution-of-a-continuous-time-markov-chain.md)

A countable [nonexplosive continuous-time Markov chain](nonexplosive-continuous-time-markov-chain.md) which is an [irreducible Markov chain](irreducible-markov-chain.md) and has an [invariant distribution](stationary-distribution.md) $\pi$ is [positive recurrent](positive-recurrent-markov-chain.md); its [transition probabilities](transition-probability.md) tend to $\pi$ from every initial [Markov chain state](markov-chain-state.md).

To see why continuous time removes periodicity, fix $h>0$. Every finite sequence of [Markov chain states](markov-chain-state.md) connected by positive [transition intensities](transition-intensity.md) has positive [probability](probability.md) of finishing before $h$, followed by no further transition until $h$. Consequently the [transition matrix](stochastic-matrix.md) $P_h$ has positive entries between every pair of communicating [Markov chain states](markov-chain-state.md), including its diagonal. It is an [irreducible Markov chain](irreducible-markov-chain.md) and an [aperiodic Markov chain](aperiodic-markov-chain.md) with [stationary distribution](stationary-distribution.md) $\pi$. The [countable-state Markov chain convergence theorem](countable-state-markov-chain-convergence-theorem.md) gives convergence at times $nh$, also in [total variation distance](total-variation-distance.md). For $t=nh+r$, $0\leq r<h$, applying $P_r$ contracts [total variation distance](total-variation-distance.md) and preserves $\pi$, giving the full continuous-time limit.

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
