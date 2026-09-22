<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For European options with the same strike and maturity, the terminal payoff identity is

$$
(S_T-X)^+-(X-S_T)^+=S_T-X.
$$

Thus long the call and short the put has the same terminal payoff as one [stock](../../../../../../stock.md) less $X$ units of the maturity-$T$ [zero-coupon bond](../../../../../../zero-coupon-bond.md). With no dividends, the [stock](../../../../../../stock.md) strategy has no intervening payments. The [law of one price](../../../../../../law-of-one-price.md) gives [put-call parity](../../../../../../put-call-parity.md):

$$
\boxed{C_E(t)-P_E(t)=S_t-XB(t,T).}
$$

Equivalently the two nonnegative terminal-payoff [portfolios](../../../../../../investment-portfolio.md), call plus strike bond and put plus [stock](../../../../../../stock.md), agree in every state. The parity proof does not require lognormal [stock](../../../../../../stock.md) prices or positive interest.

For [American options](../../../../../../american-option.md) the exercise times can differ, so equality of their maturity payoffs is not an identity between their full rights. Under the nonnegative-interest, non-dividend assumptions of part (a), $C_A=C_E$ while $P_A=P_E+\Pi_P$ with early-exercise premium $\Pi_P\ge0$. Hence

$$
C_A-P_A=S_t-XB(t,T)-\Pi_P,
$$

which generally differs from European parity. For a concrete limiting state, if the [stock](../../../../../../stock.md) is zero and remains zero and interest is positive, then $C_A=C_E=0$, $P_A=X$ and $P_E=XB(t,T)<X$. **European parity is not a general American-option equality.** It holds in a particular case only when the relevant early-exercise premiums cancel, or both vanish.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
