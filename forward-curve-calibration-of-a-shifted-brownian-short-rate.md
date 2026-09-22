# Forward-curve calibration of a shifted Brownian short rate

↑ **Parent:** [Gaussian short-rate model with a deterministic shift](gaussian-short-rate-model-with-a-deterministic-shift.md)

To match a prescribed initial [instantaneous forward rate](instantaneous-forward-rate.md) curve $F_0(T)$ in the [Gaussian short-rate model with a deterministic shift](gaussian-short-rate-model-with-a-deterministic-shift.md), choose

$$
g(T)=F_0(T)+\tfrac12\sigma^2T^2.
$$

Since $W_0^Q=0$, its model forward rate is then $f_0(T)=g(T)-\sigma^2T^2/2=F_0(T)$. Moreover,

$$
P_0(T)=\exp\left[-\int_0^Tg(s)ds+\frac{\sigma^2T^3}{6}\right]=\exp\left[-\int_0^TF_0(s)ds\right],
$$

so the initial [zero-coupon bond](zero-coupon-bond.md) curve matches as well. A continuous initial forward curve gives pointwise calibration; a locally integrable curve gives the corresponding almost-everywhere interpretation of the [instantaneous forward rate](instantaneous-forward-rate.md).

## ↑ Ancestors (9)

1. [Gaussian short-rate model with a deterministic shift](gaussian-short-rate-model-with-a-deterministic-shift.md)
2. [Short rate](short-rate.md)
3. [Interest rate](interest-rate.md)
4. [Fixed-income security](fixed-income-security.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/6/ii/solution.md)
