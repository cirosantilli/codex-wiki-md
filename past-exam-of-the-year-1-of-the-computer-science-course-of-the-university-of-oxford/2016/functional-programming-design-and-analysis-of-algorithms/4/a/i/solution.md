<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the source's `type Matrix a = [[a]]`. For its nonempty rectangular [matrices](../../../../../../matrix.md), the number of rows and the first row's length determine the dimensions:
```
dimensions :: Matrix a -> (Int,Int)
dimensions rows = (length rows, length (head rows))

addMat :: Num a => Matrix a -> Matrix a -> Matrix a
addMat a b
  | dimensions a /= dimensions b = error "addMat: incompatible sizes"
  | otherwise = [[x + y | (x,y) <- zip r s]
                         | (r,s) <- zip a b]
```
The outer [list comprehension](../../../../../../list-comprehension.md) pairs corresponding rows; the inner one pairs corresponding entries. Checking both dimensions before using `zip` prevents silent truncation. Thus **the result has entries $c_{ij}=a_{ij}+b_{ij}$**, the definition of [matrix addition](../../../../../../matrix-addition.md). The `Num` constraint supplies the addition operation.

## ↑ Ancestors (13)

1. [I](../i.md)
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
