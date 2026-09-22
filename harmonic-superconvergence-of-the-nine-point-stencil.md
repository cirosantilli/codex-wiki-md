# Harmonic superconvergence of the nine-point stencil

↑ **Parent:** [Nine-point finite-difference stencil](nine-point-finite-difference-stencil.md)

For the square-grid [nine-point finite-difference stencil](nine-point-finite-difference-stencil.md) for the [Laplacian](laplacian.md),

$$
D_9u=\Delta u+\frac{h^2}{12}\Delta^2u+\frac{h^4}{360}(u_{xxxxxx}+u_{yyyyyy}+5u_{xxxxyy}+5u_{xxyyyy})+O(h^6).
$$

If $\Delta u=0$, both displayed correction terms vanish: the mixed sixth [derivatives](derivative.md) sum to $\Delta u_{xxyy}=0$, and the pure sixth [derivatives](derivative.md) sum to the negative of that sum. Expanding two orders further yields $D_9u=h^6u_{xxxxxxxx}/3024+O(h^8)$ for a smooth [harmonic function](harmonic-function.md). Thus the compact harmonic scheme has sixth-order normalized [consistency of a numerical method](consistency-of-a-numerical-method.md) and, with the [discrete maximum principle](discrete-maximum-principle.md) inverse bound, sixth-order nodal convergence on a square with exact smooth [Dirichlet boundary data](dirichlet-boundary-data.md). For example $\operatorname{Re}(x+iy)^8$ shows that the sixth-order term need not vanish.

## ↑ Ancestors (8)

1. [Nine-point finite-difference stencil](nine-point-finite-difference-stencil.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/7/solution.md)
