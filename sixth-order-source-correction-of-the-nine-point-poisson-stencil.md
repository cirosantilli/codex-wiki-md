# Sixth-order source correction of the nine-point Poisson stencil

↑ **Parent:** [Fourth-order correction of the nine-point Poisson stencil](fourth-order-correction-of-the-nine-point-poisson-stencil.md)

The [nine-point finite-difference stencil](nine-point-finite-difference-stencil.md) for the [Laplacian](laplacian.md) has expansion $D_9u=\Delta u+h^2\Delta^2u/12+h^4(u_{xxxxxx}+u_{yyyyyy}+5u_{xxxxyy}+5u_{xxyyyy})/360+O(h^6)$. If $\Delta u=f$, differentiating this equation gives $u_{xxxxyy}+u_{xxyyyy}=f_{xxyy}$ and $u_{xxxxxx}+u_{yyyyyy}=\Delta^2f-3f_{xxyy}$. Hence the corrected compact equation

$$
D_9U=f+\frac{h^2}{12}\Delta f+\frac{h^4}{360}(f_{xxxx}+4f_{xxyy}+f_{yyyy})
$$

has sixth-order normalized [consistency of a numerical method](consistency-of-a-numerical-method.md). Source [derivatives](derivative.md) can be supplied analytically; numerical approximation of $\Delta f$ must be fourth order and of the fourth [derivatives](derivative.md) second order. With exact square-grid [Dirichlet boundary data](dirichlet-boundary-data.md) and uniformly smooth solution, the [discrete maximum principle](discrete-maximum-principle.md) inverse bound converts this residual into sixth-order nodal convergence. The unknown stencil stays compact even if more distant known source values are used.

## ↑ Ancestors (9)

1. [Fourth-order correction of the nine-point Poisson stencil](fourth-order-correction-of-the-nine-point-poisson-stencil.md)
2. [Nine-point finite-difference stencil](nine-point-finite-difference-stencil.md)
3. [Finite difference method](finite-difference-method.md)
4. [Finite difference](finite-difference-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/7/solution.md)
