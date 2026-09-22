<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose each row from the [permutations](../../../../../permutation.md) of the symbols:
```
squaresRows :: Int -> [[[Int]]]
squaresRows n
  | n < 0     = error "negative order"
  | otherwise = cp (replicate n (perms [1..n]))

latinRows :: Int -> [[[Int]]]
latinRows = filter valid . squaresRows
```
Every [Latin square](../../../../../latin-square.md) remains a candidate, because each of its rows is one of those [permutations](../../../../../permutation.md). Conversely every candidate has valid rows, so only its columns still need checking. There are **$(n!)^n$** candidates instead of $n^{n^2}$: at order four, $331\,776$ rather than more than four billion. The improvement is substantial but does not make exhaustive generation practical at arbitrary orders. One can replace `valid` by a column-only test here, since row validity is guaranteed by construction.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
