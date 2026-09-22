# Minimum of an upward-biased random walk

↑ **Parent:** [Biased random walk](biased-random-walk.md)

Let $S_0=0$ and let the [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) $S_n-S_{n-1}$ be $+1$ with [probability](probability.md) $p>1/2$ and $-1$ with [probability](probability.md) $q=1-p>0$. The [strong law of large numbers](strong-law-of-large-numbers.md) gives $S_n\to+\infty$ [almost surely](almost-sure-convergence.md), so the global [minimum](minimum-of-a-subset-of-a-total-order.md) $W$ is finite and attained. For each [nonnegative integer](natural-number.md) $m$, the unit-step property and translation of the starting point give

$$
\mathbb P(-W\geq m)=\mathbb P_0(T_{-m}<\infty)
=\mathbb P_m(T_0<\infty)=(q/p)^m
$$

by the [biased random walk hitting probability](biased-random-walk-hitting-probability.md). Subtracting consecutive tails gives the displayed zero-based [geometric distribution](geometric-distribution.md), with success parameter $1-q/p$. Inclusion of time zero is important: it ensures $-W\geq0$. Reflecting the sign of the path yields the corresponding [maximum of a downward-biased random walk](maximum-of-a-downward-biased-random-walk.md).

## ↑ Ancestors (11)

1. [Biased random walk](biased-random-walk.md)
2. [Simple random walk on the integer line](simple-random-walk-on-the-integer-line.md)
3. [Random walk on a graph](random-walk-on-a-graph.md)
4. [Random walk](random-walk-split.md)
5. [Markov chain](markov-chain-split.md)
6. [Markov process](markov-process-split.md)
7. [Probability theory](probability-theory-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2015/3/c/i/solution.md)
