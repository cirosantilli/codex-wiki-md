# Full-weighting restriction

↑ **Parent:** [Multigrid method](multigrid-method.md)

Full-weighting restriction transfers a fine-grid residual to a coarser grid by local averaging. In one dimension its weights are $(1,2,1)/4$; in two dimensions they are the tensor-product stencil $\left(\begin{smallmatrix}1&2&1\\2&4&2\\1&2&1\end{smallmatrix}\right)/16$. For linear or bilinear interpolation $P$ and coarsening by two in every direction, it equals $2^{-d}P^T$ in unweighted coordinates. This scaling makes restriction the adjoint of interpolation for mesh-weighted inner products.

## ↑ Ancestors (6)

1. [Multigrid method](multigrid-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/7/solution.md)
- [Two-grid Poisson factor with weighted Jacobi](two-grid-poisson-factor-with-weighted-jacobi.md)
