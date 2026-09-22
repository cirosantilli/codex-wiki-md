# Forward-start call option

↑ **Parent:** [Forward start option](forward-start-option.md)

A [forward start option](forward-start-option.md) whose [call option](call-option.md) strike is fixed at time $T_1$ as $\lambda S_{T_1}$, with expiry $T_2>T_1$ and $\lambda>0$. Its terminal [financial payoff](contingent-claim-payoff.md) depends on the intermediate [stock](stock.md) price as well as the final price. Two paths ending at the same price can therefore have different payoffs, so a recombining stock tree must retain enough history to value the contract.

In a homogeneous dividend-free [Black-Scholes model](black-scholes-model.md), let $c(1,\lambda,T_2-T_1)$ be the [European call option](european-call-option.md) price with current stock one and strike $\lambda$ over the remaining duration. Homogeneity gives value $S_{T_1}c(1,\lambda,T_2-T_1)$ when the strike is fixed. The discounted [stock](stock.md) is a [martingale](martingale-split.md), so [risk-neutral pricing](risk-neutral-pricing.md) before that date gives

$$
V_t=S_t c(1,\lambda,T_2-T_1),\qquad t<T_1.
$$

The same argument holds in a homogeneous [binomial options pricing model](binomial-options-pricing-model.md) with the corresponding remaining-step call value. It depends on the normalized future pricing rule being independent of the stock level at the fixing date.

## ↑ Ancestors (9)

1. [Forward start option](forward-start-option.md)
2. [European contingent claim](european-contingent-claim.md)
3. [Contingent claim](contingent-claim.md)
4. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing-split.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Call option](call-option.md)
- [Forward start option](forward-start-option.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2015/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3/29j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3/29k/d/solution.md)
