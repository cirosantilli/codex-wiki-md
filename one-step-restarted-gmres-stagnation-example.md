# One-step restarted GMRES stagnation example

↑ **Parent:** [Generalized minimal residual method](generalized-minimal-residual-method.md)

One step of restarted [GMRES](generalized-minimal-residual-method.md) searches along the current residual. In the displayed nonsingular system, the first residual minimization is $\min_\alpha[(1-\alpha)^2+(1+\alpha)^2]$, whose minimizer is zero. Restarting then repeats the same problem forever and never moves. Unrestarted [GMRES](generalized-minimal-residual-method.md) instead solves exactly at step two, since $b,Ab$ span the entire space. Thus a smaller search-space cost can come at the price of stagnation; nonsingularity alone does not guarantee progress for one-step restarting.

## ↑ Ancestors (9)

1. [Generalized minimal residual method](generalized-minimal-residual-method.md)
2. [Krylov subspace](krylov-subspace.md)
3. [Conjugate gradient method](conjugate-gradient-method.md)
4. [Gradient descent](gradient-descent-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/a/4/c/solution.md)
