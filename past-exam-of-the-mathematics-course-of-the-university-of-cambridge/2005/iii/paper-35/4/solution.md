<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [self-financing portfolio](../../../../../self-financing-portfolio.md) changes its holdings using only its existing wealth. If it holds $g_t$ shares and $h_t$ units of a traded bond or [bank account](../../../../../bank-account.md) $B_t$, its value $V_t=g_tS_t+h_tB_t$ obeys the gain identity

$$
dV_t=g_t\,dS_t+h_t\,dB_t.
$$

The changes in holdings do not add or withdraw capital. Set $T=t_0$, $B_t=e^{-\rho(T-t)}$, so $dB_t=\rho B_tdt$, and let $dS_t=\mu S_tdt+\sigma S_tdW_t$, with $\sigma>0$. Write $V_t=p(S_t,t)$ and suppress the arguments of the smooth holdings $g,h$.

Differentiate $p=xg+B_th$:

$$
p_x=g+xg_x+B_th_x,\qquad p_t=xg_t+B_th_t+\rho B_th.
$$

The [Itô formula](../../../../../ito-s-lemma.md) minus the proposed [portfolio](../../../../../investment-portfolio.md) gains gives

$$
dp-g\,dS-h\,dB=\sigma S_t(p_x-g)dW_t+\left[p_t+\mu S_t(p_x-g)+\frac12\sigma^2S_t^2p_{xx}-\rho B_th\right]dt.
$$

Uniqueness of the local-martingale and finite-variation decomposition shows that self-financing requires $p_x=g$. Since $S_t$ has full support on $(0,\infty)$ for each $t>0$, smoothness gives the corresponding functional identity for every positive $x$, and continuity extends it to the interval endpoints. Thus

$$
xg_x+B_th_x=0.
$$

Differentiating this identity once more in $x$ gives $g_x+xg_{xx}+B_th_{xx}=0$, so $p_{xx}=g_x$. Substitute both identities into the drift condition to obtain

$$
\boxed{xg_x+B_th_x=0,\qquad\frac12\sigma^2x^2g_x+xg_t+B_th_t=0.}
$$

Conversely these equations give $p_x=g$, $p_{xx}=g_x$ and zero drift and diffusion in the displayed gain difference. They therefore prove the claimed [self-financing conditions for smooth stock and bond holdings](../../../../../self-financing-conditions-for-smooth-stock-and-bond-holdings.md) in both directions.

Using $B_th=p-xg$ in the gain identity and setting $g=p_x$, self-financing implies

$$
\boxed{p_t+\frac12\sigma^2x^2p_{xx}+\rho xp_x-\rho p=0.}
$$

This is the [Black-Scholes equation](../../../../../black-scholes-equation.md), independent of the physical drift $\mu$. Conversely, if a smooth $p$ satisfies it, define its [delta hedge](../../../../../delta-hedge.md) by

$$
g=p_x,\qquad h=\frac{p-xp_x}{B_t}.
$$

The preceding [Itô formula](../../../../../ito-s-lemma.md) verifies that these holdings are self-financing.

**For prescribed arbitrary holdings, the value equation alone is insufficient.** The corrected equivalence is the [Black-Scholes value equation needs delta-compatible holdings](../../../../../black-scholes-value-equation-needs-delta-compatible-holdings.md): a specified [portfolio](../../../../../investment-portfolio.md) is self-financing if and only if its value solves the equation and $g=p_x$. Indeed $p=0$, $g=1$, $h=-x/B_t$ satisfies the value equation but its proposed gains are $dS_t-\rho S_tdt$, which have nonzero Brownian part while $dp=0$. Thus the printed final equivalence is valid as an existence assertion for the delta hedge, not for every decomposition of the same value. No change to the valid two holdings equations is needed.

With continuous underlying [stock](../../../../../stock.md) dividends, the [stock](../../../../../stock.md)'s gain is $dS_t+\theta S_tdt$, so self-financing becomes $dV_t=g_t(dS_t+\theta S_tdt)+h_tdB_t$. Under the [risk-neutral measure](../../../../../risk-neutral-measure.md) the ex-dividend [stock](../../../../../stock.md) drift is $(\rho-\theta)S_t$. Matching its diffusion still gives $g=p_x$, and matching its gain drift gives the [Black-Scholes equation with continuous stock dividends](../../../../../black-scholes-equation-with-continuous-stock-dividends.md)

$$
\boxed{p_t+\frac12\sigma^2x^2p_{xx}+(\rho-\theta)xp_x-\rho p=0.}
$$

Only the coefficient of $xp_x$ changes. The $-\rho p$ discount term remains, because the claim is financed at the bank rate; there is no separate source term for a dividend paid by the claim itself. The dividends here are paid by the underlying [stock](../../../../../stock.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
