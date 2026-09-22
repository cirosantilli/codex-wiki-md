# Lax-Wendroff advection scheme

↑ **Parent:** [Finite difference method](finite-difference-method.md)

For the [advection equation](transport-equation.md) $u_t+cu_x=0$ on a uniform grid, the Lax-Wendroff update is

$$
 U_j^{n+1}=U_j^n-\frac\nu2(U_{j+1}^n-U_{j-1}^n)+\frac{\nu^2}2(U_{j+1}^n-2U_j^n+U_{j-1}^n),\qquad \nu=c\Delta t/\Delta x.
$$

Its [amplification factor](amplification-factor.md) is $G=1-i\nu\sin\theta+\nu^2(\cos\theta-1)$, with $|G|^2=1-4\nu^2(1-\nu^2)\sin^4(\theta/2)$. Thus [von Neumann stability analysis](von-neumann-stability-analysis.md) on an infinite or periodic grid gives stability for $|\nu|\leq1$. The scheme has second [order of a numerical method](order-of-a-numerical-method.md) for sufficiently smooth solutions; finite-interval [boundary conditions](boundary-condition.md) still need separate treatment.

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/6/solution.md)
