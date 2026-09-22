<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Compute either the common depth of the [leaves of a rooted tree](../../../../../leaf-of-a-rooted-tree.md), or failure when the depths differ. A [tree fold](../../../../../tree-fold.md) can return a `Maybe Integer`: `Just h` means that the [rose tree](../../../../../rose-tree.md) is a [perfect rose tree](../../../../../perfect-rose-tree.md) with all leaves at depth $h$ relative to its root; `Nothing` means it is not perfect.
```
perfect :: RTree a -> Bool
perfect t =
  case foldRTree step t of
    Nothing -> False
    Just _  -> True
  where
    step :: a -> [Maybe Integer] -> Maybe Integer
    step _ [] = Just 0
    step _ (Nothing : _) = Nothing
    step _ (Just h : hs)
      | all (== Just h) hs = Just (h + 1)
      | otherwise        = Nothing
```
A leaf has depth zero. An internal [vertex](../../../../../vertex-graph-theory.md) has equally deep leaves exactly when every child [rose tree](../../../../../rose-tree.md) is perfect and their returned depths agree; adding one accounts for the edge to each child. This proves the stated meaning of the result by [structural induction](../../../../../structural-induction.md). In particular, unary branching is allowed, and a single leaf is perfect. **`perfect` returns precisely the required Boolean.** Its [time complexity](../../../../../time-complexity.md) is linear in the number of [vertices](../../../../../vertex-graph-theory.md), assuming unit-cost depth arithmetic; labels are never compared or evaluated.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
