# Vasicek model

↑ **Parent:** [Short rate](short-rate.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vasicek_model)

A Gaussian [short rate](short-rate.md) model with [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md) dynamics under the chosen pricing measure. For $a>0$, its unit [zero-coupon bond](zero-coupon-bond.md) value is $P(t,T)=A(\tau)e^{-B(\tau)r_t}$, where $\tau=T-t$, $B(\tau)=(1-e^{-a\tau})/a$ and

$$
\log A(\tau)=\left(b-\frac{\eta^2}{2a^2}\right)(B(\tau)-\tau)-\frac{\eta^2}{4a}B(\tau)^2.
$$

Solve the linear [stochastic differential equation](stochastic-differential-equation.md), integrate over future time, and use the [exponential moment](exponential-moment.md) of the resulting Gaussian integral to obtain this price. Its Gaussian law permits negative [short rates](short-rate.md).

## ↑ Ancestors (8)

1. [Short rate](short-rate.md)
2. [Interest rate](interest-rate.md)
3. [Fixed-income security](fixed-income-security.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Affine diffusion bond pricing](affine-diffusion-bond-pricing.md)
- [Hull-White model](hull-white-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32/6/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32/6/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/6/solution.md)
