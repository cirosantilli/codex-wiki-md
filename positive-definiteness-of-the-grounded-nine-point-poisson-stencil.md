# Positive definiteness of the grounded nine-point Poisson stencil

↑ **Parent:** [Finite difference method](finite-difference-method.md)

On a rectangular grid with zero [Dirichlet boundary conditions](dirichlet-boundary-condition.md), the nine-point [Poisson equation](poisson-equation.md) matrix has diagonal $10/3$, axial off-diagonal entries $-2/3$, and diagonal-neighbor entries $-1/6$. Its [quadratic form](quadratic-form.md) is the sum of squared differences over internal links, weighted by $2/3$ or $1/6$, plus the weighted squares of values linked to the fixed zero boundary. The connected axial grid forces a zero [quadratic form](quadratic-form.md) to have all entries zero. This proves [positive-definite matrix](positive-definite-matrix.md) in every ordering. The [Jacobi method](jacobi-method.md) converges because its nonnegative iteration matrix has row sums at most one, with a strict deficit at boundary-adjacent vertices; a hypothetical unit-modulus eigenvector would propagate its maximum modulus to such a deficit row, which is impossible.

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
