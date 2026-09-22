<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Emit the root label, then concatenate the [depth-first traversals](../../../../../../depth-first-search.md) of the child [rose trees](../../../../../../rose-tree.md) in order:

```
dft :: RTree a -> [a]
dft (Node x ts) = x : concatMap dft ts
```

This is [preorder traversal](../../../../../../preorder-traversal.md):

$$
\boxed{\operatorname{dft}(\operatorname{Node}\ x\ [t_1,\ldots,t_k])=[x]\mathbin{++}\operatorname{dft}(t_1)\mathbin{++}\cdots\mathbin{++}\operatorname{dft}(t_k).}
$$

The [Haskell concatMap function](../../../../../../haskell-concatmap-function.md) preserves child order and finishes each child subtree before moving to the next. A leaf yields its singleton label; the source example yields `[1,2,3,4,5,6,7]`.

## ↑ Ancestors (13)

1. [I](../i.md)
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
