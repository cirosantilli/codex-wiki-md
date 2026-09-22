<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For an [autoregressive moving-average model](../../../../../autoregressive-moving-average-model.md), the driving-to-output transfer function is $A(z)=\theta(z)/\phi(z)$, and the inverse transfer function is $A(z)^{-1}=\phi(z)/\theta(z)$. The [causality and invertibility root criteria for an ARMA model](../../../../../causality-and-invertibility-root-criteria-for-an-arma-model.md) require these respective rational functions to have power series about zero converging on a disk larger than the unit disk. If the two polynomials have no common factor, the conditions become

$$
\boxed{\phi(z)\ne0\text{ for }|z|\leq1\quad\text{(causality)},\qquad
\theta(z)\ne0\text{ for }|z|\leq1\quad\text{(invertibility)}.}
$$

Indeed, outside-disk roots leave a radius of convergence greater than one, so the coefficients decay geometrically and are absolutely summable. Conversely an uncancelled pole inside or on the unit disk prevents the required stable power series. If factors are common, apply the criterion after cancellation, to the noise-driven solution rather than additional homogeneous components. The [backshift operator](../../../../../backshift-operator.md) translates these power series into the desired one-sided filters.

The original representation has $\phi(z)=1-2z$ and $\theta(z)=1+2z$, with roots $1/2$ and $-1/2$. There is no cancellation. Hence **it is neither causal nor invertible** relative to its specified driving noise. [Stationarity](../../../../../stationary-process.md) is nevertheless possible through a two-sided solution: expanding the autoregressive inverse in negative powers gives

$$
X_t=-\epsilon_t-2\sum_{j\geq1}2^{-j}\epsilon_{t+j}.
$$

This is an [anticausal time series](../../../../../anticausal-time-series.md) representation with square-summable coefficients.

To establish the alternative representation on the same process, define

$$
\eta_t=\frac{1-\tfrac12B}{1+\tfrac12B}X_t
=X_t+2\sum_{j\geq1}\left(-\frac12\right)^jX_{t-j}.
$$

The inverse of $1+\tfrac12B$ is a stable one-sided filter. For $|z|=1$, the identities $|1+2z|^2=4|1+z/2|^2$ and $|1-2z|^2=4|1-z/2|^2$ give

$$
\left|\frac{1-z/2}{1+z/2}\right|^2
\left|\frac{1+2z}{1-2z}\right|^2=1.
$$

The [time-series spectral density](../../../../../spectral-density-of-a-stationary-process.md) of $X$ is $\sigma^2|1+2e^{-i\omega}|^2/(2\pi|1-2e^{-i\omega}|^2)$; therefore the defined $\eta$ has constant [time-series spectral density](../../../../../spectral-density-of-a-stationary-process.md) $\sigma^2/(2\pi)$. Its mean is zero, its [variance](../../../../../variance-split.md) is $\sigma^2$, and all its nonzero-lag [autocovariances](../../../../../autocovariance.md) vanish. It is thus [weak white noise](../../../../../weak-white-noise.md). Its definition directly gives

$$
\boxed{X_t=\frac12X_{t-1}+\frac12\eta_{t-1}+\eta_t.}
$$

This [root reflection of an ARMA representation](../../../../../root-reflection-of-an-arma-representation.md) has roots $2,-2$, so is causal and invertible. A constant spectrum proves whiteness, not independence of non-Gaussian coordinates; no Gaussian assumption is needed for the required [white noise](../../../../../white-noise.md) representation.

For [best linear prediction from an infinite past](../../../../../best-linear-prediction-from-an-infinite-past.md), let $\mathcal H_0$ be the closed linear span of $X_t$ with $t\leq0$. The causal representation expresses every such $X_t$ in present and past $\eta$ values, while invertibility puts every $\eta_t$ with $t\leq0$ in $\mathcal H_0$. In particular $\eta_1$ is orthogonal to $\mathcal H_0$. The representation at time one then gives the [orthogonal projection](../../../../../orthogonal-projection.md)

$$
\widehat X_1=\frac12X_0+\frac12\eta_0
=X_0-\frac12X_{-1}+\frac14X_{-2}-\cdots.
$$

Consequently **the best linear predictor and its error variance are**

$$
\boxed{\widehat X_1=\sum_{j\geq0}\left(-\frac12\right)^jX_{-j},\qquad
X_1-\widehat X_1=\eta_1,\qquad \operatorname{Var}(X_1-\widehat X_1)=\sigma^2.}
$$

Orthogonality proves optimality among linear predictors in the closed past span, without asserting that the predictor must be the conditional mean for a non-Gaussian process.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
