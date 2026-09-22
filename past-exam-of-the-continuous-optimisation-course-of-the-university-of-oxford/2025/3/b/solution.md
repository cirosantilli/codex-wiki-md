<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With inequalities written as $c_i\geq0$, use the [optimization Lagrangian](../../../../optimization-lagrangian.md) $L(x,\lambda)=f(x)-\sum_i\lambda_ic_i(x)$. The [Karush-Kuhn-Tucker conditions](../../../../karush-kuhn-tucker-conditions.md) at $(x_*,\lambda_*)$ are

$$
c_i(x_*)\geq0,\quad\lambda_{*,i}\geq0,\quad\lambda_{*,i}c_i(x_*)=0,\quad\nabla f(x_*)=\sum_i\lambda_{*,i}\nabla c_i(x_*).
$$

For any [feasible point](../../../../feasible-point.md) $z$, the first-order inequalities for a [convex function](../../../../convex-function.md) and a [concave function](../../../../concave-function.md) give

$$
\begin{aligned}
f(z)-f(x_*)&\geq\nabla f(x_*)^T(z-x_*)\\
&=\sum_i\lambda_{*,i}\nabla c_i(x_*)^T(z-x_*)\\
&\geq\sum_i\lambda_{*,i}\bigl(c_i(z)-c_i(x_*)\bigr)\\
&=\sum_i\lambda_{*,i}c_i(z)\geq0.
\end{aligned}
$$

The last equality uses [complementary slackness](../../../../complementary-slackness.md). Thus $x_*$ is a [global minimizer](../../../../global-minimizer.md). [Slater's condition](../../../../slater-s-condition.md) is useful for necessity and existence of [Lagrange multipliers](../../../../lagrange-multiplier.md), but is not required for this sufficiency argument once a [KKT point](../../../../kkt-point.md) is supplied.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
