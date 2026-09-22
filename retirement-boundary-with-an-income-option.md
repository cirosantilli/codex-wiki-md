# Retirement boundary with an income option

↑ **Parent:** [Merton consumption-investment problem](merton-consumption-investment-problem.md)

Consider irreversible [optimal stopping](optimal-stopping.md) of employment paying income $\varepsilon>0$ and imposing disutility $\lambda>0$. Assume $r,\rho>0$, nonzero [market price of risk](market-price-of-risk.md) $\kappa$, a positive [Merton consumption constant](merton-consumption-constant.md), and solvency allowing borrowing against perpetual income up to $\varepsilon/r$ before retirement. Let $m<0$ solve $\kappa^2m(m-1)/2+(\rho-r)m-\rho=0$. The retirement threshold is the displayed wealth level.

To derive it, apply the [wealth-variable Legendre dual](wealth-variable-legendre-dual.md). The working dual equals the retired dual plus $h(z)=\varepsilon z/r-\lambda/\rho+Dz^m$. Excluding the growing homogeneous solution enforces the solvency asymptotic. Value matching and [smooth fit](smooth-pasting.md) at the retirement marginal value $z_*$ give $h(z_*)=h'(z_*)=0$, hence $z_*=(\lambda r/(\varepsilon\rho))m/(m-1)$ and $D=-\varepsilon z_*^{1-m}/(rm)>0$. The retired inverse marginal value gives $\overline w=\gamma_M^{-1}z_*^{-1/R}$.

The root equation implies $z_*/(\lambda/\varepsilon)=1+\kappa^2m/(2\rho)<1$. Thus the boundary exceeds the instantaneous gain-zero level $\gamma_M^{-1}(\varepsilon/\lambda)^{1/R}$. A tighter borrowing constraint changes this free-boundary problem. Smooth fit matches the first derivative; matching the second derivative would incorrectly remove the income option.

## ↑ Ancestors (10)

1. [Merton consumption-investment problem](merton-consumption-investment-problem.md)
2. [Investment-consumption problem](investment-consumption-problem.md)
3. [Expected utility maximization](expected-utility-maximization.md)
4. [Expected utility hypothesis](expected-utility-hypothesis.md)
5. [Utility function](utility-function-split.md)
6. [Mathematical finance](mathematical-finance-split.md)
7. [Mathematical optimization](mathematical-optimization-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-40/3/solution.md)
