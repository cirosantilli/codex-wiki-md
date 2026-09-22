<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Repeated root removal gives the conventional [list](../../../../../list-abstract-data-type.md):
```
toList :: List a -> [a]
toList rs
  | null rs   = []
  | otherwise = head rs : toList (tail rs)
```
The representation interpretation satisfies `toList (cons x rs) = x : toList rs`; alternatively, [structural induction](../../../../../structural-induction.md) on the number of stored elements proves that each step emits exactly the next [preorder traversal](../../../../../preorder-traversal.md) value. The output has $n$ cons cells, and each step takes [constant time](../../../../../constant-time.md), so fully consuming it costs **$\Theta(n)$ time**. No repeated [list concatenation](../../../../../list-concatenation.md) is needed.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [2](../../2.md)
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
