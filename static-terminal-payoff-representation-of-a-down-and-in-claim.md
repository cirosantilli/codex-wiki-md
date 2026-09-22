# Static terminal-payoff representation of a down-and-in claim

↑ **Parent:** [Down-and-in claim](down-and-in-claim.md)

For initial spot $s>b$ in the [Black-Scholes model](black-scholes-model.md), put $\nu=(\rho-\sigma^2/2)/\sigma$ and $\kappa=(s/b)^2$. A [down-and-in claim](down-and-in-claim.md) with terminal payoff $f$ has the same initial price as the terminal claim $g(x)=f(x)\mathbf1_{x\le b}+\kappa^{-\nu/\sigma}f(x/\kappa)\mathbf1_{x>\kappa b}$. Reflection of the log-price endpoint above the lower barrier changes its [normal probability density](normal-density.md) to $e^{2\nu\ell}\phi_T(y-2\ell-\nu T)$, where $\ell=\log(b/s)/\sigma$. Substitution $z=y-2\ell$ gives the payoff identity. This is price equality, not pathwise equality of payments.

## ↑ Ancestors (9)

1. [Down-and-in claim](down-and-in-claim.md)
2. [Barrier option](barrier-option.md)
3. [Contingent claim](contingent-claim.md)
4. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35/5/solution.md)
