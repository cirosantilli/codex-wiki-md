<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix any admissible pair of [Kantorovich potentials](../../../../../../kantorovich-potential.md) $(u,v)$ and any [transport plan](../../../../../../transport-plan.md) $\pi\in\Pi(\mu,\nu)$. Its [marginal distributions](../../../../../../marginal-distribution.md) give

$$
\int_Xu\,d\mu+\int_Yv\,d\nu
=\int_{X\times Y}(u(x)+v(y))\,d\pi(x,y).
$$

The right side is well defined because $u(x)$ and $v(y)$ are [Lebesgue integrable](../../../../../../lebesgue-integrable-function.md) with respect to $\pi$. Integrating their pointwise feasibility inequality gives

$$
\int_Xu\,d\mu+\int_Yv\,d\nu\leq\int_{X\times Y}c(x,y)\,d\pi(x,y).
$$

Since this holds for every feasible pair and every [transport plan](../../../../../../transport-plan.md),

$$
\boxed{\sup_{(u,v)\in\mathcal A_c}\left(\int u\,d\mu+\int v\,d\nu\right)\leq\inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi).}
$$

This proves the required inequality directly from the transport constraints, without any [convex optimization](../../../../../../convex-optimization-split.md) duality theorem. Whenever the extrema are attained, the supremum and infimum can respectively be written as a maximum and minimum. Even the [Kantorovich duality theorem](../../../../../../kantorovich-duality-theorem.md) is unnecessary for this direction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
