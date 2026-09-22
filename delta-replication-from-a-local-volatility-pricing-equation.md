# Delta replication from a local-volatility pricing equation

↑ **Parent:** [Pricing equation for a local volatility model](pricing-equation-for-a-local-volatility-model.md)

If $V$ satisfies the [pricing equation for a local volatility model](pricing-equation-for-a-local-volatility-model.md), hold $h^S_t=V_S(t,S_t)$ stocks and $h^B_t=[V(t,S_t)-S_tV_S(t,S_t)]/B_t$ units of the [bank account](bank-account.md). Their value is $V(t,S_t)$. The [pricing equation for a local volatility model](pricing-equation-for-a-local-volatility-model.md) and [Itô formula](ito-s-lemma.md) give

$$
dV(t,S_t)=rV(t,S_t)dt+\sigma(S_t)S_tV_S(t,S_t)dW_t^Q=h^B_t\,dB_t+h^S_t\,dS_t.
$$

Thus this is a [self-financing strategy](self-financing-portfolio.md), with terminal value $g(S_T)$. It is a [delta hedge](delta-hedge.md), and nonnegative $V$ makes its wealth an [admissible trading strategy](admissible-trading-strategy.md). The stock and bank wealth amounts are $S_tV_S$ and $V-S_tV_S$, rather than the asset-unit holdings.

## ↑ Ancestors (8)

1. [Pricing equation for a local volatility model](pricing-equation-for-a-local-volatility-model.md)
2. [Local volatility model](local-volatility-model.md)
3. [Local volatility](local-volatility.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/5/ii/solution.md)
