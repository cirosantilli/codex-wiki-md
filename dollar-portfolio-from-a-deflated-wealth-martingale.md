# Dollar portfolio from a deflated wealth martingale

↑ **Parent:** [Deflator-based claim replication](deflator-based-claim-replication.md)

In the completed [natural Brownian filtration](natural-brownian-filtration.md), suppose $dS_t/S_t=\mu_tdt+\sigma_tdW_t$ with $\sigma_t\ne0$, and let $d\zeta_t=-\zeta_t(r_tdt+\kappa_tdW_t)$, $\kappa_t=(\mu_t-r_t)/\sigma_t$. For an affordable nonnegative terminal claim $X$, represent the [conditional-expectation martingale](conditional-expectation-martingale.md) $N_t=\mathbb E[\zeta_TX\mid\mathcal F_t]$ as $dN_t=h_tdW_t$. Then $w_t=N_t/\zeta_t$ and the displayed dollar amount in the [stock](stock.md) replicate $X$. The [Itô product rule](ito-product-rule.md) gives $d(\zeta w)=\zeta(\sigma\theta-\kappa w)dW$, proving the formula; share holdings are $\theta_t/S_t$.

## ↑ Ancestors (9)

1. [Deflator-based claim replication](deflator-based-claim-replication.md)
2. [Local martingale deflator](local-martingale-deflator.md)
3. [Martingale deflator](martingale-deflator.md)
4. [Risk-neutral measure](risk-neutral-measure.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40/2/solution.md)
