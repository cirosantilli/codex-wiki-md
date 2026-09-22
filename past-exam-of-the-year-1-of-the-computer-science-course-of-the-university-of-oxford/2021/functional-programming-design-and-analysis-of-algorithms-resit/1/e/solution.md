<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the finite total inputs just specified, a recursive implementation is
```
spanP :: (a -> Bool) -> [a] -> ([a], [a])
spanP p [] = ([], [])
spanP p whole@(x:xs)
  | p x       = let (ys,zs) = spanP p xs in (x:ys,zs)
  | otherwise = ([],whole)
```
At a true test, the head belongs to the [list prefix](../../../../../prefix-of-a-list.md) and splitting continues on the tail; at a false test, the complete remaining [list](../../../../../list-abstract-data-type.md) is the [list suffix](../../../../../suffix-of-a-list.md). [Induction](../../../../../mathematical-induction.md) proves that the first projection is the longest accepted [list prefix](../../../../../prefix-of-a-list.md) and the second projection is the remaining [list suffix](../../../../../suffix-of-a-list.md).

There is a small partial-value distinction behind the paper's displayed pair identity. The conventional recursive `span` is strict in an entirely undefined [list](../../../../../list-abstract-data-type.md), whereas the literal expression `(takeWhile p undefined, dropWhile p undefined)` exposes an outer pair with two undefined components. The equality as a pair therefore needs the stated defined-input convention, or an interpretation that compares the two projections. This does not affect the finite total answers here.[§3.17, pattern matching; Chapter 9, definitions of span and the prefix operations](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
