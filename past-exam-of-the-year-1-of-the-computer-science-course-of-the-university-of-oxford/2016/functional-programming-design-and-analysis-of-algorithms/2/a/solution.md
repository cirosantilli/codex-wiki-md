<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [tree fold](../../../../../tree-fold.md) first folds every child [rose tree](../../../../../rose-tree.md), then supplies the resulting [list](../../../../../list-abstract-data-type.md) and the current label to the combining function:
```
foldRTree :: (a -> [b] -> b) -> RTree a -> b
foldRTree f (Node x children) =
  f x (map (foldRTree f) children)
```
The label type `a` and result type `b` are independent, so the [polymorphic type](../../../../../polymorphic-type.md) needs no class constraint. With `f x ys = x + sum ys`, every label is counted exactly once; the illustrated labels sum to **28**.

The printed source gives the signature `exampleRTree` but binds `exampleRTRee`, with different capitalization. They are different [Haskell](../../../../../haskell.md) names; the demonstration requires using one spelling consistently. This typo does not affect the [tree fold](../../../../../tree-fold.md) definition.

## ↑ Ancestors (12)

1. [A](../a.md)
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
