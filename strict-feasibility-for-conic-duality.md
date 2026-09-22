# Strict feasibility for conic duality

↑ **Parent:** [Conic dual problem](conic-dual-problem.md)

For a [proper cone](proper-cone.md) $K$, suppose a point satisfies $Ax-b\in\operatorname{int}K$ and $p_*$ is finite. This generalized [Slater condition](slater-s-condition.md) gives [strong duality](strong-duality.md) and attainment of the [conic dual problem](conic-dual-problem.md)'s optimum. It does not by itself assert primal attainment.[§5.9.1, printed p. 265: generalized Slater condition, strong duality and dual attainment](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

The two worked examples have strict primal points: $(u,v)=(2,2)$ has slack $(2,2,1)$ in the interior of the [nonnegative orthant](nonnegative-orthant.md), and $(t,z)=(2,0)$ has slack $(2,1,0)$ in the interior of the [second-order cone](second-order-cone.md). Both optima were already certified by explicit feasible pairs. [Slater's condition](slater-s-condition.md) explains why a matching optimal [dual variable](dual-variable.md) can be expected under these hypotheses; checking a supplied zero-gap pair needs only [weak duality](weak-duality.md).

Changing cone geometry preserves the bound mechanism. For a [positive semidefinite cone](positive-semidefinite-cone.md), the [dual cone](dual-cone.md) pairing is the [Frobenius inner product](frobenius-inner-product.md) of two [matrices](matrix.md). This connects the same certificate idea to [semidefinite programming](semidefinite-programming.md), while the [central path](central-path.md) uses strictly interior primal and dual points to approach vanishing gap.

In 1995, [Lieven Vandenberghe](lieven-vandenberghe.md) and [Stephen Boyd](stephen-boyd.md) presented a primal-dual [interior-point method](interior-point-method.md) for [convex optimization](convex-optimization-split.md) with [matrix](matrix.md) inequalities. Their algorithmic study included exploiting problem structure and allowing incomplete [Conjugate gradient method](conjugate-gradient-method.md) solves within an iteration. This illustrates how the primal-dual viewpoint guides computation as well as checking a final answer.[Publication record and authored abstract: A Primal-Dual Potential Reduction Method for Problems Involving Matrix Inequalities, Mathematical Programming, Series B, 69(1), 205–236 (1995)](a-primal-dual-potential-reduction-method-for-problems-involving-matrix-inequalities-by-lieven-vandenberghe-and-stephen-boyd.md)

## ↑ Ancestors (7)

1. [Conic dual problem](conic-dual-problem.md)
2. [Conic optimization](conic-optimization.md)
3. [Convex optimization](convex-optimization-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
