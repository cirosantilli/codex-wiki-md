<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

An unfold expands a seed into either no node or a bucket and two new seeds:
```
unfoldTree :: (s -> Maybe (s,[a],s)) -> s -> Tree a
unfoldTree split seed =
  case split seed of
    Nothing -> Empty
    Just (left,equal,right) ->
      Node (unfoldTree split left) equal (unfoldTree split right)

toTreeUnfold :: Ord a => [a] -> Tree a
toTreeUnfold = unfoldTree split
  where
    split [] = Nothing
    split (pivot:xs) =
      let (lo,eq,hi) = partition3 pivot xs
      in Just (lo,pivot:eq,hi)
```
The seed is the remaining [list](../../../../../list-abstract-data-type.md). Expanding a nonempty seed partitions it exactly as `toTree` does, and both child seeds are shorter. [Induction](../../../../../mathematical-induction.md) establishes **`toTreeUnfold = toTree`** and [algorithm termination](../../../../../algorithm-termination.md) on finite inputs. The unfold separates the local decomposition rule from the recursive construction of the tree.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
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
