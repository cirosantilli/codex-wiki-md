# Cell-average projection

↑ **Parent:** [L2-compatible initialization of grid data](l2-compatible-initialization-of-grid-data.md)

The cell-average projection replaces a function by its average on each grid cell. It is independent of the representative of an [L2 function](square-integrable-function.md), unlike point sampling. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $h|U_m|^2\le\int_{\text{cell }m}|u|^2dx$, hence $h\sum_m|U_m|^2\le\|u\|_{L^2}^2$. Viewed as a piecewise constant function, the projection is the [orthogonal projection](orthogonal-projection.md) onto the grid's piecewise constant [linear subspace](vector-subspace.md). Density of continuous compactly supported functions and the contraction estimate give convergence in the [L2 norm](l2-norm.md) as the mesh tends to zero.

## ↑ Ancestors (8)

1. [L2-compatible initialization of grid data](l2-compatible-initialization-of-grid-data.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/3/b/solution.md)
