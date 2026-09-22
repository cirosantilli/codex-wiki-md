<h1 id="27i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Under the given [risk-neutral measure](../../../../../../risk-neutral-measure.md), the option price is $V(t,S)=e^{-r(T-t)}\mathbb E[\phi(S_T)\mid S_t=S]$. Thus $e^{-rt}V(t,S_t)$ is a [martingale](../../../../../../martingale-split.md). This valuation also follows from [delta hedging](../../../../../../delta-hedge.md): cancel the Brownian exposure with $V_S$ units of stock, after which absence of arbitrage makes the locally riskless remainder earn $r$.

Set $f(t,b)=e^{-rt}V(t,S_0e^{\sigma b+(r-\sigma^2/2)t})$. The stated Brownian martingale identity and the chain rule give

$$
f_t+\tfrac12f_{bb}=e^{-rt}\left(V_t+\tfrac12\sigma^2S^2V_{SS}+rSV_S-rV\right).
$$

The drift vanishes because discounted option value is a [martingale](../../../../../../martingale-split.md). Consequently the [Black-Scholes equation](../../../../../../black-scholes-equation.md) is

$$
\boxed{V_t+\tfrac12\sigma^2S^2V_{SS}+rSV_S-rV=0,\qquad V(T,S)=\phi(S).}
$$

For bounded measurable payoffs, the conditional-expectation solution is smooth for $t<T$; terminal values are interpreted in the usual limiting sense at continuity points, or in the bounded measurable pricing sense.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27I](../../27i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
