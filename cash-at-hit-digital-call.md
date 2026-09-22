# Cash-at-hit digital call

↑ **Parent:** [Digital call option](digital-call-option.md)

A barrier claim paying a fixed cash amount at the first time the [stock](stock.md) reaches a higher level, provided this happens before expiry. In the [Black-Scholes model](black-scholes-model.md), take $a=\log(c/S_0)/\sigma$ and $b=(\sigma^2/2-\rho)/\sigma$. Its unit-cash price is $\mathbb E_Q[e^{-\rho T_{a,b}}\mathbf1_{\{T_{a,b}\leq T\}}]$, given by [truncated discounted Brownian first passage](truncated-discounted-brownian-first-passage.md). The effective square root $\sqrt{b^2+2\rho}=|\rho+\sigma^2/2|/\sigma$ is real for every real interest rate.

## ↑ Ancestors (10)

1. [Digital call option](digital-call-option.md)
2. [Binary option](binary-option.md)
3. [European contingent claim](european-contingent-claim.md)
4. [Contingent claim](contingent-claim.md)
5. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
6. [Mathematical finance](mathematical-finance-split.md)
7. [Mathematical optimization](mathematical-optimization-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41/3/solution.md)
