# Geometric Asian option

↑ **Parent:** [Asian option](asian-option.md)

An [Asian option](asian-option.md) whose averaging uses the [geometric mean](geometric-mean.md). In the constant-coefficient [Black-Scholes model](black-scholes-model.md), the logarithm of the continuous geometric average is Gaussian with mean $\log S_0+(r-\sigma^2/2)T/2$ and variance $\sigma^2T/3$, because $\operatorname{Var}(\int_0^TW_t\,dt)=T^3/3$. Its forward mean is $S_0e^{rT/2-\sigma^2T/12}$. The discounted lognormal call formula gives its price. It is strictly cheaper than the terminal European call when $\sigma,K,T>0$ and $r\geq-\sigma^2/6$, since both its forward mean and log-variance are no larger, with strictly smaller variance. No unconditional comparison holds for arbitrary negative interest rates: for $r<-\sigma^2/6$, sufficiently small positive strikes reverse the inequality.

**Table of contents**

- [Conditional geometric-average Asian option formula](conditional-geometric-average-asian-option-formula.md)
- [Discrete geometric average under the stock-numeraire measure](discrete-geometric-average-under-the-stock-numeraire-measure.md)
  - [Stock-delivery option with a geometric average](stock-delivery-option-with-a-geometric-average.md)

## ↑ Ancestors (9)

1. [Asian option](asian-option.md)
2. [European contingent claim](european-contingent-claim.md)
3. [Contingent claim](contingent-claim.md)
4. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/29j/ii/solution.md)
