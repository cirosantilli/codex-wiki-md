<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Follow the unique branch in which the new key could belong. At an equal key, keep the existing node so that duplicate insertion does not change the represented [set](../../../../../set-split.md):

```
insert :: Ord a => a -> STree a -> STree a
insert y Empty = Node Empty y Empty
insert y (Node left x right) =
  case compare y x of
    LT -> Node (insert y left) x right
    EQ -> Node left x right
    GT -> Node left x (insert y right)
```

The [Haskell Ord class](../../../../../haskell-ord-class.md) supplies the three-way comparison. Each visited nonempty node costs one such comparison; rebuilding a node preserves all untouched subtrees. The inserted key satisfies every comparison along its search path, so it obeys both the local and ancestor [binary search tree](../../../../../binary-search-tree.md) inequalities.

For [height of a binary tree](../../../../../height-of-a-binary-tree.md) $h$, the worst search costs $\boxed{\Theta(h)\text{ comparisons}}$ when it reaches the bottom. With $n$ existing nodes, a chain can require $n$ comparisons, giving a worst case of $\Theta(n)$. Under the standard random-insertion model, distinct keys arrive in a uniformly random order and the expected path length is $\Theta(\log(n+1))$. Thus the usual average-case answer is $\boxed{\Theta(\log n)}$ for growing $n$, but this expectation needs the stated distribution: an arbitrary unbalanced [binary search tree](../../../../../binary-search-tree.md) has no logarithmic guarantee.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
