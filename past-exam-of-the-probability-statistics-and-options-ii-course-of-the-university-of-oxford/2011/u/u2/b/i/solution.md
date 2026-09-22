<h1 id="u/u2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The recursive worker extends a current path by one uniformly selected unused neighbour. A trapped extension returns `NULL` all the way to the outer loop, which restarts from the origin. It does not backtrack and try a different branch of the same attempt, since the stated process restarts the entire walk.

```
saw <- function(N) {
  stopifnot(length(N) == 1L, is.finite(N), N >= 0,
            N == floor(N))
  steps <- rbind(c(1L, 0L), c(-1L, 0L),
                 c(0L, 1L), c(0L, -1L))
  grow <- function(path) {
    if (nrow(path) == N + 1L) return(path)
    last <- path[nrow(path), ]
    candidates <- sweep(steps, 2L, last, "+")
    keep <- vapply(seq_len(nrow(candidates)), function(i) {
      !row.match(path, candidates[i, ])
    }, logical(1))
    candidates <- candidates[keep, , drop = FALSE]
    if (nrow(candidates) == 0L) return(NULL)
    j <- sample.int(nrow(candidates), 1L)
    grow(rbind(path, candidates[j, ]))
  }
  repeat {
    path <- grow(matrix(c(0L, 0L), nrow = 1L))
    if (!is.null(path)) return(path)
  }
}
```

The base case has exactly $N+1$ visited vertices. Every extension is a unit horizontal or vertical step to a new [vertex](../../../../../../vertex-graph-theory.md), proving the output dimensions and self-avoidance by induction. A straight path has positive [probability](../../../../../../probability.md), so each independent attempt has a positive chance of success and repeated attempts terminate almost surely.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [U2](../../../u2.md)
4. [U](../../../../u.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
