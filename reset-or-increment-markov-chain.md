# Reset-or-increment Markov chain

↑ **Parent:** [Discrete-time Markov chain](discrete-time-markov-chain.md)

For $0<p<1$, consider the [Markov chain](markov-chain-split.md) on the nonnegative integers with the displayed [transition probabilities](transition-probability.md). From zero it starts a new upward run; from each positive state it either increments or resets. Writing $q=1-p$, its [stationary distribution](stationary-distribution.md) is

$$
\pi_0=\frac{q}{1+q},\qquad \pi_k=\frac{q}{1+q}p^{k-1}\quad(k\geq1).
$$

The balance equations give $\pi_1=\pi_0$ and $\pi_k=p\pi_{k-1}$ for $k\geq2$; the [geometric series](geometric-series.md) normalizes the result, and the zero-state equation $\pi_0=q(1-\pi_0)$ agrees. It is an [irreducible Markov chain](irreducible-markov-chain.md) and is [positive recurrent](positive-recurrent-markov-chain.md). Equivalently, its [first return time](first-return-time.md) to zero is one plus a [geometric random variable](geometric-distribution.md) with success probability $q$, so its [mean recurrence time](mean-recurrence-time.md) is $1+1/q$. Return paths of lengths two and three also make it [aperiodic](aperiodic-markov-chain.md).

**Table of contents**

- [Growth rate of two-column sticky deposition](growth-rate-of-two-column-sticky-deposition.md)

## ↑ Ancestors (8)

1. [Discrete-time Markov chain](discrete-time-markov-chain.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Growth rate of two-column sticky deposition](growth-rate-of-two-column-sticky-deposition.md)
- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2017/3/b/i/solution.md)
