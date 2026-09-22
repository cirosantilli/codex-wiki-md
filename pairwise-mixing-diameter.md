# Pairwise mixing diameter

↑ **Parent:** [Mixing time of a Markov chain](mixing-time-of-a-markov-chain.md)

For a finite [Markov chain](markov-chain.md) with [transition matrix](stochastic-matrix.md) $P$, define $\bar d(t)=\max_{x,y}\|P^t(x,\cdot)-P^t(y,\cdot)\|_{\mathrm{TV}}$. If $\pi$ is a [stationary distribution](stationary-distribution.md) and $d(t)=\max_x\|P^t(x,\cdot)-\pi\|_{\mathrm{TV}}$, then $d(t)\leq\bar d(t)\leq2d(t)$. The first bound follows by writing $\pi=\sum_y\pi(y)P^t(y,\cdot)$ and using the [triangle inequality](triangle-inequality.md); the second uses the [triangle inequality](triangle-inequality.md) through $\pi$.

## ↑ Ancestors (8)

1. [Mixing time of a Markov chain](mixing-time-of-a-markov-chain.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/1/c/solution.md)
