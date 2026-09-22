# Maximum of a downward-biased random walk

↑ **Parent:** [Biased random walk](biased-random-walk.md)

For a nearest-neighbour [random walk](random-walk.md) with upward probability $0<p<q=1-p$, start at $S_0=0$ and put $M=\sup_{n\geq0}S_n$. Its [probability distribution](probability-distribution.md) is geometric on the nonnegative integers, with the displayed mass and [expected value](expected-value.md) $p/(q-p)$. To prove this, the [exponential martingale of a biased simple random walk](exponential-martingale-of-a-biased-simple-random-walk.md) $Z_n=(q/p)^{S_n}$ has expectation one. Stop at the first hit $H_k$ of $k$. Before that hit, $Z_{n\wedge H_k}\leq(q/p)^k$; the [strong law of large numbers](strong-law-of-large-numbers.md) gives $S_n\to-\infty$ on paths without a hit. [Dominated convergence theorem](dominated-convergence-theorem.md) therefore gives $1=(q/p)^k\mathbb P(H_k<\infty)$. Taking differences of $\mathbb P(M\geq k)=(p/q)^k$ yields the mass. If time zero is excluded, the maximum can equal $-1$ with probability $q-p$ and does not have this nonnegative [geometric distribution](geometric-distribution.md).

## ↑ Ancestors (10)

1. [Biased random walk](biased-random-walk.md)
2. [Random walk on a graph](random-walk-on-a-graph.md)
3. [Random walk](random-walk.md)
4. [Markov chain](markov-chain.md)
5. [Markov process](markov-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/1/c/iii/solution.md)
