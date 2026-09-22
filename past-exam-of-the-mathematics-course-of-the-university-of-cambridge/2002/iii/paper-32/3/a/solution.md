<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual frictionless option model with nonnegative deterministic [interest rates](../../../../../../interest-rate.md) and no [stock](../../../../../../stock.md) dividends. Let $B(t,T)\le1$ be the price of a unit [zero-coupon bond](../../../../../../zero-coupon-bond.md), $C_E$ the European call price, and $C_A$ the American call price. A call payoff dominates $S_T-X$, so no-arbitrage pricing gives $C_E\ge S_t-XB(t,T)$, and $C_A\ge C_E$. If $S_t>X$, then

$$
C_A\ge C_E\ge S_t-XB(t,T)\ge S_t-X.
$$

The last term is the immediate exercise payoff. Waiting retains downside optionality and defers payment of the strike. For positive interest and $X>0$ the inequality is strict while exercise has positive payoff. If $S_t\le X$, exercising for a zero payoff provides no advantage over keeping the right. Thus **early exercise of a non-dividend-paying call is never strictly beneficial** under these assumptions, and $C_A=C_E$. For completeness, discounted European call value is a true [martingale](../../../../../../martingale-split.md) in the standard pricing model. For any exercise [stopping time](../../../../../../stopping-time.md) $\tau\le T$, its pointwise dominance of immediate payoff gives $\mathbb E_Q[B(t,\tau)(S_\tau-X)^+\mid\mathcal F_t]\le\mathbb E_Q[B(t,\tau)C_E(\tau)\mid\mathcal F_t]=C_E(t)$. Taking the [supremum](../../../../../../supremum.md) over exercise rules proves $C_A\le C_E$, and waiting to maturity gives the reverse inequality. This proves [no early exercise of a call without dividends](../../../../../../no-early-exercise-of-a-call-without-dividends.md).

The contrast for a put is the interest earned on a strike received sooner. The European put has payoff at most $X$, so $P_E\le XB(t,T)$. When interest is positive and $S_t<X(1-B(t,T))$, immediate exercise gives $X-S_t>XB(t,T)\ge P_E$. Hence committing never to exercise before maturity is worse than an available early-exercise strategy in such a deep-in-the-money state. This does not say that every put should be exercised early, only that a general prohibition is not rational.

The interest-rate hypothesis is essential to the printed claim. If $r<0$ and the [stock](../../../../../../stock.md) is deterministic, $S_u=S_te^{r(u-t)}$ with no dividends, choose spot sufficiently large that it stays in the money through $T$. The European call price is $S_t-Xe^{-r(T-t)}<S_t-X$, so immediate exercise is better. At zero interest, early exercise can be indifferent in degenerate cases; it is the usual positive-interest setting that makes the non-exercise comparison strict.

## ↑ Ancestors (11)

1. [A](../a.md)
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
