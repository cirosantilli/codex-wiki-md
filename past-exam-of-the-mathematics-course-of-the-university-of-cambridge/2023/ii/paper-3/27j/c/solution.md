<h1 id="27j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [M/M/1 queue](../../../../../../m-m-1-queue.md), the first service lasts on average $1/\mu$. During it, the mean number of arrivals is $\lambda/\mu$, and each arrival initiates another statistically identical busy-period family. Thus, when $\lambda<\mu$,

$$
\mathbb EB
=\frac1\mu+\frac\lambda\mu\mathbb EB,
$$

so the [mean busy period of an M-M-1 queue](../../../../../../mean-busy-period-of-an-m-m-1-queue.md) is

$$
\boxed{\mathbb EB_{M/M/1}=\frac1{\mu-\lambda}.}
$$

For $\lambda=\mu$ the busy period is almost surely finite but has infinite mean, while for $\lambda>\mu$ it is infinite with positive probability; in either case its expectation is infinite.

For an [M-M-infinity queue](../../../../../../m-m-%E2%88%9E-queue.md), stationary occupancy is [Poisson](../../../../../../poisson-distribution.md) with mean $\rho=\lambda/\mu$, so the long-run probability of an empty system is

$$
\pi_0=e^{-\rho}.
$$

The process alternates between idle periods and busy periods. An idle period waits for the next [Poisson arrival](../../../../../../poisson-process.md), so its mean is $1/\lambda$. The [renewal-reward theorem](../../../../../../renewal-reward-theorem.md), with reward equal to time spent empty, gives

$$
e^{-\rho}
=\frac{1/\lambda}{1/\lambda+\mathbb EB}.
$$

Solving yields the [mean busy period of an M-M-infinity queue](../../../../../../mean-busy-period-of-an-m-m-infinity-queue.md):

$$
\boxed{
\mathbb EB_{M/M/\infty}
=\frac{e^{\lambda/\mu}-1}{\lambda}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27J](../../27j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
