# Finite-difference option Greeks

↑ **Parent:** [Explicit log-price scheme for local-volatility pricing](explicit-log-price-scheme-for-local-volatility-pricing.md)

The logarithmic coordinate requires the displayed chain-rule factors for [option delta](option-delta.md) and [option gamma](option-gamma.md). If only a value error bound $\|e_h\|_\infty=O(h^2)$ is known, central differentiation gives $D_xe_h=O(h)$ and $D_{xx}e_h=O(1)$. Thus first and second Greek convergence do not follow with the same order from a value bound alone. With a smooth spatial error expansion $e_h=h^2E+o(h^2)$ and corresponding derivative control, both Greeks can instead retain second-order convergence away from a nonsmooth payoff or boundary. Refinement and Greek-specific regularity are essential to distinguish these situations.

## ↑ Ancestors (9)

1. [Explicit log-price scheme for local-volatility pricing](explicit-log-price-scheme-for-local-volatility-pricing.md)
2. [Pricing equation for a local volatility model](pricing-equation-for-a-local-volatility-model.md)
3. [Local volatility model](local-volatility-model.md)
4. [Local volatility](local-volatility.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48/3/f/solution.md)
