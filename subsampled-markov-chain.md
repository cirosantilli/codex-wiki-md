# Subsampled Markov chain

↑ **Parent:** [Markov chain](markov-chain-split.md)

Let $(X_n)$ be a time-homogeneous [Markov chain](markov-chain-split.md) with [transition matrix](stochastic-matrix.md) $P$, and let $d$ be a positive integer. Then $Y_n=X_{dn}$ is a [Markov chain](markov-chain-split.md) with [transition matrix](stochastic-matrix.md) $P^d$ and the same initial distribution. The Markov property and the [Chapman-Kolmogorov equation](chapman-kolmogorov-equation.md) give $P(X_{d(n+1)}=j\mid X_0,\ldots,X_{dn})=(P^d)_{X_{dn},j}$. Conditioning again on the smaller history $(Y_0,\ldots,Y_n)$ leaves the right-hand side unchanged, since it is determined by $Y_n$. This proves the Markov property of the sampled sequence, rather than only identifying its marginal transition probabilities. Periodicity of the original chain may split the sampled chain into several closed classes.

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2010/m/m2/b/solution.md)
