# One-period quadratic hedge

↑ **Parent:** [Claim replication](claim-replication.md)

A one-period quadratic hedge minimizes $\mathbb E[(\xi-\phi R-\pi\cdot S_1)^2]$ over deterministic holdings, where $R\ne0$ is the riskless gross return, $\mu=\mathbb E S_1$, and the [covariance matrix](covariance-matrix.md) $V$ is invertible. For a square-integrable claim, the unique solution is $\pi^*=V^{-1}\operatorname{Cov}(S_1,\xi)$ and $\phi^*=(\mathbb E\xi-\pi^*\cdot\mu)/R$. Centering separates the squared bias from the quadratic error. Completing the square gives the excess error as $(\pi-\pi^*)^TV(\pi-\pi^*)$ after the bias is minimized. Unlike [claim replication](claim-replication.md), the residual need not vanish.

**Table of contents**

- [Fixed-capital quadratic hedge in a one-period market](fixed-capital-quadratic-hedge-in-a-one-period-market.md)
- [Minimal martingale measure in a one-period market](minimal-martingale-measure-in-a-one-period-market.md)
  - [Negative minimal density in an arbitrage-free one-period market](negative-minimal-density-in-an-arbitrage-free-one-period-market.md)
- [Signed martingale measure](signed-martingale-measure.md)
- [Gaussian quadratic hedge](gaussian-quadratic-hedge.md)
- [Minimum-norm one-period pricing weight](minimum-norm-one-period-pricing-weight.md)

## ↑ Ancestors (8)

1. [Claim replication](claim-replication.md)
2. [Contingent claim](contingent-claim.md)
3. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Gaussian quadratic hedge](gaussian-quadratic-hedge.md)
- [Minimal martingale measure in a one-period market](minimal-martingale-measure-in-a-one-period-market.md)
- [Minimum-norm one-period pricing weight](minimum-norm-one-period-pricing-weight.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/6/b/solution.md)
