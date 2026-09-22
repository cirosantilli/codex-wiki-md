# Monotone half-grid diffusion update

↑ **Parent:** [Symmetric half-grid diffusion consistency](symmetric-half-grid-diffusion-consistency.md)

For $0<a(x)\le\beta$, the explicit conservative diffusion update has weights $ka_{m-1/2}/h^2$, $1-k(a_{m-1/2}+a_{m+1/2})/h^2$, and $ka_{m+1/2}/h^2$. Under the displayed restriction they are nonnegative and sum to one. With zero [Dirichlet boundary conditions](dirichlet-boundary-condition.md), each new value is a [convex combination](convex-combination.md) of old interior and boundary values, proving contraction in the discrete [maximum norm](supremum-norm.md). The spatial [matrix](matrix.md) is also [symmetric](symmetric-relation.md) with $v^TL_hv=-h^{-2}\sum a_{m+1/2}(v_{m+1}-v_m)^2$. This puts its [eigenvalues](eigenvalue.md) in $[-4\beta/h^2,0]$, so the same restriction gives [L2 norm](l2-norm.md) contraction. A stable recurrence need not be consistent with a different proposed differential equation.

## ↑ Ancestors (8)

1. [Symmetric half-grid diffusion consistency](symmetric-half-grid-diffusion-consistency.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/2/b/solution.md)
