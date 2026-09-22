# Gaussian short-rate model with constant coefficients

↑ **Parent:** [Short rate](short-rate.md)

For $dr_t=a_0dt+b_0dW_t$ under a [risk-neutral measure](risk-neutral-measure.md), the [instantaneous forward rate](instantaneous-forward-rate.md) and [zero-coupon bond](zero-coupon-bond.md) prices are

$$
f_t(T)=r_t+a_0(T-t)-\frac12b_0^2(T-t)^2,\qquad P(t,T)=\exp\left(-(T-t)r_t-\frac{a_0}2(T-t)^2+\frac{b_0^2}6(T-t)^3\right).
$$

Indeed, conditional on current information, $\int_t^T r_sds$ is Gaussian with mean $(T-t)r_t+a_0(T-t)^2/2$ and variance $b_0^2(T-t)^3/3$. Its negative exponential expectation gives the bond formula, and differentiating its logarithm gives the [instantaneous forward rate](instantaneous-forward-rate.md). Equivalently the affine forward-rate equation has $A'=0$, $A(0)=1$, and $B'=a_0-b_0^2\theta$, $B(0)=0$. This is the constant-drift instance of the Ho-Lee Gaussian [short rate](short-rate.md) model; the model permits negative short rates.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32/6/solution.md)
