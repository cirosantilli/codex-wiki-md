# Backlog-aware ALOHA with arrival-adjusted attempt probabilities

↑ **Parent:** [Slotted ALOHA](slotted-aloha.md)

In infinite-population [slotted ALOHA](slotted-aloha.md), suppose new arrivals form an independent Poisson variable of mean $\eta$ per slot and attempt immediately. At backlog $b\ge1$, let old packets attempt independently with probability $p_b$. Their total attempted load tends to $1-\eta$, so the total offered attempts tend to one and the success probability tends to $e^{-1}$. For $0<\eta<e^{-1}$ the backlog has strictly negative drift outside a finite set, and [Foster theorem](foster-s-theorem.md) proves a [positive recurrent Markov chain](positive-recurrent-markov-chain.md). This mathematical benchmark requires exact backlog information; a practical feedback estimate needs its own analysis.

// Target: probability-and-statistics.bigb

## ↑ Ancestors (9)

1. [Slotted ALOHA](slotted-aloha.md)
2. [Random access network](random-access-network.md)
3. [Stochastic network](stochastic-network.md)
4. [Queueing theory](queueing-theory-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-73/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35/3/solution.md)
