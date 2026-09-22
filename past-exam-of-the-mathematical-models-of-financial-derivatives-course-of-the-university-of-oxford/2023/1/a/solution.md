<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [self-financing portfolio](../../../../self-financing-portfolio.md) which holds $\Delta=V_S$ shares and $V-SV_S$ in the [bank account](../../../../bank-account.md), withdrawing the claim's cash flow $C\,dt$. A share's total gain includes the [continuous dividend yield](../../../../continuous-dividend-yield.md), so its gain is $dS+DS\,dt$. Matching the claim's total gain gives

$$
dV+C\,dt=V_S(dS+DS\,dt)+r(V-SV_S)\,dt.
$$

By the [Itô formula](../../../../ito-s-lemma.md),

$$
dV=\left[V_t+(\mu-D)SV_S+\frac12\sigma^2S^2V_{SS}\right]dt+\sigma SV_S\,dW.
$$

The [delta hedge](../../../../delta-hedge.md) cancels the [Brownian motion](../../../../brownian-motion-split.md) term. Comparing the remaining drifts yields the [Black-Scholes equation with claim dividends](../../../../black-scholes-equation-with-claim-dividends.md), with the stock's own dividend yield included:

$$
\boxed{V_t+\frac12\sigma^2S^2V_{SS}+(r-D)SV_S-rV=-C(S,t),\qquad V(S,T)=S}.
$$

This gain calculation accounts for rebalancing through the [self-financing portfolio](../../../../self-financing-portfolio.md) condition. The physical expected-return parameter $\mu$ cancels, as required by [risk-neutral pricing](../../../../risk-neutral-pricing.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
