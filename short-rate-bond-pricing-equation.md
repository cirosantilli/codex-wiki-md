# Short-rate bond pricing equation

↑ **Parent:** [One-factor short-rate model](one-factor-short-rate-model.md)

For pricing drift $\mu_Q$, a unit [zero-coupon bond](zero-coupon-bond.md) price $P(t,r;T)$ satisfies $P_t+\mu_QP_r+\eta^2P_{rr}/2-rP=0$, with $P(T,r;T)=1$. [Itô formula](ito-s-lemma.md) makes its bank-account-discounted value a local [martingale](martingale-split.md); suitable integrability gives $P(t,r;T)=\mathbb E^Q[\exp(-\int_t^T r_sds)\mid r_t=r]$. The rate kills the diffusion semigroup, as in the [Feynman-Kac formula](feynman-kac-formula.md).

**Table of contents**

- [Short-rate diffusion hedging](short-rate-diffusion-hedging.md)
- [Affine diffusion bond pricing](affine-diffusion-bond-pricing.md)

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35/6/solution.md)
