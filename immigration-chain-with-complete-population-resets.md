# Immigration chain with complete population resets

↑ **Parent:** [Markov chain](markov-chain-split.md)

From state zero the chain always goes to one. From a positive [integer](integer-split.md) $j$, it resets to zero with probability $p$ and goes to $j+1$ otherwise. The stationary equations give $\pi_1=\pi_0$ and $\pi_j=(1-p)^{j-1}\pi_0$, and normalization gives the displayed distribution. The chain is [irreducible](irreducible-representation.md) and [positive recurrent](positive-recurrent-markov-chain.md); its return lengths two and three also make it [aperiodic](aperiodic-markov-chain.md). The long-run proportion of time above a positive [integer](integer-split.md) $K$ is $(1-p)^K/(1+p)$.

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
