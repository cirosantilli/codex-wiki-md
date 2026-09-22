# Midpoint flux stencil for one-dimensional diffusion

↑ **Parent:** [Finite difference method](finite-difference-method.md)

For $u_t=(au_x)_x$, this conservative [finite difference method](finite-difference-method.md) uses coefficient samples at edge midpoints. For smooth $a,u$, its spatial residual is $h^2(au_{xxxx}/12+a'u_{xxx}/6+a''u_{xx}/8+a'''u_x/24)+O(h^4)$. With zero [Dirichlet boundary conditions](dirichlet-boundary-condition.md), $-v^TL_hv=h^{-2}\sum_j a_{j+1/2}(v_{j+1}-v_j)^2$. If $0<a\leq a_+$, its [eigenvalues](eigenvalue.md) lie in $[-4a_+/h^2,0]$, giving the mesh-independent [Forward Euler method](euler-method.md) bound $\Delta t/h^2\leq1/(2a_+)$. Constant $a=a_+$ proves sharpness as the grid is refined.

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/3/a/solution.md)
