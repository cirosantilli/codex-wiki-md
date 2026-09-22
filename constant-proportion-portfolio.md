# Constant-proportion portfolio

↑ **Parent:** [Self-financing portfolio](self-financing-portfolio.md)

A [constant-proportion portfolio](constant-proportion-portfolio.md) holds a fixed fraction $\gamma$ of its [portfolio wealth](portfolio-wealth.md) in the [stock](stock.md). In the [Black-Scholes model](black-scholes-model.md) with bank rate $\rho$, initial wealth $V_0$, and no [consumption](consumption.md), its value is

$$
V_t=V_0(S_t/S_0)^\gamma\exp\left((1-\gamma)(\rho+\tfrac12\gamma\sigma^2)t\right).
$$

The [stock](stock.md) holding is $\gamma V_t/S_t$ and the remaining value $(1-\gamma)V_t$ is invested in the [bank account](bank-account.md). The [Itô formula](ito-s-lemma.md) verifies $dV_t/V_t=[\rho+\gamma(\mu-\rho)]dt+\gamma\sigma dW_t$ when the physical stock drift is $\mu$.

## ↑ Ancestors (7)

1. [Self-financing portfolio](self-financing-portfolio.md)
2. [Arbitrage](arbitrage.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Constant-proportion portfolio](constant-proportion-portfolio.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/4/solution.md)
