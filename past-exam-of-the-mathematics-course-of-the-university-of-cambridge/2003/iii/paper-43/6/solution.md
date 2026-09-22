<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For the usual causal, stable [autoregressive moving-average model](../../../../../autoregressive-moving-average-model.md) with zero-mean [white noise](../../../../../white-noise.md), sufficient conditions for a stationary invertible representation are

$$
\boxed{|\phi|<1,\qquad|\theta|<1.}
$$

The roots of $1-\phi z$ and $1+\theta z$ then lie outside the closed unit disc. For a minimal representation these are the usual [causality and invertibility root criteria for an ARMA model](../../../../../causality-and-invertibility-root-criteria-for-an-arma-model.md). A genuinely minimal ARMA(1,1) additionally has nonzero coefficients and no cancellation $\phi+\theta=0$; if a coefficient vanishes the order is lower. Common factors can reduce the process to white noise, so inequalities on an unreduced representation should not be asserted as necessary for every reduced process. A noncausal stationary solution of an unstable autoregressive equation is a different representation, and does not give the requested innovation-based Wold coefficients below.

Using the [backshift operator](../../../../../backshift-operator.md) $B$, write $(1-\phi B)X_t=(1+\theta B)\epsilon_t$. The absolutely summable geometric series gives

$$
\frac{1+\theta B}{1-\phi B}=1+(\phi+\theta)\sum_{j=1}^{\infty}\phi^{j-1}B^j.
$$

Thus the [Wold representation](../../../../../wold-decomposition.md) is

$$
\boxed{X_t=\epsilon_t+(\phi+\theta)\sum_{j=1}^{\infty}\phi^{j-1}\epsilon_{t-j}.}
$$

Its coefficients are square-summable, so the series converges in mean square and defines a [weakly stationary process](../../../../../weakly-stationary-process.md). Invertibility makes the closed spans of past observations and past innovations equal. Since the current driving white noise is orthogonal to all past innovations, it is orthogonal to all past observations and is the [linear innovation](../../../../../linear-innovation-process.md) of this causal invertible process.

The [spectral density of an ARMA process](../../../../../spectral-density-of-an-arma-process.md) follows from the squared frequency response of the [linear filter of a stationary time series](../../../../../linear-filter-of-a-stationary-time-series.md):

$$
\boxed{f_X(\omega)=\frac{\sigma^2}{2\pi}\frac{1+\theta^2+2\theta\cos\omega}{1+\phi^2-2\phi\cos\omega},\qquad-\pi\le\omega\le\pi.}
$$

This displayed density uses the usual two-sided convention. For the [one-sided spectral density](../../../../../one-sided-spectral-density-of-a-real-stationary-time-series.md) used in Question 5, multiply it by two and restrict to $0\le\omega\le\pi$.

Let $\psi_0=1$ and $\psi_j=(\phi+\theta)\phi^{j-1}$ for $j\ge1$. Orthogonality of the driving [white noise](../../../../../white-noise.md) gives $\gamma(h)=\sigma^2\sum_{j\ge0}\psi_j\psi_{j+h}$ for $h\ge0$. Hence

$$
\boxed{\gamma(0)=\sigma^2\left(1+\frac{(\phi+\theta)^2}{1-\phi^2}\right)=\frac{\sigma^2(1+\theta^2+2\phi\theta)}{1-\phi^2}.}
$$

For $h\ge1$, separate the $j=0$ term and sum the remaining geometric series:

$$
\begin{aligned}
\gamma(h)&=\sigma^2\left[(\phi+\theta)\phi^{h-1}+\frac{(\phi+\theta)^2\phi^h}{1-\phi^2}\right]\\
&=\boxed{\frac{\sigma^2(\phi+\theta)(1+\phi\theta)}{1-\phi^2}\phi^{h-1}.}
\end{aligned}
$$

Negative lags satisfy $\gamma(-h)=\gamma(h)$. With $\phi=0$, interpret the lag-one factor as one and later powers as zero, recovering the MA(1) covariance.

To express prediction entirely through observations, invert the moving-average factor:

$$
\epsilon_t=\frac{1-\phi B}{1+\theta B}X_t=X_t-(\phi+\theta)\sum_{j=1}^{\infty}(-\theta)^{j-1}X_{t-j}.
$$

The best [linear predictor](../../../../../linear-predictor.md) from the whole past is therefore

$$
\boxed{\widehat X_t=(\phi+\theta)\sum_{j=1}^{\infty}(-\theta)^{j-1}X_{t-j}=\phi X_{t-1}+\theta\epsilon_{t-1}.}
$$

Indeed $X_t-\widehat X_t=\epsilon_t$ is orthogonal to the closed linear span of the past. For any other past-measurable linear predictor $L$, the [mean squared error](../../../../../mean-squared-error.md) decomposes as $E[(X_t-L)^2]=\sigma^2+E[(\widehat X_t-L)^2]$, establishing optimality and error [variance](../../../../../variance-split.md) $\sigma^2$. The result only uses second-order properties; identifying this linear predictor with a full conditional expectation requires stronger assumptions such as independent innovations or joint Gaussianity. In the cancellation case $\theta=-\phi$ within the stable range, $X_t=\epsilon_t$, the off-zero covariances and predictor vanish, and the spectrum is constant.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
