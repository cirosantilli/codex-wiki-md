# Fixed-capital quadratic hedge in a one-period market

↑ **Parent:** [One-period quadratic hedge](one-period-quadratic-hedge.md)

For a discounted [contingent claim](contingent-claim.md) $H$ and gain vector $Y$, fix initial capital $v$ and minimize $\mathbb E(H-v-\theta^TY)^2$. Differentiation gives the [least-squares normal equations](normal-equations-for-linear-least-squares.md) $G\theta=\mathbb E[Y(H-v)]$, where $G=\mathbb E[YY^T]$ is assumed invertible. This gives the displayed hedge. Optimizing capital as well instead centers the gains and uses their [covariance matrix](covariance-matrix.md): $\theta^*=\operatorname{Cov}(Y)^{-1}\operatorname{Cov}(Y,H)$ and $v^*=\mathbb EH-(\theta^*)^T\mathbb EY$. Fixing the initial capital is therefore a different quadratic problem.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/1/solution.md)
