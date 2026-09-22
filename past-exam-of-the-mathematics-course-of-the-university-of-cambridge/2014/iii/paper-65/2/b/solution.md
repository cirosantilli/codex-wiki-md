<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $r(u)=\|u-g\|_2^2$ and fix the reference noise budget $\sigma$. Define the [convex perturbation function](../../../../../../convex-perturbation-function.md)

$$
f(u,z)=\operatorname{TV}(u)+\delta_{(-\infty,0]}(r(u)-\sigma-z).
$$

Positive $z$ increases the allowed squared noise level. The feasible epigraph set $r(u)\leq\sigma+z$ is convex and closed, so this is a proper [lower semicontinuous](../../../../../../lower-semicontinuity.md) jointly convex perturbation. Writing the inequality indicator as a supremum over its multiplier gives

$$
\boxed{\inf_u\sup_{\lambda\geq0}L(u,\lambda),\qquad
L(u,\lambda)=\operatorname{TV}(u)+\lambda(r(u)-\sigma).}
$$

The [Lagrange dual function](../../../../../../lagrange-dual-function.md) is $d(\lambda)=\inf_uL(u,\lambda)$ for $\lambda\geq0$. In the signed [convex conjugate](../../../../../../convex-conjugate.md) convention of part (a), $y=-\lambda$; positive $y$ gives dual objective $-\infty$ because the perturbation can be made arbitrarily large.

The feasible ball is nonempty and compact, so [lower semicontinuity](../../../../../../lower-semicontinuity.md) of [total variation](../../../../../../total-variation.md) gives a primal minimizer. For $\sigma>0$, $u=g$ satisfies $r(g)=0<\sigma$, providing the [Slater condition](../../../../../../slater-s-condition.md). Total variation is finite everywhere in the given discretization and hence continuous. [Strong duality](../../../../../../strong-duality.md) and dual attainment give a finite optimal $\lambda^*\geq0$. The pair satisfies the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md)

$$
r(u^*)\leq\sigma,\quad\lambda^*\geq0,\quad
\lambda^*(r(u^*)-\sigma)=0,\quad
0\in\partial\operatorname{TV}(u^*)+2\lambda^*(u^*-g).
$$

Equivalently,

$$
\boxed{L(u^*,\lambda)\leq L(u^*,\lambda^*)\leq L(u,\lambda^*)\quad
\text{for all }u\text{ and }\lambda\geq0.}
$$

Thus the set of saddle points is nonempty. Compactness handles primal attainment, while strict feasibility supplies a finite multiplier; these are distinct steps. An inactive constraint can yield $\lambda^*=0$. At $\sigma=0$, feasibility still forces $u=g$, but this strict-feasibility argument does not apply.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
