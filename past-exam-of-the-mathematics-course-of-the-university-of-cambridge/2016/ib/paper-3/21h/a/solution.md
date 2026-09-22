<h1 id="21h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a minimization problem over a domain $D$ with inequality constraints $g_j(x)\leq0$ and equality constraints $h_\ell(x)=0$, let

$$
\mathcal L(x,\lambda,\mu)=f(x)+\sum_j\lambda_jg_j(x)+\sum_\ell\mu_\ell h_\ell(x).
$$

The [Lagrangian sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) states: if $x_*$ is feasible, $\lambda_j\geq0$, $\lambda_jg_j(x_*)=0$, and $x_*$ globally minimizes $\mathcal L(\cdot,\lambda,\mu)$ on $D$, then $x_*$ globally minimizes the constrained objective. Equality multipliers have no sign restriction.

For any feasible $x$, the sign of the inequality multipliers gives $\mathcal L(x,\lambda,\mu)\leq f(x)$. Feasibility and [complementary slackness](../../../../../../complementary-slackness.md) give $\mathcal L(x_*,\lambda,\mu)=f(x_*)$. Therefore

$$
\boxed{f(x_*)=\mathcal L(x_*,\lambda,\mu)
\leq\mathcal L(x,\lambda,\mu)\leq f(x).}
$$

This proves the theorem. No convexity is necessary if the global minimization of the Lagrangian is already known. In a differentiable [convex optimization](../../../../../../convex-optimization-split.md) problem with convex inequalities and affine equalities, a stationary point of this convex Lagrangian is automatically a global minimizer, which gives the familiar sufficiency of the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
