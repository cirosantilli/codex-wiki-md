<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Count the number of nonempty levels on the longest root-to-leaf branch, taking the empty [binary search tree](../../../../../binary-search-tree.md) to have depth zero:

```
depth :: STree a -> Integer
depth = foldSTree (\left _ right -> 1 + max left right) 0
```

Thus $\boxed{d(\operatorname{Empty})=0,\quad d(\operatorname{Node}\ l\ x\ r)=1+\max(d(l),d(r))}$. A singleton has depth one under this convention. If [height of a binary tree](../../../../../height-of-a-binary-tree.md) is instead counted in edges, subtract one for a nonempty [tree](../../../../../tree-graph-theory-split.md). The complete [tree fold](../../../../../tree-fold.md) takes $\Theta(n)$ operations.

## ↑ Ancestors (12)

1. [F](../f.md)
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
