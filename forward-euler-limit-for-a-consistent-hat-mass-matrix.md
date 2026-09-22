# Forward Euler limit for a consistent hat mass matrix

↑ **Parent:** [Semidiscrete finite element heat equation](semidiscrete-finite-element-heat-equation.md)

For a uniform piecewise-linear Galerkin heat discretization, the consistent [mass matrix](mass-matrix.md) is $M=(h/6)\operatorname{tridiag}(1,4,1)$ and the [stiffness matrix](stiffness-matrix.md) is $K=h^{-1}\operatorname{tridiag}(-1,2,-1)$. The generalized [eigenvalues](eigenvalue.md) are $6(1-\cos\theta)/[h^2(2+\cos\theta)]$. Applying [Forward Euler method](euler-method.md) requires $k\lambda\leq2$, giving the displayed uniform bound for $\mu=k/h^2$. For $J$ intervals with Dirichlet endpoints the exact finite-grid upper bound is $(2-\cos(\pi/J))/[3(1+\cos(\pi/J))]$, which approaches $1/6$. Replacing the consistent [mass matrix](mass-matrix.md) by a lumped one changes the [stability](stability-of-a-numerical-method.md) restriction.

## ↑ Ancestors (7)

1. [Semidiscrete finite element heat equation](semidiscrete-finite-element-heat-equation.md)
2. [Finite element method](finite-element-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/5/b/solution.md)
