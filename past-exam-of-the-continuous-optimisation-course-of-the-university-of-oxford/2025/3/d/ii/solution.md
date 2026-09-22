<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A precise conditional convergence statement is: with the smoothness and [convexity](../../../../../convex-function.md) assumptions of the question, a strict [feasible point](../../../../../feasible-point.md), $\mu_k\downarrow0$, and barrier stationarity residuals

$$
r_k=\nabla f(x^k)-\sum_i\lambda_i^k\nabla c_i(x^k)\longrightarrow0,
$$

every convergent sequence of strictly [feasible points](../../../../../feasible-point.md) $x^k\to x_*$ has a [global minimizer](../../../../../global-minimizer.md) as its [limit](../../../../../limit-of-a-function.md). The [Lagrange multiplier](../../../../../lagrange-multiplier.md) estimates are bounded and have a [subsequence](../../../../../subsequence.md) converging to multipliers satisfying the [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md). The theorem does not assert convergence of the primal sequence without further assumptions.

First, [continuity](../../../../../continuous-function.md) gives $c_i(x_*)\geq0$. For an inactive [optimization constraint](../../../../../optimization-constraint.md), $c_i(x_*)>0$, so

$$
\boxed{\lambda_i^k=\mu_k/c_i(x^k)\longrightarrow0}.
$$

For the [active constraints](../../../../../active-constraint.md), the hint permits assuming $\lambda_i^k\to\lambda_i^*$. Combining this with the inactive limits gives $\lambda_*\geq0$, and passage to the [limit](../../../../../limit-of-a-function.md) in the residual equation proves stationarity. Since $\lambda_i^kc_i(x^k)=\mu_k\to0$, [complementary slackness](../../../../../complementary-slackness.md) also holds. All [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md) follow, and part (b) proves global optimality.

The hint's multiplier assumption can in fact be weakened to selecting a [subsequence](../../../../../subsequence.md). To see why the estimates are bounded, choose a strict [feasible point](../../../../../feasible-point.md) $z$ and put $\delta=\min_i c_i(z)>0$. [Concavity](../../../../../concave-function.md) gives

$$
\delta\|\lambda^k\|_1\leq\sum_i\lambda_i^kc_i(z)\leq p\mu_k+(\nabla f(x^k)-r_k)^T(z-x^k).
$$

The right side is bounded because $x^k\to x_*$ and $r_k\to0$. This is the [bounded barrier multipliers under Slater's condition](../../../../../bounded-barrier-multipliers-under-slater-s-condition.md) argument. A convergent multiplier [subsequence](../../../../../subsequence.md) then gives the same [KKT point](../../../../../kkt-point.md), which suffices to prove that the assumed primal [limit](../../../../../limit-of-a-function.md) is globally optimal.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Continuous optimisation course of the University of Oxford](../../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
