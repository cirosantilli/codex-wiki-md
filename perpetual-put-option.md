# Perpetual put option

↑ **Parent:** [American put option](american-put-option.md)

For risk-neutral [stock](stock.md) dynamics $dS=(r-\delta)Sdt+\sigma S dW$, with $r>0$ and $\sigma>0$, let $\beta_-<0$ solve $\sigma^2\beta(\beta-1)/2+(r-\delta)\beta-r=0$. A fixed downward trigger $L\in(0,X)$ gives continuation value $(X-L)(S/L)^{\beta_-}$ for $S>L$. Optimizing over the trigger, or imposing [smooth fit](smooth-pasting.md), gives the displayed boundary. The optimal value equals $X-S$ below $S^*$ and the continuation expression above. A verification argument uses its payoff majorization and nonpositive discounted generator. At $r=0$ and $\delta\ge0$, the perpetual value is $X$ for positive spot, approached by triggers tending to zero rather than attained at a positive finite trigger.

**Table of contents**

- [Dividend-yield sensitivity of the perpetual put trigger](dividend-yield-sensitivity-of-the-perpetual-put-trigger.md)

## ↑ Ancestors (9)

1. [American put option](american-put-option.md)
2. [Put option](put-option.md)
3. [Contingent claim](contingent-claim.md)
4. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32/4/b/solution.md)
