# Option theta

↑ **Parent:** [Greeks (finance)](greeks-finance.md)

The derivative of an option's value with respect to calendar time at fixed current underlying price and other parameters. In the dividend-free [Black-Scholes model](black-scholes-model.md), the [Black-Scholes equation](black-scholes-equation.md) gives

$$
\Theta=\rho(V-xV_x)-\frac12\sigma^2x^2V_{xx}.
$$

The first term is the interest earned on the bond value of the [replicating portfolio](replicating-strategy.md), while the second uses [option gamma](option-gamma.md). A [convex](convex-function.md) payoff with a short bond position has $\Theta\leq0$ when $\rho\geq0$; a [concave](concave-function.md) payoff with a long bond position has $\Theta\geq0$. Negative [interest rates](interest-rate.md) need not obey these signs: the affine payoff $x-K$ has $\Theta=-\rho Ke^{-\rho(T-t)}$. For a fixed payoff function, remaining-maturity sensitivity is $-\Theta$.

## ↑ Ancestors (6)

1. [Greeks (finance)](greeks-finance.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/5/solution.md)
