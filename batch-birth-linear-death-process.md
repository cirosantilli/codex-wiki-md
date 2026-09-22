# Batch-birth linear-death process

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

A batch-birth linear-death process has transitions

$$
n\longrightarrow n+k\quad\hbox{at rate }\lambda,
\qquad
n\longrightarrow n-1\quad\hbox{at rate }\beta n.
$$

Writing $P_n(t)=\mathbb P(N_t=n)$ and taking $P_j=0$ for $j<0$, its master equation is

$$
\dot P_n=\lambda P_{n-k}+\beta(n+1)P_{n+1}-(\lambda+\beta n)P_n.
$$

**Table of contents**

- [Moments of a batch-birth linear-death process](moments-of-a-batch-birth-linear-death-process.md)

## ↑ Ancestors (8)

1. [Continuous-time Markov chain](continuous-time-markov-chain.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/6c/solution.md)
