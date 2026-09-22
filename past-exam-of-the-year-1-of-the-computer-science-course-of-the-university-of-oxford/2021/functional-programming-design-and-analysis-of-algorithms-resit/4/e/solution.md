<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Preserve absence and transform only a present value:
```
map' :: (a -> b) -> List a -> List b
map' g (List f) = List (\i -> case f i of
                              Nothing -> Nothing
                              Just x  -> Just (g x))
```
Every query keeps its presence status, so the represented length and the no-holes [invariant](../../../../../invariant-mathematics.md) are unchanged. The transformed element is computed only when demanded.

## ↑ Ancestors (12)

1. [E](../e.md)
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
