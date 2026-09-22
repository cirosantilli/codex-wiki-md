<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [weakly stationary process](../../../../../../weakly-stationary-process.md) with [mean](../../../../../../expected-value.md) $m$ and nonzero [variance](../../../../../../variance-split.md), put $\gamma(h)=\operatorname{Cov}(X_{t+h},X_t)$ and $\rho(h)=\gamma(h)/\gamma(0)$. The function $\rho$ is its [autocorrelation function](../../../../../../autocorrelation.md). For observations $x_1,\ldots,x_N$, one common [sample autocorrelation function](../../../../../../sample-autocorrelation-function.md) is

$$
\widehat\gamma(h)=\frac1N\sum_{t=1}^{N-h}(x_t-\overline x)(x_{t+h}-\overline x),
\qquad \widehat\rho(h)=\frac{\widehat\gamma(h)}{\widehat\gamma(0)}.
$$

A [correlogram](../../../../../../correlogram.md) plots these estimates against lag; the population analogue plots $\rho(h)$.

The lag-$h$ [partial autocorrelation function](../../../../../../partial-autocorrelation-function.md) measures the [correlation](../../../../../../pearson-correlation-coefficient.md) between $X_t$ and $X_{t-h}$ after removing their [linear projections](../../../../../../projection-linear-algebra.md) on the intervening observations. Its sample counterpart can be calculated by the [Yule-Walker equations](../../../../../../yule-walker-equations.md): solve

$$
\widehat R_h\widehat\phi_h=\widehat r_h,
\qquad (\widehat R_h)_{ij}=\widehat\rho(|i-j|),
\qquad (\widehat r_h)_i=\widehat\rho(i),
$$

and take $\widehat\alpha(h)=\widehat\phi_{h,h}$, assuming the matrix is nonsingular. This defines a standard [sample partial autocorrelation function](../../../../../../sample-partial-autocorrelation-function.md).

For a minimal causal [autoregressive model](../../../../../../autoregressive-model.md) of order $p$, the [autocorrelation](../../../../../../autocorrelation.md) typically decays geometrically, possibly with damped oscillations, whereas the [partial autocorrelation function](../../../../../../partial-autocorrelation-function.md) is zero beyond lag $p$: after those $p$ preceding values have been projected out, the innovation is orthogonal to older values. For a [moving-average model](../../../../../../moving-average-model.md) of order $q$, nonoverlapping sets of driving [white noise](../../../../../../white-noise.md) give $\gamma(h)=0$ for $|h|>q$; its [partial autocorrelation function](../../../../../../partial-autocorrelation-function.md) generally tails off when the representation is invertible. Thus **an ACF cutoff suggests an MA order; a PACF cutoff suggests an AR order**. An [ARMA](../../../../../../autoregressive-moving-average-model.md) model generally has neither cutoff. These are population properties; sample noise makes cutoffs approximate, so fitted residuals and uncertainty should also be inspected. Under [independent](../../../../../../independent-random-variables.md) [white noise](../../../../../../white-noise.md), fixed-lag sample [correlations](../../../../../../pearson-correlation-coefficient.md) have approximate standard error $N^{-1/2}$, giving a rough diagnostic band rather than a universal simultaneous test.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
