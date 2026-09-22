<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The direct [tree fold](../../../../../tree-fold.md) for an inorder traversal is
```
flattenFold :: Tree a -> [a]
flattenFold = foldTree (\ls x rs -> ls ++ (x:rs)) []
```
By [structural induction](../../../../../structural-induction.md), the child lists are ascending; the [binary search tree](../../../../../binary-search-tree.md) property places every left value below the root and every right value above it. The displayed [list concatenation](../../../../../list-concatenation.md) therefore gives an ascending list containing every stored value exactly once.

For a version with linear [time complexity](../../../../../time-complexity.md) on every tree shape, use an accumulator:
```
flatten :: Tree a -> [a]
flatten t = onto t []
  where
    onto Empty zs = zs
    onto (Tree l x r) zs = onto l (x : onto r zs)
```
This also has a higher-order [tree fold](../../../../../tree-fold.md) expression using [difference lists](../../../../../difference-list.md):
```
flattenLinear :: Tree a -> [a]
flattenLinear t =
  foldTree (\l x r -> l . (x:) . r) id t []
```
Its folded value is a function that prepends the inorder traversal to a supplied tail. The accumulator invariant is `onto t zs = flattenFold t ++ zs`. Each node contributes one constructor, giving $\Theta(n)$ time to consume the output. By contrast, the direct list-valued fold can take $\Theta(n^2)$ on a left-skewed tree because `++` repeatedly copies left traversals.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
