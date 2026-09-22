<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the smooth claim value as $V(t,S)$. [Itô's formula](../../../../../ito-s-lemma.md) gives

$$
dV=\left(V_t+\mu SV_S+\tfrac12\sigma^2S^2V_{SS}\right)dt
+\sigma SV_S\,dW.
$$

A replicating [self-financing strategy](../../../../../self-financing-portfolio.md) with stock holding $\Delta=V_S$ and bank value $V-SV_S$ has gains

$$
dV=V_S\,dS+r(V-SV_S)dt.
$$

The Brownian terms then agree. Equating the drift terms cancels $\mu SV_S$ and gives

$$
\boxed{V_t+\tfrac12\sigma^2S^2V_{SS}+rSV_S-rV=0,
\qquad V(T,S)=\Psi(S).}
$$

The terminal condition enforces replication of the [contingent claim payoff](../../../../../contingent-claim-payoff.md). Subject to the usual admissibility and growth conditions for the replicating price, this is the [Black-Scholes equation](../../../../../black-scholes-equation.md). Its [independence](../../../../../independent-random-variables.md) of the physical drift is a consequence of hedge cancellation, not an assumption that the drift equals the risk-free rate.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
