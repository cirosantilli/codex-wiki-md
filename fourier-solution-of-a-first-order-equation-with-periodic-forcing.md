# Fourier solution of a first-order equation with periodic forcing

↑ **Parent:** [Fourier series](fourier-series-split.md)

Let $\alpha,\beta$ be nonzero real constants and let $f$ be a [smooth](smooth-function.md) [periodic function](periodic-function.md) of period $2\pi$, with real [Fourier coefficients](fourier-coefficient.md) $c_n,d_n$. Write the unknown [periodic solution](periodic-solution.md) with [Fourier coefficients](fourier-coefficient.md) $a_n,b_n$. [Fourier orthogonality](fourier-orthogonality.md) applied to the equation gives

$$
\beta a_0=c_0,\qquad
\beta a_n+\alpha n b_n=c_n,\qquad
\beta b_n-\alpha n a_n=d_n.
$$

Solving these two-by-two [linear systems](system-of-linear-equations.md) gives

$$
a_n=\frac{\beta c_n-\alpha n d_n}{\beta^2+\alpha^2n^2},\qquad
b_n=\frac{\alpha n c_n+\beta d_n}{\beta^2+\alpha^2n^2}\quad(n\geq1).
$$

The smooth forcing has rapidly decreasing [Fourier coefficients](fourier-coefficient.md), so the resulting series and its [derivatives](derivative.md) converge and satisfy the equation. Uniqueness follows because the difference of two solutions is $Ce^{-\beta x/\alpha}$, which is periodic only when $C=0$. A single sinusoidal forcing therefore gives a single sinusoidal response with changed amplitude and phase.

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/14/d/solution.md)
