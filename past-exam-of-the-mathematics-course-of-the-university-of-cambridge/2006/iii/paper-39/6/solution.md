<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

An [interest rate](../../../../../interest-rate.md) model must describe a whole [term structure of interest rates](../../../../../yield-curve.md), not just one future scalar rate. Let $P(t,T)$ be the time-$t$ price of a unit [zero-coupon bond](../../../../../zero-coupon-bond.md) maturing at $T$. For a sufficiently regular maturity curve, define the [instantaneous forward rate](../../../../../instantaneous-forward-rate.md) and [short rate](../../../../../short-rate.md) by

$$
f(t,T)=-\partial_T\log P(t,T),\qquad r_t=f(t,t).
$$

Since $P(t,t)=1$, integration gives

$$
P(t,T)=\exp\left(-\int_t^T f(t,u)\,du\right),\qquad
B_t=\exp\left(\int_0^t r_s\,ds\right).
$$

Here $B$ is the [continuous-time bank account](../../../../../continuous-time-bank-account.md). Thus modelling the two-parameter field $f(t,T)$ determines both the bonds and the discounting account. A [Gaussian random field](../../../../../gaussian-random-field.md) means that every finite collection of its values is jointly Gaussian; merely making each individual forward rate normally distributed is insufficient.

A useful arbitrage-free construction works under a money-market [risk-neutral measure](../../../../../risk-neutral-measure.md) $Q$. Take independent [Brownian motions](../../../../../brownian-motion-split.md) $W^j$, deterministic coefficient sequences $\sigma_j(t,T)$, and a deterministic initial forward curve $f(0,T)$. With the coefficients viewed as vectors in a separable [Hilbert space](../../../../../hilbert-space-split.md) $H$, write

$$
df(t,T)=\alpha(t,T)dt+\langle\sigma(t,T),dW_t\rangle_H,\qquad0\leq t\leq T.
$$

For infinitely many factors, the last term means the $L^2$ limit of $\sum_j\sigma_j(t,T)dW_t^j$, not an assumption that the infinite vector of [Brownian motions](../../../../../brownian-motion-split.md) is itself $H$-valued. Require $\int_0^t\|\sigma(s,T)\|_H^2ds<\infty$ and the maturity/time regularity needed for stochastic integration and exchange of integrals. Deterministic [drift](../../../../../drift-coefficient.md) and volatility make this a [Gaussian forward-rate field](../../../../../gaussian-forward-rate-field.md).

The field [covariance](../../../../../covariance.md) is determined by

$$
c_t(T,U)=\langle\sigma(t,T),\sigma(t,U)\rangle_H,\qquad
\operatorname{Cov}(f(t,T),f(s,U))=\int_0^{\min(t,s)}c_v(T,U)\,dv.
$$

For every finite set of maturities, $(c_t(T_i,T_j))$ must be [positive semidefinite](../../../../../positive-semidefinite-matrix.md). A one-factor model has rank-one instantaneous [covariance](../../../../../covariance.md), while additional or infinitely many factors permit richer correlations along the [yield curve](../../../../../yield-curve.md). Equivalently one can drive the curve with a maturity-correlated Brownian field $Z_t(T)$ satisfying $d\langle Z(T),Z(U)\rangle_t=c(T,U)dt$. A [Brownian sheet](../../../../../brownian-sheet.md) gives the example

$$
\operatorname{Cov}(Z_t(T),Z_s(U))=\min(t,s)\min(T,U).
$$

Multiplication by deterministic maturity-dependent amplitudes, or deterministic increasing changes of the two sheet coordinates, gives further Gaussian [covariance](../../../../../covariance.md) structures. A [covariance](../../../../../covariance.md) specification alone is not sufficient: the forward [drift](../../../../../drift-coefficient.md) must also obey absence of [arbitrage](../../../../../arbitrage.md).

To derive that [drift](../../../../../drift-coefficient.md) restriction, put

$$
\Sigma(t,T)=\int_t^T\sigma(t,u)\,du.
$$

Differentiate the moving lower endpoint in $\log P(t,T)=-\int_t^T f(t,u)du$ to obtain

$$
d\log P(t,T)=\left(r_t-\int_t^T\alpha(t,u)du\right)dt-\langle\Sigma(t,T),dW_t\rangle_H.
$$

The [Itô formula](../../../../../ito-s-lemma.md) therefore gives

$$
\frac{dP(t,T)}{P(t,T)}
=\left(r_t-\int_t^T\alpha(t,u)du+\tfrac12\|\Sigma(t,T)\|_H^2\right)dt
-\langle\Sigma(t,T),dW_t\rangle_H.
$$

Discounted bond prices must be [martingales](../../../../../martingale-split.md) under $Q$. Their [drift](../../../../../drift-coefficient.md) vanishes precisely when $\int_t^T\alpha(t,u)du=\tfrac12\|\Sigma(t,T)\|_H^2$. Differentiating in maturity gives the [Heath-Jarrow-Morton model](../../../../../heath-jarrow-morton-model.md) restriction

$$
\boxed{\alpha(t,T)=\langle\sigma(t,T),\Sigma(t,T)\rangle_H
=\int_t^T c_t(T,u)\,du.}
$$

For scalar amplitudes $v(t,T)$ multiplying a field with [covariance](../../../../../covariance.md) kernel $c(T,U)$, this becomes $\alpha(t,T)=v(t,T)\int_t^T v(t,u)c(T,u)du$. The extra maturity correlation factor cannot in general be dropped.

The complete Gaussian specification is consequently

$$
f(t,T)=f(0,T)+\int_0^t\int_s^T c_s(T,u)\,du\,ds
+\int_0^t\langle\sigma(s,T),dW_s\rangle_H.
$$

Its mean and [covariance](../../../../../covariance.md) follow immediately from deterministic integration and the [Itô isometry](../../../../../ito-isometry.md). The initial [yield curve](../../../../../yield-curve.md) is an input, so fitting initial bond prices requires choosing $f(0,T)$ rather than changing a few scalar parameters. With the displayed [drift](../../../../../drift-coefficient.md), the discounted bond obeys

$$
\frac{d(P(t,T)/B_t)}{P(t,T)/B_t}=-\langle\Sigma(t,T),dW_t\rangle_H.
$$

On finite horizons, deterministic [square-integrable](../../../../../square-integrable-function.md) bond volatility gives an expectation-one [stochastic exponential](../../../../../doleans-dade-exponential.md), hence a true [discounted bond price martingale](../../../../../discounted-bond-price-martingale.md). This supplies an arbitrage-free pricing model for admissible [portfolios](../../../../../investment-portfolio.md) in any finite collection of these bonds. Under a physical measure, a [market price of risk](../../../../../market-price-of-risk.md) vector changes the [drift](../../../../../drift-coefficient.md): if $dW_t^Q=dW_t^P+\lambda_tdt$, then the physical forward [drift](../../../../../drift-coefficient.md) is $\alpha(t,T)+\langle\sigma(t,T),\lambda_t\rangle_H$. Historical mean changes must therefore not be inserted in place of the risk-neutral [drift](../../../../../drift-coefficient.md) restriction. Gaussianity under both measures additionally requires suitable deterministic [drift](../../../../../drift-coefficient.md) changes; state-dependent risk premiums need not preserve Gaussianity under the physical measure.

There is also a useful general consistency test for a proposed Gaussian field beyond this independent-increment construction. Define

$$
L_t^T=\int_0^t f(s,s)\,ds+\int_t^T f(t,u)\,du,
\qquad B_t^{-1}P(t,T)=e^{-L_t^T}.
$$

In the filtration generated by a Gaussian field, conditional distributions of such linear functionals are Gaussian. For $s\leq t\leq T$, the [martingale](../../../../../martingale-split.md) requirement is therefore exactly

$$
\boxed{\mathbb E_Q[L_t^T\mid\mathcal F_s]-\tfrac12\operatorname{Var}_Q(L_t^T\mid\mathcal F_s)=L_s^T.}
$$

This follows by taking the conditional exponential moment and equating it to $e^{-L_s^T}$. It constrains both the deterministic mean and the covariance-induced conditional mean. Matching only unconditional discounted bond [expectations](../../../../../expected-value.md) does not suffice. For the Brownian-field construction, the [Heath-Jarrow-Morton model](../../../../../heath-jarrow-morton-model.md) restriction realizes this consistency condition through local [drift](../../../../../drift-coefficient.md) cancellation.

Gaussian structure makes [risk-neutral pricing](../../../../../risk-neutral-pricing.md) particularly tractable. As a finite-factor example, take the [Vasicek model](../../../../../vasicek-model.md) under $Q$:

$$
dr_t=a(b-r_t)dt+\eta dW_t^Q,\qquad a>0.
$$

Solving this [Ornstein-Uhlenbeck process](../../../../../ornstein-uhlenbeck-process.md) gives, for $u\geq t$,

$$
r_u=b+(r_t-b)e^{-a(u-t)}+\eta\int_t^u e^{-a(u-v)}dW_v^Q.
$$

Hence, with $\tau=T-t$ and $B(\tau)=(1-e^{-a\tau})/a$, the conditional Gaussian integral $I=\int_t^T r_u du$ has

$$
\mathbb E[I\mid\mathcal F_t]=b\tau+(r_t-b)B(\tau),
\qquad
\operatorname{Var}(I\mid\mathcal F_t)=\frac{\eta^2}{a^2}\left[\tau-2B(\tau)+\frac{1-e^{-2a\tau}}{2a}\right].
$$

The [exponential moment](../../../../../exponential-moment.md) identity for a normal variable now gives the [zero-coupon bond](../../../../../zero-coupon-bond.md) price $P(t,T)=\mathbb E_Q[e^{-I}\mid\mathcal F_t]=A(\tau)e^{-B(\tau)r_t}$, where

$$
\log A(\tau)=\left(b-\frac{\eta^2}{2a^2}\right)(B(\tau)-\tau)-\frac{\eta^2}{4a}B(\tau)^2.
$$

This outlines the derivation of the familiar exponential-affine form without assuming a deterministic future discount rate. More general forward-field models need not reduce to a finite-dimensional Markov short-rate process.

For another application, a call at time $T$ on a unit maturity-$U$ bond, with $t<T<U$ and strike $K>0$, is priced under the [T-forward measure](../../../../../t-forward-measure.md), using $P(t,T)$ as [numéraire](../../../../../numeraire.md). The bond-price ratio $F_s=P(s,U)/P(s,T)$ is a [martingale](../../../../../martingale-split.md) under that measure and has deterministic volatility $-(\Sigma(s,U)-\Sigma(s,T))$. It is consequently lognormal, with integrated log-variance

$$
V=\int_t^T\|\Sigma(s,U)-\Sigma(s,T)\|_H^2ds.
$$

Integrating the lognormal payoff gives the [Gaussian bond-option formula](../../../../../gaussian-bond-option-formula.md)

$$
\boxed{C_t=P(t,U)\Phi(d_1)-KP(t,T)\Phi(d_2),\quad
d_1=\frac{\log(P(t,U)/(KP(t,T)))+V/2}{\sqrt V},\quad d_2=d_1-\sqrt V.}
$$

At $V=0$ use $(P(t,U)-KP(t,T))^+$. The same idea prices other suitable Gaussian-rate derivatives through forward measures and normal exponential moments.

The attractions are exact initial-curve fitting, explicit [covariance](../../../../../covariance.md) control across maturities, and tractable bond and option prices. The limitations are also structural: Gaussian [short rates](../../../../../short-rate.md) and [instantaneous forward rates](../../../../../instantaneous-forward-rate.md) generally can be negative; finite-factor specifications restrict maturity correlations; and deterministic volatilities cannot reproduce arbitrary stochastic changes in rate dispersion. An infinite-factor model allows richer [covariance](../../../../../covariance.md) but typically leaves risks that cannot be spanned by finitely many traded bonds. Thus Gaussianity is a useful modelling choice, not by itself a guarantee of positivity, [market completeness](../../../../../complete-market.md), or absence of [arbitrage](../../../../../arbitrage.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
