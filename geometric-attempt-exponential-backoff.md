# Geometric-attempt exponential backoff

↑ **Parent:** [Exponential backoff](exponential-backoff.md)

A packet with $k$ previous collisions attempts independently in each slot with probability $p_k=p_0 2^{-k}$. On failure it advances to stage $k+1$, and on success it leaves. The [Markov chain](markov-chain.md) state records the number of packets at every stage, rather than only the total backlog. This memoryless-window model is related to [binary exponential backoff](binary-exponential-backoff.md), but its geometric waiting times differ from uniform counters in finite retry windows.

// Target: probability-and-statistics.bigb

**Table of contents**

- [Mean delay under independent exponential-backoff failures](mean-delay-under-independent-exponential-backoff-failures.md)

## ↑ Ancestors (9)

1. [Exponential backoff](exponential-backoff.md)
2. [Random access network](random-access-network.md)
3. [Stochastic network](stochastic-network.md)
4. [Queueing theory](queueing-theory-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Mean delay under independent exponential-backoff failures](mean-delay-under-independent-exponential-backoff-failures.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35/3/solution.md)
