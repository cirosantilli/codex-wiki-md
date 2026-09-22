# Compact fourth-order Helmholtz stencil

↑ **Parent:** [Nine-point finite-difference stencil](nine-point-finite-difference-stencil.md)

Let $\Gamma_9$ have center weight $-10/3$, axial weights $2/3$ and diagonal weights $1/6$, and let $M_h$ have center weight $2/3$ and axial weights $1/12$. [Taylor expansion](taylor-expansion.md) gives $h^{-2}\Gamma_9u=\Delta u+h^2\Delta^2u/12+O(h^4)$ and $M_hu=u+h^2\Delta u/12+O(h^4)$. On a smooth solution of the constant-coefficient [Helmholtz equation](helmholtz-equation.md), the second-order term becomes $h^2\Delta(\Delta u+\lambda u)/12=0$. Thus the normalized PDE residual is fourth order, while the original unscaled stencil residual is sixth order. This local cancellation alone does not prove uniform global accuracy at or near a resonance.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/5/c/solution.md)
