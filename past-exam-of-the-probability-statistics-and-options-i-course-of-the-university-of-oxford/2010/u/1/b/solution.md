<h1 id="u/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [inverse transform sampling](../../../../../inverse-transform-sampling.md) for the categorical draw. Validate a finite nonnegative [probability](../../../../../probability.md) vector, allowing only a small rounding tolerance in its total, then compare a single uniform draw with the cumulative probabilities:

```
sim1 <- function(p) {
  if (!is.numeric(p) || length(p) == 0L ||
      any(!is.finite(p)) || any(p < 0) ||
      abs(sum(p) - 1) > 1e-12) {
    stop("p must be a nonempty finite probability vector")
  }
  p <- p / sum(p)
  cumulative <- cumsum(p)
  cumulative[length(p)] <- 1
  u <- runif(1)
  as.integer(which(u < cumulative)[1L])
}
```

The returned value is $j$ when $u$ falls in the interval between the previous cumulative sum and the $j$th one. That interval has length $p_j$, so the output has the required probabilities. Strict comparison skips zero-[probability](../../../../../probability.md) categories even if a simulated uniform value equals an interval boundary. Exactly one call to `runif(1)` is made.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [U](../../../u.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
