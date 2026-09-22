# Explicit time stepping for bounded reaction diffusion

↑ **Parent:** [Forward Euler diffusion scheme](forward-euler-diffusion-scheme.md)

Let $D_h$ be the scaled [Dirichlet discrete Laplacian](dirichlet-discrete-laplacian.md) and $V_h$ a bounded diagonal reaction matrix. If $0\leq k/h_x^2\leq1/2$, the heat update $H_h=I+kD_h$ is contractive in both the maximum [norm](norm.md) and the mesh-weighted [L2 norm](l2-norm.md). For $\|V_h\|\leq A$,

$$
 \|(H_h+kV_h)^n\|\leq(1+kA)^n\leq e^{Ank}.
$$

This proves finite-time mesh-uniform [stability](stability-of-a-numerical-method.md) without requiring the full update to have nonnegative entries or to be contractive. Negative reaction terms can destroy nonnegativity at the endpoint $k/h_x^2=1/2$, so it is the heat part alone that is treated as a nonnegative contraction.

## ↑ Ancestors (9)

1. [Forward Euler diffusion scheme](forward-euler-diffusion-scheme.md)
2. [von Neumann stability analysis](von-neumann-stability-analysis.md)
3. [Finite difference method](finite-difference-method.md)
4. [Finite difference](finite-difference-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/5/b/solution.md)
