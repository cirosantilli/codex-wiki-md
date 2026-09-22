<h1 id="28j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

As $\sigma\downarrow0$, the [Black-Scholes formula](../../../../../../black-scholes-formula.md) tends to $\boxed{(S_0-Ke^{-rT})^+}$. This also follows by discounting the deterministic zero-volatility payoff; at equality $S_0=Ke^{-rT}$ the limiting value is zero.

If $S_0>Ke^{-rT}$ and a call trades at $C<S_0-Ke^{-rT}$, buy a call, short one share, and buy a bond paying $K$ at maturity. Invest the positive initial surplus $S_0-Ke^{-rT}-C$. At maturity the call, share and bond together pay $(S_T-K)^+-S_T+K=(K-S_T)^+\geq0$, in addition to the strictly positive invested surplus. If the lower bound is zero, violating it means $C<0$: buy the call and invest the cash received, obtaining a nonnegative option payoff and a strictly positive bank payoff. Both strategies are [arbitrages](../../../../../../arbitrage.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
