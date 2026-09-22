<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The child results supplied by the [tree fold](../../../../../../tree-fold.md) are already their [depth-first traversals](../../../../../../depth-first-search.md). Prepend the current label to their [list concatenation](../../../../../../list-concatenation.md):

```
dftF :: RTree a -> [a]
dftF = foldRTree visit
  where
    visit :: a -> [[a]] -> [a]
    visit x childLists = x : concat childLists
```

Thus $\boxed{\operatorname{dftF}=\operatorname{foldRTree}\bigl(\lambda x\ rs.\ x:\operatorname{concat}(rs)\bigr)}$. Substituting the equation for the [tree fold](../../../../../../tree-fold.md) gives exactly the recursive [preorder traversal](../../../../../../preorder-traversal.md) equation from part (i), proving equality by [structural induction](../../../../../../structural-induction.md) on a finite [rose tree](../../../../../../rose-tree.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
