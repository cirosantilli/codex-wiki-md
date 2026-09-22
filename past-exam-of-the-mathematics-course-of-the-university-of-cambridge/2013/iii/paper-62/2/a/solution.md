<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the maximizing-dual convention. For the [perturbation function](../../../../../../perturbation-function.md) $f(x,u)$, define

$$
\boxed{\varphi(x)=f(x,0),\qquad
\psi(y)=-f^*(0,y),\qquad
p(u)=\inf_x f(x,u),\qquad
q(v)=\sup_y[-f^*(v,y)].}
$$

The [primal problem](../../../../../../primal-problem.md) is $\inf_x\varphi(x)=p(0)$; the [Lagrangian dual problem](../../../../../../lagrangian-dual-problem.md) is $\sup_y\psi(y)=q(0)$. The sign convention makes the dual marginal $q$ concave for jointly convex data; some formulations negate $q$ to express a minimization problem.

The central [convex perturbation duality](../../../../../../convex-perturbation-duality.md) calculation is

$$
p^*(y)=\sup_{u,x}\{\langle y,u\rangle-f(x,u)\}=f^*(0,y),
\qquad
q(0)=p^{**}(0)\leq p(0).
$$

The last inequality is [weak duality](../../../../../../weak-duality.md). A sufficient finite-dimensional condition for [strong duality](../../../../../../strong-duality.md) with dual attainment is: $f$ is jointly proper and convex, $p$ is proper with $p(0)$ finite, and $p$ is finite on a neighborhood of zero. More generally $0\in\operatorname{ri}(\operatorname{dom}p)$ suffices.

Indeed [continuity of a convex function](../../../../../../continuity-of-a-convex-function.md) on the interior of its domain gives a supporting [subgradient](../../../../../../subgradient.md) $y_*\in\partial p(0)$, so

$$
p(u)\geq p(0)+\langle y_*,u\rangle
\quad\Longrightarrow\quad
p^*(y_*)=-p(0).
$$

Therefore $\psi(y_*)=p(0)$ and the dual maximum is attained. **This qualification establishes equality and dual attainment; it does not by itself establish a primal minimizer.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
