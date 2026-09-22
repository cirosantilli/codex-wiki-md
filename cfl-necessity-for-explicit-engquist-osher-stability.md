# CFL necessity for explicit Engquist-Osher stability

↑ **Parent:** [Engquist-Osher method](engquist-osher-method.md)

[Monotonicity](monotonic-function.md) of the explicit update requires $(k/h)\sup_{[m,M]}|f'|\le1$ on its invariant state interval. [Convexity](convex-function.md) and a unique [sonic point of a scalar flux](sonic-point-of-a-scalar-flux.md) do not remove this time-step restriction. For $f(u)=u^2/2$, linearization about a positive constant $U$ gives an [upwind finite difference scheme](upwind-finite-difference-scheme.md) for [advection equation](transport-equation.md): $v_j^{n+1}=(1-rU)v_j^n+rUv_{j-1}^n$, where $r=k/h$. At [Fourier frequency](fourier-frequency.md) $\pi$ the multiplier is $1-2rU$, whose modulus exceeds one when $rU>1$. Thus a [CFL condition](courant-friedrichs-lewy-condition.md) is essential to the claimed nonlinear [stability](stability-of-a-numerical-method.md).

## ↑ Ancestors (8)

1. [Engquist-Osher method](engquist-osher-method.md)
2. [Monotone conservative scheme](monotone-conservative-scheme.md)
3. [Finite volume method](finite-volume-method.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/6/solution.md)
