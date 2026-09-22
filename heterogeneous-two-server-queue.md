# Heterogeneous two-server queue

↑ **Parent:** [Queueing theory](queueing-theory-split.md)

A queue with a [Poisson process](poisson-process.md) of arrivals and two independent [service times](service-time.md) with [exponential distributions](exponential-distribution.md) of different rates must distinguish the two possible single-customer states. If an arrival chooses either idle server with probability $1/2$, the [continuous-time Markov chain](continuous-time-markov-chain.md) is [reversible](reversible-markov-chain.md). Write $a,b$ for the states with only server one or two busy, and $n\geq2$ for total population. Its [detailed balance equations](detailed-balance.md) give $\pi_a=\pi_0\nu/(2\mu_1)$, $\pi_b=\pi_0\nu/(2\mu_2)$ and $\pi_n=\pi_0\nu^2(\nu/\mu)^{n-2}/(2\mu_1\mu_2)$. These weights normalize exactly when $\nu<\mu$. In equilibrium, reversed upward transitions have total rate $\nu$ in every state, so [time reversal of a continuous-time Markov chain](time-reversal-of-a-continuous-time-markov-chain.md) makes the departure stream a [Poisson process](poisson-process.md) of rate $\nu$. This output conclusion requires stationarity.

## ↑ Ancestors (6)

1. [Queueing theory](queueing-theory-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30/1/i/solution.md)
