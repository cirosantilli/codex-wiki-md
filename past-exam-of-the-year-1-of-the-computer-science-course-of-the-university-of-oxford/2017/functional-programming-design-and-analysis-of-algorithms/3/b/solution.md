<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The recursive [Cartesian product](../../../../../cartesian-product.md) is:

```
cpRec :: [[a]] -> [[a]]
cpRec [] = [[]]
cpRec (xs:xss) = [x:ys | x <- xs, ys <- cpRec xss]
```

The corresponding [right fold](../../../../../list-fold.md) is:

```
cpFold :: [[a]] -> [[a]]
cpFold = foldr step [[]]
  where
    step :: [a] -> [[a]] -> [[a]]
    step xs acc = [x:ys | x <- xs, ys <- acc]

cp :: [[a]] -> [[a]]
cp = cpRec
```

The base `[[]]` is essential: there is one way to choose from no factors, namely the empty selection. For a nonempty outer list, choose its first coordinate and prepend it to each selection from the remaining factors. This also proves equality with the [right fold](../../../../../list-fold.md) by [structural induction](../../../../../structural-induction.md). An empty factor produces no selections.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
