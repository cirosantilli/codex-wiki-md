<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $f_j=(f_j(x_{1j}),\ldots,f_j(x_{nj}))^T$ for the training values of each component in the [additive regression model](../../../../../../additive-regression-model.md). Separate the [regression intercept](../../../../../../regression-intercept.md) from the smooth components by imposing $\mathbf1^Tf_j=0$ for every $j$. Without these constraints, adding a constant to a component and subtracting it from the intercept gives exactly the same mean function. A population alternative is $\mathbb E f_j(X_j)=0$ when those expectations exist. Additional [identifiability of additive regression components](../../../../../../identifiability-of-additive-regression-components.md) requirements exclude redundant component directions, as discussed below.

The [backfitting algorithm](../../../../../../backfitting-algorithm.md) proceeds as follows:

- Initialize $\widehat\beta_0=\overline y$ and $\widehat f_j=0$ for all $j$, or use another centered starting fit. Choose the smoother and its tuning parameters for each predictor.
- Cycle through $j=1,\ldots,p$. Form the [partial residual](../../../../../../partial-residual.md) $r_j=y-\widehat\beta_0\mathbf1-\sum_{k\ne j}\widehat f_k$, using the newest available component estimates.
- Apply the generic smoother in predictor $j$: $g_j=S(x_j)[r_j]$. Center its fitted values and replace the current component by $\widehat f_j=g_j-(\mathbf1^Tg_j/n)\mathbf1$. The same centering constant is subtracted from its function when predicting at a new predictor value.
- Repeat complete cycles until the components and fitted sum change by less than the chosen numerical tolerance. Return $\widehat f(x)=\widehat\beta_0+\sum_j\widehat f_j(x_j)$.

Because every component remains centered, the least-squares update of the intercept remains $\overline y$ throughout. The essential update is

$$
\boxed{\widehat f_j\leftarrow\operatorname{center}\!\left[S(x_j)\left\{y-\overline y\mathbf1-\sum_{k\ne j}\widehat f_k\right\}\right].}
$$

For penalized least-squares smoothers these updates are [coordinate descent](../../../../../../coordinate-descent.md) on the additive fitting objective. For a completely arbitrary smoother, convergence is an additional property to establish, not a consequence of merely specifying the iteration. Centering removes the constant ambiguity but does not by itself remove [concurvity](../../../../../../concurvity.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
