<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $z_p=\Phi^{-1}(p)$ denote a [quantile](../../../../../../quantile-function.md) of the [standard normal distribution](../../../../../../standard-normal-distribution.md). Reject when $W_n>z_{1-\alpha}$. The [statistical power](../../../../../../statistical-power.md) at the specified positive effect is

$$
P_{\delta^*}(W_n>z_{1-\alpha})=1-\Phi\left(z_{1-\alpha}-\frac{\sqrt n\delta^*}{\sigma}\right).
$$

Equating this to $1-\beta$ and using $z_\beta=-z_{1-\beta}$ gives $\sqrt n\delta^*/\sigma=z_{1-\alpha}+z_{1-\beta}$. Thus, for the usual target $1-\beta>\alpha$,

$$
\boxed{n=\left\lceil\frac{\sigma^2}{(\delta^*)^2}\left(z_{1-\alpha}+z_{1-\beta}\right)^2\right\rceil.}
$$

Rounding up ensures at least the target [statistical power](../../../../../../statistical-power.md). This [normal-mean sample size calculation](../../../../../../normal-mean-sample-size-calculation.md) assumes a positive integer [sample size](../../../../../../sample-size.md); if a requested power is at most $\alpha$, every positive [sample size](../../../../../../sample-size.md) already exceeds that target for $\delta^*>0$, and one should not square a negative [quantile](../../../../../../quantile-function.md) sum to impose an unnecessary lower bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
