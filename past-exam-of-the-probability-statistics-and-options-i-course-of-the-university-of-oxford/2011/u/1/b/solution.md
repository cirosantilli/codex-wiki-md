<h1 id="u/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The following [R](../../../../../r-programming-language.md) function uses the factored polynomial for evaluation, handles endpoint and midpoint roots, and returns a midpoint only once its error bound is at most `eps`:

```
bisect <- function(a, b, eps = 1e-8, maxiter = 1000L) {
  f <- function(x) x * (x - 1) * (x - 2) * (x - 5)
  stopifnot(length(a) == 1L, length(b) == 1L,
            is.finite(a), is.finite(b), a < b,
            length(eps) == 1L, is.finite(eps), eps > 0)
  fa <- f(a)
  fb <- f(b)
  if (fa == 0) return(a)
  if (fb == 0) return(b)
  if (sign(fa) == sign(fb)) stop("Endpoints must bracket a sign change")
  for (i in seq_len(maxiter)) {
    m <- a + (b - a) / 2
    fm <- f(m)
    if (fm == 0 || (b - a) / 2 <= eps) return(m)
    if (sign(fm) == sign(fa)) {
      a <- m
      fa <- fm
    } else {
      b <- m
    }
  }
  stop("Iteration limit reached")
}
```

Each update preserves the sign-changing bracket, and the stopping bound is the half-width of that bracket. Thus [continuity](../../../../../continuous-function.md) and the [intermediate value theorem](../../../../../intermediate-value-theorem.md) justify the returned root approximation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [U](../../../u.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
