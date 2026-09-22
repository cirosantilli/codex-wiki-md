# Uniform depletion and refill Markov chain

↑ **Parent:** [Uniform depletion Markov chain](uniform-depletion-markov-chain.md)

Refill the stock to a fixed positive size $N$ immediately whenever a step empties it. The resulting [Markov chain](markov-chain-split.md) has [state space](state-space.md) $\{1,\ldots,N\}$ and transitions $P(i,j)=1/i$ for $j<i$ and $P(i,N)=1/i$. It is [irreducible](irreducible-markov-chain.md) and [aperiodic](aperiodic-markov-chain.md), since every state reaches $N$, $N$ reaches every state, and $P(N,N)>0$. Its unique [stationary distribution](stationary-distribution.md) is $\pi_N=1/H_N$ and $\pi_k=1/((k+1)H_N)$ for $k<N$. Normalization is the [harmonic number](harmonic-number.md) identity. For $k<N$, stationarity follows from $\sum_{j=k+1}^{N-1}1/(j(j+1))+1/N=1/(k+1)$; the same telescoping sum starting at $1$ gives stationarity at $N$. The finite-state convergence theorem therefore makes this [stationary distribution](stationary-distribution.md) the limiting distribution from every initial state.

## ↑ Ancestors (8)

1. [Uniform depletion Markov chain](uniform-depletion-markov-chain.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2011/m/m5/b/ii/solution.md)
