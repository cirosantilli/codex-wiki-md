<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Clamp a nonpositive count to zero. Taking restricts the domain of present indices; dropping translates that domain:
```
take' :: Int -> List a -> List a
take' count (List f) = List query
  where
    k = max 0 count
    query i
      | i < 0 || i >= k = Nothing
      | otherwise      = f i

drop' :: Int -> List a -> List a
drop' count (List f) = List query
  where
    k = max 0 count
    query i
      | i < 0 || i > maxBound - k = Nothing
      | otherwise                = f (i+k)

length' :: List a -> Int
length' (List f) = countFrom 0
  where
    countFrom i = case f i of
                    Nothing -> i
                    Just _  -> countFrom (i+1)
```
For finite length $m$, the first two operations give lengths $\min(k,m)$ and $\max(m-k,0)$, respectively. The length loop reaches the first absent index, namely $m$, so it terminates for a total finite representation. It does not terminate on an infinite represented [sequence](../../../../../sequence.md). There is no assumption that an arbitrary stored query [function](../../../../../function-split.md) takes constant time.

## ↑ Ancestors (12)

1. [F](../f.md)
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
