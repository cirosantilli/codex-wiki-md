<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use a [risk-neutral measure](../../../../../risk-neutral-measure.md) $Q$, and let $P_{s,t}$ be the price at time $s$ of a [zero-coupon bond](../../../../../zero-coupon-bond.md) paying one at its maturity $t$. The information available at $s$ is the [filtration](../../../../../filtration-probability-theory.md) $\mathcal F_s$. For positive differentiable bond prices, the [instantaneous forward rate](../../../../../instantaneous-forward-rate.md) is

$$
f(s,t)=-\partial_t\log P_{s,t},\qquad P_{s,t}=\exp\left(-\int_s^t f(s,u)\,du\right),
$$

with $P_{t,t}=1$. The [short rate](../../../../../short-rate.md) is $R_s=f(s,s)$. The [continuous-time bank account](../../../../../continuous-time-bank-account.md) $B_s=\exp(\int_0^sR_u\,du)$ is the discounting [numéraire](../../../../../numeraire.md).

If $P_{s,t}/B_s$ is a true [martingale](../../../../../martingale-split.md) for each fixed maturity, then its terminal value is $B_t^{-1}$ and

$$
\frac{P_{s,t}}{B_s}=\mathbb E_Q[B_t^{-1}\mid\mathcal F_s].
$$

Multiplication by the $\mathcal F_s$-measurable $B_s$ gives

$$
\boxed{P_{s,t}=\mathbb E_Q\left[e^{-\int_s^tR_u\,du}\mid\mathcal F_s\right].}
$$

Conversely this conditional-expectation formula makes the discounted bond a [martingale](../../../../../martingale-split.md) by the [tower property of conditional expectation](../../../../../law-of-total-expectation.md). The equivalence uses integrability and true [martingales](../../../../../martingale-split.md), rather than merely local [martingales](../../../../../martingale-split.md).

Forward-rate modelling specifies the stochastic evolution of $f(s,t)$ as $s$ varies at fixed maturity. For example, with one Brownian driver, write $df(s,t)=\alpha(s,t)ds+\beta(s,t)dW_s^Q$. Differentiation of the integral representation and [Itô formula](../../../../../ito-s-lemma.md) give the bond's relative volatility $-\int_s^t\beta(s,u)du$ and drift $R_s-\int_s^t\alpha(s,u)du+\frac12(\int_s^t\beta(s,u)du)^2$. The discounted-bond condition therefore imposes

$$
\int_s^t\alpha(s,u)du=\frac12\left(\int_s^t\beta(s,u)du\right)^2,
$$

or, after differentiation in maturity, $\alpha(s,t)=\beta(s,t)\int_s^t\beta(s,u)du$. This illustrates how the no-arbitrage condition constrains forward-rate drift.

For the [Gaussian short-rate model with constant coefficients](../../../../../gaussian-short-rate-model-with-constant-coefficients.md), let $dR_s=\theta ds+\sigma dW_s^Q$ and fix $\Delta=t-s$. Future Brownian increments are independent of $\mathcal F_s$, giving

$$
\int_s^tR_u\,du=\Delta R_s+\frac\theta2\Delta^2+\sigma\int_s^t(t-v)\,dW_v^Q.
$$

The last stochastic integral is Gaussian with mean zero and variance $\Delta^3/3$, by the [Itô isometry](../../../../../ito-isometry.md). Its [Gaussian moment-generating function](../../../../../moment-generating-function-of-a-normal-distribution.md) therefore gives

$$
\boxed{P_{s,t}=\exp\left[-\Delta R_s-\frac\theta2\Delta^2+\frac{\sigma^2}{6}\Delta^3\right],\quad b_{s,t}=\Delta,\quad a_{s,t}=-\frac\theta2\Delta^2+\frac{\sigma^2}{6}\Delta^3.}
$$

When $\sigma\neq0$ and the initial rate is deterministic, the Brownian and short-rate filtrations coincide because $W_s^Q=(R_s-R_0-\theta s)/\sigma$. If $\sigma=0$, the same bond formula holds deterministically, while the asserted filtration equivalence is unnecessary.

For a deterministic drift function $\theta_v$, the same calculation gives

$$
P_{s,t}=\exp\left[-(t-s)R_s-\int_s^t(t-v)\theta_v\,dv+\frac{\sigma^2}{6}(t-s)^3\right].
$$

Let the observed initial curve be $P^{\rm obs}_{0,t}>0$, normalized by $P^{\rm obs}_{0,0}=1$, and define $f_0(t)=-\frac d{dt}\log P^{\rm obs}_{0,t}$. For a differentiable initial forward curve choose

$$
\boxed{R_0=f_0(0),\qquad\theta_t=f_0'(t)+\sigma^2t.}
$$

Indeed the model's initial forward rate is $R_0+\int_0^t\theta_vdv-\sigma^2t^2/2=f_0(t)$, so integrating it gives exactly the observed bond curve. This is [forward-curve calibration of a shifted Brownian short rate](../../../../../forward-curve-calibration-of-a-shifted-brownian-short-rate.md), with $R_t=f_0(t)+\sigma^2t^2/2+\sigma W_t^Q$. Every finite collection of positive bond quotes can first be fitted by a smooth positive curve; an arbitrary entire curve requires the stated smoothness or an appropriate weaker integral interpretation. The freedom is in the deterministic drift, and the initial short rate must match the initial forward rate.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
