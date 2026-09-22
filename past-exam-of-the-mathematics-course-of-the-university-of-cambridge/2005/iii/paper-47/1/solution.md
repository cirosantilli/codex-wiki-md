<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A real [weakly stationary process](../../../../../weakly-stationary-process.md) has finite [second moments](../../../../../second-moment.md), a time-independent [mean](../../../../../expected-value.md) $\mu$, and [autocovariance function](../../../../../autocovariance.md) $\gamma_k=\operatorname{Cov}(X_t,X_{t+k})$ depending only on the lag. Use the angular-frequency convention

$$
\gamma_k=\int_{-\pi}^{\pi}e^{ik\lambda}f_X(\lambda)\,d\lambda,\qquad
\boxed{f_X(\lambda)=\frac1{2\pi}\sum_{k\in\mathbb Z}\gamma_k e^{-ik\lambda}.}
$$

The [time-series spectral density](../../../../../spectral-density-of-a-stationary-process.md) is nonnegative and integrates to $\gamma_0$. The displayed [Fourier series](../../../../../fourier-series-split.md) is ordinarily justified by $\sum_k|\gamma_k|<\infty$. More generally, [weak stationarity](../../../../../weakly-stationary-process.md) gives a [spectral measure of a stationary time series](../../../../../spectral-measure-of-a-stationary-time-series.md), not necessarily a [spectral density](../../../../../spectral-density-of-a-stationary-process.md). If a [spectral density](../../../../../spectral-density-of-a-stationary-process.md) exists without this summability, its Fourier inversion can be understood using [Fejér sums](../../../../../fejer-sum.md), which converge in $L^1$ and at its Lebesgue points. Thus [spectral density](../../../../../spectral-density-of-a-stationary-process.md) existence should not be inferred from [weak stationarity](../../../../../weakly-stationary-process.md) alone.

A [white noise process](../../../../../white-noise.md) $WN(0,\sigma^2)$ has [mean](../../../../../expected-value.md) zero and $\operatorname{Cov}(\varepsilon_t,\varepsilon_s)=\sigma^2\mathbf1_{\{t=s\}}$. Neither [independence](../../../../../independent-random-variables.md) nor a [normal distribution](../../../../../normal-distribution.md) is needed for this second-order definition. Its [autocovariance function](../../../../../autocovariance.md) is zero at nonzero lags, so

$$
\boxed{f_\varepsilon(\lambda)=\frac{\sigma^2}{2\pi}.}
$$

For a real absolutely summable filter $(c_r)$, the series defining $Y_t$ has [mean-square convergence](../../../../../convergence-in-l2.md): its tails have $L^2$ norm at most $\|X_0\|_2\sum_{\text{tail}}|c_r|$. Its [mean](../../../../../expected-value.md) is $\mu\sum_rc_r$, and

$$
\gamma_Y(k)=\sum_{r,s\in\mathbb Z}c_rc_s\gamma_X(k+r-s).
$$

The sum is absolutely convergent, since $|\gamma_X(j)|\leq\gamma_X(0)$ by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). It depends only on $k$, proving that the output is a [weakly stationary process](../../../../../weakly-stationary-process.md). Substitute the spectral integral for $\gamma_X$ and interchange the sums and integral, justified by $f_X\in L^1$ and $\sum_{r,s}|c_rc_s|<\infty$. This gives

$$
\gamma_Y(k)=\int_{-\pi}^{\pi}e^{ik\lambda}
C(e^{i\lambda})C(e^{-i\lambda})f_X(\lambda)\,d\lambda.
$$

Because the coefficients are real, the two factors are [complex conjugates](../../../../../complex-conjugate.md). Hence the [spectral density transformation under a linear filter](../../../../../spectral-density-transformation-under-a-linear-filter.md) is

$$
\boxed{f_Y(\lambda)=|C(e^{-i\lambda})|^2f_X(\lambda).}
$$

For complex coefficients the same formula holds with the conjugate-covariance convention.

Applying this result to the order-two [moving-average model](../../../../../moving-average-model.md) yields

$$
\boxed{f_X(\lambda)=\frac{\sigma^2}{2\pi}|1+\theta_1e^{-i\lambda}+\theta_2e^{-2i\lambda}|^2
=\frac{\sigma^2}{2\pi}\left[1+\theta_1^2+\theta_2^2+2\theta_1(1+\theta_2)\cos\lambda+2\theta_2\cos2\lambda\right].}
$$

Equivalently, its nonzero [autocovariances](../../../../../autocovariance.md) are $\gamma_0=\sigma^2(1+\theta_1^2+\theta_2^2)$, $\gamma_1=\sigma^2\theta_1(1+\theta_2)$ and $\gamma_2=\sigma^2\theta_2$, together with $\gamma_{-k}=\gamma_k$.

For the order-one [moving-average process](../../../../../moving-average-model.md), invert its filter by a [geometric series](../../../../../geometric-series.md). The required coefficients are

$$
\boxed{c_r=(-\theta)^r,\qquad r=0,1,2,\ldots.}
$$

They are absolutely summable for $|\theta|<1$. Direct cancellation gives

$$
\sum_{r=0}^n(-\theta)^rX_{t-r}
=\varepsilon_t-(-\theta)^{n+1}\varepsilon_{t-n-1}
\longrightarrow\varepsilon_t
$$

with [mean-square convergence](../../../../../convergence-in-l2.md). Thus the inverse filter recovers exactly the original [white noise process](../../../../../white-noise.md), including its [variance](../../../../../variance-split.md); it is an [invertible time-series representation](../../../../../invertible-time-series-representation.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
