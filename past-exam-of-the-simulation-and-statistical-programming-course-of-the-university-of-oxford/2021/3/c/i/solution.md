<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Taking the [logarithm](../../../../../logarithm.md) of the normalized [probability density function](../../../../../probability-density-function.md), then summing over the [independent](../../../../../independent-random-variables.md) observations, gives the [log-likelihood](../../../../../log-likelihood.md)

$$
\boxed{\ell(p,\beta;x)
=n\{\log\beta-\log(-\log p)+\log(1-p)\}
-\beta\sum_{i=1}^nx_i
-\sum_{i=1}^n\log\!\left(1-(1-p)e^{-\beta x_i}\right).}
$$

Both $p$ and $\beta$ are parameters being inferred, so their contributions to the [normalizing constant](../../../../../normalizing-constant.md) must be retained. The following [R](../../../../../r-programming-language.md) implementation validates the arguments and returns one number:

```
ll_f <- function(p, beta, x) {
  scalar <- function(v) {
    is.numeric(v) && !is.complex(v) && length(v) == 1L &&
      is.finite(v)
  }
  if (!scalar(p) || p <= 0 || p >= 1)
    stop("p must lie strictly between 0 and 1")
  if (!scalar(beta) || beta <= 0)
    stop("beta must be positive")
  if (!is.numeric(x) || is.complex(x) || !is.null(dim(x)) ||
      any(!is.finite(x)) || any(x <= 0))
    stop("x must be a vector of finite positive numbers")
  if (length(x) == 0L) return(0)
  t <- log1p(-p) - beta * x
  length(x) * (log(beta) - log(-log(p))) +
    sum(t - log(-expm1(t)))
}
```

Here $t_i=\log(1-p)-\beta x_i<0$ and `-expm1(t)` computes $1-e^t$ accurately near zero. The empty-data [likelihood function](../../../../../likelihood-function.md) is one, so its [log-likelihood](../../../../../log-likelihood.md) is zero. Invalid parameter values produce errors in this evaluator; the next algorithm rejects candidates outside the parameter [support](../../../../../support.md) before calling it.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
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
