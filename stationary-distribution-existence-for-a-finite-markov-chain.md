# Stationary distribution existence for a finite Markov chain

↑ **Parent:** [Stationary distribution](stationary-distribution.md)

Every [finite Markov chain](finite-markov-chain.md) has a [stationary distribution](stationary-distribution.md), without requiring [Markov chain irreducibility](irreducible-markov-chain.md) or [aperiodicity](aperiodic-markov-chain.md). For a row-[stochastic matrix](stochastic-matrix.md) $P$, put $B=P^T$ and choose a column [probability vector](probability-vector.md) $q$. Every $B^jq$ lies in the [probability simplex](probability-simplex.md). Their arithmetic averages $x_N=N^{-1}\sum_{j=0}^{N-1}B^jq$ therefore lie in this [compact set](compact-space.md), while telescoping gives

$$
Bx_N-x_N=\frac{B^Nq-q}{N},\qquad \|Bx_N-x_N\|_1\leq\frac2N.
$$

A [convergent subsequence](convergent-subsequence.md) has a [limit](limit-of-a-function.md) $x$ in the [probability simplex](probability-simplex.md). [Continuity](continuous-function.md) of [matrix multiplication](matrix-multiplication.md) gives $Bx=x$, so $\pi=x^T$ is a [stationary distribution](stationary-distribution.md). The individual iterates need not converge: a deterministic two-state swap alternates its point masses forever.

## ↑ Ancestors (8)

1. [Stationary distribution](stationary-distribution.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/2/d/solution.md)
