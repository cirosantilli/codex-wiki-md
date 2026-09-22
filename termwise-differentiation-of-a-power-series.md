# Termwise differentiation of a power series

↑ **Parent:** [Power series](power-series.md)

Inside its [radius of convergence](radius-of-convergence.md), a [power series](power-series.md) $f(z)=\sum_{n\ge0}a_n(z-c)^n$ can be differentiated term by term:

$$
f'(z)=\sum_{n\ge1}na_n(z-c)^{n-1}.
$$

The differentiated series has the same [radius of convergence](radius-of-convergence.md). The conclusion concerns the interior, including [uniform convergence](uniform-convergence.md) on smaller closed disks; it does not assert that differentiated boundary series converge wherever the original did. For example, $\sum_{n\ge1}z^n/n$ converges conditionally at $z=-1$, but its differentiated series $\sum_{n\ge1}z^{n-1}$ does not.

Applied to the [geometric series](geometric-series.md), it gives the useful identity

$$
\frac1{(1-z)^2}=\sum_{n=1}^{\infty}nz^{n-1},\qquad |z|<1.
$$

Differentiation turns the plain coefficients into integer weights. This is one way [generating functions](generating-function.md) translate a weighted counting question into an operation on a known series. A proof controls the original and differentiated tails on smaller disks; the [Weierstrass M-test](weierstrass-m-test.md) provides the needed uniform bounds. See [Lebl, Basic Analysis, §11.3: power-series differentiation and analyticity](https://www.jirka.org/ra/html/sec_analfuncs.html).

## ↑ Ancestors (7)

1. [Power series](power-series.md)
2. [Sequence and series](sequence-and-series-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Boundary convergence of a power series](boundary-convergence-of-a-power-series.md)
- [Coefficient recovery and factorial moments of a probability generating function](coefficient-recovery-and-factorial-moments-of-a-probability-generating-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/12f/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/12f/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/12f/b/ii/solution.md)
- [Power series](power-series.md)
