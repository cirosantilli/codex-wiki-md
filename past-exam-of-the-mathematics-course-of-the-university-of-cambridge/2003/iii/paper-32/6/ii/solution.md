<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [Gaussian forward-rate field](../../../../../../gaussian-forward-rate-field.md) models the whole [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) curve. Let $H$ be a real separable [Hilbert space](../../../../../../hilbert-space-split.md), let $W$ be a [cylindrical Brownian motion](../../../../../../cylindrical-brownian-motion.md), and let deterministic $\sigma(t,T)\in H$ satisfy the maturity-integrability and square-integrability conditions needed below. For a deterministic initial curve, specify under $Q$

$$
df(t,T)=\alpha(t,T)dt+\langle\sigma(t,T),dW_t\rangle,\qquad 0\leq t\leq T.
$$

Using an orthonormal basis, the noise is $\sum_j\sigma_j(t,T)dW_t^j$; an infinite-dimensional cylindrical noise need not exist as an $H$-valued random vector. Its covariation kernel across maturities is the positive semidefinite kernel $C_t(T,U)=\langle\sigma(t,T),\sigma(t,U)\rangle$. Thus arbitrary suitable maturity-correlation kernels can be represented by Hilbert-space factors, while finitely many factors give finite-rank kernels.

No [arbitrage](../../../../../../arbitrage.md) requires a drift restriction. Define the [zero-coupon bond](../../../../../../zero-coupon-bond.md) price and integrated volatility by

$$
P(t,T)=\exp\!\left(-\int_t^T f(t,u)du\right),\qquad\Sigma(t,T)=\int_t^T\sigma(t,u)du,\qquad r_t=f(t,t).
$$

Differentiation of the moving lower endpoint and the [Itô formula](../../../../../../ito-s-lemma.md) give

$$
\frac{dP(t,T)}{P(t,T)}=\left[r_t-\int_t^T\alpha(t,u)du+\frac12\|\Sigma(t,T)\|^2\right]dt-\langle\Sigma(t,T),dW_t\rangle.
$$

The discounted bond must have zero drift. Differentiating $\int_t^T\alpha(t,u)du=\tfrac12\|\Sigma(t,T)\|^2$ with respect to maturity yields the [Heath-Jarrow-Morton model](../../../../../../heath-jarrow-morton-model.md) restriction

$$
\boxed{\alpha(t,T)=\langle\sigma(t,T),\Sigma(t,T)\rangle=\int_t^T C_t(T,u)du.}
$$

This is why forward-rate drift and covariance cannot be selected independently in an arbitrage-free random-field model. With deterministic volatilities square-integrable on the finite horizon, the discounted bond stochastic exponential is a true [martingale](../../../../../../martingale-split.md), not only a [local martingale](../../../../../../local-martingale.md).

The solution is explicitly Gaussian:

$$
f(t,T)=f(0,T)+\int_0^t\alpha(s,T)ds+\int_0^t\langle\sigma(s,T),dW_s\rangle,
$$

with mean given by the first two terms and covariance

$$
\boxed{\operatorname{Cov}(f(t,T),f(s,U))=\int_0^{\min(t,s)}C_v(T,U)dv.}
$$

The entire [Gaussian random field](../../../../../../gaussian-random-field.md) can therefore be calibrated through its initial curve and maturity covariance structure. Bond prices are exponential functionals of these Gaussian rates; conditional bond ratios have lognormal laws under appropriate [forward measures](../../../../../../forward-measure.md). Negative rates are possible. A large or infinite volatility space provides rich maturity correlations, but Gaussianity alone supplies neither a low-dimensional Markov state nor positivity of rates.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
