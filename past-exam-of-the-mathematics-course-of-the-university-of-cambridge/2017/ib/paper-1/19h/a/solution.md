<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [sufficient statistic](../../../../../../sufficient-statistic.md) has a conditional distribution of the full data given its value that is independent of the unknown parameter. A [minimal sufficient statistic](../../../../../../minimal-sufficient-statistic.md) is sufficient and is a function of every other [sufficient statistic](../../../../../../sufficient-statistic.md), up to null sets. For a dominated family with common positive support, the [likelihood-ratio criterion for minimal sufficiency](../../../../../../likelihood-ratio-criterion-for-minimal-sufficiency.md) states that $T$ is minimal sufficient if $T(x)=T(y)$ holds exactly when $p_\theta(x)/p_\theta(y)$ is independent of $\theta$.

For $S=\sum_iX_i$, the joint [probability mass function](../../../../../../probability-mass-function.md) is

$$
p_\theta(x)=\theta^{-n}(1-1/\theta)^{S-n},\qquad x_i\ge1.
$$

The [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md) proves sufficiency of $S$. For two samples, the likelihood ratio is $(1-1/\theta)^{S(x)-S(y)}$, independent of $\theta>1$ exactly when their sums agree. Thus $S$ is minimal sufficient. Any one-to-one transformation of it is also minimal sufficient, so choose

$$
\boxed{T=\overline X=\frac Sn,\qquad\mathbb E_\theta T=\theta}.
$$

This chosen [estimator](../../../../../../estimator.md) is an [unbiased estimator](../../../../../../unbiased-estimator.md), since each observation has mean $\theta$. If instead the statistic is reported as $S$, its expectation is $n\theta$, and as an estimator of $\theta$ it has [bias](../../../../../../bias-of-an-estimator.md) $(n-1)\theta$ (zero only when $n=1$). Being a [minimal sufficient statistic](../../../../../../minimal-sufficient-statistic.md) is unchanged by this rescaling; being an [unbiased estimator](../../../../../../unbiased-estimator.md) is not.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
