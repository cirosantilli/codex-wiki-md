<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A numerical [power series](../../../../../power-series.md) evaluation needs a stopping rule. For $r=|z|<1$ and integer $a\geq0$, the absolute remainder after $N$ terms satisfies the [polylogarithm series remainder bound](../../../../../polylogarithm-series-remainder-bound.md)

$$
\boxed{\left|\operatorname{Li}_a(z)-\sum_{k=1}^{N}\frac{z^k}{k^a}\right|
\leq\frac{r^{N+1}}{(N+1)^a(1-r)}.}
$$

Indeed $k^{-a}\leq(N+1)^{-a}$ for $k>N$, and the remaining powers sum as a [geometric series](../../../../../geometric-series.md). This also covers negative $z$. The code sums terms in vectors of at most 4096 entries, checking the bound after each block; there is no loop over individual terms.

```
polylog <- function(a, z, tol = 1e-10, max_terms = 1000000) {
  scalar <- function(v) {
    is.numeric(v) && !is.complex(v) && length(v) == 1L &&
      is.finite(v)
  }
  if (!scalar(a) || a < 0 || a != floor(a))
    stop("a must be a nonnegative integer")
  if (!scalar(z) || abs(z) >= 1)
    stop("z must be real with abs(z) < 1")
  if (!scalar(tol) || tol <= 0 || tol >= 1)
    stop("tol must lie strictly between 0 and 1")
  if (!scalar(max_terms) || max_terms < 1 ||
      max_terms != floor(max_terms))
    stop("max_terms must be a positive integer")
  if (z == 0) return(0)
  r <- abs(z)
  N <- 0
  ans <- 0
  repeat {
    if (N >= max_terms)
      stop("requested truncation tolerance not reached")
    B <- min(4096, max_terms - N)
    k <- seq.int(N + 1, N + B)
    ans <- ans + sum(z^k * exp(-a * log(k)))
    N <- N + B
    log_bound <- (N + 1) * log(r) - a * log(N + 1) - log1p(-r)
    if (log_bound <= log(tol)) return(ans)
  }
}
```

This accepts every positive integer order in the question, and also order zero if $0\in\mathbb N$ is the convention adopted. The bound controls absolute truncation error; floating-point rounding is a separate source of error. Close to $|z|=1$, convergence can be slow. If the resource limit is reached, the function reports failure instead of silently claiming the requested accuracy. Useful exact checks are $\operatorname{Li}_1(z)=-\log(1-z)$ and $\operatorname{Li}_0(z)=z/(1-z)$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
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
