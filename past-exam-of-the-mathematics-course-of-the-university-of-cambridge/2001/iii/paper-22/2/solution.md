<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Fix a finite horizon $N$, a [filtration](../../../../../filtration-probability-theory.md) $(\mathcal F_n)$, a positive [bank account](../../../../../bank-account.md) $B_n$ with predictable one-step growth, ex-dividend risky prices $S_n$, and asset dividends $D_n$ paid at date $n$. Put $s_n=S_n/B_n$ and $d_n=D_n/B_n$. An [equivalent martingale measure](../../../../../risk-neutral-measure.md) $Q$ makes the discounted cum-dividend gains

$$
g_n=s_n+\sum_{j=1}^n d_j
$$

[martingales](../../../../../martingale-split.md); equivalently $\mathbb E_Q[s_n-s_{n-1}+d_n\mid\mathcal F_{n-1}]=0$. It is these gains, not necessarily the discounted ex-dividend prices alone, which enter the definition.

Let $\theta_n$ be risky holdings chosen at date $n-1$ and carried to date $n$. Let $C_n$ be the portfolio's net cash distribution to its owner at date $n$, and $V_n$ its remaining value after that distribution and rebalancing. A [self-financing portfolio](../../../../../self-financing-portfolio.md) with these distributions has the budget identity

$$
\frac{V_n}{B_n}-\frac{V_{n-1}}{B_{n-1}}
=\theta_n^T(s_n-s_{n-1}+d_n)-\frac{C_n}{B_n}.
$$

To see this, value the previous [stock](../../../../../stock.md) and bank holdings at the new prices, add the asset dividends, subtract the owner distribution, and observe that the discounted bank holding is unchanged. Rebalancing then alters holdings but not value. An asset dividend reinvested in the portfolio is already in the gain term; it is not also an owner distribution.

For a predictable strategy whose gains are integrable under $Q$ (bounded holdings in a finite-state market suffice), conditioning the gain increment gives zero. Therefore discounted remaining wealth plus cumulative discounted owner payments is a [martingale](../../../../../martingale-split.md). Conditioning its terminal value proves the [multi-period dividend pricing identity](../../../../../multi-period-dividend-pricing-identity.md)

$$
\boxed{V_n=B_n\mathbb E_Q\left[\frac{V_N}{B_N}+\sum_{j=n+1}^N\frac{C_j}{B_j}\,\middle|\,\mathcal F_n\right].}
$$

The relation holds under every [equivalent martingale measure](../../../../../risk-neutral-measure.md) for which these integrability conditions hold. Each payment is discounted from its own payment date, not from one common terminal date. The expression inside the [expectation](../../../../../expected-value.md) is in [bank account](../../../../../bank-account.md) units; multiplication by $B_n$ returns current currency units.

When the portfolio is liquidated and all its final value is paid out, $V_N=0$ after liquidation and that value is included in $C_N$. The displayed identity then involves only future discounted distributions. Without liquidation, the terminal value must remain. A [bank account](../../../../../bank-account.md) holding with no coupons before redemption has positive value despite having no intervening dividends; omitting its redemption or terminal holding value would plainly give the wrong result. In an infinite horizon, deleting the terminal term instead requires a [dividend-price transversality condition](../../../../../dividend-price-transversality-condition.md), namely convergence of its conditional discounted [expectation](../../../../../expected-value.md) to zero.

For a traded asset the same proof gives its discounted expected dividends plus terminal sale value. For a replicated claim paid only at $N$, it gives $V_n=B_n\mathbb E_Q[H/B_N\mid\mathcal F_n]$. In a [complete market](../../../../../complete-market.md) this prices every admissible claim uniquely. In an [incomplete market](../../../../../incomplete-market.md) only the portfolio's attainable payout stream has this common value under all measures; an arbitrary unattainable payoff can have different [expectations](../../../../../expected-value.md) under different measures. For a merely dominated measure the conditional identity holds $Q$-almost surely; it makes no assertion on physical states assigned zero mass by $Q$. External capital injections must also be counted, as negative owner distributions. Thus the valuation principle follows from the gain [martingale](../../../../../martingale-split.md) and the trading budget, together with the terminal convention and integrability, rather than from unconditional averaging of arbitrary future cash flows.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
