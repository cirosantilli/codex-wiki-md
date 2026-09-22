# Mean delay under independent exponential-backoff failures

↑ **Parent:** [Geometric-attempt exponential backoff](geometric-attempt-exponential-backoff.md)

For [geometric-attempt exponential backoff](geometric-attempt-exponential-backoff.md), assume each attempted transmission fails independently with a fixed probability $q<1$. The probability of reaching stage $k$ is $q^k$, and its mean waiting time is $2^k/p_0$. The [Tonelli theorem](tonelli-theorem.md) gives $\mathbb ET=p_0^{-1}\sum_{k\ge0}(2q)^k$, finite exactly when $q<1/2$. The packet succeeds almost surely for every $q<1$, so almost-sure success does not guarantee finite mean delay. A fixed independent failure probability is a simplifying assumption, not a theorem about collisions in an interacting network.

// Target: probability-and-statistics.bigb

## ↑ Ancestors (10)

1. [Geometric-attempt exponential backoff](geometric-attempt-exponential-backoff.md)
2. [Exponential backoff](exponential-backoff.md)
3. [Random access network](random-access-network.md)
4. [Stochastic network](stochastic-network.md)
5. [Queueing theory](queueing-theory-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35/3/solution.md)
