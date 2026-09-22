# Compact semidiscrete nine-point diffusion

↑ **Parent:** [Mehrstellen method](mehrstellen-method.md)

On a square grid, let $C_h$ sum the four axial neighbors and $K_h$ the four diagonal neighbors. With $M_h=2I/3+C_h/12$ and $L_h=(-10I/3+2C_h/3+K_h/6)/h^2$, the [method of lines](method-of-lines.md) has fourth-order normalized spatial [numerical consistency](consistency-of-a-numerical-method.md). Its mass symbol is $(4+\cos\xi+\cos\eta)/6\geq1/3$, and its diffusion symbol is $[-10+4(\cos\xi+\cos\eta)+2\cos\xi\cos\eta]/(3h^2)\leq0$. Every continuous-time mode therefore contracts, and [Parseval identity](parseval-identity.md) gives mesh-independent discrete L2 [stability](stability-of-a-numerical-method.md). No time-step restriction is involved until a time integrator is selected.

## ↑ Ancestors (8)

1. [Mehrstellen method](mehrstellen-method.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/1/a/solution.md)
