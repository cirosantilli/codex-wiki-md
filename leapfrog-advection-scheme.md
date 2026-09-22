# Leapfrog advection scheme

↑ **Parent:** [Amplification polynomial of a multilevel finite difference scheme](amplification-polynomial-of-a-multilevel-finite-difference-scheme.md)

Centered space and leapfrog time discretization of $u_t+cu_x=0$ gives

$$
u_j^{n+1}=u_j^{n-1}-\nu(u_{j+1}^n-u_{j-1}^n),
\qquad \nu=c\Delta t/\Delta x.
$$

Its amplification polynomial is $G^2+2i\nu\sin\theta\,G-1$. The two roots have unit modulus for $|\nu\sin\theta|\leq1$, but a repeated unit root at equality violates the uniform root condition.

**Table of contents**

- [Two-dimensional leapfrog stability threshold](two-dimensional-leapfrog-stability-threshold.md)
- [Two-level stability at the leapfrog Courant boundary](two-level-stability-at-the-leapfrog-courant-boundary.md)

## ↑ Ancestors (9)

1. [Amplification polynomial of a multilevel finite difference scheme](amplification-polynomial-of-a-multilevel-finite-difference-scheme.md)
2. [von Neumann stability analysis](von-neumann-stability-analysis.md)
3. [Finite difference method](finite-difference-method.md)
4. [Finite difference](finite-difference-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/38c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/38c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/40e/c/solution.md)
