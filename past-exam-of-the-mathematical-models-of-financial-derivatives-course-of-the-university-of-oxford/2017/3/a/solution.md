<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [European call option](../../../../european-call-option.md) has nonnegative [financial payoff](../../../../contingent-claim-payoff.md), so its price is nonnegative under [no-arbitrage](../../../../no-arbitrage.md). A second [arbitrage](../../../../arbitrage.md) comparison buys one call and a [zero-coupon bond](../../../../zero-coupon-bond.md) paying $K$, and shorts one share. Its terminal value is $(S_T-K)^++K-S_T=(K-S_T)^+\geq0$, so its initial cost cannot be negative. Consequently

$$
\boxed{C_t^e\geq\max(S_t-Ke^{-r(T-t)},0).}
$$

The holder of an [American call option](../../../../american-call-option.md) can choose to wait until expiry, so $C_t^a\geq C_t^e$. Since $r>0$ and $t<T$, an in-the-money call has $C_t^a\geq S_t-Ke^{-r(T-t)}>S_t-K$: immediate exercise sacrifices value. An out-of-the-money exercise pays zero and cannot improve the holder's position. This proves [no early exercise of a call without dividends](../../../../no-early-exercise-of-a-call-without-dividends.md): waiting is always at least as good, and is strictly better for positive immediate exercise payoff. In a degenerate market with zero continuation value an out-of-the-money holder can be indifferent; the [Black-Scholes model](../../../../black-scholes-model.md) with positive volatility gives strictly positive continuation value before expiry.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
