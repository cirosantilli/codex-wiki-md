# Gauss-Seidel method

↑ **Parent:** [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss–Seidel_method)

With $A=D+L+U$, the [Gauss-Seidel method](gauss-seidel-method.md) solves $(D+L)x^{(k+1)}=b-Ux^{(k)}$. It uses each newly computed coordinate immediately in the remaining [triangular solve](triangular-solve.md). It is [successive over-relaxation](successive-over-relaxation.md) with parameter one, and converges from every start when $A$ is a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md).

To solve a [linear system](system-of-linear-equations.md) $Ax=b$, split its [matrix](matrix.md) into the [diagonal matrix](diagonal-matrix.md) $D$ and the strictly lower and upper parts $L,U$, retaining their actual signs. Every diagonal entry must be nonzero. A sweep updates coordinates in order:

$$
x_i^{(k+1)}=\frac{b_i-\sum_{j<i}a_{ij}x_j^{(k+1)}-\sum_{j>i}a_{ij}x_j^{(k)}}{a_{ii}}.
$$

The [Jacobi method](jacobi-method.md) uses the old [vector](vector.md) throughout; the [Gauss-Seidel method](gauss-seidel-method.md) reuses each fresh coordinate. Thus the update order is part of the method.[Math 221, Matrix Computations, Fall 2009; Gauss-Seidel: component loop, splitting and update-order remark, web lines 372–380](math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009.md)

The [matrix splitting](matrix-splitting.md) has $M=D+L$, $N=-U$, so its [iteration matrix](iteration-matrix.md) is

$$
H=-(D+L)^{-1}U,\qquad x^{(k+1)}=Hx^{(k)}+(D+L)^{-1}b.
$$

Compute the update by [forward substitution](forward-substitution.md) with the [lower triangular matrix](lower-triangular-matrix.md) $D+L$, rather than forming a [matrix inverse](matrix-inverse-split.md). For a [sparse matrix](sparse-matrix.md), a sweep only visits stored entries and can overwrite the working [vector](vector.md). Dependencies on fresh coordinates constrain parallel execution. This makes the [Gauss-Seidel method](gauss-seidel-method.md) an inexpensive solver component, including in a [multigrid method](multigrid-method-split.md).[Math 221, Matrix Computations, Fall 2009; Basic iterative methods, cheap splitting requirement; Gauss-Seidel loop and red-black ordering; opening list of solver building blocks](math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009.md)

**Table of contents**

- [Gauss-Seidel iteration for a two-variable positive-definite system](gauss-seidel-iteration-for-a-two-variable-positive-definite-system.md)
  - [Exact error contraction of a two-variable Gauss-Seidel iteration](exact-error-contraction-of-a-two-variable-gauss-seidel-iteration.md)
- [Gauss-Seidel convergence from diagonal dominance and positive definiteness](gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness.md)
  - [Gauss-Seidel iteration can diverge for an invertible matrix](gauss-seidel-iteration-can-diverge-for-an-invertible-matrix.md)

## ↑ Ancestors (7)

1. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Exact error contraction of a two-variable Gauss-Seidel iteration](exact-error-contraction-of-a-two-variable-gauss-seidel-iteration.md)
- [Gauss-Seidel convergence from diagonal dominance and positive definiteness](gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness.md)
- [Gauss-Seidel iteration can diverge for an invertible matrix](gauss-seidel-iteration-can-diverge-for-an-invertible-matrix.md)
- [Gauss-Seidel method](gauss-seidel-method.md)
- [Jacobi iteration for a three-variable tridiagonal system](jacobi-iteration-for-a-three-variable-tridiagonal-system.md)
- [Matrix splitting](matrix-splitting.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/19f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/37e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/39a/solution.md)
- [Skew-tridiagonal Jacobi and Gauss-Seidel iterations](skew-tridiagonal-jacobi-and-gauss-seidel-iterations.md)
- [Successive over-relaxation](successive-over-relaxation.md)
