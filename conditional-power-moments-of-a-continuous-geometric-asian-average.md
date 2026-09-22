# Conditional power moments of a continuous geometric Asian average

↑ **Parent:** [Conditional geometric-average Asian option formula](conditional-geometric-average-asian-option-formula.md)

Let $A_t=\exp(t^{-1}\int_0^t\log S_u\,du)$ for a positive [geometric Brownian motion](geometric-brownian-motion.md) in the non-dividend-paying [Black-Scholes model](black-scholes-model.md), and put $\tau=T-t$. Under the [risk-neutral measure](risk-neutral-measure.md), the future log-average is

$$
\log A_T=\frac tT\log A_t+\frac\tau T\log S_t+\frac{r-\sigma^2/2}{2T}\tau^2
+\frac\sigma T\int_t^T(W_u-W_t)du.
$$

The final integral is a centred normal variable independent of the past, with variance $\tau^3/3$. Applying the [moment-generating function of a normal distribution](moment-generating-function-of-a-normal-distribution.md) proves the displayed identity for every real $p$. Multiplication by $e^{-r\tau}$ prices the payoff $A_T^p$. The historical average must remain a state variable; terminal stock price alone does not determine this payoff.

## ↑ Ancestors (11)

1. [Conditional geometric-average Asian option formula](conditional-geometric-average-asian-option-formula.md)
2. [Geometric Asian option](geometric-asian-option.md)
3. [Asian option](asian-option.md)
4. [European contingent claim](european-contingent-claim.md)
5. [Contingent claim](contingent-claim.md)
6. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing-split.md)
7. [Mathematical finance](mathematical-finance-split.md)
8. [Mathematical optimization](mathematical-optimization-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2010/b/5/d/solution.md)
