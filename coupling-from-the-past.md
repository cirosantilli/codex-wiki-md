# Coupling from the past

↑ **Parent:** [Markov chain Monte Carlo](markov-chain-monte-carlo.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coupling_from_the_past)

[Coupling from the past](coupling-from-the-past.md) uses a fixed two-sided sequence of random update maps for a finite [Markov chain](markov-chain.md). Increase a backward horizon until the composition from that horizon to time zero sends every starting state to the same state. Retain the maps at previously exposed times. The resulting common image is an exact stationary sample. If a length-$m$ block has positive probability $\varepsilon$ of mapping every state to one state, independent disjoint blocks imply failure to coalesce by horizon $T$ has probability at most $(1-\varepsilon)^{\lfloor T/m\rfloor}$. For a deterministic horizon, a stationary initial state yields a stationary final state, and agrees with the algorithm's output on coalescence. Letting the deterministic horizon tend to infinity proves the output has the stationary law without conditioning on a random stopping horizon.

**Table of contents**

- [Monotone coupling from the past](monotone-coupling-from-the-past.md)

## ↑ Ancestors (7)

1. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Coupling from the past](coupling-from-the-past.md)
