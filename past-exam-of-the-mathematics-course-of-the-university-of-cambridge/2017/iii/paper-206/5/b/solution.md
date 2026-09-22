<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a known mean zero, a common [sample autocovariance function](../../../../../../sample-autocovariance-function.md) convention is

$$
\widehat\gamma_n(h)=\frac1n\sum_{t=1}^{n-h}Y_tY_{t+h},\qquad 0\le h<n.
$$

The [weakly stationary process](../../../../../../weakly-stationary-process.md) property gives $\mathbb E[Y_tY_{t+h}]=\gamma(h)$, so

$$
\boxed{\mathbb E\widehat\gamma_n(h)=\left(1-\frac hn\right)\gamma(h).}
$$

The lag-zero estimate is unbiased, but at nonzero lags the divisor $n$ causes a finite-sample multiplicative [bias](../../../../../../bias-of-an-estimator.md). An alternative convention uses $(n-h)^{-1}$ instead; for that convention the [expectation](../../../../../../expected-value.md) is exactly $\gamma(h)$. These are two normalizations of the [sample autocovariance function](../../../../../../sample-autocovariance-function.md), so the divisor must be specified. Here no estimated-mean centering term occurs because zero is known. Replacing zero by a sample mean would introduce additional [bias](../../../../../../bias-of-an-estimator.md) terms. Extend to negative lags by symmetry; there are no observed lagged pairs for $h\ge n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
