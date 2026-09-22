<h1 id="u/u2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A simple square-lattice polygon has even perimeter at least four. Generate a [self-avoiding walk](../../../../../../self-avoiding-walk.md) of length $M-1$, reject unless its endpoint is a neighbour of the origin, then add the final [edge](../../../../../../edge-of-a-graph.md) to close it.

```
sap <- function(M) {
  stopifnot(length(M) == 1L, is.finite(M), M >= 4,
            M == floor(M), M %% 2 == 0)
  repeat {
    path <- saw(M - 1L)
    if (sum(abs(path[nrow(path), ])) == 1L) {
      return(rbind(path, c(0L, 0L)))
    }
  }
}
```

The output has $M+1$ coordinate rows and $M$ unit edges. The first $M$ vertices are distinct by the call to `saw`; the last row repeats only the origin. Neighbouring lattice edges cannot create an additional crossing without a repeated [vertex](../../../../../../vertex-graph-theory.md). A rectangle of perimeter $M$ exists for every permitted even $M$, giving a positive [probability](../../../../../../probability.md) of eventual acceptance.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
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
