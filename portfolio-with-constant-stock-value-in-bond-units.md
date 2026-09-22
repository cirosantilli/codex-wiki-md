# Portfolio with constant stock value in bond units

↑ **Parent:** [Self-financing portfolio](self-financing-portfolio.md)

In the [Black-Scholes model](black-scholes-model.md), take $B_t=e^{-\rho(T-t)}$ as a [zero-coupon bond](zero-coupon-bond.md) [numéraire](numeraire.md). Holding the fixed stock value $\theta B_t$ requires $g_t=\theta B_t/S_t$ shares. The [self-financing conditions for smooth stock and bond holdings](self-financing-conditions-for-smooth-stock-and-bond-holdings.md) give

$$
h_t=\frac{w_0}{B_0}-\theta+\theta\log(S_t/S_0)+\theta(\sigma^2/2-\rho)t
$$

units of the bond. Since $V_t=g_tS_t+h_tB_t$, this yields the displayed wealth. Under the [risk-neutral measure](risk-neutral-measure.md), $V_t/B_t=w_0/B_0+\theta\sigma W_t^Q$: the discounted gain is a constant multiple of [Brownian motion](brownian-motion-split.md).

## ↑ Ancestors (7)

1. [Self-financing portfolio](self-financing-portfolio.md)
2. [Arbitrage](arbitrage.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/4/solution.md)
