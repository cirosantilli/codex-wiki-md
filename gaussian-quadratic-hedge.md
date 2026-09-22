# Gaussian quadratic hedge

↑ **Parent:** [One-period quadratic hedge](one-period-quadratic-hedge.md)

If $S_1$ has a [multivariate normal distribution](multivariate-normal-distribution.md) with mean $\mu$ and invertible covariance $V$, and $g$ has bounded gradient, [Gaussian integration by parts](stein-s-lemma-probability.md) gives $\operatorname{Cov}(S_1,g(S_1))=V\mathbb E[\nabla g(S_1)]$. Consequently the risky holdings of its [one-period quadratic hedge](one-period-quadratic-hedge.md) equal the expected payoff gradient. The initial cost is $R^{-1}\mathbb E[g(S_1)]+(S_0-R^{-1}\mu)\cdot\mathbb E[\nabla g(S_1)]$. Bounded gradient ensures linear growth and square integrability, even if the payoff is not bounded.

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

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/6/d/solution.md)
