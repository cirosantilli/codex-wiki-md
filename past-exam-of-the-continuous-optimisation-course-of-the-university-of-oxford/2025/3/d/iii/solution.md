<h1 id="3/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For an [active constraint](../../../../../active-constraint.md) with $\lambda_i^*>0$, the perturbed [complementary slackness](../../../../../complementary-slackness.md) equation gives $c_i(x^k)\sim\mu_k/\lambda_i^*$. The [Hessian matrix](../../../../../hessian-matrix.md) from part (c) therefore includes

$$
\frac{\mu_k}{c_i(x^k)^2}\nabla c_i(x^k)\nabla c_i(x^k)^T\sim\frac{(\lambda_i^*)^2}{\mu_k}\nabla c_i(x_*)\nabla c_i(x_*)^T.
$$

If $\nabla c_i(x_*)\ne0$, curvature normal to that boundary grows like $1/\mu_k$. By contrast, a direction tangent to every [active constraint](../../../../../active-constraint.md) annihilates these large normal [outer products](../../../../../outer-product.md) at the limiting point, and its curvature may remain of order one. A large spread of [eigenvalues](../../../../../eigenvalue.md) then makes the Newton linear system poorly conditioned. Under bounded remaining curvature and a positive bounded tangential curvature, the [condition number](../../../../../condition-number.md) typically grows like $1/\mu_k$; this is the usual [ill-conditioning of a logarithmic barrier](../../../../../ill-conditioning-of-a-logarithmic-barrier.md).

It is not a universal rate: there may be no nonzero common tangent direction, some limiting [Lagrange multipliers](../../../../../lagrange-multiplier.md) may vanish, or all curvatures may grow together. The [Hessian](../../../../../hessian-matrix.md) formula identifies the source of the difficulty without assuming these extra nondegeneracy conditions.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Continuous optimisation course of the University of Oxford](../../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
