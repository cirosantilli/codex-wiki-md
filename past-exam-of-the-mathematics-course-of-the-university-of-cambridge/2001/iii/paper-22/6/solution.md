<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The entire term structure is naturally indexed by observation time and maturity. Work under a [risk-neutral measure](../../../../../risk-neutral-measure.md) $Q$ and let $f(t,T)$ be the [instantaneous forward rate](../../../../../instantaneous-forward-rate.md), with $0\le t\le T$. Define the [short rate](../../../../../short-rate.md) $r_t=f(t,t)$, the [bank account](../../../../../bank-account.md) $B_t=\exp(\int_0^t r_sds)$ and the [zero-coupon bond](../../../../../zero-coupon-bond.md) price

$$
P(t,T)=\exp\left(-\int_t^T f(t,u)du\right).
$$

An arbitrary Gaussian mean and [covariance](../../../../../covariance.md) need not make these bond prices consistent. Absence of [arbitrage](../../../../../arbitrage.md) requires the discounted traded bonds to be [martingales](../../../../../martingale-split.md) under a suitable equivalent measure. We derive the constraint explicitly.

Consider the [Gaussian forward-rate field](../../../../../gaussian-forward-rate-field.md) $f(t,T)=m(t,T)+X(t,T)$ with deterministic mean and centered [Gaussian random field](../../../../../gaussian-random-field.md) satisfying

$$
\operatorname{Cov}(X(s,T),X(t,U))=c(s\wedge t;T,U),\qquad c(0;T,U)=0.
$$

The maturity kernel is symmetric, and its increments in the first parameter must be positive semidefinite kernels. Assume continuity, separability and sufficient integrability for the following mean-square integrals and maturity derivatives. This [covariance](../../../../../covariance.md) gives independent observation-time increments, while permitting correlated fluctuations across all maturities. The [filtration](../../../../../filtration-probability-theory.md) contains the history of the whole observed forward curve.

For a fixed maturity $T$, collect the past [short rate](../../../../../short-rate.md) and the present curve into the [integrated Gaussian forward-rate process](../../../../../integrated-gaussian-forward-rate-process.md)

$$
Y(t,T)=\int_0^T X(t\wedge u,u)du,
\quad A(t,T)=\int_0^t m(u,u)du+\int_t^T m(t,u)du.
$$

Then $P(t,T)/B_t=e^{-A(t,T)-Y(t,T)}$. Its centered Gaussian [variance](../../../../../variance-split.md) is

$$
v(t,T)=\int_0^T\int_0^T c(t\wedge u\wedge w;u,w)du\,dw.
$$

For $s<t$ and an observed field coordinate $X(z,U)$ with $z\le s$, the [covariance](../../../../../covariance.md) of $Y(t,T)-Y(s,T)$ with it is zero: the integrand is

$$
c(t\wedge u\wedge z;u,U)-c(s\wedge u\wedge z;u,U)=0.
$$

The [uncorrelated jointly Gaussian variables are independent](../../../../../uncorrelated-jointly-normal-variables-are-independent.md) principle therefore makes the increment independent of the earlier field [filtration](../../../../../filtration-probability-theory.md). Its [variance](../../../../../variance-split.md) is $v(t,T)-v(s,T)$, since the same [covariance](../../../../../covariance.md) calculation gives $\operatorname{Cov}(Y(t,T),Y(s,T))=v(s,T)$. Conditional Gaussian exponential [expectation](../../../../../expected-value.md) now gives

$$
\mathbb E_Q[e^{-A(t,T)-Y(t,T)}\mid\mathcal F_s]
=e^{-A(t,T)-Y(s,T)+[v(t,T)-v(s,T)]/2}.
$$

Hence the exact bond-martingale condition is

$$
A(t,T)-A(0,T)=\frac12v(t,T).
$$

Differentiating in maturity, using symmetry of the [covariance](../../../../../covariance.md), gives the [Gaussian forward-rate covariance drift restriction](../../../../../gaussian-forward-rate-covariance-drift-restriction.md)

$$
\boxed{m(t,T)=f(0,T)+\int_0^T c(t\wedge u;u,T)du.}
$$

This is necessary and sufficient. For sufficiency, the derivatives of the half-variance identity agree by the displayed restriction. Its integration constant also agrees at $T=t$, because

$$
A(t,t)-A(0,t)=\int_0^t\int_0^u c(w;w,u)dw\,du=\frac12v(t,t).
$$

Thus the full identity follows for every $T\ge t$, and the [conditional expectation](../../../../../conditional-expectation.md) calculation proves a true [martingale](../../../../../martingale-split.md), not merely zero formal drift. The initial mean $f(0,T)=-\partial_T\log P(0,T)$ fits the observed initial curve exactly; thereafter the mean adjustment is fixed by the [covariance](../../../../../covariance.md).

If $c(t;T,U)=\int_0^t k_s(T,U)ds$ is time-differentiable, the forward drift is $a(t,T)=\int_t^T k_t(T,u)du$. Writing

$$
k_t(T,U)=\langle\sigma(t,T),\sigma(t,U)\rangle
$$

with deterministic finite- or Hilbert-space factor loadings gives the [Heath-Jarrow-Morton model](../../../../../heath-jarrow-morton-model.md)

$$
df(t,T)=\left\langle\sigma(t,T),\int_t^T\sigma(t,u)du\right\rangle dt
+\langle\sigma(t,T),dW_t^Q\rangle.
$$

With $\Sigma(t,T)=\int_t^T\sigma(t,u)du$, [Itô formula](../../../../../ito-s-lemma.md) independently verifies bond drift $r_t-\int_t^Ta(t,u)du+\|\Sigma(t,T)\|^2/2=r_t$. Finite-factor models give low-rank maturity correlations; a genuine random field or an infinite factor space permits a much richer [covariance](../../../../../covariance.md) structure. Gaussian forward rates and [short rates](../../../../../short-rate.md) may be negative, although the exponential bond prices stay positive. Under a physical measure, a [Girsanov theorem](../../../../../girsanov-theorem.md) market-risk-premium change adds $\langle\sigma,\lambda\rangle$ to the forward drift; deterministic premia preserve Gaussianity, whereas arbitrary adapted premia need not.

For a concrete two-parameter example, let $X$ be a standard [Brownian sheet](../../../../../brownian-sheet.md), so $c(t;T,U)=t\min(T,U)$. The restriction gives

$$
m(t,T)=f(0,T)+\frac12tT^2-\frac16t^3\qquad(t\le T).
$$

Indeed $\int_0^T\min(t,u)u\,du=t^3/3+t(T^2-t^2)/2$. This demonstrates directly how a [Gaussian random field](../../../../../gaussian-random-field.md) determines the compensating forward drift.

For the one-factor constant-volatility case, $\sigma(t,T)=\eta$, the [Constant-coefficient Ho-Lee model](../../../../../gaussian-short-rate-model-with-constant-coefficients.md) has

$$
f(t,T)=f(0,T)+\eta^2(tT-t^2/2)+\eta W_t^Q,
\qquad r_t=f(0,t)+\eta^2t^2/2+\eta W_t^Q,
$$

and

$$
P(t,T)=\frac{P(0,T)}{P(0,t)}
\exp\left[-\eta(T-t)W_t^Q-\frac12\eta^2tT(T-t)\right].
$$

These follow by integrating the explicit curve, not by assigning the short-rate drift independently. Exponentially decaying loadings $\eta e^{-\kappa(T-t)}$ instead give a Gaussian mean-reverting [Hull-White model](../../../../../hull-white-model.md), with bond-rate loading $(1-e^{-\kappa(T-t)})/\kappa$.

A practical advantage is an explicit [Gaussian bond-option formula](../../../../../gaussian-bond-option-formula.md). For a call of strike $K>0$ exercised at $T$ on a bond maturing at $U>T$, use the [T-forward measure](../../../../../t-forward-measure.md) with numéraire $P(t,T)$. The forward bond ratio $F_t=P(t,U)/P(t,T)$ has a [lognormal distribution](../../../../../log-normal-distribution.md) under that measure, with remaining integrated [variance](../../../../../variance-split.md)

$$
q=\int_t^T\|\Sigma(s,U)-\Sigma(s,T)\|^2ds.
$$

Its [martingale](../../../../../martingale-split.md) property makes the conditional log mean $\log F_t-q/2$. Evaluating the positive-part lognormal integral gives

$$
\boxed{C_t=P(t,U)\Phi(d_1)-KP(t,T)\Phi(d_2),\quad
 d_1=\frac{\log(F_t/K)+q/2}{\sqrt q},\quad d_2=d_1-\sqrt q.}
$$

For $q=0$, the limit is $(P(t,U)-KP(t,T))^+$. The forward measure accounts for the stochastic [short rate](../../../../../short-rate.md); discounting by one deterministic interest rate would generally be wrong. Calibration selects a positive-semidefinite [covariance](../../../../../covariance.md) structure fitting observed rate co-movements and option prices, with the no-arbitrage mean restriction imposed afterward. With more independent factors than the available traded bond exposures span, the market is incomplete and additional claims need a specified pricing measure or risk-premium model. The Gaussian field is therefore a flexible curve model with explicit consistency and pricing equations, rather than a claim that all possible rate risks are hedgeable.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
