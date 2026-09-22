# Reflected European payoff for an up-and-in option

↑ **Parent:** [Up-and-in claim](up-and-in-claim.md)

For an [up-and-in claim](up-and-in-claim.md) in the dividend-free [Black-Scholes model](black-scholes-model.md), set $\nu=(\rho-\sigma^2/2)/\sigma$, $\kappa=(S_0/b)^2$ and assume finite absolute payoff expectations. Its initial price equals the [risk-neutral pricing](risk-neutral-pricing.md) value of the displayed [European option](european-contingent-claim.md). To prove this, express the log-price as $\sigma(W_t+\nu t)$ and apply the [joint endpoint and maximum law for drifted Brownian motion](joint-endpoint-and-maximum-law-for-drifted-brownian-motion.md). Above the logarithmic barrier $a=\log(b/S_0)/\sigma$, use the unrestricted endpoint density. Below it, the density of paths which hit the barrier is $e^{2a\nu}\phi_T(y-2a-\nu T)$. Substitution $z=y-2a$ gives the scaled payoff, the threshold $\kappa b$, and the factor $\kappa^{-\nu/\sigma}$. This is an initial-price identity, not a pathwise equality of terminal payoffs.

## ↑ Ancestors (9)

1. [Up-and-in claim](up-and-in-claim.md)
2. [Barrier option](barrier-option.md)
3. [Contingent claim](contingent-claim.md)
4. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/3/solution.md)
