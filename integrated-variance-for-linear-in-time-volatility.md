# Integrated variance for linear-in-time volatility

↑ **Parent:** [Black-Scholes model](black-scholes-model.md)

Deterministic time-varying [volatility](financial-volatility.md) enters the European [Black-Scholes formula](black-scholes-formula.md) through its integrated square, not its arithmetic mean. For $\sigma(t)=\alpha(1+t)$ over one year, the arithmetic mean is $3\alpha/2$ but its square is only $9\alpha^2/4$, strictly below the actual integrated [variance](variance-split.md) by $\alpha^2/12$ when $\alpha\neq0$. Positive [option vega](option-vega.md) therefore makes the arithmetic-mean-volatility call price too small. If the deterministic [volatility](financial-volatility.md) path is known exactly in the complete frictionless model, the pricing difference can be locked in by buying the cheaper claim and selling its correctly computed [replicating strategy](replicating-strategy.md).

## ↑ Ancestors (6)

1. [Black-Scholes model](black-scholes-model.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
