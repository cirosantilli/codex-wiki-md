<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a single claim $x$, [quota share reinsurance](../../../../../quota-share-reinsurance.md) with retained fraction $\alpha\in[0,1]$ makes the direct insurer pay $\alpha x$ and the reinsurer pay $(1-\alpha)x$. Under [excess of loss reinsurance](../../../../../excess-of-loss-reinsurance.md) with retention $M\geq0$, the direct insurer pays $\min(x,M)$ and the reinsurer pays the [positive part](../../../../../positive-part-of-a-real-valued-function.md) $(x-M)_+$. Thus the concise payout pairs are

$$
\boxed{(x_I,x_R)=(\alpha x,(1-\alpha)x)quad\hbox{or}\quad(\min(x,M),(x-M)_+).}
$$

The cap in [excess of loss reinsurance](../../../../../excess-of-loss-reinsurance.md) applies separately to every claim; it is not a cap on the entire annual aggregate.

For the following [variance](../../../../../variance-split.md) calculations take $\lambda>0$ and $\mathbb E[X^2]<\infty$, so the displayed [variances](../../../../../variance-split.md) are finite. For any per-claim payout $Y$, the [law of total variance](../../../../../law-of-total-variance.md) in a [compound Poisson distribution](../../../../../compound-poisson-distribution.md) gives

$$
\operatorname{Var}\left(\sum_{j=1}^NY_j\right)
=\mathbb E[N]\operatorname{Var}(Y)+\operatorname{Var}(N)(\mathbb E[Y])^2
=\lambda\mathbb E[Y^2].
$$

The final term is the raw [second moment](../../../../../second-moment.md), not the single-claim [variance](../../../../../variance-split.md). Both parties' totals are [retained compound Poisson aggregates](../../../../../retained-compound-poisson-aggregate.md), with different payout functions of the same claims; they are generally dependent.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
