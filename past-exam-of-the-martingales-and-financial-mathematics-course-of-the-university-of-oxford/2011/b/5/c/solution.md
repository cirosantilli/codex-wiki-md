<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For this stock-dependent payoff, replace the stock drift by $r$ under a [risk-neutral measure](../../../../../risk-neutral-measure.md). Conditional lognormal moments then give, with $\tau=T-t$,

$$
\boxed{V_t=e^{-r\tau}\mathbb E^Q[S_T^3\mid\mathcal F_t]
=S_t^3e^{(2r+3\sigma^2)\tau}.}
$$

This is the [Power payoff in the Black-Scholes model](../../../../../power-payoff-in-the-black-scholes-model.md). The [delta hedge](../../../../../delta-hedge.md) is $\Delta_t=\partial V/\partial S=3V_t/S_t$ shares, so the stock holding is worth $3V_t$. The rest is a bank position worth $-2V_t$, or $-2V_t/B_t$ units of the bank asset. This gives a [replicating portfolio](../../../../../replicating-strategy.md); its self-financing identity follows from Itô's formula and the Black-Scholes pricing equation, and its terminal value is $S_T^3$.

The full two-Brownian filtration contains an additional orthogonal noise direction, but this particular payoff is replicated using the traded stock and bank asset, so that extra noise does not affect its price.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
