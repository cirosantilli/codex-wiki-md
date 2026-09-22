<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Retain the first element, filter all its further occurrences out of the tail, and recurse:

```
removedup :: Eq a => [a] -> [a]
removedup []     = []
removedup (x:xs) = x : removedup (filter (/= x) xs)
```

The boxed specification is $\boxed{\text{each distinct input value occurs once, in first-occurrence order}}$. The [Haskell type class](../../../../../haskell-type-class.md) `Eq` is needed for comparing values. [Structural induction](../../../../../structural-induction.md) on a finite [list](../../../../../list-abstract-data-type.md) proves [duplicate removal](../../../../../duplicate-removal.md): filtering removes every further `x`, and the recursive result contains each remaining distinct value exactly once. In the worst case of all distinct values, successive filters give quadratic [time complexity](../../../../../time-complexity.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
