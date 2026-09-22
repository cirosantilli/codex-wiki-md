<h1 id="u/u2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Compare every complete row with the given [vector](../../../../../vector.md), returning as soon as a match is found. The length check prevents recycling of the [vector](../../../../../vector.md); `seq_len` also handles an empty [matrix](../../../../../matrix.md) correctly. This implementation treats a missing comparison as a nonmatch and always returns a Boolean.

```
row.match <- function(X, y) {
  stopifnot(is.matrix(X), length(y) == ncol(X))
  for (i in seq_len(nrow(X))) {
    eq <- X[i, ] == y
    if (all(!is.na(eq) & eq)) return(TRUE)
  }
  FALSE
}
```

For the integer-coordinate matrices used below there are no missing values, so this is ordinary exact row equality.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [U2](../../u2.md)
3. [U](../../../u.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
