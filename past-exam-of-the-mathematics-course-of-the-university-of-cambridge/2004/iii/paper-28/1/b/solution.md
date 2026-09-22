<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $\mathcal F_m=\sigma(\xi_1,\ldots,\xi_m)$ and $S_0=0$. [Independence](../../../../../../independent-random-variables.md) and zero [means](../../../../../../expected-value.md) imply $\mathbb E[S_{m+1}\mid\mathcal F_m]=S_m$, so the partial sums form a [square-integrable](../../../../../../square-integrable-function.md) [martingale](../../../../../../martingale-split.md). More explicitly,

$$
\mathbb E[S_{m+1}^2\mid\mathcal F_m]=S_m^2+\mathbb E\xi_{m+1}^2\geq S_m^2.
$$

Thus $S_m^2$ is a nonnegative [submartingale](../../../../../../submartingale.md). The [Doob maximal inequality](../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) at threshold $x^2$ now proves the [Kolmogorov maximal inequality](../../../../../../kolmogorov-maximal-inequality.md):

$$
\boxed{\mathbb P\left(\max_{0\leq m\leq n}|S_m|\geq x\right)
=\mathbb P\left(\max_{m\leq n}S_m^2\geq x^2\right)
\leq\frac{\mathbb ES_n^2}{x^2}.}
$$

Finally, expanding the terminal square and using [independence](../../../../../../independent-random-variables.md) and the zero [means](../../../../../../expected-value.md) gives $\mathbb ES_n^2=\sum_{j=1}^n\mathbb E\xi_j^2$. Identical distributions are not required.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
