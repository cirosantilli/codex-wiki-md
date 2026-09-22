# Karush-Kuhn-Tucker conditions

↑ **Parent:** [Mathematical optimization](mathematical-optimization-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Karush-Kuhn-Tucker_conditions)

The [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) combine membership of the [feasible set](feasible-region.md) with a balance of [gradients](gradient.md) and [complementary slackness](complementary-slackness.md). For a [minimization problem](minimization-problem.md) with [differentiable functions](differentiable-function.md) on an [open subset](open-set.md) of $\mathbb R^n$, write

$$
\min_x f(x),\qquad g_i(x)\leq0\ (1\leq i\leq m),\qquad h_j(x)=0\ (1\leq j\leq p),
$$

and use the [optimization Lagrangian](optimization-lagrangian.md)

$$
L(x,\lambda,\mu)=f(x)+\sum_{i=1}^m\lambda_i g_i(x)+\sum_{j=1}^p\mu_j h_j(x).
$$

A candidate $(x_*,\lambda,\mu)$ satisfies the [KKT conditions](karush-kuhn-tucker-conditions.md) exactly when all four requirements hold:
- Primal feasibility: $g_i(x_*)\leq0$ and $h_j(x_*)=0$, so $x_*$ is a [feasible point](feasible-point.md).
- Dual sign feasibility: $\lambda_i\geq0$. The equality [Lagrange multipliers](lagrange-multiplier.md) $\mu_j$ are unrestricted [real numbers](real-number.md).
- Stationarity: the [gradient](gradient.md) of the [optimization Lagrangian](optimization-lagrangian.md) in the decision variables vanishes,$$
  \nabla_x L(x_*,\lambda,\mu)=\nabla f(x_*)+\sum_i\lambda_i\nabla g_i(x_*)+\sum_j\mu_j\nabla h_j(x_*)=0.
  $$
- [Complementary slackness](complementary-slackness.md): $\lambda_i g_i(x_*)=0$ for every inequality [optimization constraint](optimization-constraint.md).[Lecture 7, §L7.1.1, Definition L7.1, printed p. 3: the four KKT requirements](nonlinear-optimization-mit-6-7220-and-15-084-spring-2025/lecture-7-lagrange-multipliers-and-kkt-conditions.md)

The sign of each inequality [Lagrange multiplier](lagrange-multiplier.md) follows the chosen convention $g_i\leq0$: on the [feasible set](feasible-region.md), $\lambda_i g_i\leq0$ makes the [optimization Lagrangian](optimization-lagrangian.md) a lower bound on the [objective function](objective-function.md). An equality contributes zero on the [feasible set](feasible-region.md) for either sign of its [Lagrange multiplier](lagrange-multiplier.md). [Complementary slackness](complementary-slackness.md) says an inequality with $g_i(x_*)<0$ must have $\lambda_i=0$, while $\lambda_i>0$ implies an [active constraint](active-constraint.md). An [active constraint](active-constraint.md) can still have zero [Lagrange multiplier](lagrange-multiplier.md); the [quadratic minimization with a moving upper bound](quadratic-minimization-with-a-moving-upper-bound.md) below gives an explicit example.

The name records [William Karush](william-karush.md)'s 1939 master's thesis and the 1951 work of [Harold W. Kuhn](harold-w-kuhn.md) and [Albert W. Tucker](albert-w-tucker.md).[Chapter 5 bibliography, printed p. 272, and bibliography entries KT51 and Kuh76](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

**Table of contents**

- [KKT regularity at a local minimum](kkt-regularity-at-a-local-minimum.md)
- [Convex KKT optimality certificate](convex-kkt-optimality-certificate.md)
- [Quadratic minimization with a moving upper bound](quadratic-minimization-with-a-moving-upper-bound.md)
- [Shadow price of an inequality constraint](shadow-price-of-an-inequality-constraint.md)
- [Active-set transition in capped resource allocation](active-set-transition-in-capped-resource-allocation.md)

## ↑ Ancestors (4)

1. [Mathematical optimization](mathematical-optimization-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (50)

- [Constraint qualification](constraint-qualification.md)
- [Convex optimization](convex-optimization-split.md)
- [Debiased-Lasso remainder bound](debiased-lasso-remainder-bound.md)
- [Entropy maximization for loss-network occupancy](entropy-maximization-for-loss-network-occupancy.md)
- [Equality slice of a feasible triangle](equality-slice-of-a-feasible-triangle.md)
- [Feasible triangle with a squared-distance objective](feasible-triangle-with-a-squared-distance-objective.md)
- [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md)
- [Lagrangian duality for a quadratic threshold](lagrangian-duality-for-a-quadratic-threshold.md)
- [Lasso sign recovery from cone invertibility](lasso-sign-recovery-from-cone-invertibility.md)
- [Lasso support bound from sparse eigenvalues](lasso-support-bound-from-sparse-eigenvalues.md)
- [Nodewise-Lasso residual identity](nodewise-lasso-residual-identity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/29j/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-39/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-65/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-39/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/21h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/21h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-205/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-205/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-205/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/7h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-205/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-339/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2/7h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-205/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-339/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-205/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-218/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-205/1/solution.md)
- [Prediction inequality from Lasso stationarity](prediction-inequality-from-lasso-stationarity.md)
- [Primal-dual optimal point](primal-dual-optimal-point.md)
- [Soft-margin support vector machine](soft-margin-support-vector-machine.md)
- [Subdifferential of the L1 norm](subdifferential-of-the-l1-norm.md)
- [Support-vector leave-one-out error bound](support-vector-leave-one-out-error-bound.md)
- [Tuning relation between Lasso and square-root Lasso](tuning-relation-between-lasso-and-square-root-lasso.md)
- [User-network decomposition of concave utility maximization](user-network-decomposition-of-concave-utility-maximization.md)
