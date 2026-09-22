# Minimal martingale measure in a one-period market

↑ **Parent:** [One-period quadratic hedge](one-period-quadratic-hedge.md)

Let $m=\mathbb EY$ and $C=\operatorname{Cov}(Y)$ be an invertible [covariance matrix](covariance-matrix.md) of discounted gains. The displayed [signed martingale measure](signed-martingale-measure.md) leaves unchanged the mean-zero [random variables](random-variable-split.md) orthogonal to the martingale part $Y-m$: if $\mathbb EL=0$ and $\mathbb E[(Y-m)L]=0$, then $\mathbb E[Z_*L]=0$. Conversely, preservation of all these orthogonal directions forces the density to lie in the span of $1,Y-m$, and its pricing constraints give the displayed formula. If $Z_*>0$ it is an [equivalent martingale measure](risk-neutral-measure.md); if $Z_*\geq0$ it is a [dominated martingale measure](dominated-martingale-measure.md). Positivity is an extra condition, not a consequence of absence of [arbitrage](arbitrage.md) alone. In one period this density also minimizes $\mathbb EZ^2$ among square-integrable signed pricing densities, because every other such density differs by a vector orthogonal to $1,Y-m$. The initial capital in the unrestricted [one-period quadratic hedge](one-period-quadratic-hedge.md) of a discounted payoff $H$ is $\mathbb E[Z_*H]$.

**Table of contents**

- [Negative minimal density in an arbitrage-free one-period market](negative-minimal-density-in-an-arbitrage-free-one-period-market.md)

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

## ← Incoming links (4)

- [Negative minimal density in an arbitrage-free one-period market](negative-minimal-density-in-an-arbitrage-free-one-period-market.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/1/solution.md)
