# Upwind finite difference scheme

↑ **Parent:** [Finite difference method](finite-difference-method.md)

For constant-speed advection $u_t+a u_x=0$ with $a>0$, the explicit upwind scheme uses $U_j^{n+1}=(1-\nu)U_j^n+\nu U_{j-1}^n$, $\nu=ak/h$. For $a<0$ the neighbour must be on the other side. When $0\leq\nu\leq1$, the update is a convex combination and is contractive in the maximum [norm](norm.md) on a periodic grid, or with appropriate controlled inflow data.

On a periodic grid, [von Neumann stability analysis](von-neumann-stability-analysis.md) gives $G=1-\nu+\nu e^{-i\theta}$ and $|G|^2=1-2\nu(1-\nu)(1-\cos\theta)$, proving the same exact contraction range in the discrete [L2 norm](l2-norm.md). Boundary estimates are still required on a finite interval; stable scalar [eigenvalues](eigenvalue.md) of a triangular boundary update alone need not give a mesh-uniform bound.

**Table of contents**

- [Dissipative second-order forward advection stencil](dissipative-second-order-forward-advection-stencil.md)

## ↑ Ancestors (7)

1. [Finite difference method](finite-difference-method.md)
2. [Finite difference](finite-difference-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (10)

- [CFL necessity for explicit Engquist-Osher stability](cfl-necessity-for-explicit-engquist-osher-stability.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/7/solution.md)
