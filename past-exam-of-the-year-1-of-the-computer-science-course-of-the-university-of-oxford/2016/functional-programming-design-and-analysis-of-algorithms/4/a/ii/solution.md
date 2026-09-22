<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With `dimensions` as in part (i), the alternative definition is
```
addMat :: Num a => Matrix a -> Matrix a -> Matrix a
addMat a b
  | dimensions a /= dimensions b = error "addMat: incompatible sizes"
  | otherwise = zipWith (zipWith (+)) a b
```
The inner `zipWith` adds corresponding entries; the outer one applies that row operation to corresponding rows. **This computes the same [matrix addition](../../../../../../matrix-addition.md)**, with the same rejection of unequal dimensions. Under the valid-input assumptions, either implementation takes $\Theta(mn)$ unit-cost arithmetic work for $m\times n$ inputs.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
