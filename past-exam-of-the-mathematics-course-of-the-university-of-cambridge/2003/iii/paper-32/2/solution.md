<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Specify the trading conventions first. Let the [bank account](../../../../../bank-account.md) have value $R_r>0$, with $R_0=1$ and its next gross return known at time $r$. Write $B_r=1/R_r$ for the [discount factor](../../../../../discount-factor.md). Let $S_r$ be the ex-dividend asset-price vector, and $d_r$ the vector of cash dividends paid per unit at time $r$; set $d_r=0$ for non-dividend-paying assets. Under an [equivalent martingale measure](../../../../../risk-neutral-measure.md) $Q$, each discounted cumulative asset gain

$$
G_r=B_rS_r+\sum_{j=1}^rB_jd_j
$$

is a [martingale](../../../../../martingale-split.md). Equivalently, $\mathbb E_Q[B_{r+1}(S_{r+1}+d_{r+1})\mid\mathcal F_r]=B_rS_r$. This is the gain-process form of risk-neutral pricing, rather than a martingale assumption on raw ex-dividend prices.

Let $X_r$ be the $\mathcal F_r$-[measurable](../../../../../measurability.md) holdings after trading and distributions at time $r$. The previous holdings $X_{r-1}$ earn the next price change and dividends. Define the strategy's net cash payment and its residual [portfolio wealth](../../../../../portfolio-wealth.md) by

$$
D_r^X=X_{r-1}^\top(S_r+d_r)-X_r^\top S_r,\qquad V_r=X_r^\top S_r.
$$

A negative payment is an external infusion; a [self-financing portfolio](../../../../../self-financing-portfolio.md) with no consumption has $D_r^X=0$. The discounted budget equation is

$$
B_rV_r-B_{r-1}V_{r-1}+B_rD_r^X=X_{r-1}^\top(G_r-G_{r-1}).
$$

Assume these gains and payments are [integrable](../../../../../integrability.md) under $Q$, for example by bounded predictable holdings and integrable discounted asset gains. Then

$$
M_r=B_rV_r+\sum_{j=1}^rB_jD_j^X
$$

is a true [martingale](../../../../../martingale-split.md), by conditioning the displayed one-step gains. Merely assuming a local martingale without appropriate [integrability](../../../../../integrability.md) would not justify the conditional equality.

Conditioning $M_n$ on $\mathcal F_r$ proves the general [multi-period dividend pricing identity](../../../../../multi-period-dividend-pricing-identity.md)

$$
\boxed{B_rX_r^\top S_r=\mathbb E_Q\!\left[B_nV_n+\sum_{j=r+1}^nB_jD_j^X\,\middle|\,\mathcal F_r\right].}
$$

For a strategy liquidated at time $n$, $X_n=0$ and all liquidation proceeds are included in $D_n^X$. The terminal value disappears, giving exactly the requested dividend-only relation. That liquidation convention is necessary: holding one unit of the bank account with no payments would otherwise have a positive left side and zero right side.

An [attainable claim](../../../../../attainable-european-contingent-claim.md) $H$ paid at $n$ can be replicated by a strategy with no earlier payments and final liquidation payment $D_n^X=H$. Its time-$r$ value is therefore

$$
\boxed{V_r=\frac1{B_r}\mathbb E_Q[B_nH\mid\mathcal F_r].}
$$

Two admissible replicating strategies have the same value by this identity, and the value is the same under every [equivalent martingale measure](../../../../../risk-neutral-measure.md) for which the replication gains are true [martingales](../../../../../martingale-split.md). For unattainable claims this expectation is a possible model price, but the replication argument does not establish a unique price. With density process $Z_r=\mathbb E_P[dQ/dP\mid\mathcal F_r]$, the equivalent [state-price density](../../../../../state-price-density.md) form is $V_r=(B_rZ_r)^{-1}\mathbb E_P[B_nZ_nH\mid\mathcal F_r]$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
