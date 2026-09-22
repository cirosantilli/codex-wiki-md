<h1 id="u/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The function below counts the initial uniformly chosen state as the first of the $n$ visited states, and then generates $n-1$ transitions using the appropriate row of $P$:

```
simchain <- function(n, P) {
  if (!is.numeric(n) || length(n) != 1L || !is.finite(n) ||
      n < 1 || n != floor(n)) stop("n must be a positive integer")
  if (!is.matrix(P) || !is.numeric(P) || nrow(P) == 0L ||
      nrow(P) != ncol(P) || any(!is.finite(P)) ||
      any(P < 0) || any(abs(rowSums(P) - 1) > 1e-12)) {
    stop("P must be a finite square stochastic matrix")
  }
  k <- nrow(P)
  state <- sim1(rep(1/k, k))
  counts <- numeric(k)
  counts[state] <- 1
  if (n > 1) {
    for (step in seq_len(n - 1)) {
      state <- sim1(P[state, ])
      counts[state] <- counts[state] + 1
    }
  }
  counts / n
}
```

Conditional on the current state $i$, `sim1(P[i, ])` selects $j$ with [probability](../../../../../probability.md) $P_{ij}$, proving the [Markov property](../../../../../markov-property.md) with the desired [transition matrix](../../../../../stochastic-matrix.md). Initialization is uniform by the same sampler. Dividing the visit counts by $n$ gives the requested [Empirical occupation proportions of a finite Markov chain](../../../../../empirical-occupation-proportions-of-a-finite-markov-chain.md), including a valid result when $n=1$.

## ↑ Ancestors (13)

1. [C](../c.md)
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
