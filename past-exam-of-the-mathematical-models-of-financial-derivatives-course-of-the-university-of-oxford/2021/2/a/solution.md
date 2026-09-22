<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [self-financing replicating portfolio](../../../../replicating-strategy.md) for a terminal payoff $F(S_T)$ has the same terminal value on every relevant path, with all earlier rebalancing funded internally. In a [complete market](../../../../complete-market.md) its initial cost is unique under [no-arbitrage](../../../../no-arbitrage.md): otherwise buy the cheaper payoff and sell the more expensive identical payoff.

In the [Black-Scholes model](../../../../black-scholes-model.md), the portfolio holds $V_s$ shares and bond value $V-SV_s$, where $V$ solves the [Black-Scholes equation](../../../../black-scholes-equation.md) with terminal data $F$. [Itô's formula](../../../../ito-s-lemma.md) verifies the [self-financing condition](../../../../self-financing-condition.md). Equivalently,

$$
\boxed{V(t,s)=e^{-r\tau}\mathbb E_{\mathbb Q}[F(S_T)\mid S_t=s],\qquad dS_t=rS_t\,dt+\sigma S_t\,dW_t^{\mathbb Q}.}
$$

This relates [claim replication](../../../../claim-replication.md), the [Black-Scholes equation](../../../../black-scholes-equation.md), and [risk-neutral valuation](../../../../risk-neutral-pricing.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
