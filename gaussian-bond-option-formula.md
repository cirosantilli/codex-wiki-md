# Gaussian bond-option formula

↑ **Parent:** [Gaussian forward-rate field](gaussian-forward-rate-field.md)

For a maturity-$T$ call on a unit maturity-$U$ [zero-coupon bond](zero-coupon-bond.md), where $t<T<U$, deterministic forward-rate volatilities make the bond-price ratio lognormal under the [T-forward measure](t-forward-measure.md). Its integrated variance is $V=\int_t^T\|\Sigma(s,U)-\Sigma(s,T)\|^2ds$. For $V>0$, put $d_1=[\log(P(t,U)/(KP(t,T)))+V/2]/\sqrt V$ and $d_2=d_1-\sqrt V$. Integrating the [lognormal distribution](log-normal-distribution.md) above the strike gives the displayed price. At $V=0$, the price is $(P(t,U)-KP(t,T))^+$. The [forward measure](forward-measure.md) is essential: the raw bond price has a stochastic discount rate under the money-market measure.

## ↑ Ancestors (9)

1. [Gaussian forward-rate field](gaussian-forward-rate-field.md)
2. [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)
3. [Interest rate](interest-rate.md)
4. [Fixed-income security](fixed-income-security.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32/6/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/6/solution.md)
