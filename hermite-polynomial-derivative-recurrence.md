# Hermite polynomial derivative recurrence

↑ **Parent:** [Hermite polynomial](hermite-polynomial.md)

For the physicists' [Hermite polynomials](hermite-polynomial.md) $H_n=(-1)^ne^{x^2}D^ne^{-x^2}$, the displayed recurrence holds for $n\geq1$, while $H_0'=0$ separately. Put $u=e^{-x^2}$. Differentiating $u'+2xu=0$ exactly $n$ times using the [Leibniz rule](leibniz-rule.md) yields

$$
(D+2x)D^nu=-2nD^{n-1}u.
$$

Differentiating the defining product for $H_n$ then gives

$$
H_n'=(-1)^ne^{x^2}(D+2x)D^nu
=2n(-1)^{n-1}e^{x^2}D^{n-1}u=2nH_{n-1}.
$$

The nonnegative integer convention is essential for the derivative-based definition; no negative-order derivative or $H_{-1}$ is needed.

## ↑ Ancestors (7)

1. [Hermite polynomial](hermite-polynomial.md)
2. [Orthogonal polynomial](orthogonal-polynomial-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/20/c/solution.md)
