<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A statistic $T$ is [sufficient](../../../../../../sufficient-statistic.md) for $\theta$ if the conditional distribution of the full sample given $T$ does not depend on $\theta$. It is [minimal sufficient](../../../../../../minimal-sufficient-statistic.md) if it is a function of every sufficient statistic.

The likelihood factors as

$$
L(\theta;\mathbf x)=(2\theta)^{-n}\mathbf1_{\{M\le2\theta\}},
$$

so the [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md) shows that $M$, and hence its one-to-one transform $\widehat\theta=M/2$, is sufficient. Moreover, for two samples $\mathbf x$ and $\mathbf y$, the ratio $L(\theta;\mathbf x)/L(\theta;\mathbf y)$ is independent of $\theta$ exactly when their maxima agree. The likelihood-ratio criterion for minimal sufficiency therefore shows that $M$ and $\widehat\theta$ are minimal sufficient.

For $n\ge2$, the [sample mean](../../../../../../sample-mean.md) $\widetilde\theta$ is not sufficient: two samples can have the same mean but different maxima, and their likelihood ratio then depends on $\theta$ through the support indicators. It is consequently not minimal sufficient. For the degenerate special case $n=1$, the sample mean and maximum coincide and both conclusions reverse.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
