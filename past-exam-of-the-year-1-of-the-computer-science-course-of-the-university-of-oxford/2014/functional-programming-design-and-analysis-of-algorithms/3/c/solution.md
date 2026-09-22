<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [rose tree](../../../../../rose-tree.md), fold each child recursively, retaining their order, and supply the resulting [list](../../../../../list-abstract-data-type.md) with the current label to the combining function:

```
foldRTree :: (a -> [b] -> b) -> RTree a -> b
foldRTree f (Node x ts) = f x (map (foldRTree f) ts)
```

The defining [tree fold](../../../../../tree-fold.md) equation is $\boxed{\operatorname{foldRTree}\ f\ (\operatorname{Node}\ x\ ts)=f\ x\ (\operatorname{map}(\operatorname{foldRTree}\ f)\ ts)}$. A leaf passes `[]` as the list of child results; an internal node passes one result per child. Thus the combining function controls both cases without a separate leaf constructor.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
