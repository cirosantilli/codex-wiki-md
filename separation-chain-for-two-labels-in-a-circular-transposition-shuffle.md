# Separation chain for two labels in a circular transposition shuffle

↑ **Parent:** [Random transposition shuffle](random-transposition-shuffle.md)

In a [random transposition shuffle](random-transposition-shuffle.md) on a six-cycle, the shorter circular distance between two distinguished labels takes values $1,2,3$. The symmetry of the cycle and exchangeability of other labels make this a [lumped Markov chain](lumped-markov-chain.md). Counting the fifteen possible transpositions gives [transition matrix](stochastic-matrix.md) $P=\frac1{15}\begin{pmatrix}9&4&2\\4&9&2\\4&4&7\end{pmatrix}$. Its [stationary distribution](stationary-distribution.md) is $(2/5,2/5,1/5)$ and $P=\frac13I+\frac23\Pi$, where each row of $\Pi$ is this [stationary distribution](stationary-distribution.md). Consequently the probability of opposite labels after $n$ steps from adjacent labels is $(1-3^{-n})/5$.

## ↑ Ancestors (8)

1. [Random transposition shuffle](random-transposition-shuffle.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/19d/solution.md)
