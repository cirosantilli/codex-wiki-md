<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [Bayesian rejection sampling for a segregating-site count](../../../../../../bayesian-rejection-sampling-for-a-segregating-site-count.md). Independently propose $\theta\sim\pi$ and $T_j\sim\operatorname{Exp}(\lambda_j)$ for $j=2,\ldots,n$, and calculate $L=\sum_jjT_j$. Draw an independent uniform $U$ on $(0,1)$ and accept the whole proposed vector exactly when

$$
\boxed{U\le e^{-\theta L/2}\frac{(\theta L/2)^k}{k!}.}
$$

Repeat after a rejection. The right side is a [probability mass function](../../../../../../probability-mass-function.md) value of a [Poisson distribution](../../../../../../poisson-distribution.md) and is therefore between zero and one. On acceptance, the [probability density function](../../../../../../probability-density-function.md) of a proposed vector is its [prior density](../../../../../../prior-density.md) multiplied by this acceptance [probability](../../../../../../probability.md), divided by the [probability](../../../../../../probability.md) of acceptance. Part (c) shows that this is precisely $f(\theta,T\mid S=k)$. Independent proposals and uniforms produce independent posterior draws. Equivalently, one could simulate a count from a [Poisson distribution](../../../../../../poisson-distribution.md) with mean $\theta L/2$ and retain the proposal when that count equals $k$; the uniform version avoids simulating that extra count.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
