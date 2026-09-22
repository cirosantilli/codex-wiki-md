<h1 id="s9/1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume a non-dividend-paying tradable asset follows [geometric Brownian motion](../../../../../geometric-brownian-motion.md) $dS=\mu S\,dt+\sigma S\,dW$, with constant volatility $\sigma$ and risk-free rate $r$. Trading is continuous, frictionless and divisible; borrowing and lending occur at the same rate, short selling is allowed, the strategy is self-financing, and there are no jumps or arbitrage opportunities. These are modelling assumptions, not assertions that market returns are exactly Gaussian or that hedging is costless in practice.

For a smooth option price $V(S,t)$, [Itô's formula](../../../../../ito-s-lemma.md) gives

$$
dV=\left(V_t+\mu S V_S+\tfrac12\sigma^2S^2V_{SS}\right)dt+\sigma S V_S\,dW.
$$

Replicate it by $\Delta$ shares and a cash account of value $b=V-\Delta S$. Self-financing requires $dV=\Delta\,dS+rb\,dt$. Matching the stochastic term fixes $\Delta=V_S$. Matching the remaining drift and cancelling the physical drift $\mu$ then gives

$$
\boxed{V_t+\frac12\sigma^2S^2V_{SS}+rSV_S-rV=0.}
$$

This is the [Black-Scholes equation](../../../../../black-scholes-equation.md). The cancellation does not assert that the actual expected asset return equals $r$; risk-neutral valuation is a consequence of replication under these assumptions.

For a European call, impose $V(S,T)=(S-K)^+$, with $V(0,t)=0$ and $V(S,t)\sim S-Ke^{-r(T-t)}$ for large $S$. Its writer hedges the short option by holding $\Delta=\partial V/\partial S$ shares and investing or borrowing the residual cash $V-\Delta S$, rebalancing as $S$ and time change. In the constant-parameter model $\Delta=N(d_1)$, where $d_1=[\log(S/K)+(r+\sigma^2/2)(T-t)]/[\sigma\sqrt{T-t}]$ and $N$ is the standard normal cumulative distribution. Continuous rebalancing is an ideal limit: transaction costs, discrete trading, jumps and changing volatility create residual hedge risk. Writing the self-financing gains equation explicitly avoids incorrectly adding an unfinanced $S\,d\Delta$ term to the strategy.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [1](../../1.md)
3. [S9](../../../s9.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
