<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The following [R](../../../../../r-programming-language.md) function performs [inverse transform sampling](../../../../../inverse-transform-sampling.md) with [vectorized numerical computation](../../../../../vectorized-numerical-computation.md). It checks finite real scalar parameters, including a nonnegative integer sample count, and gives `beta` its requested default.

```
r_sample_f <- function(n, p, beta = 1) {
  scalar <- function(v) {
    is.numeric(v) && !is.complex(v) && length(v) == 1L &&
      is.finite(v)
  }
  if (!scalar(n) || n < 0 || n != floor(n))
    stop("n must be a nonnegative integer")
  if (!scalar(p) || p <= 0 || p >= 1)
    stop("p must lie strictly between 0 and 1")
  if (!scalar(beta) || beta <= 0)
    stop("beta must be positive")
  if (n == 0) return(numeric(0))
  v <- runif(n)
  (log1p(-p) - log(-expm1(v * log(p)))) / beta
}
```

Here $V=1-U$ is again a [uniform distribution](../../../../../continuous-uniform-distribution.md) draw, so the expression is the [quantile function](../../../../../quantile-function.md) from (ii). The function `expm1(t)` evaluates $e^t-1$ accurately when $t$ is small, avoiding cancellation in $1-p^V$; `log1p(-p)` evaluates $\log(1-p)$. For default bounds, `runif` excludes both endpoints, so this implementation does not deliberately generate the infinite endpoint of the [quantile function](../../../../../quantile-function.md). It returns a numeric [vector](../../../../../vector.md) of length `n`, including an empty [vector](../../../../../vector.md) when `n = 0`. [Official R documentation: default runif draws exclude both endpoints](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/Uniform.html) [Official R documentation: log1p and expm1 accurately evaluate small differences](https://stat.ethz.ch/R-manual/R-devel/library/base/html/Log.html)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
