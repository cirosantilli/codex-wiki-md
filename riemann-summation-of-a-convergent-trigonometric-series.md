# Riemann summation of a convergent trigonometric series

↑ **Parent:** [Fourier series](fourier-series-split.md)

Suppose the symmetric partial sums converge at a fixed point. Group positive and negative frequencies together, let $S_n$ be the resulting partial sums and set $w(x)=(\sin x/x)^2$, with $w(0)=1$. [Summation by parts](abel-s-summation-formula.md) expresses the weighted sum as $\sum_{n\ge0}S_n[w(nk)-w((n+1)k)]$, where $k=|h|/2$. The total variation of these weights is at most $\int_0^\infty|w'(x)|dx<\infty$, independently of $k$, and each fixed difference tends to zero. Subtract the limiting value of $S_n$ and split into a finite prefix and a uniformly small tail to prove convergence to that value. This is a regular summation method even though the sinc-squared weights need not decrease monotonically.

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-7/4/ii/solution.md)
- [Symmetric second derivative](symmetric-second-derivative.md)
- [Uniqueness of a trigonometric series outside a finite set](uniqueness-of-a-trigonometric-series-outside-a-finite-set.md)
