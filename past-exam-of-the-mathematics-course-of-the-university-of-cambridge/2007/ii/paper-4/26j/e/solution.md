<h1 id="26j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Treat each arriving caterpillar as one customer in an [M-G-infinity queue](../../../../../../general-service-infinite-server-queue.md), with arrival rate $\lambda$ and service time equal to the sum of its three independent exponential stage lifetimes. This is an Erlang distribution of shape three and rate $\mu$, of mean $3/\mu$. Poisson arrivals independently retained according to whether their service has ended give, in stationarity, a Poisson number in service with mean

$$
\lambda\int_0^\infty P(S>s)\,ds=\lambda\mathbb ES=3\lambda/\mu.
$$

This is exactly the marginal law of $N$ found above. Each individual remains in service across both metamorphoses; counting a fresh service arrival at each stage would be incorrect.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [26J](../../26j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
