<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With nonpositive counts treated as in the standard [list](../../../../../list-abstract-data-type.md) operations:
```
takeSeq :: Integer -> Seq a -> Seq a
takeSeq n s
  | n <= 0 = const []
  | otherwise = \v -> takeWhile (< n) (s v)

dropSeq :: Integer -> Seq a -> Seq a
dropSeq n s
  | n <= 0 = s
  | otherwise = \v -> map (subtract n) (dropWhile (< n) (s v))
```
An occurrence survives `takeSeq n` exactly when its original index is less than $n$, and its index stays unchanged. It survives `dropSeq n` exactly when its original index is at least $n$, and its new index is the original one minus $n$. Sorted occurrence lists justify `takeWhile` and `dropWhile`. No equality constraint on the element type is needed because the operations only transform positions. The first guard also lets `takeSeq 0 s v` return `[]` without inspecting `s v`.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
