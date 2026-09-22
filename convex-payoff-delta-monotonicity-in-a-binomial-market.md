# Convex-payoff delta monotonicity in a binomial market

↑ **Parent:** [Replicating portfolio in a binomial market](replicating-portfolio-in-a-binomial-market.md)

A [convex](convex-function.md) terminal payoff has a convex pricing extension in the [binomial market](discrete-time-binomial-market.md), because [risk-neutral pricing](risk-neutral-pricing.md) is a positive weighted sum of rescaled copies of the payoff. Let the stock factors be $u,d$, the riskless gross factor be $R$, and $q=(R-d)/(u-d)$. The [replicating portfolio in a binomial market](replicating-portfolio-in-a-binomial-market.md) satisfies

$$
\Delta_r(s)=\frac{qu}{R}\Delta_{r+1}(us)+\frac{(1-q)d}{R}\Delta_{r+1}(ds).
$$

The weights sum to one. Convexity orders the secant slopes on the adjacent intervals $[d^2s,uds]$ and $[uds,u^2s]$, proving the displayed inequalities. The inequalities need not be strict: an affine payoff has constant stock holding.

## ↑ Ancestors (8)

1. [Replicating portfolio in a binomial market](replicating-portfolio-in-a-binomial-market.md)
2. [Discrete-time binomial market](discrete-time-binomial-market.md)
3. [Binomial options pricing model](binomial-options-pricing-model.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/2/solution.md)
