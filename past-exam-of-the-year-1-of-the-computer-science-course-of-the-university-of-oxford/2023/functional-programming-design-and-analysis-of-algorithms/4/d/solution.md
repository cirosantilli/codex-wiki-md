<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the remaining ascending [list](../../../../../list-abstract-data-type.md) itself as the seed:
```
buildUnfold :: [a] -> Tree a
buildUnfold = unfoldTree split
  where
    split [] = Nothing
    split xs =
      let (ls,x:rs) = splitAt (length xs `div` 2) xs
      in Just (ls,x,rs)
```
The empty seed produces `Empty`. Every nonempty seed produces exactly the midpoint and two child seeds used by `build`. Thus the defining equations agree, and [structural induction](../../../../../structural-induction.md) on the finite input proves `buildUnfold xs = build xs`. The balance and ordering arguments carry over unchanged.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
