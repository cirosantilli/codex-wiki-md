# Logarithmic barrier

↑ **Parent:** [Barrier function](barrier-function.md)

For [optimization constraints](optimization-constraint.md) $c_i(x)\geq0$ and $\mu>0$, the [logarithmic barrier](logarithmic-barrier.md) objective is $f_\mu(x)=f(x)-\mu\sum_i\log c_i(x)$ on $D=\{x:c_i(x)>0\ \forall i\}$. Its derivatives are defined only on this strictly feasible [open subset](open-set.md). One may extend its value to $+\infty$ off $D$ to formulate an extended-real [convex function](convex-function.md). The penalty alone is $-\sum_i\log c_i$, while $f_\mu$ includes the original [objective function](objective-function.md).

When $f$ is [convex](convex-function.md) and each $c_i$ is [concave](concave-function.md), $D$ is a [convex set](convex-set-split.md) and

$$
\nabla f_\mu=\nabla f-\sum_i\frac{\mu}{c_i}\nabla c_i,\qquad
\nabla^2f_\mu=\nabla^2f-\sum_i\frac{\mu}{c_i}\nabla^2c_i+\sum_i\frac{\mu}{c_i^2}\nabla c_i\nabla c_i^T.
$$

Every term of this [Hessian matrix](hessian-matrix.md) is a [positive semidefinite matrix](positive-semidefinite-matrix.md), so $f_\mu$ is [convex](convex-function.md). Its [critical point](critical-point.md) satisfies the stationarity part of the [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) with estimates $\lambda_i=\mu/c_i(x)>0$ and perturbed [complementary slackness](complementary-slackness.md) $\lambda_ic_i(x)=\mu$.

**Table of contents**

- [Quadratic-ball barrier eigenvalue branch](quadratic-ball-barrier-eigenvalue-branch.md)
- [Barrier method KKT convergence theorem](barrier-method-kkt-convergence-theorem.md)
- [Bounded barrier multipliers under Slater's condition](bounded-barrier-multipliers-under-slater-s-condition.md)
- [Ill-conditioning of a logarithmic barrier](ill-conditioning-of-a-logarithmic-barrier.md)

## ↑ Ancestors (8)

1. [Barrier function](barrier-function.md)
2. [Interior-point method](interior-point-method.md)
3. [Conic optimization](conic-optimization.md)
4. [Convex optimization](convex-optimization-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Barrier function](barrier-function.md)
- [Bounded barrier multipliers under Slater's condition](bounded-barrier-multipliers-under-slater-s-condition.md)
- [Logarithmic barrier](logarithmic-barrier.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/3/c/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/3/d/i/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/8/iii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2009/b/6/c/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/b/6/ii/solution.md)
- [Penalty method](penalty-method.md)
