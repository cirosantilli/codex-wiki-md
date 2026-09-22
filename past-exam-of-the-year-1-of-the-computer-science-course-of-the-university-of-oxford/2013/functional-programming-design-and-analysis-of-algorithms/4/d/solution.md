<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the empty [list](../../../../../list-abstract-data-type.md) for an empty subtree, and join the left result, the current label and the right result:

```
flatten :: STree a -> [a]
flatten = foldSTree (\left x right -> left ++ (x : right)) []
```

Thus $\boxed{\operatorname{flatten}(\operatorname{Node}\ l\ x\ r)=\operatorname{flatten}(l)\mathbin{+\!+}[x]\mathbin{+\!+}\operatorname{flatten}(r)}$. This is an [inorder traversal](../../../../../inorder-traversal.md). By [structural induction](../../../../../structural-induction.md), each subtree produces its labels in order; the [binary search tree](../../../../../binary-search-tree.md) invariant places every left label below $x$ and every right label above $x$, proving that the whole result is increasing. The definition works for any binary-tree shape, although its result is sorted only when the ordering invariant holds. Repeated [list concatenation](../../../../../list-concatenation.md) can give quadratic cost on a left chain; the question asks for a [tree fold](../../../../../tree-fold.md) definition, rather than an optimal traversal implementation.

## ↑ Ancestors (12)

1. [D](../d.md)
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
