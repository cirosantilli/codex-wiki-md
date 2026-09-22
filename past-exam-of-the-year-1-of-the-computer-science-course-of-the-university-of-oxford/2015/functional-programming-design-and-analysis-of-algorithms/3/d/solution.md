<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [principal type](../../../../../principal-type.md) needs an [equality type class](../../../../../eq-type-class.md) constraint:
```
isPrefix :: Eq a => [a] -> [a] -> Bool
isPrefix [] _ = True
isPrefix (_:_) [] = False
isPrefix (x:xs) (y:ys) = x == y && isPrefix xs ys
```
The empty [list](../../../../../list-abstract-data-type.md) is a [prefix](../../../../../prefix-of-a-list.md) of every [list](../../../../../list-abstract-data-type.md), witnessed by the second list itself as the remaining suffix. A nonempty prefix cannot fit in the empty [list](../../../../../list-abstract-data-type.md). Otherwise the first elements must agree, and the remaining first list must be a [prefix](../../../../../prefix-of-a-list.md) of the remaining second list. These cases prove correctness by [structural induction](../../../../../structural-induction.md) on the candidate prefix. The `Eq a` constraint is required by `x == y`; no ordering constraint is needed.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
