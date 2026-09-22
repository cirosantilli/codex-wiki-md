# Gauss-Seidel energy decrease identity

↑ **Parent:** [Gauss-Seidel method](gauss-seidel-method.md)

For a real [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) $A=D+L+L^T$, let $e_k$ be the [Gauss-Seidel method](gauss-seidel-method.md) error and $d_k=e_k-e_{k+1}$. Its recurrence gives $Ae_k=(D+L)d_k$. Expanding the two squared [energy norms](energy-norm.md) yields $2d_k^TAe_k-d_k^TAd_k=d_k^TDd_k$. Every diagonal entry of $D$ is positive, so the error energy strictly decreases unless $d_k=0$. In that case $Ae_k=0$ and the exact solution has already been reached. This identity exhibits the method as a sequence of energy-reducing coordinate corrections.

## ↑ Ancestors (8)

1. [Gauss-Seidel method](gauss-seidel-method.md)
2. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2009/a/2/solution.md)
