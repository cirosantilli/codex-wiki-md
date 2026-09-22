# Power series solutions of the Hermite differential equation

↑ **Parent:** [Hermite differential equation](hermite-differential-equation.md)

For $y''-2xy'+2\lambda y=0$, substitute a [power series](power-series.md) $y=\sum_{n\geq0}a_nx^n$ to obtain the displayed [recurrence relation](recurrence-relation.md). It separates into an [even](even-function.md) solution with $a_0=1,a_1=0$ and an [odd](odd-function.md) solution with $a_0=0,a_1=1$:

$$
y_e=1-\lambda x^2+\frac{\lambda(\lambda-2)}6x^4+\cdots,\qquad y_o=x+\frac{1-\lambda}3x^3+\frac{(1-\lambda)(3-\lambda)}{30}x^5+\cdots.
$$

The ratio of successive terms within each parity tends to zero at every fixed complex $x$, giving infinite [radius of convergence](radius-of-convergence.md). The two initial-value vectors are independent, so these solutions span the solution space. A nonzero [polynomial](polynomial-split.md) solution exists precisely when $\lambda=N$ is a nonnegative [integer](integer-split.md): its highest power forces this value, and the recurrence terminates the matching parity. These terminating solutions are nonzero [scalar multiples](scalar-multiple.md) of the [Hermite polynomials](hermite-polynomial.md). Multiplication by $e^{-x^2/2}$ connects them to [Hermite oscillator quantization](hermite-oscillator-quantization.md).

## ↑ Ancestors (5)

1. [Hermite differential equation](hermite-differential-equation.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/6/ii/solution.md)
