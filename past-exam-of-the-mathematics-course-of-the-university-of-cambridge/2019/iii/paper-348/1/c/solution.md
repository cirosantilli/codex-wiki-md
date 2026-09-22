<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The intended [monotone rearrangement](../../../../../../monotone-rearrangement.md) is

$$
\boxed{T^\dagger(x)=G^{-1}(F(x))\quad\mu\text{-almost everywhere}.}
$$

Here $G^{-1}$ is the [quantile function](../../../../../../quantile-function.md) of $\nu$, agreeing with the ordinary inverse when $G$ is continuous and strictly increasing. With an [atomless measure](../../../../../../non-atomic-measure.md) $\mu$, its [cumulative distribution function](../../../../../../cumulative-distribution-function.md) $F$ is continuous, and the [probability integral transform](../../../../../../probability-integral-transform.md) makes $F(X)$ uniform on $(0,1)$ for $X\sim\mu$. Thus $G^{-1}(F(X))\sim\nu$. The one-dimensional [monotone rearrangement](../../../../../../monotone-rearrangement.md) theorem says this [transport map](../../../../../../transport-map.md) minimizes the cost $d(x-y)$ for [convex](../../../../../../convex-function.md) continuous $d$, whenever the cost integrals are well defined. Values at exceptional endpoints may be chosen arbitrarily.

**The printed assumptions omit an essential source condition.** Invertibility of $G$ alone does not ensure an admissible [transport map](../../../../../../transport-map.md). For example, $\mu=\delta_0$ and $\nu$ a [standard normal distribution](../../../../../../standard-normal-distribution.md) satisfy the stated condition on $G$, but $T_\#\delta_0$ is always a [Dirac measure](../../../../../../dirac-measure.md). There is no solution to the [Monge optimal transport problem](../../../../../../monge-optimal-transport-problem.md) in this example. The boxed answer therefore requires the additional assumption that $\mu$ is an [atomless measure](../../../../../../non-atomic-measure.md), or an equivalent condition making the displayed map admissible. For arbitrary sources the always admissible monotone [transport plan](../../../../../../transport-plan.md) is $(F^{-1},G^{-1})_\#\mathcal U(0,1)$, which need not be induced by a map.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
