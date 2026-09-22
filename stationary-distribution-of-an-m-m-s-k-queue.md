# Stationary distribution of an M-M-s-K queue

↑ **Parent:** [M-M-s-K queue](m-m-s-k-queue.md)

Put $\rho=\lambda/\mu$. The unique stationary distribution of an $M/M/s/K$ queue is

$$
\pi_n=\frac1Z
\begin{cases}
\rho^n/n!,&0\leq n\leq s,\\
\rho^n/(s!s^{n-s}),&s<n\leq K,
\end{cases}
$$

where $Z$ is the sum of the displayed weights. Adjacent terms satisfy [detailed balance for a birth-death process](detailed-balance-for-a-birth-death-process.md), so the queue is reversible in equilibrium.

## ↑ Ancestors (10)

1. [M-M-s-K queue](m-m-s-k-queue.md)
2. [Birth-death process](birth-death-process.md)
3. [Continuous-time Markov chain](continuous-time-markov-chain.md)
4. [Markov chain](markov-chain.md)
5. [Markov process](markov-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/27k/b/solution.md)
