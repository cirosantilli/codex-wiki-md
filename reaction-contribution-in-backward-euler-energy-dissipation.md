# Reaction contribution in backward Euler energy dissipation

↑ **Parent:** [Reaction-diffusion finite element matrix](reaction-diffusion-finite-element-matrix.md)

For $u_t-u_{xx}+u=0$ with homogeneous mixed Dirichlet and [Neumann boundary conditions](neumann-boundary-condition.md), testing the [Backward Euler method](backward-euler-method.md) [finite element](finite-element.md) equation with the new solution gives the displayed identity. Both the squared [derivative](derivative.md) [norm](norm.md) and the squared function [norm](norm.md) are required in the dissipation, because diffusion and reaction contribute separately. Replacing the full $H^1$ [norm](norm.md) by its seminorm omits the reaction term. Positivity gives unconditional decay of the $L^2$ [norm](norm.md).

## ↑ Ancestors (8)

1. [Reaction-diffusion finite element matrix](reaction-diffusion-finite-element-matrix.md)
2. [Stiffness matrix](stiffness-matrix.md)
3. [Finite element method](finite-element-method-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
