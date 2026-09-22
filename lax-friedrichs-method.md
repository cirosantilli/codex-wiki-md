# Lax-Friedrichs method

↑ **Parent:** [Finite difference method](finite-difference-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lax–Friedrichs_method)

For $u_t+cu_x=0$ on a uniform grid, the update $U_m^{n+1}=(U_{m-1}^n+U_{m+1}^n)/2-\nu(U_{m+1}^n-U_{m-1}^n)/2$ has symbol $\cos\theta-i\nu\sin\theta$, where $\nu=c\Delta t/h$. Its squared modulus is $1+(\nu^2-1)\sin^2\theta$, giving contraction exactly for $|\nu|\leq1$. Stability is separate from the dissipative and dispersive approximation errors.

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
