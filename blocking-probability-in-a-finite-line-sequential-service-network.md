# Blocking probability in a finite-line sequential-service network

↑ **Parent:** [Closed migration process](closed-migration-process.md)

Represent $N$ telephone lines by a [closed migration process](closed-migration-process.md) with free-line, operator and automated-service colonies. Accepted arrivals have rate $\nu$ when a free line exists, $c$ operators complete at rate $\lambda\min(k,c)$, and $i$ automated calls complete at rate $\mu i$. Define $D_c(k)=\prod_{h=1}^k\min(h,c)$ and

$$
H_c(n)=\sum_{i=0}^n\frac{(\nu/\lambda)^{n-i}(\nu/\mu)^i}{D_c(n-i)i!}.
$$

The [product-form stationary distribution of a closed migration process](product-form-stationary-distribution-of-a-closed-migration-process.md) and [Poisson arrivals see time averages](poisson-arrivals-see-time-averages.md) give the displayed blocking probability. This extends a single-operator model without treating the independent operators as a server with rate $c\lambda$ when fewer than $c$ calls are present.

// Target: probability-and-statistics.bigb

**Table of contents**

- [Stationary flow conservation in a finite-line switchboard](stationary-flow-conservation-in-a-finite-line-switchboard.md)

## ↑ Ancestors (8)

1. [Closed migration process](closed-migration-process.md)
2. [Stochastic network](stochastic-network.md)
3. [Queueing theory](queueing-theory-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-34/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35/1/solution.md)
