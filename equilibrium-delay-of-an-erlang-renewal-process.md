# Equilibrium delay of an Erlang renewal process

↑ **Parent:** [Equilibrium residual-life distribution](equilibrium-residual-life-distribution.md)

For inter-renewal times with an [Erlang distribution](erlang-distribution.md) of integer shape $r$ and rate $\lambda$, the mean is $r/\lambda$ and survival function is $e^{-\lambda t}\sum_{j=0}^{r-1}(\lambda t)^j/j!$. The equilibrium first-delay density is survival divided by the mean,

$$
f_e(t)=\frac\lambda r e^{-\lambda t}\sum_{j=0}^{r-1}\frac{(\lambda t)^j}{j!},\qquad t>0.
$$

This is the equal mixture of Erlang distributions of shapes $1,\ldots,r$. It can be constructed by observing a Poisson clock with uniformly randomized phase modulo $r$, whose every $r$th event is a renewal.

## ↑ Ancestors (8)

1. [Equilibrium residual-life distribution](equilibrium-residual-life-distribution.md)
2. [Residual lifetime process](residual-lifetime-process.md)
3. [Renewal process](renewal-process.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/26j/d/solution.md)
