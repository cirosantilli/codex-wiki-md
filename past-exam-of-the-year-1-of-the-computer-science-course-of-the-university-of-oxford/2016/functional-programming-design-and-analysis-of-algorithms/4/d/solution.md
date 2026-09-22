<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Generate successive [matrix powers](../../../../../matrix-power.md) and take cumulative sums using [matrix addition](../../../../../matrix-addition.md):
```
seriesMat :: Num a => Matrix a -> [Matrix a]
seriesMat m = scanl1 addMat (iterate (multMat m) m)
```
For the stipulated [square matrix](../../../../../square-matrix.md), `iterate (multMat m) m` produces `m`, `m*m`, `m*(m*m)`, and so on. [Associativity](../../../../../associative-property.md) of exact [matrix multiplication](../../../../../matrix-multiplication.md) identifies these as $M,M^2,M^3,\ldots$. The [left scan](../../../../../left-scan.md) `scanl1 addMat` then returns

$$
\boxed{\left[M,\ M+M^2,\ M+M^2+M^3,\ldots\right]}.
$$

All dimensions remain compatible. The infinite outer [list](../../../../../list-abstract-data-type.md) is available a finite prefix at a time under [lazy evaluation](../../../../../lazy-evaluation.md); no convergence of the [matrix geometric series](../../../../../matrix-geometric-series.md) is needed. With floating-point entries, the expression specifies this particular multiplication and addition order, since machine arithmetic need not obey the exact algebraic laws.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
