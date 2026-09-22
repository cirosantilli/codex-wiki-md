# Minimum-norm one-period pricing weight

↑ **Parent:** [One-period quadratic hedge](one-period-quadratic-hedge.md)

The initial cost of the [one-period quadratic hedge](one-period-quadratic-hedge.md) is $\mathbb E[\rho^*\xi]$. This pricing weight satisfies $\mathbb E[\rho^*R]=1$ and $\mathbb E[\rho^*S_1]=S_0$. Among square-integrable weights satisfying these equations it has the smallest squared norm:

$$
\mathbb E[(\rho^*)^2]=R^{-2}+(S_0-R^{-1}\mu)^TV^{-1}(S_0-R^{-1}\mu).
$$

For another admissible weight $\rho$, its difference from $\rho^*$ is orthogonal to $1$ and all coordinates of $S_1$, hence to $\rho^*$. The [Pythagorean theorem in an inner-product space](pythagorean-theorem-in-an-inner-product-space.md) gives $\mathbb E[\rho^2]=\mathbb E[(\rho^*)^2]+\mathbb E[(\rho-\rho^*)^2]$. This weight can be signed; positivity, and hence interpretation as a [state-price density](state-price-density.md), requires additional assumptions.

## ↑ Ancestors (9)

1. [One-period quadratic hedge](one-period-quadratic-hedge.md)
2. [Claim replication](claim-replication.md)
3. [Contingent claim](contingent-claim.md)
4. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/6/b/solution.md)
