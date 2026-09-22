<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a centered [weakly stationary process](../../../../../../weakly-stationary-process.md) with $\gamma(0)>0$, the [autocorrelation function](../../../../../../autocorrelation.md) is

$$
\boxed{\rho(h)=\gamma(h)/\gamma(0).}
$$

For $h\geq2$, let $P$ be [orthogonal projection](../../../../../../orthogonal-projection.md) in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) onto the linear span of $X_{t-1},\ldots,X_{t-h+1}$. The lag-$h$ [partial autocorrelation function](../../../../../../partial-autocorrelation-function.md) is the [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) of $X_t-PX_t$ and $X_{t-h}-PX_{t-h}$. It removes the linear contribution of the intervening observations. At lag one it is just $\rho(1)$. For nonsingular prediction [covariance](../../../../../../covariance.md) matrices, it is equivalently the last coefficient $a_{hh}$ in the order-$h$ linear predictor of $X_t$ from $X_{t-1},\ldots,X_{t-h}$. Equal residual variances, by stationarity, identify that coefficient with the residual correlation. If a residual has zero [variance](../../../../../../variance-split.md), this correlation is undefined; the nondegeneracy condition matters.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
