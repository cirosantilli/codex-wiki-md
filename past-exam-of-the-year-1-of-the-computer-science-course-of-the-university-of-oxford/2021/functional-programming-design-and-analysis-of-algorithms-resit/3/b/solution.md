<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a nonnegative order, first enumerate every possible row and then every possible ordered selection of rows:
```
squares :: Int -> [[[Int]]]
squares n
  | n < 0     = error "negative order"
  | otherwise = cp (replicate n (cp (replicate n [1..n])))
```
Every one of the $n^2$ positions chooses one of $n$ symbols independently. Consequently the enumeration contains **$n^{n^2}$** candidate squares for $n\geq1$, each exactly once. The conventional order-zero extension produces one empty square. This is generation only; repeated symbols have not yet been rejected.

## ↑ Ancestors (12)

1. [B](../b.md)
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
