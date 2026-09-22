# Gaussian short-rate model with a deterministic shift

↑ **Parent:** [Short rate](short-rate.md)

Under a [risk-neutral measure](risk-neutral-measure.md) $Q$, let the [short rate](short-rate.md) be $r_t=g(t)+\sigma W_t^Q$, with deterministic locally integrable $g$ and constant $\sigma>0$. For a [zero-coupon bond](zero-coupon-bond.md) paying one at $T$, the [risk-neutral pricing](risk-neutral-pricing.md) value is

$$
P_t(T)=\exp\left[-\int_t^Tg(s)ds-\sigma(T-t)W_t^Q+\frac{\sigma^2(T-t)^3}{6}\right].
$$

Indeed, conditional on $\mathcal F_t$, the random part of the integrated future [short rate](short-rate.md) is $\sigma\int_t^T(T-u)dW_u^Q$, which is Gaussian with mean zero and variance $\sigma^2(T-t)^3/3$. Its [exponential moment](exponential-moment.md) gives the formula. At points where $g$ is continuous, the [instantaneous forward rate](instantaneous-forward-rate.md) is

$$
f_t(T)=-\partial_T\log P_t(T)=g(T)+\sigma W_t^Q-\tfrac12\sigma^2(T-t)^2.
$$

For merely locally integrable $g$, the same identity holds almost everywhere. The model allows negative [short rates](short-rate.md) and gives explicit bond prices and forward curves.

**Table of contents**

- [Forward-curve calibration of a shifted Brownian short rate](forward-curve-calibration-of-a-shifted-brownian-short-rate.md)

## ↑ Ancestors (8)

1. [Short rate](short-rate.md)
2. [Interest rate](interest-rate.md)
3. [Fixed-income security](fixed-income-security.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Forward-curve calibration of a shifted Brownian short rate](forward-curve-calibration-of-a-shifted-brownian-short-rate.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/6/i/solution.md)
