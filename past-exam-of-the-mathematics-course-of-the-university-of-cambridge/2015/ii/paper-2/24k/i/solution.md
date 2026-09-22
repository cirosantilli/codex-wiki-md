<h1 id="24k/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A rate-$\lambda$ [Poisson process](../../../../../../poisson-process.md) is a counting process starting at zero, with right-continuous nondecreasing integer-valued paths, independent stationary increments, and $N_t-N_s\sim\operatorname{Pois}(\lambda(t-s))$ for $0\leq s<t$. Its jumps have size one almost surely.

For independent [Poisson processes](../../../../../../poisson-process.md) $N,M$, increments of $N+M$ on disjoint intervals are independent, because all the corresponding increments of the two processes are jointly independent. On an interval of length $t$, multiplying their [probability generating functions](../../../../../../probability-generating-function.md) gives

$$
\exp(\lambda t(z-1))\exp(\mu t(z-1))=\exp((\lambda+\mu)t(z-1)).
$$

Thus the increment is Poisson with mean $(\lambda+\mu)t$. The path requirements hold, and independent processes almost surely have no simultaneous jumps. Therefore **$N+M$ is a [Poisson process](../../../../../../poisson-process.md) of rate $\lambda+\mu$**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [24K](../../24k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
