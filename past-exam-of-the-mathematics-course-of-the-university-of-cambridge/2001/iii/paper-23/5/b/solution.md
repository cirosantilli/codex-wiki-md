<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the specified [risk-neutral measure](../../../../../../risk-neutral-measure.md), the [Itô product rule](../../../../../../ito-product-rule.md) and $d(B_t^{-1})=-r_tB_t^{-1}dt$ give

$$
d(B_t^{-1}P(t,T))=B_t^{-1}P(t,T)\Sigma(t,T)dW_t.
$$

Thus discounted traded [zero-coupon bonds](../../../../../../zero-coupon-bond.md) have zero drift. Assume the usual integrability and admissibility conditions that make discounted replicating values true [martingales](../../../../../../martingale-split.md), not merely [local martingales](../../../../../../local-martingale.md). If $X$ is an attainable [financial payoff](../../../../../../contingent-claim-payoff.md) with $\mathbb E_Q|B_T^{-1}X|<\infty$, its [self-financing portfolio](../../../../../../self-financing-portfolio.md) value $V_t$ has terminal value $V_T=X$ and satisfies

$$
B_t^{-1}V_t=\mathbb E_Q[B_T^{-1}X\mid\mathcal F_t].
$$

Multiplying by $B_t$ yields

$$
\boxed{V_t=\mathbb E_Q\left[\exp\left(-\int_t^Tr_sds\right)X\mid\mathcal F_t\right].}
$$

This proves the requested conditional pricing formula. In a [Brownian filtration](../../../../../../brownian-filtration.md), the [Martingale representation theorem](../../../../../../martingale-representation-theorem.md) realizes the discounted conditional [expectation](../../../../../../expected-value.md) as a [stochastic integral](../../../../../../stochastic-integral.md). If an available bond has nonzero [Itô diffusion](../../../../../../ito-diffusion.md) exposure, its holdings can match that integral, with the remaining value in the [bank account](../../../../../../bank-account.md), giving replication under the usual square-integrability conditions.

These attainability or [market completeness](../../../../../../complete-market.md) hypotheses matter for a completely arbitrary [contingent claim](../../../../../../contingent-claim.md): existence of a [risk-neutral measure](../../../../../../risk-neutral-measure.md) alone need not imply a unique price for every unspanned [financial payoff](../../../../../../contingent-claim-payoff.md), and a zero-drift [local martingale](../../../../../../local-martingale.md) alone need not satisfy the displayed terminal [expectation](../../../../../../expected-value.md) identity. In the general path-dependent [Heath-Jarrow-Morton model](../../../../../../heath-jarrow-morton-model.md), write the value as $V_t$; notation $V(t,r_t)$ is justified only when the current [short rate](../../../../../../short-rate.md) is a sufficient state for the [financial payoff](../../../../../../contingent-claim-payoff.md) and dynamics.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
