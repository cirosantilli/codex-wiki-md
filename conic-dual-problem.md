# Conic dual problem

↑ **Parent:** [Conic optimization](conic-optimization.md)

A [conic dual problem](conic-dual-problem.md) searches for a lower bound on a [conic optimization](conic-optimization.md) problem. A [feasible point](feasible-point.md) exhibits an attainable cost; a feasible [dual variable](dual-variable.md) explains why every allowed decision costs at least a specified amount. If the two costs agree, the pair certifies a [global minimum](global-minimum.md) without relying on how the points were found.

Fix a real [matrix](matrix.md) $A\in\mathbb R^{m\times n}$, [vectors](vector.md) $b\in\mathbb R^m$, $c\in\mathbb R^n$, and a [closed convex cone](closed-convex-cone.md) $K\subseteq\mathbb R^m$. With unrestricted $x\in\mathbb R^n$, use the convention

$$
p_* = \inf\{c^Tx:Ax-b\in K\},\qquad
d_* = \sup\{b^Ty:A^Ty=c,\ y\in K^*\},
$$

where the [dual cone](dual-cone.md) is $K^*=\{y:y^Ts\geq0\text{ for every }s\in K\}$. The [conic dual problem](conic-dual-problem.md) uses $K^*$ because it must turn every allowed [slack variable](slack-variable.md) $s=Ax-b$ into a nonnegative [dot product](dot-product.md). Taking $K=\mathbb R_+^m$ gives componentwise [linear inequalities](linear-inequality.md); taking a [second-order cone](second-order-cone.md) gives a [Euclidean norm](euclidean-norm.md) constraint. A [self-dual cone](self-dual-cone.md) has $K^*=K$, but this equality does not guarantee a [feasible point](feasible-point.md) or [strong duality](strong-duality.md).

The [Lagrangian](lagrangian.md) supplies a short derivation. For $y\in K^*$,

$$
L(x,y)=c^Tx-y^T(Ax-b)=(c-A^Ty)^Tx+b^Ty.
$$

Its [infimum](infimum.md) over unrestricted $x$ is $b^Ty$ when $A^Ty=c$, and $-\infty$ otherwise. Maximizing the resulting [Lagrange dual function](lagrange-dual-function.md) gives the stated [conic dual problem](conic-dual-problem.md). The minus sign matches the convention $Ax-b\in K$.

**Table of contents**

- [Nonnegative-orthant optimality certificate](nonnegative-orthant-optimality-certificate.md)
- [Second-order-cone optimality certificate](second-order-cone-optimality-certificate.md)
- [Conic primal-dual gap](conic-primal-dual-gap.md)
- [Strict feasibility for conic duality](strict-feasibility-for-conic-duality.md)

## ↑ Ancestors (6)

1. [Conic optimization](conic-optimization.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Conic dual problem](conic-dual-problem.md)
- [Nonnegative-orthant optimality certificate](nonnegative-orthant-optimality-certificate.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-62/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/4/a/solution.md)
- [Strict feasibility for conic duality](strict-feasibility-for-conic-duality.md)
