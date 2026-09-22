# Embedded departure chain of an M-G-1 queue

↑ **Parent:** [M/G/1 queue](m-g-1-queue.md)

Let $Q_n$ be the number left immediately after departure $n$, and let $A_n$ be the arrivals during the next service. Then

$$
Q_{n+1}=Q_n-\mathbf1_{\{Q_n>0\}}+A_n.
$$

Conditional on service duration $S$, $A_n$ is Poisson with parameter $\lambda S$, so

$$
\mathbb EA_n=\lambda\mathbb ES,
\qquad
\mathbb EA_n^2=\lambda\mathbb ES+\lambda^2\mathbb ES^2.
$$

**Table of contents**

- [Pollaczek-Khinchine formula](pollaczek-khinchine-formula.md)
  - [Pollaczek-Khinchine mean formula](pollaczek-khinchine-mean-formula.md)

## ↑ Ancestors (7)

1. [M/G/1 queue](m-g-1-queue.md)
2. [Queueing theory](queueing-theory-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/27j/solution.md)
