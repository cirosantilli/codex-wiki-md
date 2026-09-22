<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Compare the two heads, emitting one copy of a tie and advancing both inputs in that case:

```
merge :: Ord a => [a] -> [a] -> [a]
merge [] ys = ys
merge xs [] = xs
merge xs@(x:xt) ys@(y:yt)
  | x < y     = x : merge xt ys
  | x > y     = y : merge xs yt
  | otherwise = x : merge xt yt
```

The emitted head is the smallest remaining value, so [induction](../../../../../mathematical-induction.md) preserves strict order and removes duplicates. The extra empty-input cases also make the definition useful on finite lists.

There is a mathematical qualification to the unrestricted infinite-input claim: the union must be enumerable in this order. If one input increases to one from below and the other starts at two, no finite output position can contain two. [Locally finite sorted-stream merge](../../../../../locally-finite-sorted-stream-merge.md) excludes this obstruction, and applies to the positive [integer](../../../../../integer-split.md) streams needed below.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
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
