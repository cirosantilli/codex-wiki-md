# Harmonic function in a rectangle with one constant boundary value

↑ **Parent:** [Harmonic function](harmonic-function.md)

On $0<x<a$, $0<y<b$, the bounded [harmonic function](harmonic-function.md) with value $F$ on the open upper edge and zero on the other three open edges has the sine-hyperbolic series in the title. [Separation of variables](separation-of-variables.md) gives the modes, and the [Fourier sine series](fourier-sine-series.md) of a constant selects only odd $n$. The series converges exponentially on compact subsets of the interior, justifying its derivatives in [Laplace's equation](laplace-equation.md).

For $F\ne0$, the upper corners have incompatible one-sided boundary limits, so the solution cannot extend continuously to them. Assigning isolated corner values does not alter the bounded interior [Dirichlet problem](dirichlet-problem.md). For numerical evaluation, the stable mode ratio is

$$
\frac{\sinh(ky)}{\sinh(kb)}=e^{-k(b-y)}\frac{1-e^{-2ky}}{1-e^{-2kb}},\qquad k>0.
$$

This avoids overflow from separately evaluating large hyperbolic sines.

## ↑ Ancestors (6)

1. [Harmonic function](harmonic-function.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1/12/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/12/b/solution.md)
