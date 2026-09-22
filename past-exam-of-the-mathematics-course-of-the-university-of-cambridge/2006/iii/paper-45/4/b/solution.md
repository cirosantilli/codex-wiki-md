<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [infinite sites mutation model](../../../../../../infinite-sites-mutation-model.md), mutations occur as independent [Poisson processes](../../../../../../poisson-process.md) at rate $\theta/2$ per lineage per unit of the coalescent time used in part (a). Conditional on the genealogy, superposition over branches gives a [Poisson distribution](../../../../../../poisson-distribution.md) with mean $\theta L/2$. Since this depends only on $L$, conditioning on total length alone gives

$$
\boxed{S\mid L,\theta\sim\operatorname{Poisson}(\theta L/2).}
$$

Each mutation occurs at a new site and below the common ancestor, so it contributes exactly one [segregating site](../../../../../../segregating-site.md). The [law of iterated expectation](../../../../../../law-of-total-expectation.md) therefore gives, with $a_{n-1}=\sum_{i=1}^{n-1}1/i$,

$$
\boxed{E[S\mid\theta]=\frac\theta2 EL=\theta a_{n-1}.}
$$

Here $\theta$ is fixed when taking the [expectation](../../../../../../expected-value.md). If it is also random under a proper prior with finite mean, the unconditional [expectation](../../../../../../expected-value.md) is $a_{n-1}E\theta$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
