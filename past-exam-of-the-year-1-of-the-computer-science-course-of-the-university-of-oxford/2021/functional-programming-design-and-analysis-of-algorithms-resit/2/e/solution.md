<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A [tree fold](../../../../../tree-fold.md) replaces each constructor by its interpretation:
```
foldTree :: (b -> [a] -> b -> b) -> b -> Tree a -> b
foldTree combine zero Empty = zero
foldTree combine zero (Node left equal right) =
  combine (foldTree combine zero left)
          equal
          (foldTree combine zero right)

fromTreeFold :: Tree a -> [a]
fromTreeFold = foldTree (\left equal right -> left ++ equal ++ right) []
```
[Induction](../../../../../mathematical-induction.md) on the finite tree shows equality with `fromTree`: the empty tree produces the empty output, and the combining [function](../../../../../function-split.md) concatenates the two correctly flattened children around the node's bucket. The result type $b$ is independent of the key type; other choices can compute a size or another summary using the same [structural recursion](../../../../../structural-recursion.md).

## ↑ Ancestors (12)

1. [E](../e.md)
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
