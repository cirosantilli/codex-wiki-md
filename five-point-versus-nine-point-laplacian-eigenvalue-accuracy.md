# Five-point versus nine-point Laplacian eigenvalue accuracy

↑ **Parent:** [Nine-point finite-difference stencil](nine-point-finite-difference-stencil.md)

For the [Dirichlet discrete Laplacian](dirichlet-discrete-laplacian.md) on a square, let $T=h^{-2}\operatorname{tridiag}(1,-2,1)$. The standard axial five-point operator is $T\otimes I+I\otimes T$, and the axial-weight $2/3$, corner-weight $1/6$ nine-point operator additionally contains $h^2T\otimes T/6$. Its [eigenvalues](eigenvalue.md) are therefore strictly larger than the five-point values for the same sine modes. Both lie above the corresponding negative continuum [Laplacian](laplacian.md) [eigenvalues](eigenvalue.md), so the five-point operator has smaller spectral error. For fixed mode numbers the leading errors are respectively $\pi^4h^2(k^4+l^4)/12$ and $\pi^4h^2(k^2+l^2)^2/12$.

## ↑ Ancestors (8)

1. [Nine-point finite-difference stencil](nine-point-finite-difference-stencil.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/1/b/solution.md)
