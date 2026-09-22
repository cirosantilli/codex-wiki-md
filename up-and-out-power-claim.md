# Up-and-out power claim

↑ **Parent:** [Barrier option](barrier-option.md)

An [up-and-out power claim](up-and-out-power-claim.md) pays a power of the terminal [stock](stock.md) price provided an upper barrier has never been reached. In the [Black-Scholes model](black-scholes-model.md), set $A=\log(c/S_0)/\sigma$ and $m_p=(\rho+(p-\tfrac12)\sigma^2)/\sigma$, where $\sigma>0$, $c>S_0$ and $T>0$. The [risk-neutral pricing](risk-neutral-pricing.md) value is

$$
S_0^p e^{[(p-1)\rho+p(p-1)\sigma^2/2]T}\left[\Phi\left(\frac{A-m_pT}{\sqrt T}\right)-e^{2m_pA}\Phi\left(\frac{-A-m_pT}{\sqrt T}\right)\right].
$$

Here $\Phi$ is the [standard normal distribution function](standard-normal-distribution-function.md). Weighting the [Brownian motion](brownian-motion-split.md) endpoint by $e^{p\sigma W_T-p^2\sigma^2T/2}$ changes the logarithmic drift to $m_p$; the [finite-horizon maximum of Brownian motion with drift](finite-horizon-maximum-of-brownian-motion-with-drift.md) then supplies the survival factor.

## ↑ Ancestors (8)

1. [Barrier option](barrier-option.md)
2. [Contingent claim](contingent-claim.md)
3. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34/3/solution.md)
- [Up-and-out power claim](up-and-out-power-claim.md)
