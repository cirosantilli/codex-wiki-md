# Gaussian forward-rate field

↑ **Parent:** [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)

With deterministic Hilbert-space-valued volatility, a deterministic initial curve and the [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md) drift restriction, the [instantaneous forward rate](instantaneous-forward-rate.md) is a [Gaussian random field](gaussian-random-field.md) indexed by observation time and maturity. Put $\Sigma(t,T)=\int_t^T\sigma(t,u)du$. Absence of [arbitrage](arbitrage.md) requires $\alpha(t,T)=\langle\sigma(t,T),\Sigma(t,T)\rangle$. Indeed, [Itô formula](ito-s-lemma.md) gives bond drift $r_t-\int_t^T\alpha(t,u)du+\|\Sigma(t,T)\|^2/2$; equating it to the [short rate](short-rate.md) and differentiating in maturity yields this restriction. The field covariance is

$$
\operatorname{Cov}(f(t,T),f(s,U))=\int_0^{\min(t,s)}\langle\sigma(v,T),\sigma(v,U)\rangle dv.
$$

Finite-dimensional volatility spaces give finite-factor models; an infinite-dimensional space permits much richer maturity correlations. Gaussian rates can be negative. Deterministic volatility gives explicit [zero-coupon bond](zero-coupon-bond.md) and bond-option formulas.

**Table of contents**

- [Integrated Gaussian forward-rate process](integrated-gaussian-forward-rate-process.md)
  - [Gaussian forward-rate covariance drift restriction](gaussian-forward-rate-covariance-drift-restriction.md)
- [Musiela forward-curve equation](musiela-forward-curve-equation.md)
  - [Stationary Gaussian forward curve](stationary-gaussian-forward-curve.md)
- [Gaussian bond-option formula](gaussian-bond-option-formula.md)

## ↑ Ancestors (8)

1. [Heath-Jarrow-Morton model](heath-jarrow-morton-model.md)
2. [Interest rate](interest-rate.md)
3. [Fixed-income security](fixed-income-security.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Brownian sheet](brownian-sheet.md)
- [Gaussian caplet bond-put formula](gaussian-caplet-bond-put-formula.md)
- [Integrated Gaussian forward-rate process](integrated-gaussian-forward-rate-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32/6/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32/6/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/6/solution.md)
