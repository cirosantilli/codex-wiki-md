# Prolongation operator

↑ **Parent:** [Multigrid method](multigrid-method-split.md)

A prolongation operator transfers a coarse-grid correction to a finer [mesh](finite-element-mesh.md). For nested one-dimensional grids of spacings $2h$ and $h$, linear interpolation sets $(Pe)_{2j}=e_j$ and $(Pe)_{2j+1}=(e_j+e_{j+1})/2$, with zero endpoint values for homogeneous correction boundary conditions. The associated [full-weighting restriction](full-weighting-restriction.md) is $R=P^T/2$, and the [Galerkin coarse-grid operator](galerkin-coarse-grid-operator.md) is $RA_hP$. The correction equation acts on the residual so that a coarse representation of the error can improve the fine-grid approximation.

## ↑ Ancestors (6)

1. [Multigrid method](multigrid-method-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2010/b/4/c/solution.md)
