<h1 id="6/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

A one-sample [U-statistic](../../../../../../u-statistic.md) of fixed degree $m$ has a symmetric [U-statistic kernel](../../../../../../kernel-of-a-u-statistic.md) $h$ and averages it over all distinct subsets of an iid sample:

$$
U_n=\binom nm^{-1}\sum_{i_1<\cdots<i_m}h(X_{i_1},\ldots,X_{i_m}).
$$

It is unbiased for $\theta=\mathbb E h(X_1,\ldots,X_m)$. With finite second moment, define the first [Hoeffding projection](../../../../../../hoeffding-projection.md) $h_1(x)=\mathbb E[h(x,X_2,\ldots,X_m)]-\theta$. Orthogonality of the higher projections gives

$$
U_n-\theta=\frac mn\sum_i h_1(X_i)+R_n,\qquad\mathbb E R_n^2=O(n^{-2}).
$$

If $\zeta_1=\operatorname{Var}(h_1(X))>0$, the [central limit theorem](../../../../../../central-limit-theorem.md) therefore proves the [U-statistic central limit theorem](../../../../../../u-statistic-central-limit-theorem.md)

$$
\boxed{\sqrt n(U_n-\theta)\Rightarrow N(0,m^2\zeta_1),\quad\operatorname{Var}(U_n)=\frac{m^2\zeta_1}{n}+O(n^{-2}).}
$$

Equivalently the [influence function of a U-statistic](../../../../../../influence-function-of-a-u-statistic.md) is $m h_1(x)$, obtained by differentiating its population functional $\int h\,dF^m$ in each distribution argument. If $\zeta_1=0$, the root-$n$ limit degenerates and the second or higher projection determines a different, often nonnormal, limit.

For example, $h(x,y)=(x-y)^2/2$ gives the unbiased sample variance with denominator $n-1$. Its first projection is $[(x-\mu)^2-\sigma^2]/2$, so the influence function is $(x-\mu)^2-\sigma^2$. When the fourth moment is finite, the leading variance of the sample variance is $(\mathbb E(X-\mu)^4-\sigma^4)/n$. This example connects unbiased symmetric estimation to the functional influence calculation.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [6](../../6.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
