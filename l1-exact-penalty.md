# L1 exact penalty

↑ **Parent:** [Constrained optimization](constrained-optimization.md)

An L1 penalty can enforce a constraint exactly at a finite weight, rather than only in an infinite-weight limit. For a convex equality-constrained problem with an optimal multiplier $y_*$ and [optimization Lagrangian](optimization-lagrangian.md) $f-y^Tc$, the lower bound $f(x)-y_*^Tc(x)\geq f(x_*)$ gives

$$
f(x)+\rho\|c(x)\|_1\geq f(x_*)+(\rho-\|y_*\|_\infty)\|c(x)\|_1.
$$

Thus $\rho>\|y_*\|_\infty$ makes every penalty minimizer feasible and optimal. Local versions require appropriate regularity and second-order assumptions. The nonsquared norm is essential to this finite-threshold property; a [quadratic penalty method](quadratic-penalty-method.md) usually approaches feasibility only as its weight diverges.

## ↑ Ancestors (6)

1. [Constrained optimization](constrained-optimization.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/b/5/iv/solution.md)
- [Sl1QP](sl1qp.md)
