# Trapezoidal contractivity for a semidiscrete heat equation

↑ **Parent:** [Semidiscrete finite element heat equation](semidiscrete-finite-element-heat-equation.md)

If $M$ is symmetric positive definite and $K$ symmetric negative semidefinite, the update $(M-\Delta tK/2)U^{k+1}=(M+\Delta tK/2)U^k$ is uniquely solvable for every positive step. Multiply its difference form by $(U^{k+1}+U^k)^T$ to obtain

$$
\|U^{k+1}\|_M^2-\|U^k\|_M^2
=\frac{\Delta t}2(U^{k+1}+U^k)^TK(U^{k+1}+U^k)\leq0.
$$

For finite element heat flow, the mass norm is precisely the spatial $L^2$ norm, giving unconditional stability of the [Crank-Nicolson method](crank-nicolson-method.md).

## ↑ Ancestors (7)

1. [Semidiscrete finite element heat equation](semidiscrete-finite-element-heat-equation.md)
2. [Finite element method](finite-element-method-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
