# Log-optimal investment with Gaussian drift learning

↑ **Parent:** [Logarithmic utility](logarithmic-utility.md)

For a [stock](stock.md) with observed dynamics $dS_t/S_t=\sigma d\widehat W_t+\sigma m_tdt$ and constant riskless [interest rate](interest-rate.md) $r$, the [finite-horizon pricing density for Gaussian drift learning](finite-horizon-pricing-density-for-gaussian-drift-learning.md) with $k=r/\sigma$ gives $\zeta_t=e^{-rt}D_t$. The terminal [logarithmic utility](logarithmic-utility.md) condition $1/w_T^*=\lambda\zeta_T$ and the [state-price budget constraint](state-price-budget-constraint.md) give $\lambda=1/w_0$. Replication then gives $w_t^*=w_0/\zeta_t$ at every time. The [Itô formula](ito-s-lemma.md) for $1/\zeta$ makes the optimal dollar stock fraction $(m_t-r/\sigma)/\sigma$. Its finite expected log return follows from finite posterior second moments on finite horizons.

## ↑ Ancestors (8)

1. [Logarithmic utility](logarithmic-utility.md)
2. [Constant relative risk aversion utility](constant-relative-risk-aversion-utility.md)
3. [Utility function](utility-function-split.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40/3/solution.md)
