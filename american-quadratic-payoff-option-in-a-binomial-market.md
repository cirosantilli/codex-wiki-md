# American quadratic-payoff option in a binomial market

↑ **Parent:** [American option](american-option.md)

In a [discrete-time binomial market](discrete-time-binomial-market.md) with $B_t=(1+r)^t$ and one-step [stock](stock.md) factors $1\pm\varepsilon$, use the [risk-neutral probability](risk-neutral-probability.md) $p=(1+r/\varepsilon)/2$, where $0\le r<\varepsilon<1$. For the exercise payoff $S_t^2$, the discounted one-step reward multiplier has mean

$$
\lambda=\frac{1+2r+\varepsilon^2}{1+r}>1.
$$

The [Snell envelope of a multiplicative process](snell-envelope-of-a-multiplicative-process.md) gives the value $V_t=S_t^2\lambda^{T-t}$. Continuation strictly exceeds exercise before maturity, so the optimal exercise time is $T$. The [replicating portfolio in a binomial market](replicating-portfolio-in-a-binomial-market.md) holds $2S_t\lambda^{T-t-1}$ shares on the next step, found by subtracting the two next-state values and dividing by the stock-price difference. At time zero the price is $S_0^2\lambda^T$.

## ↑ Ancestors (6)

1. [American option](american-option.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
