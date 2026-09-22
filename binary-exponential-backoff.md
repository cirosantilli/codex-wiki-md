# Binary exponential backoff

↑ **Parent:** [Exponential backoff](exponential-backoff.md)

After $k$ collisions a packet chooses an independent counter uniformly from $\{0,\ldots,2^k-1\}$ and retries when it expires. The window doubles after a further collision. This is an example of [exponential backoff](exponential-backoff.md) with a nonconstant retry rule, contrasting with constant-probability [slotted ALOHA](slotted-aloha.md).

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

## ← Incoming links (3)

- [Geometric-attempt exponential backoff](geometric-attempt-exponential-backoff.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32/3/solution.md)
