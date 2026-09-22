# Ill-conditioning of a logarithmic barrier

↑ **Parent:** [Logarithmic barrier](logarithmic-barrier.md)

Near an [active constraint](active-constraint.md) with limiting [Lagrange multiplier](lagrange-multiplier.md) $\lambda_i^*>0$, a convergent barrier sequence has $c_i(x_k)\sim\mu_k/\lambda_i^*$. Its [Hessian matrix](hessian-matrix.md) therefore contains the term

$$
\frac{\mu_k}{c_i(x_k)^2}\nabla c_i(x_k)\nabla c_i(x_k)^T\sim\frac{(\lambda_i^*)^2}{\mu_k}\nabla c_i(x_*)\nabla c_i(x_*)^T.
$$

For a nonzero constraint [gradient](gradient.md), this gives large curvature in a direction normal to the boundary. If a nonzero common tangent direction retains positive curvature of order one, while the remaining terms stay bounded, the [condition number](condition-number.md) typically grows like $1/\mu_k$. This is a mechanism rather than a universal rate: there may be no tangent direction, all curvatures may grow together, or an [active constraint](active-constraint.md) may have zero limiting [Lagrange multiplier](lagrange-multiplier.md).

## ↑ Ancestors (9)

1. [Logarithmic barrier](logarithmic-barrier.md)
2. [Barrier function](barrier-function.md)
3. [Interior-point method](interior-point-method.md)
4. [Conic optimization](conic-optimization.md)
5. [Convex optimization](convex-optimization-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/3/d/iii/solution.md)
