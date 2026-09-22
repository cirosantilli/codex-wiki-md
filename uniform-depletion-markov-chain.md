# Uniform depletion Markov chain

↑ **Parent:** [Markov chain](markov-chain-split.md)

A finite stock decreases by choosing a uniformly random positive number of its remaining items at every step. The remaining stock is a [Markov chain](markov-chain-split.md) with $P(i,j)=1/i$ for $0\leq j<i$ and $P(0,0)=1$. State $0$ is an [absorbing state](absorbing-state.md), and every positive state is a [transient state](transient-state.md). If $e_i$ denotes the expected number of positive-stock steps before absorption, a first-step decomposition gives $e_0=0$ and $ie_i=i+\sum_{j<i}e_j$. Subtracting consecutive equations yields $e_i-e_{i-1}=1/i$, so $e_i=H_i$, the $i$th [harmonic number](harmonic-number.md).

**Table of contents**

- [Uniform depletion and refill Markov chain](uniform-depletion-and-refill-markov-chain.md)

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2011/m/m5/a/v/solution.md)
