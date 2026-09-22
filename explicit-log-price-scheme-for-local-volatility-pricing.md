# Explicit log-price scheme for local-volatility pricing

↑ **Parent:** [Pricing equation for a local volatility model](pricing-equation-for-a-local-volatility-model.md)

With $x=\log S$ and $u=e^{r(T-t)}V(e^x,t)$, a [local volatility](local-volatility.md) pricing equation becomes the displayed backward equation. [Central finite differences](central-finite-difference.md) and the [explicit Euler method](euler-method.md) give $u_i^{j-1}=u_i^j+k[a_i^jD_{xx}u_i^j+b_i^jD_xu_i^j]$. Nonnegative weights require $k\sigma_i^2/h^2\leq1$ and $|b_i|h\leq\sigma_i^2$. Under these conditions the update is a convex combination, yielding maximum-norm stability. With smooth coefficients, positive diffusion, fixed positive remaining maturity and suitable consistent boundary treatment, its ordinary error is $O(k+h^2)$. Volatility bounds alone do not imply all this regularity or a Greek error expansion.

**Table of contents**

- [Finite-difference option Greeks](finite-difference-option-greeks.md)

## ↑ Ancestors (8)

1. [Pricing equation for a local volatility model](pricing-equation-for-a-local-volatility-model.md)
2. [Local volatility model](local-volatility-model.md)
3. [Local volatility](local-volatility.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48/3/c/solution.md)
- [Trinomial tree](trinomial-tree.md)
