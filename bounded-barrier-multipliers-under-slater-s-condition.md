<h1 id="bounded-barrier-multipliers-under-slater-s-condition">Bounded barrier multipliers under Slater's condition</h1>

↑ **Parent:** [Logarithmic barrier](logarithmic-barrier.md)

Let $c_i$ be [concave](concave-function.md) and [continuously differentiable](continuously-differentiable-function.md), and let a strict [feasible point](feasible-point.md) $z$ satisfy $\delta=\min_i c_i(z)>0$. Suppose $x_k\to x_*$, $c_i(x_k)>0$, $\mu_k\to0$, and the [logarithmic barrier](logarithmic-barrier.md) residuals $r_k=\nabla f(x_k)-\sum_i\lambda_{k,i}\nabla c_i(x_k)$ tend to zero, where $\lambda_{k,i}=\mu_k/c_i(x_k)$. By [concavity](concave-function.md),

$$
\delta\|\lambda_k\|_1\leq\sum_i\lambda_{k,i}c_i(z)\leq p\mu_k+(\nabla f(x_k)-r_k)^T(z-x_k).
$$

The right-hand side is bounded when $\nabla f$ is [continuous](continuous-function.md) near $x_*$. Thus the nonnegative [Lagrange multiplier](lagrange-multiplier.md) estimates are bounded. A convergent [subsequence](subsequence.md) gives $\lambda_*\geq0$; passing to the [limit](limit-of-a-function.md) in stationarity and $\lambda_{k,i}c_i(x_k)=\mu_k$ proves the [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) at $x_*$. An inactive [optimization constraint](optimization-constraint.md) has $c_i(x_*)>0$ and hence $\lambda_{k,i}\to0$ even without selecting a [subsequence](subsequence.md). With a [convex](convex-function.md) [objective function](objective-function.md), these conditions certify a [global minimum](global-minimum.md). This result is conditional on the stated residual and primal convergence assumptions; it does not assert that every barrier subproblem has a [minimizer](global-minimizer.md).

## ↑ Ancestors (9)

1. [Logarithmic barrier](logarithmic-barrier.md)
2. [Barrier function](barrier-function.md)
3. [Interior-point method](interior-point-method.md)
4. [Conic optimization](conic-optimization.md)
5. [Convex optimization](convex-optimization-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/3/d/ii/solution.md)
