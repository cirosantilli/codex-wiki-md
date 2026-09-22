<h1 id="20h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For an independent second sample, let

$$
\widetilde S_{XX}=\sum_{j=1}^{\widetilde n}
(\widetilde X_j-\overline{\widetilde X})^2.
$$

Under $H_0:\sigma^2=\widetilde\sigma^2$, independence and the two chi-squared laws give the [F-distribution](../../../../../../f-distribution.md)

$$
\boxed{F=
\frac{S_{XX}/(n-1)}{\widetilde S_{XX}/(\widetilde n-1)}
\sim F_{n-1,\widetilde n-1}}.
$$

For the one-sided alternative $\sigma^2>\widetilde\sigma^2$, reject for large $F$, using the upper $\alpha$ critical value.

**No values of the unknown means enter this statistic:** centering by the sample means removes them. If both means are known, one may instead use sums about the known means; the corresponding degrees of freedom are $n$ and $\widetilde n$, rather than $n-1$ and $\widetilde n-1$. Thus knowledge of the means changes the degrees of freedom and critical value, while the variance-ratio principle is unchanged.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [20H](../../20h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
