# Displacement stability of a symmetric semidiscrete wave equation

↑ **Parent:** [Method of lines](method-of-lines.md)

Let $K_h$ be a symmetric nonnegative [matrix](matrix.md) and consider $U''=(\alpha I-K_h)U$ with fixed real $\alpha$. In any [inner product](inner-product.md) for which $K_h$ is self-adjoint, [diagonalization of a matrix](diagonalization-of-a-matrix.md) gives

$$
\|U(t)\|\leq e^{\sqrt{\max(\alpha,0)}t}
\bigl(\|U(0)\|+t\|U'(0)\|\bigr).
$$

Indeed each modal coefficient is either a cosine and sine divided by its frequency, a linear function at zero frequency, or a hyperbolic cosine and sine divided by its growth rate. The bounds $|\cos(\omega t)|\leq1$, $|\sin(\omega t)/\omega|\leq t$, and $\sinh(\beta t)/\beta\leq t e^{\beta t}$ prove the estimate. It is uniform in the spectrum of $K_h$ and therefore gives finite-time displacement [stability](stability-of-a-numerical-method.md). Uniform velocity estimates need additional control of the initial spatial energy. All-time displacement bounds require a strictly positive lower bound for $K_h-\alpha I$, a different condition.

**Table of contents**

- [All-time boundedness of a semidiscrete reaction wave equation](all-time-boundedness-of-a-semidiscrete-reaction-wave-equation.md)

## ↑ Ancestors (8)

1. [Method of lines](method-of-lines.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [All-time boundedness of a semidiscrete reaction wave equation](all-time-boundedness-of-a-semidiscrete-reaction-wave-equation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/3/ii/solution.md)
