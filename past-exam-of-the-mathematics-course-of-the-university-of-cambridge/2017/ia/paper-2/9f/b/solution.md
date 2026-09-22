<h1 id="9f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed $k$ and sufficiently large $N$,

$$
p_k(N,\lambda/N)
=\frac{\lambda^k}{k!}\left[\prod_{j=0}^{k-1}\left(1-\frac jN\right)\right]
\left(1-\frac\lambda N\right)^N
\left(1-\frac\lambda N\right)^{-k}.
$$

The finite product and last factor tend to one, while $(1-\lambda/N)^N\to e^{-\lambda}$. Thus the [Poisson limit theorem](../../../../../../poisson-limit-theorem.md) gives

$$
\boxed{\lim_{N\to\infty}p_k(N,\lambda/N)=e^{-\lambda}\frac{\lambda^k}{k!}.}
$$

These numbers form a [probability mass function](../../../../../../probability-mass-function.md) because they are nonnegative and their sum is $e^{-\lambda}\sum_{k\geq0}\lambda^k/k!=1$, by the [exponential series](../../../../../../exponential-series.md). They define the [Poisson distribution](../../../../../../poisson-distribution.md) of parameter $\lambda$. Only $N\geq\lambda$ is needed to make the binomial parameter valid, which is sufficient for the limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
