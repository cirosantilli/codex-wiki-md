# Cubic convergence of Newton optimization for an even quartic

↑ **Parent:** [Local quadratic convergence of Newton iteration](local-quadratic-convergence-of-newton-iteration.md)

For the [strictly convex](strictly-convex-function.md) [polynomial](polynomial-split.md) $f(x)=x^2/2+x^4/4$, applying [Newton root-finding iteration](newton-root-finding-iteration.md) to $f'(x)=x+x^3$ gives

$$
x_{k+1}=x_k-\frac{x_k+x_k^3}{1+3x_k^2}=\frac{2x_k^3}{1+3x_k^2}.
$$

The unique [minimum](minimum-of-a-subset-of-a-total-order.md) is at zero. For any sufficiently small nonzero initial point, the errors satisfy $|x_{k+1}|/|x_k|^3\to2$, so the order is cubic, not merely quadratic. This provides a simple counterexample to treating the usual [quadratic convergence](quadratic-convergence.md) theorem as an upper bound on possible orders. In general, the quadratic coefficient for [Newton optimization](newton-root-finding-iteration.md) near a nondegenerate [stationary point](stationary-point.md) is $f^{(3)}(x_*)/(2f''(x_*))$; when it vanishes, a higher order is possible.

## ↑ Ancestors (7)

1. [Local quadratic convergence of Newton iteration](local-quadratic-convergence-of-newton-iteration.md)
2. [Newton root-finding iteration](newton-root-finding-iteration.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
