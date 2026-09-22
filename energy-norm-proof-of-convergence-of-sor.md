# Energy-norm proof of convergence of SOR

↑ **Parent:** [Successive over-relaxation](successive-over-relaxation.md)

Let $A=D+L+L^T$ be a real [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md), with $D$ diagonal and $L$ strictly lower triangular. Put $B=D/\omega+L$ and $C_\omega=I-B^{-1}A$ for $\omega\ne0$. The [matrix norm induced by an energy norm](matrix-norm-induced-by-an-energy-norm.md) reduces the question to $T=A^{1/2}C_\omega A^{-1/2}$. Direct multiplication and $B+B^T-A=(2/\omega-1)D$ give

$$
T^TT=I-\left(\frac2\omega-1\right)A^{1/2}B^{-T}DB^{-1}A^{1/2}.
$$

The left side is [positive semidefinite](positive-semidefinite-matrix.md). The [matrix](matrix.md) following the scalar coefficient on the right is [positive-definite](positive-definite-bilinear-form.md), since $D$ has positive diagonal and $B^{-1}A^{1/2}$ is an [invertible matrix](invertible-matrix.md). For $0<\omega<2$, every [eigenvalue](eigenvalue.md) of $T^TT$ therefore lies in $[0,1)$. Hence its [spectral radius](spectral-radius.md) is below one and $\|C_\omega\|_A=\|T\|_2<1$. Iteration errors consequently decay geometrically in the [energy norm](energy-norm.md). The argument proves convergence from every initial [vector](vector.md), without requiring the original [iteration matrix](iteration-matrix.md) to be [symmetric](symmetric-relation.md).

## ↑ Ancestors (8)

1. [Successive over-relaxation](successive-over-relaxation.md)
2. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2011/2/d/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2011/2/e/solution.md)
