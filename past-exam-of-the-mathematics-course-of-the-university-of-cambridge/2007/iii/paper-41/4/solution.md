<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $T=t_0$ and $B_t=e^{-\rho(T-t)}$ for the risk-free asset paying one at $T$. Under the physical measure, $dS_t=\mu S_t\,dt+\sigma S_t\,dW_t$, with $\sigma>0$, while $dB_t=\rho B_t\,dt$. A [self-financing portfolio](../../../../../self-financing-portfolio.md) with predictable [stock](../../../../../stock.md) and bond holdings $g_t,h_t$ has value $V_t=g_tS_t+h_tB_t$ and gains

$$
dV_t=g_t\,dS_t+h_t\,dB_t.
$$

Rebalancing therefore adds no outside money and withdraws none. This gains equation, rather than merely the value decomposition, defines [self-financing](../../../../../self-financing-portfolio.md).

Let $p(x,t)=xg(x,t)+B_th(x,t)$. The [Itô formula](../../../../../ito-s-lemma.md) gives

$$
dp(S_t,t)=\left(p_t+\mu S_t p_x+\frac12\sigma^2S_t^2p_{xx}\right)dt+\sigma S_t p_x\,dW_t.
$$

The prescribed [portfolio](../../../../../investment-portfolio.md) gains instead have diffusion coefficient $\sigma S_tg$ and drift $\mu S_tg+\rho B_th$. Equality of diffusion coefficients requires $p_x=g$, equivalently

$$
\boxed{xg_x+B_th_x=0.}
$$

Under this condition, $p_{xx}=g_x$. Equality of drifts is then $p_t+\frac12\sigma^2x^2g_x=\rho B_th$. Since $p_t=xg_t+B_th_t+\rho B_th$, this becomes

$$
\boxed{\frac12\sigma^2x^2g_x+xg_t+B_th_t=0.}
$$

These conditions are also sufficient by the same [Itô formula](../../../../../ito-s-lemma.md). Necessity initially holds along the [stock](../../../../../stock.md) process. Its positive transition density on $(0,\infty)$ for every positive time, together with continuity of the coefficient functions, extends the identities to all $x>0$ and then to the time endpoints by continuity.

For a [self-financing portfolio](../../../../../self-financing-portfolio.md), substitute $g=p_x$ and $B_th=p-xp_x$ into the drift identity to obtain the [Black-Scholes equation](../../../../../black-scholes-equation.md)

$$
\boxed{p_t+\frac12\sigma^2x^2p_{xx}+\rho xp_x-\rho p=0.}
$$

Conversely, a smooth solution of this equation gives a [self-financing portfolio](../../../../../self-financing-portfolio.md) by choosing the [delta hedge](../../../../../delta-hedge.md)

$$
\boxed{g=p_x,\qquad h=\frac{p-xp_x}{B_t}.}
$$

Its value is $p$, and both coefficient identities follow directly.

The printed deduction needs this holdings qualification: the [Black-Scholes value equation needs delta-compatible holdings](../../../../../black-scholes-value-equation-needs-delta-compatible-holdings.md). A value function alone cannot make an arbitrary prescribed decomposition self-financing. As a counterexample, take $p=0$, $g=1$, $h=-x/B_t$. The value function solves the [Black-Scholes equation](../../../../../black-scholes-equation.md), but this zero-value [portfolio](../../../../../investment-portfolio.md) has gains $dS_t-\rho S_t\,dt$, which contain the nonzero term $\sigma S_t\,dW_t$. Thus for the originally specified $g,h$, the exact equivalence is the pricing equation together with $g=p_x$, not the pricing equation alone.

For a claim paying the holder at rate $k(S_t)$, let $p$ denote its remaining, ex-dividend value. A replicating [portfolio](../../../../../investment-portfolio.md) pays out $k(S_t)dt$, so its net wealth equation is $dp=g\,dS+h\,dB-k(S_t)dt$. The [delta hedge](../../../../../delta-hedge.md) is still $g=p_x$, but the [Black-Scholes equation](../../../../../black-scholes-equation.md) becomes

$$
\boxed{p_t+\frac12\sigma^2x^2p_{xx}+\rho xp_x-\rho p+k(x)=0.}
$$

If there is a terminal payoff $f$, set $p(x,T)=f(x)$; with no terminal payment set it to zero. The corresponding [risk-neutral valuation](../../../../../risk-neutral-pricing.md) is

$$
p(x,t)=\mathbb E_Q\left[e^{-\rho(T-t)}f(S_T)+\int_t^T e^{-\rho(u-t)}k(S_u)\,du\ \middle|\ S_t=x\right].
$$

Each intervening payment is discounted from its own payment time.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
