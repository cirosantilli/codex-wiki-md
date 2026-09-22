# Power iteration

↑ **Parent:** [Numerical linear algebra](numerical-linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Power_iteration)

[Power iteration](power-iteration.md) finds a [dominant eigenvalue](dominant-eigenvalue.md) and its [eigenvector](eigenvector.md) by repeatedly applying a [matrix](matrix.md) and rescaling the resulting [vector](vector.md). The essential idea is selective amplification: components along different [eigenvectors](eigenvector.md) grow at different rates, so one direction can eventually dominate. It is the computational form of the [power method](power-method.md) and is useful when applying a large [sparse matrix](sparse-matrix.md) to a [vector](vector.md) is cheap but computing its whole [spectral decomposition](spectral-decomposition.md) is expensive.

For a square [matrix](matrix.md) over the [real numbers](real-number.md) or [complex numbers](complex-number.md) $A$, choose a [unit vector](unit-vector.md) $x_0$ and repeat

$$
y_{k+1}=Ax_k,\qquad x_{k+1}=\frac{y_{k+1}}{\|y_{k+1}\|_2}.
$$

Here $\|\cdot\|_2$ is the [Euclidean norm](euclidean-norm.md). If $y_{k+1}=0$, stop before division: the current [vector](vector.md) is an [eigenvector](eigenvector.md) for the [zero eigenvalue](zero-eigenvalue.md), and this iteration cannot continue. Otherwise, in exact arithmetic,

$$
x_k=\frac{A^kx_0}{\|A^kx_0\|_2}.
$$

Repeated normalization keeps the stored [vectors](vector.md) at manageable size without changing their directions; it does not guarantee that an individual multiplication cannot exceed the range of [floating-point arithmetic](floating-point-arithmetic-split.md). The [dominant eigenvalue](dominant-eigenvalue.md) means largest [modulus](modulus.md), which need not mean largest signed real value.[Power Method](templates-for-the-solution-of-algebraic-eigenvalue-problems-a-practical-guide/power-method.md)

**Table of contents**

- [Exact two-dimensional power iteration](exact-two-dimensional-power-iteration.md)
- [Power iteration convergence for a diagonalizable matrix](power-iteration-convergence-for-a-diagonalizable-matrix.md)
  - [Power iteration direction error](power-iteration-direction-error.md)
- [Sign and phase in power iteration](sign-and-phase-in-power-iteration.md)
- [Power iteration eigenpair diagnostics](power-iteration-eigenpair-diagnostics.md)
- [Power iteration failure cases](power-iteration-failure-cases.md)

## ↑ Ancestors (6)

1. [Numerical linear algebra](numerical-linear-algebra-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Exact two-dimensional power iteration](exact-two-dimensional-power-iteration.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335/2/iii/solution.md)
- [Power iteration](power-iteration.md)
- [Power iteration convergence for a diagonalizable matrix](power-iteration-convergence-for-a-diagonalizable-matrix.md)
- [Power iteration failure cases](power-iteration-failure-cases.md)
- [Power method](power-method.md)
