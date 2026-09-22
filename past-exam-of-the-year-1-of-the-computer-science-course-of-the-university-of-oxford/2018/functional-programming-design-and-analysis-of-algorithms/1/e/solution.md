<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Emit the root [subtree](../../../../../subtree.md) first, then the occurrences inside its children:

```
subs :: Tree a -> [Tree a]
subs t@(One _)   = [t]
subs t@(Two l r) = t : (subs l ++ subs r)
```

This is a [preorder traversal](../../../../../preorder-traversal.md) of [subtree](../../../../../subtree.md) occurrences. Equal-valued occurrences are retained: the answer is a [list](../../../../../list-abstract-data-type.md), not a deduplicated [set](../../../../../set-split.md). Every occurrence is either the root or lies in exactly one child, which proves completeness by [structural induction](../../../../../structural-induction.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
