# Gershgorin stability bound for a variable-coefficient diffusion stencil

↑ **Parent:** [Gershgorin circle theorem](gershgorin-circle-theorem.md)

A [symmetric matrix](symmetric-matrix.md) obtained from a conservative five-point discretization of a [diffusion equation](diffusion-equation-split.md) has row centre $-s_i/h^2$ and radius at most $s_i/h^2$, where $h>0$ is the grid spacing and $s_i$ is the sum of its four nonnegative edge coefficients. Here the [matrix](matrix.md) represents the diffusion generator, with nonnegative off-diagonal entries; boundary elimination may reduce the row radius. If every coefficient is at most $a_{\max}>0$, then $s_i\leq4a_{\max}$, and the [Gershgorin bounds for symmetric matrices](gershgorin-bounds-for-symmetric-matrices.md) place every [eigenvalue](eigenvalue.md) in $[-8a_{\max}/h^2,0]$.

For the [Forward Euler method](euler-method.md), an [eigenvalue](eigenvalue.md) $\lambda\leq0$ has amplification factor $1+\Delta t\lambda$. Requiring $|1+\Delta t\lambda|\leq1$ for every such [eigenvalue](eigenvalue.md) gives the sufficient [absolute stability](linear-stability-domain.md) condition $\Delta t/h^2\leq1/(4a_{\max})$. Symmetry makes this also prevent growth of the [Euclidean norm](euclidean-norm.md). For $a_{\max}=2$ and $h=0.1$, the bound is $\lambda\in[-1600,0]$ and $\Delta t\leq0.00125$. At that step size the [interval](interval-mathematics.md) maps to amplification factors in $[-1,1]$. This illustrates why cheap [Gershgorin disc](gershgorin-disc.md) bounds can select a stable time step before any [eigenvalues](eigenvalue.md) are computed.

## ↑ Ancestors (6)

1. [Gershgorin circle theorem](gershgorin-circle-theorem.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/40c/b/ii/solution.md)
