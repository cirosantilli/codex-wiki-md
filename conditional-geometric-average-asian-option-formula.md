# Conditional geometric-average Asian option formula

↑ **Parent:** [Geometric Asian option](geometric-asian-option.md)

For $I_t=\int_0^t\log S_u\,du$ and $G_T=\exp(T^{-1}I_T)$ in the [Black-Scholes model](black-scholes-model.md), the conditional law of $\log G_T$ under the [risk-neutral measure](risk-neutral-measure.md) has a [normal distribution](normal-distribution.md) with mean $m_t$ and variance $q_t$. The future Brownian integral equals $\int_t^T(T-u)\,dW_u$, so the [Itô isometry](ito-isometry.md) gives the variance. For strike $K>0$ and $t<T$, the call price is $e^{-\rho(T-t)}[e^{m_t+q_t/2}\Phi(d_1)-K\Phi(d_2)]$, where $d_2=(m_t-\log K)/\sqrt{q_t}$ and $d_1=d_2+\sqrt{q_t}$. This follows by completing the square in the truncated normal exponential moment; the known past integral must be included in the mean.

## ↑ Ancestors (10)

1. [Geometric Asian option](geometric-asian-option.md)
2. [Asian option](asian-option.md)
3. [European contingent claim](european-contingent-claim.md)
4. [Contingent claim](contingent-claim.md)
5. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
6. [Mathematical finance](mathematical-finance-split.md)
7. [Mathematical optimization](mathematical-optimization-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/5/solution.md)
