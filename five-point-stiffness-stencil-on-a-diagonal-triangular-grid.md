# Five-point stiffness stencil on a diagonal triangular grid

↑ **Parent:** [Stiffness matrix](stiffness-matrix.md)

For conforming piecewise affine elements on uniform squares split along their positive diagonals, a lower-triangle element matrix is $\frac12[[1,-1,0],[-1,2,-1],[0,-1,1]]$ in consecutive vertex order. [Finite element assembly](finite-element-assembly.md) gives diagonal entry 4 and four axis-neighbor entries $-1$. The diagonal mesh edges contribute zero coupling because the corresponding local shape-function gradients are perpendicular. Strong Dirichlet elimination removes known-neighbor columns and adjusts the load.

## ↑ Ancestors (7)

1. [Stiffness matrix](stiffness-matrix.md)
2. [Finite element method](finite-element-method-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
