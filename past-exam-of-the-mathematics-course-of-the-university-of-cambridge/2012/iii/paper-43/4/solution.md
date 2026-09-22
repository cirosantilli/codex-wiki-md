<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the [quadratic Ornstein-Uhlenbeck state-price density](../../../../../quadratic-ornstein-uhlenbeck-state-price-density.md), apply the [Itô's formula](../../../../../ito-s-lemma.md) under the reference probability measure. Since $f'(x)=x$ and $f''(x)=1$,

$$
d\zeta_t=e^{-\alpha t}\sigma X_t\,dB_t-e^{-\alpha t}\left[\alpha a-\tfrac12\sigma^2+(\lambda+\tfrac12\alpha)X_t^2\right]dt.
$$

The [stochastic integral](../../../../../stochastic-integral.md) is a true [martingale](../../../../../martingale-split.md) on finite horizons by the finite moments of the [Ornstein-Uhlenbeck process](../../../../../ornstein-uhlenbeck-process.md). **A uniform sufficient condition is $\boxed{\alpha\geq\sigma^2/(2a)}$**, making the finite-variation drift nonpositive. This is also the condition for nonpositive drift at every state.

Use the positive [state-price density](../../../../../state-price-density.md) $\zeta$ to price a terminal payoff $H$ by $\Pi_t(H)=\mathbb E[\zeta_TH\mid\mathcal F_t]/\zeta_t$. The riskless account must cancel the drift of $\zeta$, giving the [short rate](../../../../../short-rate.md)

$$
\boxed{r_t=\frac{\alpha a-\sigma^2/2+(\lambda+\alpha/2)X_t^2}{a+X_t^2/2}=\alpha+\frac{\lambda X_t^2-\sigma^2/2}{a+X_t^2/2}.}
$$

This pricing system is consistent with a money-market [risk-neutral measure](../../../../../risk-neutral-measure.md): with $M_t=e^{\int_0^tr_udu}$, the process $\zeta_tM_t/\zeta_0$ is a [stochastic exponential](../../../../../doleans-dade-exponential.md) whose diffusion coefficient $\sigma X_t/f(X_t)$ is bounded. The [Novikov condition](../../../../../novikov-s-condition.md) makes it a true density [martingale](../../../../../martingale-split.md). The original [Brownian motion](../../../../../brownian-motion-split.md) is for the reference measure, not automatically for this new pricing measure.

For $X_0=x_0$, the OU second moment is $\mathbb E X_T^2=x_0^2e^{-2\lambda T}+\sigma^2(1-e^{-2\lambda T})/(2\lambda)$. Thus **the [zero-coupon bond](../../../../../zero-coupon-bond.md) price is**

$$
\boxed{P(0,T)=e^{-\alpha T}\frac{a+\tfrac12x_0^2e^{-2\lambda T}+\frac{\sigma^2}{4\lambda}(1-e^{-2\lambda T})}{a+\tfrac12x_0^2}.}
$$

Conditionally at time $t$, replace $T$ by $T-t$ and $x_0$ by $X_t$.

The [short rate](../../../../../short-rate.md) is nonnegative under the condition above, increases with $X_t^2$, and lies between $\alpha-\sigma^2/(2a)$ and $\alpha+2\lambda$. The model is tractable but imposes fixed rate bounds, identical rates for opposite values of $X$, and a restricted one-factor term structure. Its long-maturity yield is $\alpha$. These structural restrictions, including exclusion of negative rates under the supermartingale condition, may be unsuitable for a general interest-rate fit.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
