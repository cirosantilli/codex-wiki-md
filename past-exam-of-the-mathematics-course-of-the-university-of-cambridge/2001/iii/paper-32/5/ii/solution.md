<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the usual two mutually independent samples, and rank their $N=n+m$ pooled observations increasingly. Continuity gives no ties with probability one. Let $R_i$ be the pooled rank of $X_i$ and define the [Wilcoxon rank sum test](../../../../../../mann-whitney-u-test.md) statistic

$$
W_X=\sum_{i=1}^nR_i,\qquad
U_X=W_X-\frac{n(n+1)}2
=\sum_{i=1}^n\sum_{j=1}^m\mathbf1_{\{Y_j<X_i\}}.
$$

The last identity counts the ranks contributed by the other sample after subtracting the within-$X$ ranks.

When $F_X\ge F_Y$, the $X$ observations are stochastically smaller, so **reject for small $W_X$, equivalently small $U_X$**. For instance,

$$
\mathbb E U_X=nm\Pr(Y<X)
=nm\int\{1-F_X(y)\}\,dF_Y(y)\le\frac{nm}{2}.
$$

The inequality follows from $F_X\ge F_Y$ and $\int F_Y\,dF_Y=1/2$ for continuous $F_Y$. A common-uniform quantile coupling also makes this direction transparent: $F_X^{-1}(u)\le F_Y^{-1}(u)$, and $U_X$ is nondecreasing in each $X_i$.

Under the common-distribution [null hypothesis](../../../../../../null-hypothesis.md), the pooled observations are [exchangeable](../../../../../../exchangeable-random-variables.md). Every selection of $n$ ranks for the $X$ labels has probability $\binom Nn^{-1}$. Thus the exact null law is

$$
\Pr_0(W_X=w)=\frac{\#\{A\subseteq\{1,\ldots,N\}:|A|=n,\ \sum_{r\in A}r=w\}}{\binom Nn}.
$$

Choose a lower-tail critical value with probability at most the desired size, optionally randomizing at its boundary to attain the size exactly. This law is independent of the unknown common distribution. Common increasing transformations leave the pooled [ranks of observations](../../../../../../rank-of-an-observation.md) unchanged, so the statistic is a function of the [maximal invariant](../../../../../../maximal-invariant.md) from part (i). Although a rank sum is not itself maximal, it is an invariant test statistic. These facts justify the test within [nonparametric statistics](../../../../../../nonparametric-statistics-split.md).

Sampling ranks without replacement gives

$$
\mathbb E_0W_X=\frac{n(N+1)}2,\qquad
\operatorname{var}_0W_X=\frac{nm(N+1)}{12},
$$

so $\mathbb E_0U_X=nm/2$ with the same [variance](../../../../../../variance-split.md). For $n,m\to\infty$ with $n/N\to\rho\in(0,1)$, the [normal approximation for a rank sum](../../../../../../normal-approximation-for-a-rank-sum.md) states

$$
\boxed{\frac{W_X-n(N+1)/2}{\sqrt{nm(N+1)/12}}
\ \xrightarrow{d}\ N(0,1).}
$$

Equivalently replace $W_X-n(N+1)/2$ by $U_X-nm/2$. The large-sample one-sided test rejects when this standardized statistic is below the lower $\alpha$ [normal distribution](../../../../../../normal-distribution.md) quantile. This is the two-sample rank-sum test, rather than the paired [Wilcoxon signed-rank test](../../../../../../wilcoxon-signed-rank-test.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
