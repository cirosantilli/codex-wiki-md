# Pricing equation for a local volatility model

↑ **Parent:** [Local volatility model](local-volatility-model.md)

For a [local volatility model](local-volatility-model.md) $dS_t=S_t(rdt+\sigma(S_t)dW_t^Q)$ with [bank account](bank-account.md) $B_t=B_0e^{rt}$, a nonnegative classical solution $V$ of

$$
V_t+rSV_S+\tfrac12\sigma(S)^2S^2V_{SS}=rV,\qquad V(T,S)=g(S),
$$

defines a possible price of a [European contingent claim](european-contingent-claim.md). Indeed, [Itô formula](ito-s-lemma.md) gives $d(V(t,S_t)/B_t)=B_t^{-1}\sigma(S_t)S_tV_S(t,S_t)dW_t^Q$, a [local martingale](local-martingale.md). Thus the same [equivalent local martingale measure](equivalent-local-martingale-measure.md) works for the market augmented by this price. For an [admissible trading strategy](admissible-trading-strategy.md) whose discounted wealth is bounded below, the discounted gains are a [local martingale](local-martingale.md) bounded below, hence a [supermartingale](supermartingale.md) by localization and the [Fatou lemma](fatou-s-lemma.md). A zero-cost terminal gain that is nonnegative and strictly positive with positive probability would then contradict the [supermartingale](supermartingale.md) expectation inequality. This proves the absence of [arbitrage](arbitrage.md) for such strategies. If $V$ is bounded on the finite time interval, its discounted value is a bounded [martingale](martingale-split.md) and consequently $V(t,S_t)=B_t\mathbb E_Q[g(S_T)/B_T\mid\mathcal F_t]$. Nonnegativity alone guarantees the [local martingale](local-martingale.md) calculation, not this latter equality for every possible solution.

**Table of contents**

- [Explicit log-price scheme for local-volatility pricing](explicit-log-price-scheme-for-local-volatility-pricing.md)
  - [Finite-difference option Greeks](finite-difference-option-greeks.md)
- [Delta replication from a local-volatility pricing equation](delta-replication-from-a-local-volatility-pricing-equation.md)

## ↑ Ancestors (7)

1. [Local volatility model](local-volatility-model.md)
2. [Local volatility](local-volatility.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Delta replication from a local-volatility pricing equation](delta-replication-from-a-local-volatility-pricing-equation.md)
- [Exponential claim in a driftless square-root model](exponential-claim-in-a-driftless-square-root-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/5/iii/solution.md)
