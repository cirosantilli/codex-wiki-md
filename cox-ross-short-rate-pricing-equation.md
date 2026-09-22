# Cox-Ross short-rate pricing equation

↑ **Parent:** [One-factor short-rate model](one-factor-short-rate-model.md)

For smooth derivative prices depending on a [Markov](markov-property.md) [short rate](short-rate.md), [Itô formula](ito-s-lemma.md) gives physical drift $m=V_t+bV_r+\sigma^2V_{rr}/2$ and exposure $s=\sigma V_r$. The common [short-rate market price of risk](short-rate-market-price-of-risk.md) gives $m-rV=\theta s$, yielding this equation. Under the [risk-neutral measure](risk-neutral-measure.md), the rate drift is $b-\sigma\theta$ and the bank-discounted price is a [martingale](martingale-split.md) under suitable integrability. A unit [zero-coupon bond](zero-coupon-bond.md) has terminal value one and price $\mathbb E^Q[\exp(-\int_t^T r_sds)\mid r_t=r]$.

## ↑ Ancestors (9)

1. [One-factor short-rate model](one-factor-short-rate-model.md)
2. [Short rate](short-rate.md)
3. [Interest rate](interest-rate.md)
4. [Fixed-income security](fixed-income-security.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35/5/c/solution.md)
