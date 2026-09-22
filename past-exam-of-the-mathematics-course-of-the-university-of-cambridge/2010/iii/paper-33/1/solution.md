<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a series with constant mean $\mu$, write $X_t=x_t-\mu$. An [autoregressive moving-average process](../../../../../autoregressive-moving-average-model.md) has the form

$$
X_t=\sum_{j=1}^p a_jX_{t-j}+w_t+\sum_{j=1}^q b_jw_{t-j},
$$

where $w_t$ is zero-mean [white noise](../../../../../white-noise.md) with [variance](../../../../../variance-split.md) $\sigma_w^2>0$. The [backshift operator](../../../../../backshift-operator.md) is $BX_t=X_{t-1}$. Define the [autoregressive polynomial](../../../../../autoregressive-polynomial.md) and the [moving-average polynomial](../../../../../moving-average-polynomial.md) by

$$
\Phi(z)=1-\sum_{j=1}^pa_jz^j,\qquad
\Theta(z)=1+\sum_{j=1}^qb_jz^j.
$$

The [autoregressive operator](../../../../../autoregressive-operator.md) and [moving-average operator](../../../../../moving-average-operator.md) give the concise equation

$$
\boxed{\Phi(B)X_t=\Theta(B)w_t.}
$$

Orders are normally specified minimally, with nonzero last coefficients and no common polynomial factor. A displayed unreduced equation can have larger orders than the process actually needs.

Causality means that the stationary process can be recovered from present and past noise:

$$
X_t=\sum_{j\ge0}\psi_jw_{t-j},\qquad\sum_j|\psi_j|<\infty.
$$

Invertibility means that the noise can be recovered from present and past observations:

$$
w_t=\sum_{j\ge0}\pi_jX_{t-j},\qquad\sum_j|\pi_j|<\infty.
$$

The [causality and invertibility root criteria for an ARMA model](../../../../../causality-and-invertibility-root-criteria-for-an-arma-model.md), for the reduced representation, are

$$
\boxed{\Phi(z)\ne0\ (|z|\le1)\quad\text{for causality},\qquad
\Theta(z)\ne0\ (|z|\le1)\quad\text{for invertibility}.}
$$

Indeed the transfer series are $\sum\psi_jz^j=\Theta(z)/\Phi(z)$ and $\sum\pi_jz^j=\Phi(z)/\Theta(z)$. When all denominator roots lie outside the closed unit disc, each rational function is analytic on a larger disc, so its Taylor coefficients decay geometrically and are absolutely summable. Conversely, a genuine denominator zero in the closed unit disc gives a pole incompatible with such a convergent filter. The reduced-representation proviso prevents a cancelled root from being mistaken for an obstruction.

For [order identification by autocorrelation cutoffs](../../../../../order-identification-by-autocorrelation-cutoffs.md), first estimate the [sample autocorrelation function](../../../../../sample-autocorrelation-function.md) and [sample partial autocorrelation function](../../../../../sample-partial-autocorrelation-function.md) from a suitably stationary, centred series. The [autocorrelation function](../../../../../autocorrelation.md) is $\rho(h)=\operatorname{Cov}(X_t,X_{t-h})/\operatorname{Var}(X_t)$. The lag-$h$ [partial autocorrelation function](../../../../../partial-autocorrelation-function.md) is the last coefficient in the best [linear regression](../../../../../linear-regression-split.md) of $X_t$ on $X_{t-1},\ldots,X_{t-h}$, equivalently the correlation left after removing the intervening lags.

For a pure [moving-average model](../../../../../moving-average-model.md) of order $q$, observations more than $q$ lags apart share no noise, so the population ACF is zero beyond $q$, while the PACF usually tails off. For a pure [autoregressive model](../../../../../autoregressive-model.md) of order $p$, the PACF is zero beyond $p$, while the ACF usually decays, possibly with damped oscillation. Thus a clear sample ACF cutoff suggests an MA order and a clear PACF cutoff suggests an AR order. For a mixed [ARMA](../../../../../autoregressive-moving-average-model.md) process both usually tail off, so these plots guide a small set of candidate orders rather than determine $p,q$ uniquely. Sampling variation blurs cutoffs; compare fitted candidates and check that their residual ACF resembles [white noise](../../../../../white-noise.md). Common-factor cancellation can also disguise the orders in a displayed equation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
