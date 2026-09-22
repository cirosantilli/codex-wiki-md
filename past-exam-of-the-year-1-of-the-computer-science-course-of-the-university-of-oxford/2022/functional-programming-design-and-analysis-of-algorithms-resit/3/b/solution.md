<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the same step from part (a):
```
groupFold :: Eq a => [a] -> [[a]]
groupFold = foldr prependRun []
```
The [right fold](../../../../../list-fold.md) obeys `groupFold [] = []` and `groupFold (x:xs) = prependRun x (groupFold xs)`, exactly the recursive equations already proved. Both implementations give the [bottom value](../../../../../bottom-value.md) for an entirely undefined input spine. Their equal behaviour on finite [partial lists](../../../../../partial-list.md), together with definable continuity, establishes equality on infinite [lazy lists](../../../../../lazy-list.md) as well. The helper's irrefutable binding is what lets the first run be produced without demanding that all subsequent runs already exist.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
