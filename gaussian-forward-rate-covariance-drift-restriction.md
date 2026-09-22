# Gaussian forward-rate covariance drift restriction

↑ **Parent:** [Integrated Gaussian forward-rate process](integrated-gaussian-forward-rate-process.md)

Suppose the [instantaneous forward rate](instantaneous-forward-rate.md) field has mean $\mu_{s,T}$ and covariance $c(s\wedge r,T,U)$, with deterministic initial curve and suitable integrability and maturity regularity. Its discounted [zero-coupon bond](zero-coupon-bond.md) prices are [martingales](martingale-split.md) exactly when the displayed mean identity holds. Put

$$
A(s,T)=\int_0^s\mu_{u,u}du+\int_s^T\mu_{s,u}du.
$$

The discounted bond price is $\exp[-A(s,T)-Y(s,T)]$, where $Y$ is the [integrated Gaussian forward-rate process](integrated-gaussian-forward-rate-process.md). Its conditional Gaussian exponential expectation gives the equivalent identity $A(s,T)-A(0,T)=v(s,T)/2$. Differentiating this in maturity gives the displayed restriction. Conversely, integrating that restriction on the diagonal and along the current curve recovers the half-variance identity, by symmetry of the covariance over the maturity square. The [Gaussian exponential martingale with deterministic variance](gaussian-exponential-martingale-with-deterministic-variance.md) then verifies the full conditional [martingale](martingale-split.md) property. This formulation does not require a time derivative of $c$.

## ↑ Ancestors (10)

1. [Integrated Gaussian forward-rate process](integrated-gaussian-forward-rate-process.md)
2. [Gaussian forward-rate field](gaussian-forward-rate-field.md)
3. [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)
4. [Interest rate](interest-rate.md)
5. [Fixed-income security](fixed-income-security.md)
6. [Mathematical finance](mathematical-finance-split.md)
7. [Mathematical optimization](mathematical-optimization-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/6/solution.md)
