# Exact forward-curve fit in the Hull-White model

↑ **Parent:** [Hull-White model](hull-white-model.md)

Let $f_0(t)$ be the initial [instantaneous forward rate](instantaneous-forward-rate.md) curve and choose $r_0=f_0(0)$. In the [Hull-White model](hull-white-model.md), take $\beta(t)=f_0'(t)+af_0(t)+\eta^2(1-e^{-2at})/(2a)$. To verify the fit, write $r_t=x_t+\phi(t)$ with $dx_t=-ax_tdt+\eta dW_t^Q$, $x_0=0$, and $\phi(t)=f_0(t)+\eta^2(1-e^{-at})^2/(2a^2)$. The [Gaussian](normal-distribution.md) exponential formula gives $-\partial_T\log P(0,T)=\phi(T)-\eta^2(1-e^{-aT})^2/(2a^2)=f_0(T)$.

## ↑ Ancestors (9)

1. [Hull-White model](hull-white-model.md)
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
