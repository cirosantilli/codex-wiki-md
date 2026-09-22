<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [Lagrange multipliers](../../../../../lagrange-multiplier.md) $\alpha_i\geq0$ for $1-\xi_i-y_i(w\cdot x_i+b)\leq0$ and $\mu_i\geq0$ for $-\xi_i\leq0$. The [optimization Lagrangian](../../../../../optimization-lagrangian.md) is

$$
L(w,b,\xi;\alpha,\mu)
=\frac12\|w\|^2+C\sum_i\xi_i^2
+\sum_i\alpha_i\bigl(1-\xi_i-y_i(w\cdot x_i+b)\bigr)-\sum_i\mu_i\xi_i.
$$

The [Lagrange dual function](../../../../../lagrange-dual-function.md) is the infimum over the now unconstrained primal variables. The [first-order optimality conditions](../../../../../first-order-optimality-condition.md) in $w$ and $b$ give

$$
w=\sum_i\alpha_i y_ix_i,\qquad\sum_i\alpha_i y_i=0.
$$

If the latter equality fails, the infimum over $b$ is $-\infty$. The [first-order optimality condition](../../../../../first-order-optimality-condition.md) in $\xi_i$ gives

$$
2C\xi_i-\alpha_i-\mu_i=0,\qquad\xi_i=\frac{\alpha_i+\mu_i}{2C}.
$$

Substitution, or completing the square separately in $w$ and each $\xi_i$, produces

$$
g(\alpha,\mu)=\sum_i\alpha_i
-\frac12\sum_{i,j}\alpha_i\alpha_jy_iy_j(x_i\cdot x_j)
-\frac1{4C}\sum_i(\alpha_i+\mu_i)^2,
$$

provided $\sum_i\alpha_iy_i=0$. For fixed nonnegative $\alpha_i$, this expression is maximized over $\mu_i\geq0$ at $\mu_i=0$. Thus the simplest [Lagrangian dual problem](../../../../../lagrangian-dual-problem.md) is

$$
\boxed{\begin{aligned}
\underset{\alpha\in\mathbb R^m}{\operatorname{maximize}}\quad&
\sum_i\alpha_i-\frac12\sum_{i,j}\alpha_i\alpha_jy_iy_j(x_i\cdot x_j)-\frac1{4C}\sum_i\alpha_i^2,\\
\text{subject to}\quad&\alpha_i\geq0,\qquad\sum_i\alpha_i y_i=0.
\end{aligned}}
$$

In particular, **there is no upper box constraint $\alpha_i\leq C$**. That constraint belongs to the linear-slack penalty; squared slack instead contributes the displayed diagonal quadratic penalty. With $Y=\operatorname{diag}(y_1,\ldots,y_m)$ and [Gram matrix](../../../../../gram-matrix.md) $G_{ij}=x_i\cdot x_j$, the objective can also be written

$$
\mathbf1^T\alpha-\frac12\alpha^T\left(YGY+\frac1{2C}I\right)\alpha.
$$

Since $G$ is [positive semidefinite](../../../../../positive-semidefinite-matrix.md) and $C>0$, the matrix in parentheses is [positive-definite](../../../../../positive-definite-bilinear-form.md). The objective of the [Lagrangian dual problem](../../../../../lagrangian-dual-problem.md) is therefore strictly concave, and the feasible maximizer is unique.

The [primal problem](../../../../../primal-problem.md) is a [convex optimization](../../../../../convex-optimization-split.md) problem, and $w=0,b=0,\xi_i=2$ is strictly feasible for both families of inequalities. [Slater's condition](../../../../../slater-s-condition.md) gives [strong duality](../../../../../strong-duality.md), so an optimum of the [Lagrangian dual problem](../../../../../lagrangian-dual-problem.md) yields a primal optimum. The [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) supply

$$
\xi_i=\frac{\alpha_i}{2C},\qquad
\alpha_i\bigl(1-\xi_i-y_i(w\cdot x_i+b)\bigr)=0.
$$

For any $i$ with $\alpha_i>0$, the intercept is consequently

$$
\boxed{b=y_i\left(1-\frac{\alpha_i}{2C}\right)-w\cdot x_i.}
$$

All such choices agree at an exact optimum. If all labels have one sign, the optimal coefficients can all be zero: choose $w=0$, $\xi=0$, and any constant intercept of that sign with magnitude at least one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Computational learning theory](../../../computational-learning-theory-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
