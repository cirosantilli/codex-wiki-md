<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Share the recursive pair and inspect the [predicate](../../../../../predicate.md) once:
```
partition :: (a -> Bool) -> [a] -> ([a],[a])
partition _ [] = ([],[])
partition p (x:xs)
  | p x       = (x:yes,no)
  | otherwise = (yes,x:no)
  where ~(yes,no) = partition p xs
```
For a finite [list](../../../../../list-abstract-data-type.md), [structural induction](../../../../../structural-induction.md) establishes that `yes` and `no` are the two required filtered subsequences. The guard evaluates `p x` once and prepends `x` to exactly one output, preserving input order in both. Fully consuming both results uses $n$ [predicate](../../../../../predicate.md) applications and $\Theta(n)$ additional work. Sharing the recursive result avoids making separate recursive traversals. This is a [stable list partition](../../../../../stable-list-partition.md).

## ↑ Ancestors (12)

1. [E](../e.md)
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
