<h1 id="u/u2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Recursively sort two halves, then merge their increasing lists by repeatedly choosing the smaller current first element. The following function preserves repetitions, as sorting a vector should:

```
R
merge_sort <- function(x) {
  n <- length(x)
  stopifnot(n >= 1L)
  if (n == 1L) return(x)
  m <- n %/% 2L
  left <- merge_sort(x[seq_len(m)])
  right <- merge_sort(x[(m + 1L):n])
  nl <- length(left)
  nr <- length(right)
  out <- integer(n)
  i <- j <- k <- 1L
  while (i <= nl && j <= nr) {
    if (left[i] <= right[j]) {
      out[k] <- left[i]
      i <- i + 1L
    } else {
      out[k] <- right[j]
      j <- j + 1L
    }
    k <- k + 1L
  }
  if (i <= nl) out[k:n] <- left[i:nl]
  if (j <= nr) out[k:n] <- right[j:nr]
  out
}
```

[Induction](../../../../../mathematical-induction.md) proves correctness: each recursive result is sorted and preserves its input [multiset](../../../../../multiset.md); each merge step removes the least remaining element from one of them, so the output is sorted and has exactly the union [multiset](../../../../../multiset.md). The base case has length one. Each merge takes linear time, yielding $O(n\log n)$ time overall. Choosing from the left first on a tie makes the sort stable. The required input is an integer vector without missing values.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [U2](../../u2.md)
3. [U](../../../u.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
