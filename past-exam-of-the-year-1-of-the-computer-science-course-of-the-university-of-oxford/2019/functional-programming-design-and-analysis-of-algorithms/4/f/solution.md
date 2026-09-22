<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Merge the rows with `fairConcat`, retaining explicit empty-input cases:

```
fairPair :: (a -> b -> c) -> [a] -> [b] -> [c]
fairPair _ [] _  = []
fairPair _ _  [] = []
fairPair f xs ys = fairConcat [[f x y | y <- ys] | x <- xs]
```

For nonempty [proper lazy lists](../../../../../proper-lazy-list.md), the occurrence `f (xs!!i) (ys!!j)` belongs to row $i$, position $j$, so the proof in part d puts it in round $i+j$. This supplies **every pair after finite work**, even when both input [lists](../../../../../list-abstract-data-type.md) are infinite. The guards also return `[]` for either empty factor without traversing infinitely many empty rows.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
