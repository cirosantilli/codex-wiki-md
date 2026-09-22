<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [weakly stationary process](../../../../../weakly-stationary-process.md) with finite second moments, let $\mu=\mathbb EX_t$ and $\gamma(h)=\operatorname{Cov}(X_{t+h},X_t)$, independent of $t$. If $\gamma(0)>0$, its [autocorrelation function](../../../../../autocorrelation.md) is $\rho(h)=\gamma(h)/\gamma(0)$. Given observations $x_1,\ldots,x_N$, one usual [sample autocovariance function](../../../../../sample-autocovariance-function.md) is

$$
\widehat\gamma(h)=\frac1N\sum_{t=1}^{N-h}(x_t-\bar x)(x_{t+h}-\bar x),\qquad\widehat\rho(h)=\frac{\widehat\gamma(h)}{\widehat\gamma(0)}.
$$

The [correlogram](../../../../../correlogram.md) plots $\widehat\rho(h)$ against lag $h$. The [partial autocorrelation function](../../../../../partial-autocorrelation-function.md) at lag $h$ is the [correlation](../../../../../pearson-correlation-coefficient.md) between $X_t$ and $X_{t-h}$ after linearly projecting each onto the intervening observations. Its sample version can be calculated by solving the Yule-Walker regression equations

$$
\widehat R_h\widehat\phi_h=(\widehat\rho(1),\ldots,\widehat\rho(h))^T,\qquad
(\widehat R_h)_{ij}=\widehat\rho(|i-j|),
$$

then taking the last coefficient $\widehat\phi_{h,h}$. Equivalently, use the corresponding residual [correlation](../../../../../pearson-correlation-coefficient.md) from the sample regressions, with a consistent [covariance](../../../../../covariance.md) convention.

For a minimal causal [autoregressive model](../../../../../autoregressive-model.md) of order $p$, the population [partial autocorrelation function](../../../../../partial-autocorrelation-function.md) is zero after lag $p$, while the [autocorrelation function](../../../../../autocorrelation.md) follows an exponentially decaying or damped oscillatory tail. For a [moving-average model](../../../../../moving-average-model.md) of order $q$, its [autocovariance](../../../../../autocovariance.md) and hence [autocorrelation](../../../../../autocorrelation.md) are zero after lag $q$, because observations farther apart share no driving-noise terms; its partial [correlations](../../../../../pearson-correlation-coefficient.md) usually tail off. These [order identification by autocorrelation cutoffs](../../../../../order-identification-by-autocorrelation-cutoffs.md) patterns suggest AR or MA candidate orders. Sample cutoffs are approximate and should be judged with sampling uncertainty and residual diagnostics; the familiar white-noise bands near $\pm1.96/\sqrt N$ are a null approximation, not universal confidence limits for a dependent series.

For the trend problem, write a symmetric [estimator](../../../../../estimator.md) as

$$
\widehat T_t=a(X_{t-2}+X_{t+2})+b(X_{t-1}+X_{t+1})+cX_t.
$$

Reproducing arbitrary constant and quadratic trends requires $2a+2b+c=1$ and $8a+2b=0$; the linear-trend condition holds automatically by symmetry. These constraints follow by expanding $T_{t+j}=T_t+j(b_0+2c_0t)+c_0j^2$ for a trend $T_t=a_0+b_0t+c_0t^2$. Thus $b=-4a$, $c=1+6a$. Since the errors are uncorrelated and the [estimator](../../../../../estimator.md) is unbiased, its [mean squared error](../../../../../mean-squared-error.md) is

$$
\sigma^2(2a^2+2b^2+c^2)=\sigma^2(70a^2+12a+1).
$$

The strictly convex quadratic is minimized at $a=-3/35$, giving the [five-point symmetric quadratic trend smoother](../../../../../five-point-symmetric-quadratic-trend-smoother.md)

$$
\boxed{\widehat T_t=\frac{-3X_{t-2}+12X_{t-1}+17X_t+12X_{t+1}-3X_{t+2}}{35},\qquad\operatorname{MSE}=\frac{17}{35}\sigma^2.}
$$

This weighted moving average allows negative coefficients; a convex average could not cancel the quadratic moment.

For three points, symmetry gives weights $(a,b,a)$. Unbiasedness for every quadratic requires $2a+b=1$ and $2a=0$, so the only solution is $(0,1,0)$. Thus **there is no nontrivial three-point quadratic-preserving smoother**. The literal claim that there is no unbiased [estimator](../../../../../estimator.md) at all is false, since $\widehat T_t=X_t$ is unbiased with error [variance](../../../../../variance-split.md) $\sigma^2$. This is the [three-point quadratic reproduction forces the identity filter](../../../../../three-point-quadratic-reproduction-forces-the-identity-filter.md) distinction.

For [seasonal extraction by a centred moving average](../../../../../seasonal-extraction-by-a-centred-moving-average.md), use the additive decomposition $X_t=T_t+S_t+\varepsilon_t$, where $S_t$ has period $m$ and its values over one period sum to zero. An average covering a full period removes the seasonal component and approximately retains a slowly changing trend. If $m$ is odd, take the centred length-$m$ average; if $m$ is even, centre it by averaging two adjacent length-$m$ averages, giving half weights at the two endpoints. Subtract this trend estimate from the data, average residuals within each seasonal phase over different cycles, and centre the resulting phase estimates to sum to zero. For a multiplicative decomposition, use ratios and normalize the phase estimates to average one.

Successive moving averages compose by [convolution](../../../../../convolution.md) of their weights. Even an initially uncorrelated noise series becomes correlated: for weights $w_j$, the filtered noise has [covariance](../../../../../covariance.md) $\sigma^2\sum_jw_jw_{j+h}$. Further smoothing changes this [covariance](../../../../../covariance.md) again and can turn random variation into apparently persistent patterns while obscuring genuine short-scale features. Spectrally, repeated use of a transfer function $H$ multiplies the spectrum by $|H|^{2r}$ after $r$ applications, so repeated smoothing is not harmless repetition of the same estimate.

In [simple exponential smoothing](../../../../../simple-exponential-smoothing.md), choose $0<\alpha<1$ and update $\ell_t=\alpha X_t+(1-\alpha)\ell_{t-1}$. Iteration gives $\ell_t=\alpha\sum_{j=0}^{t-1}(1-\alpha)^jX_{t-j}+(1-\alpha)^t\ell_0$, so older observations receive exponentially decreasing weights. Forecast $\widehat X_{t+h\mid t}=\ell_t$ for every $h\geq1$. This is appropriate for a locally stable level with no persistent trend or seasonality.

For a local linear trend, [double exponential smoothing](../../../../../double-exponential-smoothing.md) supplies level and slope. [Holt's linear trend method](../../../../../holt-s-linear-trend-method.md) uses

$$
\ell_t=\alpha X_t+(1-\alpha)(\ell_{t-1}+b_{t-1}),\qquad
b_t=\beta(\ell_t-\ell_{t-1})+(1-\beta)b_{t-1},\qquad
\boxed{\widehat X_{t+h\mid t}=\ell_t+hb_t.}
$$

Another standard convention is [Brown's double exponential smoothing](../../../../../brown-s-double-exponential-smoothing.md): smooth twice with the same gain, $s_t^{(1)}=\alpha X_t+(1-\alpha)s_{t-1}^{(1)}$ and $s_t^{(2)}=\alpha s_t^{(1)}+(1-\alpha)s_{t-1}^{(2)}$, then put $a_t=2s_t^{(1)}-s_t^{(2)}$, $b_t=\alpha(s_t^{(1)}-s_t^{(2)})/(1-\alpha)$ and forecast $a_t+hb_t$. These variants handle a nonseasonal trend; seasonal effects need separate modelling, and a long-horizon linear extrapolation assumes the current local slope persists.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
