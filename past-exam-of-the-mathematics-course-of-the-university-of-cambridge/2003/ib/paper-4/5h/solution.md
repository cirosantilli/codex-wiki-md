<h1 id="5h/solution">Solution</h1>

↑ **Parent:** [5H](../5h.md)

For [constrained optimization](../../../../../constrained-optimization.md) in minimization form, let $x\in X$, $g_i(x)\le0$ and $h_j(x)=0$, and define the [Lagrangian](../../../../../lagrangian.md)

$$
L(x,\lambda,\nu)=f(x)+\sum_i\lambda_i g_i(x)+\sum_j\nu_jh_j(x).
$$

The [Lagrangian sufficiency theorem](../../../../../lagrange-sufficiency-theorem.md) says: if $x_*$ is feasible, $\lambda_i\ge0$, $\lambda_i g_i(x_*)=0$ for every $i$, and $x_*$ minimizes $L(\cdot,\lambda,\nu)$ globally over $X$, then $x_*$ minimizes $f$ over the feasible set. Equality multipliers $\nu_j$ may have either sign.

Indeed, for every feasible $x$,

$$
f(x)\ge L(x,\lambda,\nu)\ge L(x_*,\lambda,\nu)=f(x_*).
$$

The first inequality uses the inequality-multiplier signs and the equality constraints; the last equality uses [complementary slackness](../../../../../complementary-slackness.md). This proves global optimality without assuming [convexity](../../../../../convex-function.md) or differentiability. The maximization version reverses the relevant signs, or follows by replacing $f$ with $-f$.

When $X$ is convex and the Lagrangian is differentiable and convex, the first-order condition $\nabla_xL(x_*)=0$ implies its global minimum, because $L(x)\ge L(x_*)+\nabla L(x_*)\cdot(x-x_*)$. Thus feasible stationarity plus [complementary slackness](../../../../../complementary-slackness.md) is sufficient in that convex setting. Mere stationarity in a general nonconvex problem is not the theorem's global-minimum hypothesis.

## ↑ Ancestors (10)

1. [5H](../5h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
