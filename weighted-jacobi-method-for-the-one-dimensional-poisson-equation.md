# Weighted Jacobi method for the one-dimensional Poisson equation

↑ **Parent:** [Weighted Jacobi method](weighted-jacobi-method.md)

For the centered second-difference matrix with diagonal $-2$ and off-diagonals $1$, the weighted-Jacobi eigenvalues are

$$
\lambda_k(\omega)
=1-\omega+\omega\cos\frac{k\pi}{n+1},
\qquad 1\leq k\leq n.
$$

The method converges for every grid size exactly when $0<\omega\leq1$.

Multiplying both $A$ and $b$ by $-1$ leaves $D^{-1}A$ and the [weighted Jacobi method](weighted-jacobi-method.md) unchanged. Thus the same formula applies to the positive second-difference [matrix](matrix.md) $T_n$ with diagonal $2$ and neighboring entries $-1$, the [finite difference](finite-difference-split.md) form of the one-dimensional [Poisson equation](poisson-s-equation.md) with [Dirichlet boundary conditions](dirichlet-boundary-condition.md). Its [eigenvectors](eigenvector.md) have components $\sin(jk\pi/(n+1))$, and $D^{-1}T_n$ has [eigenvalues](eigenvalue.md) $1-\cos(k\pi/(n+1))$. At $\omega=2/3$, upper-half modes have factors between $-1/3$ and $1/3$, while low-frequency factors remain close to one on fine grids. This explains why the [weighted Jacobi method](weighted-jacobi-method.md) helps a [multigrid method](multigrid-method-split.md) by reducing oscillatory errors, even when it is a slow solver on its own.[Error eigenvector expansion, coefficient 1/3 + (2/3) cos(jπ/2^i), and concluding upper-half-frequency attenuation statement](cs267-supplemental-notes-for-lecture-17-how-multigrid-damps-high-frequencies-by-james-demmel.md)

**Table of contents**

- [High-frequency smoothing factor of weighted Jacobi](high-frequency-smoothing-factor-of-weighted-jacobi.md)
  - [Exact finite-grid high-frequency Jacobi smoothing optimum](exact-finite-grid-high-frequency-jacobi-smoothing-optimum.md)

## ↑ Ancestors (9)

1. [Weighted Jacobi method](weighted-jacobi-method.md)
2. [Jacobi method](jacobi-method.md)
3. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
4. [Numerical linear algebra](numerical-linear-algebra-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
