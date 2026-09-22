<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [one-factor short-rate model](../../../../../one-factor-short-rate-model.md) uses a single scalar state, normally the [short rate](../../../../../short-rate.md) itself. Under the physical probability measure write

$$
dr_t=\mu(t,r_t)dt+\eta(t,r_t)dW_t,\qquad B_t=\exp\left(\int_0^t r_sds\right).
$$

The second process is the [continuous-time bank account](../../../../../continuous-time-bank-account.md). Specifying the physical diffusion alone does not determine bond prices: it must be accompanied by the [market price of risk](../../../../../market-price-of-risk.md) $\lambda(t,r)$, or equivalently by pricing-measure dynamics. If the [Girsanov theorem](../../../../../girsanov-theorem.md) applies to the likelihood $\mathcal E(-\int\lambda\,dW)$, then under the [risk-neutral measure](../../../../../risk-neutral-measure.md)

$$
dr_t=\mu_Q(t,r_t)dt+\eta(t,r_t)dW_t^Q,\qquad\mu_Q=\mu-\eta\lambda.
$$

Changing measure alters drift, not [quadratic variation](../../../../../quadratic-variation.md). The coefficients need conditions for a nonexplosive solution and for the relevant discounted prices and measure-change density to be true [martingales](../../../../../martingale-split.md).

A unit [zero-coupon bond](../../../../../zero-coupon-bond.md) maturing at $T$ has price

$$
\boxed{P(t,r;T)=\mathbb E^Q\left[\left.\exp\left(-\int_t^T r_sds\right)\right|r_t=r\right].}
$$

The Markov property makes current time and rate sufficient state variables. Apply [Itô formula](../../../../../ito-s-lemma.md) to $P(t,r_t;T)/B_t$. Its drift must vanish, giving the [short-rate bond pricing equation](../../../../../short-rate-bond-pricing-equation.md)

$$
P_t+\mu_QP_r+\frac12\eta^2P_{rr}-rP=0,\qquad P(T,r;T)=1.
$$

Conversely, under the appropriate boundary and integrability conditions the [Feynman-Kac formula](../../../../../feynman-kac-formula.md) identifies its solution with the displayed discounted [expectation](../../../../../expected-value.md). For a terminal rate-dependent payoff $H(r_T)$, the same equation has terminal condition $H$ instead of one. A coupon bond is a sum of such unit-bond prices weighted by the coupon payments.

The common [market price of risk](../../../../../market-price-of-risk.md) can also be derived from trading, instead of being introduced arbitrarily for each maturity. Under the physical measure a bond's diffusion exposure is $\eta P_r$ and its excess drift above bank financing is $P_t+\mu P_r+\eta^2P_{rr}/2-rP$. For two nondegenerate traded bonds, combine their holdings to cancel their Brownian exposure. Absence of [arbitrage](../../../../../arbitrage.md) requires that combination to earn the bank rate; hence their excess-drift-to-exposure ratios must coincide. Calling that common ratio $\lambda$ yields the pricing equation with $\mu_Q=\mu-\eta\lambda$ for every maturity. A derivative $V(t,r)$ is then hedged locally by holding $V_r/P_r$ units of a nondegenerate bond and financing the remaining value through the [bank account](../../../../../bank-account.md). Their Brownian exposures agree, and substituting both pricing equations proves the drift gain identity. This is [short-rate diffusion hedging](../../../../../short-rate-diffusion-hedging.md); it requires $\eta P_r\ne0$, rather than a bare assertion that one factor automatically gives completeness everywhere.

The entire [yield curve](../../../../../yield-curve.md) is generated consistently from these bond prices. The continuously compounded yield and the [instantaneous forward rate](../../../../../instantaneous-forward-rate.md) are

$$
y(t,T)=-\frac{\log P(t,r_t;T)}{T-t},\qquad f(t,T)=-\partial_T\log P(t,r_t;T),\qquad f(t,t)=r_t.
$$

These encode different summaries: the yield averages the forward rate over the remaining lifetime. Bond prices must satisfy $P(t,t)=1$ and be positive; they need not be below one in models permitting negative rates.

The [Vasicek model](../../../../../vasicek-model.md) has constant pricing dynamics

$$
dr_t=a(b-r_t)dt+\eta\,dW_t^Q,\qquad a,\eta>0.
$$

Solving the linear equation gives $r_{t+u}=b+(r_t-b)e^{-au}+\eta\int_t^{t+u}e^{-a(t+u-v)}dW_v^Q$. Consequently, with $\tau=T-t$ and $B(\tau)=(1-e^{-a\tau})/a$,

$$
\int_t^T r_sds=b\tau+(r_t-b)B(\tau)+\eta\int_t^T B(T-v)dW_v^Q.
$$

This conditional normal random variable has [variance](../../../../../variance-split.md) $\eta^2\int_0^\tau B(u)^2du$. Its normal exponential moment yields

$$
P(t,T)=A(\tau)e^{-B(\tau)r_t},\qquad\log A=-b(\tau-B)+\frac{\eta^2}{2}\int_0^\tau B(u)^2du.
$$

Evaluating the elementary integral gives

$$
\boxed{B=\frac{1-e^{-a\tau}}a,\qquad\log A=\left(b-\frac{\eta^2}{2a^2}\right)(B-\tau)-\frac{\eta^2}{4a}B^2.}
$$

This explicit form makes estimation and valuation convenient. The rate is [Gaussian](../../../../../normal-distribution.md), its conditional mean reverts to $b$, and its long-run [variance](../../../../../variance-split.md) is $\eta^2/(2a)$. Its disadvantage, when nonnegative rates are desired, is a positive probability of negative rates.

The [CIR model](../../../../../cox-ingersoll-ross-model.md) replaces constant volatility by square-root volatility:

$$
dr_t=a(b-r_t)dt+\eta\sqrt{r_t}\,dW_t^Q,\qquad a,b,\eta>0.
$$

The standard solution stays nonnegative. The [Feller positivity condition for the CIR model](../../../../../feller-positivity-condition-for-the-cir-model.md) is $2ab\ge\eta^2$ in this parameterization; with a positive initial rate it makes zero inaccessible. Below this threshold zero can be reached, although the process does not cross into negative rates. For an [affine diffusion bond pricing](../../../../../affine-diffusion-bond-pricing.md) ansatz $P=A(\tau)e^{-B(\tau)r}$, substitution into the bond equation and matching its constant and rate coefficients gives

$$
B'=1-aB-\frac12\eta^2B^2,\qquad(\log A)'=-abB,\qquad B(0)=0,\ A(0)=1.
$$

Writing $d=\sqrt{a^2+2\eta^2}$, factor the quadratic in the first equation and integrate from $B=0$; integrating the second equation then gives the [CIR bond pricing](../../../../../cir-bond-pricing.md) formulas

$$
\boxed{B(\tau)=\frac{2(e^{d\tau}-1)}{(d+a)(e^{d\tau}-1)+2d},\qquad A(\tau)=\left[\frac{2d\,e^{(a+d)\tau/2}}{(d+a)(e^{d\tau}-1)+2d}\right]^{2ab/\eta^2}.}
$$

The square-root form produces an affine term structure while respecting nonnegative rates. These parameters are pricing-measure parameters; historical mean-reversion estimates alone do not determine them without a risk-premium specification.

Both preceding constant-parameter models constrain the family of initial curves. The [Hull-White model](../../../../../hull-white-model.md) allows a deterministic time-dependent drift:

$$
dr_t=(\beta(t)-ar_t)dt+\eta\,dW_t^Q.
$$

For a smooth desired initial forward curve $f_0(t)$, its [exact forward-curve fit in the Hull-White model](../../../../../exact-forward-curve-fit-in-the-hull-white-model.md) is obtained by taking

$$
\boxed{r_0=f_0(0),\qquad\beta(t)=f_0'(t)+af_0(t)+\frac{\eta^2}{2a}(1-e^{-2at}).}
$$

To derive this rather than merely assert calibration, write $r_t=x_t+\phi(t)$, where $dx_t=-ax_tdt+\eta dW_t^Q$, $x_0=0$. The conditional Gaussian-integral calculation at time zero gives

$$
\log P(0,T)=-\int_0^T\phi(u)du+\frac{\eta^2}{2}\int_0^T B(u)^2du,
$$

so its forward curve is $\phi(T)-\eta^2B(T)^2/2$. Choose $\phi(T)=f_0(T)+\eta^2B(T)^2/2$. Differentiating this shift and adding $a\phi(t)$ gives exactly the displayed $\beta(t)$. Thus $P(0,T)=\exp(-\int_0^T f_0(u)du)$ for every maturity, while $a$ and $\eta$ govern the stochastic fluctuations. This [Gaussian](../../../../../normal-distribution.md) model still allows negative rates.

Finally, one-factor models are economical and often give explicit bond prices, but their single Brownian driver is restrictive. Bond diffusion exposures $v_i=\eta P_{i,r}$ give the instantaneous [covariance matrix](../../../../../covariance-matrix.md) $vv^T$, of rank at most one. Nondegenerate maturity changes are instantaneously perfectly correlated, with correlation $+1$ or $-1$, though their finite-horizon correlations need not equal one. A single factor therefore cannot independently describe level, slope and curvature shocks to the whole [yield curve](../../../../../yield-curve.md). Multiple factors or a full forward-rate model offer greater flexibility. **A valid one-factor model must specify the pricing drift, fit the initial curve to the required accuracy, and handle boundary and [martingale](../../../../../martingale-split.md) conditions; naming a rate diffusion alone is not a complete pricing model.**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
