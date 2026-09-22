<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Reuse `dimensions` and either [transpose](../../../../../transpose.md) definition above:
```
multMat :: Num a => Matrix a -> Matrix a -> Matrix a
multMat a b
  | colsA /= rowsB = error "multMat: incompatible sizes"
  | otherwise = [[sum (zipWith (*) row col) | col <- columnsB]
                                           | row <- a]
  where
    (_,colsA) = dimensions a
    (rowsB,_) = dimensions b
    columnsB = transpose b
```
For $A$ of size $m\times n$ and $B$ of size $n\times p$, every selected row and column has length $n$. Their [dot product](../../../../../dot-product.md) is

$$
\boxed{(AB)_{ij}=\sum_{k=1}^{n}a_{ik}b_{kj}}.
$$

The two [list comprehensions](../../../../../list-comprehension.md) place this entry in row $i$, column $j$ of an $m\times p$ result. The dimension guard checks exactly the compatibility condition for [matrix multiplication](../../../../../matrix-multiplication.md). The shared `columnsB` avoids recomputing the [transpose](../../../../../transpose.md) for each row; the arithmetic cost is $\Theta(mnp)$ in the unit-cost model.

## ↑ Ancestors (12)

1. [C](../c.md)
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
