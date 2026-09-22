<h1 id="3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $c_t=\cos(2\pi t/S)$ and assume $\sigma^2>0$. Then

$$
EY_t=c_t,\quad\operatorname{Cov}(Y_t,Y_{t-h})=\sigma^2\mathbf1_{\{h=0\}},
$$



$$
EZ_t=0,\quad\operatorname{Cov}(Z_t,Z_{t-h})=\sigma^2c_t^2\mathbf1_{\{h=0\}}.
$$

Thus $Y$ generally has a periodic mean, and $Z$ generally has a periodic [variance](../../../../../../variance-split.md). The edge cases allowed by $S\in\mathbb N^*$ matter: $Y$ is stationary when $S=1$, because the mean is then constant, and $Z$ is stationary for $S=1$ or $S=2$. In the latter case multiplying iid centered [Gaussian white noise](../../../../../../gaussian-white-noise.md) by $(-1)^t$ leaves its iid distribution unchanged. For every $S\geq3$, $c_0^2=1$ but $c_1^2<1$, so $Z$ is nonstationary. For $S>1$, $Y$ is nonstationary because $c_t$ is not constant.

Use the [seasonal difference operator](../../../../../../seasonal-difference-operator.md) $\Delta_S=1-B^S$. Since $c_t=c_{t-S}$,

$$
\boxed{\Delta_SY_t=\varepsilon_t-\varepsilon_{t-S}.}
$$

This is a stationary [moving-average model](../../../../../../moving-average-model.md) of iid [Gaussian white noise](../../../../../../gaussian-white-noise.md). Its [covariance](../../../../../../covariance.md) is $2\sigma^2$ at lag $0$, $-\sigma^2$ at lags $\pm S$, and zero otherwise.

For the [variance](../../../../../../variance-split.md)-modulated process the same operation gives

$$
\boxed{\Delta_SZ_t=c_t(\varepsilon_t-\varepsilon_{t-S}).}
$$

Its [variance](../../../../../../variance-split.md) is $2\sigma^2c_t^2$ and its [covariance](../../../../../../covariance.md) at lag $S$ is $-\sigma^2c_t^2$. Therefore it remains nonstationary for $S\geq3$, and the operation doubles the marginal [variance](../../../../../../variance-split.md) at nonzero seasons. [Seasonal differencing does not remove periodic variance](../../../../../../seasonal-differencing-does-not-remove-periodic-variance.md): it removes a periodic mean, but the periodic [variance](../../../../../../variance-split.md) generally remains. Practical alternatives are a periodic model or seasonal [variance](../../../../../../variance-split.md) standardization; at seasons with $c_t=0$ the observations are deterministically zero, so division by $c_t$ is not possible there. For the already stationary special cases $S=1,2$, filtering preserves stationarity.

A [periodically correlated process](../../../../../../periodically-correlated-process.md) with period $S$ has its mean and two-time [covariance](../../../../../../covariance.md) unchanged when both times are shifted by $S$. For $Z$, the mean is zero and

$$
\operatorname{Cov}(Z_{t+S},Z_{s+S})=\sigma^2c_{t+S}c_{s+S}\mathbf1_{\{t=s\}}
=\operatorname{Cov}(Z_t,Z_s).
$$

Hence $Z$ is a [periodically correlated process](../../../../../../periodically-correlated-process.md). Its [covariance](../../../../../../covariance.md) period can be smaller than $S$: when $S$ is even, $c_{t+S/2}^2=c_t^2$, so $S/2$ is already a [covariance](../../../../../../covariance.md) period.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
