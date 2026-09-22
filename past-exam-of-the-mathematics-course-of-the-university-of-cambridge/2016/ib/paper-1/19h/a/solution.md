<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [statistic](../../../../../../statistic.md) $T$ is a [sufficient statistic](../../../../../../sufficient-statistic.md) for $\theta$ if the conditional [distribution](../../../../../../distribution-mathematical-analysis.md) of the data given $T$ does not depend on $\theta$. For a dominated family with density or mass function $f_\theta(x)$, the [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md) states that this is equivalent to

$$
\boxed{f_\theta(x)=g_\theta(T(x))h(x),}
$$

where $h$ is nonnegative and independent of $\theta$, and $g_\theta$ is nonnegative and depends on the data only through $T$.

For a discrete sample space, suppose first that the factorization holds. If $\mathbb P_\theta(T=t)>0$, summing over the fibre gives $\mathbb P_\theta(T=t)=g_\theta(t)\sum_{T(x)=t}h(x)$, so

$$
\mathbb P_\theta(X=x\mid T=t)=\frac{h(x)}{\sum_{T(z)=t}h(z)}\quad(T(x)=t).
$$

This conditional [distribution](../../../../../../distribution-mathematical-analysis.md) is independent of $\theta$, proving that $T$ is a [sufficient statistic](../../../../../../sufficient-statistic.md). Conversely, let $q_t(x)$ be the common conditional mass function guaranteed by the [sufficient statistic](../../../../../../sufficient-statistic.md) property, for every fibre attainable under at least one parameter. Set $h(x)=q_{T(x)}(x)$ and $g_\theta(t)=\mathbb P_\theta(T=t)$. Then $\mathbb P_\theta(X=x)=g_\theta(T(x))h(x)$. Fibres never attained under any parameter can be assigned any conditional distribution, since their multiplying probability is always zero. This proves both directions of the discrete criterion, including possible parameter-dependent supports.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
