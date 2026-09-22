<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the paper's [leaf-labelled binary tree](../../../../../leaf-labelled-binary-tree.md), the combining operation receives the results of the two subtrees, and the other argument handles a leaf:

```
foldTree :: (a -> b) -> (b -> b -> b) -> Tree a -> b
foldTree f g (One x)   = f x
foldTree f g (Two l r) = g (foldTree f g l) (foldTree f g r)
```

Its constructor equation is **`foldTree One Two = id`**. More generally, a [function](../../../../../function-split.md) `h` satisfying `h (One x) = f x` and `h (Two l r) = g (h l) (h r)` equals `foldTree f g` on finite [trees](../../../../../tree-graph-theory-split.md), by [structural induction](../../../../../structural-induction.md). This is the [tree fold](../../../../../tree-fold.md) specialized to a datatype with labels only at leaves, rather than at internal nodes.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
