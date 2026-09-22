<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [weakly stationary process](../../../../../weakly-stationary-process.md) has finite second moments, a [mean](../../../../../expected-value.md) $m=E X_t$ independent of $t$, and a [covariance](../../../../../covariance.md) depending only on the separation of the observations. Its [autocovariance function](../../../../../autocovariance.md) and [autocorrelation function](../../../../../autocorrelation.md) are

$$
\gamma(h)=E[(X_{t+h}-m)(X_t-m)],\qquad \rho(h)=\gamma(h)/\gamma(0),
$$

where the [autocorrelation](../../../../../autocorrelation.md) requires $\gamma(0)>0$.

Write the [autoregressive polynomial](../../../../../autoregressive-polynomial.md) as $A(z)=1-\alpha z+\alpha z^2$, so the [autoregressive model](../../../../../autoregressive-model.md) is $A(B)X_t=\epsilon_t$, with $B$ the [backshift operator](../../../../../backshift-operator.md). It is important to distinguish a [weakly stationary process](../../../../../weakly-stationary-process.md) from a [causal time series](../../../../../causal-time-series.md): [weak stationarity](../../../../../weakly-stationary-process.md) alone does not require $X_t$ to depend only on present and past [white noise](../../../../../white-noise.md).

For a two-sided [weakly stationary process](../../../../../weakly-stationary-process.md), the [two-sided stationary inverse of an autoregressive polynomial](../../../../../two-sided-stationary-inverse-of-an-autoregressive-polynomial.md) exists and is unique if $A$ has no root on the [unit circle](../../../../../complex-unit-circle.md). To find the excluded parameters, set $z=e^{i\lambda}$. The imaginary part of $A(z)=0$ gives

$$
\alpha\sin\lambda(2\cos\lambda-1)=0.
$$

The case $\alpha=0$ is harmless. The possible frequencies are $0,\pi,\pm\pi/3$. Since $A(1)=1$, $A(-1)=1+2\alpha$ and $A(e^{\pm i\pi/3})=1-\alpha$, the exceptional parameters are $-1/2$ and $1$. Thus, with nondegenerate [white noise](../../../../../white-noise.md), the literal two-sided answer is

$$
\boxed{\alpha\in\mathbb R\setminus\{-\tfrac12,1\}.}
$$

For completeness, away from those values $1/A(z)$ has an absolutely summable [Laurent series](../../../../../laurent-series.md) on an annulus containing the [unit circle](../../../../../complex-unit-circle.md). Its bilateral coefficients define an $L^2$-convergent [linear filter of a stationary time series](../../../../../linear-filter-of-a-stationary-time-series.md) applied to $\epsilon_t$, giving the required solution. Applying the same inverse to the equation gives uniqueness. At an exceptional value, the [spectral measure of a stationary time series](../../../../../spectral-measure-of-a-stationary-time-series.md) would have to satisfy $|A(e^{i\lambda})|^2\mu_X(d\lambda)=\sigma^2d\lambda/(2\pi)$. A zero of $A$ on the [unit circle](../../../../../complex-unit-circle.md) makes the resulting density nonintegrable near that zero, contradicting finite [variance](../../../../../variance-split.md).

If the usual additional [causal time series](../../../../../causal-time-series.md) convention is intended, the [causality root criterion for an autoregressive model](../../../../../causality-root-criterion-for-an-autoregressive-model.md) requires the roots of $A$ to lie outside the closed [unit disk](../../../../../unit-disk.md). Equivalently, the roots of $u^2-\alpha u+\alpha$ lie strictly inside it. The real quadratic stability conditions reduce to $|\alpha|<1$ and $1+2\alpha>0$, giving the narrower answer

$$
\boxed{-\tfrac12<\alpha<1\quad\text{for the causal solution}.}
$$

The printed question does not explicitly impose this extra convention. Both answers have therefore been distinguished. If $\sigma^2=0$, the exceptional parameters permit nonunique stationary homogeneous solutions rather than the nonexistence conclusion above.

At $\alpha=-1/12$,

$$
A(z)=(1-z/4)(1+z/3),\qquad
\frac1{A(z)}=\frac{3/7}{1-z/4}+\frac{4/7}{1+z/3}.
$$

Consequently the [Wold representation](../../../../../wold-decomposition.md) is

$$
\boxed{X_t=\sum_{j=0}^{\infty}\psi_j\epsilon_{t-j},\qquad
\psi_j=\frac37\left(\frac14\right)^j+\frac47\left(-\frac13\right)^j.}
$$

The coefficients are absolutely summable, and $\psi_0=1$. The past of $X$ lies in the closed linear span of the past [white noise](../../../../../white-noise.md); conversely $\epsilon_t=A(B)X_t$ recovers that noise from present and past $X$. Thus $\epsilon_t$ is orthogonal to the past of $X$ and is its one-step linear prediction error, as required for the [Wold decomposition](../../../../../wold-decomposition.md). There is no deterministic component.

Using orthogonality of the [white noise](../../../../../white-noise.md), put $H=|h|$ and calculate the [autocovariance](../../../../../autocovariance.md) by geometric sums:

$$
\begin{aligned}
\gamma(h)/\sigma^2
&=\sum_{j\geq0}\psi_j\psi_{j+H}\\
&=\frac9{49}\frac{(1/4)^H}{1-1/16}
 +\frac{16}{49}\frac{(-1/3)^H}{1-1/9}
 +\frac{12}{49}\frac{(1/4)^H+(-1/3)^H}{1+1/12}\\
&=\frac{192}{455}(1/4)^H+\frac{54}{91}(-1/3)^H.
\end{aligned}
$$

Hence

$$
\boxed{\gamma(h)=\frac{6\sigma^2}{455}\left[32(1/4)^{|h|}+45(-1/3)^{|h|}\right].}
$$

In particular, $\gamma(0)=66\sigma^2/65$ and $\gamma(1)=-6\sigma^2/65$; these also satisfy the [Yule-Walker equations](../../../../../yule-walker-equations.md) for this [autoregressive model](../../../../../autoregressive-model.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
