# Barrier method KKT convergence theorem

↑ **Parent:** [Logarithmic barrier](logarithmic-barrier.md)

Suppose strictly feasible stationary points of $f(x)-\mu_k\sum_j\log c_j(x)$ form a bounded sequence. Every cluster point satisfying the [linear independence constraint qualification](linear-independence-constraint-qualification.md) is a [KKT point](kkt-point.md). Inactive multipliers tend to zero. The active gradients near the limit have uniformly bounded dual vectors, so pairing barrier stationarity with those vectors bounds the active multipliers. A convergent multiplier subsequence then gives stationarity, nonnegative multipliers and [complementary slackness](complementary-slackness.md), since $\lambda_{k,j}c_j(x_k)=\mu_k\to0$. A stationarity residual tending to zero is also allowed.

This conclusion is stationarity, not global optimality. If the subproblems are globally minimized and strictly feasible points are dense in the feasible set, any cluster point is instead a global minimizer. Compare each barrier minimum with a fixed strictly feasible point; boundedness near the cluster point bounds $\log c_j(x_k)$ above. Taking the limit gives the objective comparison on strictly feasible points, then continuity and density extend it to all feasible points.

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

- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2009/b/6/c/solution.md)
