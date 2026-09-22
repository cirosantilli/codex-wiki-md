<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the non-dividend-paying [stock](../../../../stock.md), a [self-financing portfolio](../../../../self-financing-portfolio.md) replicating a smooth [European option](../../../../european-contingent-claim.md) has $\Delta=V_S$ shares and $V-SV_S$ in the [bank account](../../../../bank-account.md). Its gain satisfies

$$
dV=V_S\,dS+r(V-SV_S)\,dt.
$$

The [Itô formula](../../../../ito-s-lemma.md) gives $dV=(V_t+\mu SV_S+\sigma^2S^2V_{SS}/2)dt+\sigma SV_SdW$. Matching its diffusion and drift with the portfolio gains cancels $\mu$, yielding

$$
\boxed{V_t+\frac12\sigma^2S^2V_{SS}+rSV_S-rV=0}.
$$

The [financial payoff](../../../../contingent-claim-payoff.md) supplies the terminal value. This is the [Black-Scholes equation](../../../../black-scholes-equation.md); the associated [risk-neutral measure](../../../../risk-neutral-measure.md) replaces the physical stock drift by $r$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
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
