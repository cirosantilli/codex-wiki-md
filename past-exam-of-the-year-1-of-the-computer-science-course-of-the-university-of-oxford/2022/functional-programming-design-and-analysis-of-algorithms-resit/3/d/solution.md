<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [list unfold](../../../../../list-unfold.md) operation has the following [type signature](../../../../../type-signature.md) and definition:
```
unfoldr :: (s -> Maybe (a,s)) -> s -> [a]
unfoldr step s = case step s of
  Nothing     -> []
  Just (x,s') -> x : unfoldr step s'

groupUnfold :: Eq a => [a] -> [[a]]
groupUnfold = unfoldr next
  where
    next [] = Nothing
    next (x:xs) = Just (x:ys,zs)
      where (ys,zs) = span (== x) xs
```
The seed is the unprocessed [suffix of a list](../../../../../suffix-of-a-list.md). An empty seed terminates the unfold; otherwise `next` returns the first maximal run and precisely the seed for the next call. Substituting the definition of `unfoldr` recovers part (c)'s equations, proving correctness. The `Just` pair and first group constructor can be produced before `span` finishes, retaining the same [lazy evaluation](../../../../../lazy-evaluation.md) behaviour.

## ↑ Ancestors (12)

1. [D](../d.md)
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
