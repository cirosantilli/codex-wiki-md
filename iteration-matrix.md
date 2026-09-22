# Iteration matrix

↑ **Parent:** [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)

For a stationary iteration $x^{(k+1)}=Hx^{(k)}+v$, the matrix $H$ propagates the error by $e^{(k+1)}=He^{(k)}$. Convergence from every initial error is equivalent to $\rho(H)<1$.

For a [matrix splitting](matrix-splitting.md) $A=M-N$, the [iteration matrix](iteration-matrix.md) is $H=M^{-1}N=I-M^{-1}A$, where $I$ is the [identity matrix](identity-matrix.md). If $Ax_*=b$, subtracting its [fixed point](fixed-point.md) equation from the update gives

$$
e^{(k)}=x^{(k)}-x_*,\qquad e^{(k+1)}=He^{(k)},\qquad e^{(k)}=H^ke^{(0)}.
$$

Thus $b$ determines the [fixed point](fixed-point.md), while $H$ determines how the [forward error](forward-error.md) moves. An [eigenvector](eigenvector.md) $v$ with [eigenvalue](eigenvalue.md) $\lambda$ is an error direction whose coefficient is multiplied by $\lambda$ on every step. A negative real [eigenvalue](eigenvalue.md) reverses its sign; a zero [eigenvalue](eigenvalue.md) removes that component in one step.

**Table of contents**

- [Convergence criterion for a stationary iteration](convergence-criterion-for-a-stationary-iteration.md)
- [Residual and forward error in a stationary iteration](residual-and-forward-error-in-a-stationary-iteration.md)

## ↑ Ancestors (7)

1. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Coarse-grid correction](coarse-grid-correction.md)
- [Convergence criterion for a stationary iteration](convergence-criterion-for-a-stationary-iteration.md)
- [Error modes of a three-variable Jacobi iteration](error-modes-of-a-three-variable-jacobi-iteration.md)
- [Exact error contraction of a two-variable Gauss-Seidel iteration](exact-error-contraction-of-a-two-variable-gauss-seidel-iteration.md)
- [Gauss-Seidel convergence from diagonal dominance and positive definiteness](gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness.md)
- [Gauss-Seidel iteration can diverge for an invertible matrix](gauss-seidel-iteration-can-diverge-for-an-invertible-matrix.md)
- [Gauss-Seidel method](gauss-seidel-method.md)
- [Iteration matrix](iteration-matrix.md)
- [Jacobi convergence from strict diagonal dominance](jacobi-convergence-from-strict-diagonal-dominance.md)
- [Jacobi method](jacobi-method.md)
- [Multigrid method](multigrid-method-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3/11a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/40e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/40e/c/solution.md)
- [Weighted Jacobi method](weighted-jacobi-method.md)
