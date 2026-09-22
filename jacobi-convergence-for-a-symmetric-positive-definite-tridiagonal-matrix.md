# Jacobi convergence for a symmetric positive-definite tridiagonal matrix

↑ **Parent:** [Jacobi method](jacobi-method.md)

If $A=D+L+L^T$ is symmetric positive definite and tridiagonal, set $S=\operatorname{diag}(1,-1,1,-1,\ldots)$. Then

$$
SAS=D-L-L^T
$$

is positive definite. Applying the [Householder-John theorem](householder-john-theorem.md) to $M=D$ and $N=-(L+L^T)$ proves that the Jacobi iteration converges.

## ↑ Ancestors (8)

1. [Jacobi method](jacobi-method.md)
2. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
3. [Numerical linear algebra](numerical-linear-algebra.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/40c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/40d/b/solution.md)
