<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The empty representation is nowhere present; prepending shifts all old positions by one:
```
nil' :: List a
nil' = List (\_ -> Nothing)

cons' :: a -> List a -> List a
cons' x (List f) = List query
  where
    query i
      | i < 0     = Nothing
      | i == 0    = Just x
      | otherwise = f (i-1)
```
For a represented length $m$, `cons'` represents length $m+1$, provided that length is representable. Index zero is the new head and each later valid index asks for the preceding old position. The no-holes [invariant](../../../../../invariant-mathematics.md) is preserved. No conventional [list](../../../../../list-abstract-data-type.md) is built by either constructor.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
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
