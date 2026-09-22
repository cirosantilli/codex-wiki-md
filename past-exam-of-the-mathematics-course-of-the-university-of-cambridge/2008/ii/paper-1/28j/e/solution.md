<h1 id="28j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [Black-Scholes implied volatility](../../../../../../black-scholes-implied-volatility.md) of a traded call price $C$ is the volatility $\sigma$ which makes the [Black-Scholes formula](../../../../../../black-scholes-formula.md) equal to $C$. For

$$
(S_0-Ke^{-rT})^+<C<S_0,
$$

the price is a continuous strictly increasing function of $\sigma>0$, by its positive [vega](../../../../../../option-vega.md), with precisely these endpoint limits. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) and strict monotonicity therefore give a unique positive implied volatility. The lower endpoint corresponds to the limiting value $\sigma=0$; the upper endpoint is reached only as $\sigma\to\infty$. Prices outside the bounds admit the [arbitrages](../../../../../../arbitrage.md) above and have no implied volatility.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [28J](../../28j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
