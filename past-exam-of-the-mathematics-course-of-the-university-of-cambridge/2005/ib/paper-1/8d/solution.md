<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

Associate free real [dual variables](../../../../../dual-variable.md) $u_i$ and $v_j$ with the row and column equality constraints. The [Lagrangian](../../../../../lagrangian.md) for the [transportation problem](../../../../../transportation-problem.md) is

$$
L(x,u,v)=\sum_i a_i u_i+\sum_j b_jv_j
+\sum_{i,j}(c_{ij}-u_i-v_j)x_{ij}.
$$

Its infimum over $x_{ij}\ge0$ is finite exactly when $u_i+v_j\le c_{ij}$ for every pair. The [linear programming duality](../../../../../linear-programming-duality.md) therefore gives

$$
\boxed{\text{maximize }\sum_i a_i u_i+\sum_j b_jv_j
\quad\text{subject to }u_i+v_j\le c_{ij},\quad u_i,v_j\in\mathbb R}.
$$

The [dual variables](../../../../../dual-variable.md) have no sign restrictions because the primal constraints are equalities.

A feasible shipment $x$ is optimal if and only if there exist feasible [transportation dual potentials](../../../../../transportation-dual-potentials.md) satisfying [complementary slackness](../../../../../complementary-slackness.md):

$$
\boxed{x_{ij}(c_{ij}-u_i-v_j)=0\quad\text{for every }i,j}.
$$

Thus every occupied route must have $u_i+v_j=c_{ij}$. To see sufficiency explicitly, the primal minus dual objective is

$$
\sum_{i,j}x_{ij}(c_{ij}-u_i-v_j)\ge0,
$$

and [complementary slackness](../../../../../complementary-slackness.md) makes it zero. This is the [weak duality](../../../../../weak-duality.md) certificate. Necessity follows from [strong duality](../../../../../strong-duality.md) for the feasible, bounded [linear program](../../../../../linear-programming.md). If the total supply $M$ is positive, $x_{ij}=a_i b_j/M$ gives feasibility; if $M=0$, $x=0$ does. The feasible shipments form a closed bounded set, so the primal optimum is attained. This also covers zero supplies and demands. The one redundant equality merely leaves the dual gauge freedom $(u,v)\mapsto(u+t,v-t)$.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
