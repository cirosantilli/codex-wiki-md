<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The condition for a causal linear-filter solution is **$|\phi|<1$**. Its mean-square expansion is $X_t=\sum_{j\geq0}\phi^jZ_{t-j}$. Summing the matching [white noise](../../../../../../white-noise.md) terms gives

$$
\gamma_X(h)=\frac{\sigma_z^2}{1-\phi^2}\phi^{|h|}.
$$

The assumed orthogonality of every $W_s$ to every $Z_t$ extends to every $X_t$ by L2 convergence of that expansion. Hence the added-noise process has mean zero and

$$
\boxed{\gamma_Y(h)=\frac{\sigma_z^2}{1-\phi^2}\phi^{|h|}+\sigma_w^2\mathbf1_{\{h=0\}}.}
$$

This depends only on lag, proving [weak stationarity](../../../../../../weakly-stationary-process.md). Its [autocorrelation](../../../../../../autocorrelation.md) has the same geometric tail as the latent autoregression, but its positive-lag correlations are reduced by the additional [variance](../../../../../../variance-split.md) at lag zero. This is the [autocovariance of an AR(1) process observed with white noise](../../../../../../autocovariance-of-an-ar-1-process-observed-with-white-noise.md). Strict stationarity or Gaussianity is not implied by [white noise](../../../../../../white-noise.md) [covariance](../../../../../../covariance.md) assumptions alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
