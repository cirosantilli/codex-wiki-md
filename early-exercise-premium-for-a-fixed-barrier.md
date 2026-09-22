# Early exercise premium for a fixed barrier

↑ **Parent:** [Barrier-triggered put](barrier-triggered-put.md)

For an alive [barrier-triggered put](barrier-triggered-put.md), the difference from the corresponding [European put option](european-put-option.md) is the displayed discounted conditional expectation, evaluated under the [risk-neutral measure](risk-neutral-measure.md). To prove it, condition the European payoff on the first hitting time or expiry and use the [Strong Markov property](strong-markov-property.md). At a hit, continuation of the European claim is worth $P(B,\tau_B;K)$, whereas the fixed exercise rule pays $K-B$ immediately. On survival to expiry the two payoffs coincide. The relevant stopped quantities are bounded, so the conditional-expectation argument is justified.

## ↑ Ancestors (10)

1. [Barrier-triggered put](barrier-triggered-put.md)
2. [American put option](american-put-option.md)
3. [Put option](put-option.md)
4. [Contingent claim](contingent-claim.md)
5. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing-split.md)
6. [Mathematical finance](mathematical-finance-split.md)
7. [Mathematical optimization](mathematical-optimization-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2021/3/b/iii/solution.md)
