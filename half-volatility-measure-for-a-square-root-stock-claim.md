# Half-volatility measure for a square-root stock claim

↑ **Parent:** [Square-root stock implied volatility](square-root-stock-implied-volatility.md)

For bounded [predictable](predictable-process.md) $\sigma$ on $[0,T]$, the [stochastic exponential](doleans-dade-exponential.md) $Z_s=\exp(\tfrac12\int_0^s\sigma_u\,dW_u-\tfrac18\int_0^s\sigma_u^2du)$ is a positive [martingale](martingale-split.md) by the [Novikov condition](novikov-s-condition.md). Under $dQ/dP=Z_T$, the [Bayes formula for conditional expectation](bayes-formula-for-conditional-expectation.md) gives

$$
\mathbb E_P[\sqrt{S_T}\mid\mathcal F_t]=\sqrt{S_t}\,\mathbb E_Q\left[\exp\left(-\frac18\int_t^T\sigma_u^2du\right)\middle|\mathcal F_t\right].
$$

Indeed, the square-root stock ratio is $(Z_T/Z_t)\exp(-\tfrac18\int_t^T\sigma_u^2du)$. This exact identity gives the bounds on [square-root stock implied volatility](square-root-stock-implied-volatility.md) by bounding integrated variance pathwise. The [Girsanov theorem](girsanov-theorem.md) gives $W^Q=W-\tfrac12\int\sigma\,du$. The measure is an auxiliary pricing identity for this payoff, not a claim that it is an [equivalent martingale measure](risk-neutral-measure.md) for the original stock.

## ↑ Ancestors (9)

1. [Square-root stock implied volatility](square-root-stock-implied-volatility.md)
2. [Square-root stock claim](square-root-stock-claim.md)
3. [Contingent claim](contingent-claim.md)
4. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/2/d/solution.md)
