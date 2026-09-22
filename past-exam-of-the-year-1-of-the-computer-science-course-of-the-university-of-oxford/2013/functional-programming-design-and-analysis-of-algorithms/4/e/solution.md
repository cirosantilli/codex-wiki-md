<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

An empty [binary search tree](../../../../../binary-search-tree.md) has zero nodes; a nonempty node contributes one in addition to the sizes of its two subtrees:

```
size :: STree a -> Integer
size = foldSTree (\left _ right -> 1 + left + right) 0
```

The answer is $\boxed{|\operatorname{Empty}|=0,\quad|\operatorname{Node}\ l\ x\ r|=1+|l|+|r|}$. The [tree fold](../../../../../tree-fold.md) visits every node once, so this takes $\Theta(n)$ arithmetic operations for $n$ nodes.

## ↑ Ancestors (12)

1. [E](../e.md)
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
