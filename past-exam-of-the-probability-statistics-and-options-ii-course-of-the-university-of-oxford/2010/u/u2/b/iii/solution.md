<h1 id="u/u2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here $f'(x)=4x^3-12x^2+4x+12$ and $f''(x)=12x^2-24x+4$. This implementation uses the undamped Newton step, checks a [stationary point](../../../../../../stationary-point.md)'s [curvature](../../../../../../second-derivative.md), and reports failure on a [two-cycle](../../../../../../period-two-orbit.md) or exhausted iteration limit:

```
R
newton_min <- function(x0, tol = 1e-10, maxit = 100L) {
  fp <- function(x) 4*x^3 - 12*x^2 + 4*x + 12
  fpp <- function(x) 12*x^2 - 24*x + 4
  x <- x0
  trace <- x
  for (k in seq_len(maxit)) {
    g <- fp(x)
    h <- fpp(x)
    if (abs(g) <= tol) {
      return(list(x = x, converged = h > 0,
                  reason = if (h > 0) "minimum" else "not a strict minimum",
                  trace = trace))
    }
    if (!is.finite(h) || abs(h) <= .Machine$double.eps)
      stop("Newton step has zero or invalid curvature")
    next_x <- x - g/h
    if (!is.finite(next_x)) stop("Nonfinite Newton iterate")
    trace <- c(trace, next_x)
    n <- length(trace)
    if (n >= 3L && abs(trace[n] - trace[n - 2L]) <= tol*(1 + abs(next_x)))
      return(list(x = next_x, converged = FALSE,
                  reason = "two-cycle", trace = trace))
    x <- next_x
  }
  list(x = x, converged = FALSE, reason = "iteration limit", trace = trace)
}
```

A sufficiently close start near $-0.7692923542$ converges to the [minimum](../../../../../../local-minimum.md). The [derivative](../../../../../../derivative.md) cubic has exactly one real root: after $x=1+t$ it is proportional to $t^3-2t+2$, whose local [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) and [minimum](../../../../../../local-minimum.md) are both positive, so it crosses zero only once, on the left. Since the quartic tends to $+\infty$ in both directions and its [curvature](../../../../../../second-derivative.md) at that [stationary point](../../../../../../stationary-point.md) is positive, this is the unique [global minimum](../../../../../../global-minimum.md). The function reports convergence rather than assuming that every starting point must reach it.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [U2](../../../u2.md)
4. [U](../../../../u.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
