<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The boundedness of $a'$ makes $a$ globally Lipschitz, so the [stock](../../../../../stock.md) [stochastic differential equation](../../../../../stochastic-differential-equation.md) has a nonexplosive strong solution. Since $a$ is bounded, $S_t-S_0=\int_0^ta(S_u)dW_u$ is a square-integrable [martingale](../../../../../martingale-split.md) on every finite horizon. Apply [Itô formula](../../../../../ito-s-lemma.md) to the option price:

$$
dV(t,S_t)=\left(V_t+\frac12a(S_t)^2V_{SS}\right)dt+a(S_t)V_S(t,S_t)dW_t
=V_S(t,S_t)dS_t.
$$

Thus both the [stock](../../../../../stock.md) and the option are [local martingales](../../../../../local-martingale.md) under the original probability measure, while cash is constant. The relevant no-arbitrage theorem is the sufficient direction of the [fundamental theorem of asset pricing](../../../../../fundamental-theorem-of-asset-pricing.md): a common equivalent measure under which all numéraire-denominated traded prices are [local martingales](../../../../../local-martingale.md) excludes [arbitrage](../../../../../arbitrage.md) by [admissible trading strategies](../../../../../admissible-trading-strategy.md). In this case the original measure itself is an [equivalent local martingale measure](../../../../../equivalent-local-martingale-measure.md). Hence **the augmented market has no admissible [arbitrage](../../../../../arbitrage.md)**. The nonnegative option-value assumption also makes the replicating wealth below admissible.

Set

$$
\boxed{U(t,S)=V_S(t,S),\qquad\pi_t=U(t,S_t).}
$$

Differentiating the pricing equation in the stock-price variable gives

$$
U_t+a(S)a'(S)U_S+\frac12a(S)^2U_{SS}=0.
$$

The limiting terminal derivative is $\mathbf1_{\{S>K\}}$ away from the strike. Its value at the strike may be assigned as the stated $\mathbf1_{\{S\ge K\}}$: the smooth positive diffusion coefficient gives a continuous terminal distribution, so that point has probability zero. This is the [call delta equation for a driftless local volatility diffusion](../../../../../call-delta-equation-for-a-driftless-local-volatility-diffusion.md).

Hold $\pi_t$ shares and $\eta_t=V(t,S_t)-\pi_tS_t$ units of cash. The [portfolio](../../../../../investment-portfolio.md) value is $V(t,S_t)$, and the preceding Itô calculation gives $dV=\pi_t dS_t+\eta_t dB_t$, with $dB_t=0$. It is therefore a [self-financing portfolio](../../../../../self-financing-portfolio.md), with initial wealth $V(0,S_0)$ and terminal wealth $(S_T-K)^+$. This proves **replication by the stated [delta hedge](../../../../../delta-hedge.md)**.

A further application of [Itô formula](../../../../../ito-s-lemma.md), now to $U$, yields

$$
d\pi_t=-a(S_t)a'(S_t)U_S(t,S_t)dt+a(S_t)U_S(t,S_t)dW_t.
$$

The density process is the strictly positive [stochastic exponential](../../../../../doleans-dade-exponential.md)

$$
Z_t=\exp\left(\int_0^ta'(S_u)dW_u-\frac12\int_0^ta'(S_u)^2du\right).
$$

Its integrand is bounded, so the [Novikov condition](../../../../../novikov-s-condition.md) proves that it is a true [martingale](../../../../../martingale-split.md). The product formula for $M=Z\pi$ gives

$$
\begin{aligned}
dM_t&=Z_td\pi_t+\pi_tdZ_t+d[Z,\pi]_t,\\
d[Z,\pi]_t&=Z_ta'(S_t)a(S_t)U_S(t,S_t)dt.
\end{aligned}
$$

The drift in $Z\,d\pi$ cancels this [quadratic covariation](../../../../../quadratic-covariation.md) term, leaving

$$
\boxed{dM_t=Z_t\bigl(a(S_t)U_S(t,S_t)+a'(S_t)U(t,S_t)\bigr)dW_t.}
$$

Thus $M$ is a [local martingale](../../../../../local-martingale.md); the expression also identifies its [stochastic integral](../../../../../stochastic-integral.md) integrand explicitly.

Under the stated assumption that $M$ is a true [martingale](../../../../../martingale-split.md) on $[0,T]$, its terminal value gives

$$
Z_t\pi_t=\mathbb E[Z_T\mathbf1_{\{S_T\ge K\}}\mid\mathcal F_t].
$$

Since $0\le Z_T\mathbf1_{\{S_T\ge K\}}\le Z_T$ and $\mathbb E[Z_T\mid\mathcal F_t]=Z_t>0$, division gives

$$
\boxed{0\le\pi_t\le1\quad\text{a.s.}}
$$

This is the [derivative-weighted call delta martingale](../../../../../derivative-weighted-call-delta-martingale.md) argument. It uses true martingality through maturity, not just local martingality before the terminal date.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
