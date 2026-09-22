# Matrix splitting

↑ **Parent:** [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_splitting)

A splitting $A=M-N$ with invertible $M$ produces

$$
x^{(k+1)}=M^{-1}Nx^{(k)}+M^{-1}b.
$$

A [matrix splitting](matrix-splitting.md) chooses an easy part $M$ of a [matrix](matrix.md) and corrects for the remaining part $N$. To solve the [linear system](system-of-linear-equations.md) $Ax=b$, first rewrite it as $Mx=Nx+b$, then use the old [vector](vector.md) on the right and solve for the new [vector](vector.md) on the left. The [matrix inverse](matrix-inverse-split.md) notation describes the update mathematically; each step should solve with $M$ rather than construct its [matrix inverse](matrix-inverse-split.md).[Math 221, Matrix Computations, Fall 2009; Basic iterative methods: definition A = M − K and recurrence (\*), with the two conditions for a useful splitting](math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009.md)

The same identity also yields a correction based on the [linear-system residual](linear-system-residual.md):

$$
x^{(k+1)}=x^{(k)}+M^{-1}(b-Ax^{(k)}),\qquad H=I-M^{-1}A.
$$

This connects a [matrix splitting](matrix-splitting.md) to [matrix preconditioning](matrix-preconditioning.md): $M^{-1}$ rescales the imbalance before adding a correction. Choosing $M=A$ gives $H=0$ and the exact solution in one step, but requires solving the original [linear system](system-of-linear-equations.md); choosing $M$ cheaply matters as much as the [convergence criterion for a stationary iteration](convergence-criterion-for-a-stationary-iteration.md).

With the sign convention $A=D+L+U$, $D$ is the [diagonal matrix](diagonal-matrix.md) of diagonal entries and $L,U$ contain the actual lower and upper entries, without reversing their signs. The [Jacobi method](jacobi-method.md) uses $M=D$, $N=-(L+U)$; the [Gauss-Seidel method](gauss-seidel-method.md) uses $M=D+L$, $N=-U$. The first requires only division by diagonal entries; the second uses a [lower triangular matrix](lower-triangular-matrix.md) and [forward substitution](forward-substitution.md). These choices explain their different information flows.

**Table of contents**

- [Householder-John theorem](householder-john-theorem.md)

## ↑ Ancestors (7)

1. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Convergence criterion for a stationary iteration](convergence-criterion-for-a-stationary-iteration.md)
- [Gauss-Seidel method](gauss-seidel-method.md)
- [Iteration matrix](iteration-matrix.md)
- [Matrix splitting](matrix-splitting.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/39a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/40c/a/solution.md)
