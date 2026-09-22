<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Inspect index zero for emptiness and the head; removing the head shifts the query in the other direction:
```
null' :: List a -> Bool
null' (List f) = case f 0 of
                  Nothing -> True
                  Just _  -> False

head' :: List a -> a
head' (List f) = case f 0 of
                  Nothing -> error "head of empty representation"
                  Just x  -> x

tail' :: List a -> List a
tail' input@(List f)
  | null' input = error "tail of empty representation"
  | otherwise   = List query
  where
    query i
      | i < 0 || i == maxBound = Nothing
      | otherwise             = f (i+1)
```
The no-holes [invariant](../../../../../invariant-mathematics.md) makes the zero-index test sufficient for emptiness. Both `head'` and `tail'` have the [precondition](../../../../../precondition.md) that the representation is nonempty and signal an error when it is violated. On a nonempty representation, `tail'` removes exactly one position. The overflow guard is consistent with finite lengths at most `maxBound`.

## ↑ Ancestors (12)

1. [D](../d.md)
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
