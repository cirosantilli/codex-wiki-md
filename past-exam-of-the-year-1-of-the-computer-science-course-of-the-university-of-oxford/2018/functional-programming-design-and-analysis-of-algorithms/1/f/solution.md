<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The head of each recursively obtained [list](../../../../../list-abstract-data-type.md) is the original child. Hence the [tree fold](../../../../../tree-fold.md) has retained enough information to reconstruct the parent:

```
subs :: Tree a -> [Tree a]
subs = fold (\x -> [One x]) combine
  where
    combine ls rs = Two (head ls) (head rs) : (ls ++ rs)
```

The invariant is that every folded result is nonempty and begins with the [subtree](../../../../../subtree.md) being folded. It holds at `One`; the displayed combining operation preserves it at `Two`. Thus neither use of `head` encounters an empty [list](../../../../../list-abstract-data-type.md), and the remaining entries agree with the recursive [preorder traversal](../../../../../preorder-traversal.md).

## ↑ Ancestors (12)

1. [F](../f.md)
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
