<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

The [Lagrange sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) says that for a convex differentiable objective and convex differentiable inequality constraints, any feasible point satisfying the [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) with nonnegative multipliers is a global minimizer.

Write

$$
f=-x_1-3x_2,\qquad
g_1=x_1^2+x_2^2-25,\qquad
g_2=-x_1+2x_2-5.
$$

The unconstrained maximizer of $x_1+3x_2$ on the disc violates $g_2\leq0$, so both boundaries are active at the optimum. Their intersections are

$$
(-5,0)\quad\text{and}\quad(3,4),
$$

and $(3,4)$ gives the smaller objective.

To certify it, at $x_*=(3,4)$ choose

$$
\lambda=\frac14,\qquad\mu=\frac12.
$$

Then

$$
\nabla f(x_*)+\lambda\nabla g_1(x_*)
+\mu\nabla g_2(x_*)=0,
$$

both multipliers are nonnegative, and complementary slackness holds because both constraints are active. The sufficiency theorem therefore gives

$$
\boxed{x_1=3,\qquad x_2=4,\qquad f_{\min}=-15}.
$$

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
