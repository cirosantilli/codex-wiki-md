<h1 id="3/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [list unfold](../../../../../../list-unfold.md) needs an explicit state describing the unvisited work. Use a [list](../../../../../../list-abstract-data-type.md) of pending [rose trees](../../../../../../rose-tree.md), with the next tree first. Emit that tree's root label, and replace it by its children followed by the remaining pending trees:

```
dftU :: RTree a -> [a]
dftU t = unfold null label advance [t]
  where
    label :: [RTree a] -> a
    label (Node x _ : _) = x

    advance :: [RTree a] -> [RTree a]
    advance (Node _ children : rest) = children ++ rest
```

The boxed state transition is $\boxed{\operatorname{Node}(x,children):rest\ \longmapsto\ children\mathbin{++}rest}$, with output $x$. The stopping test prevents either helper from being applied to `[]`.

The [loop invariant](../../../../../../loop-invariant.md) is that concatenating the [depth-first traversals](../../../../../../depth-first-search.md) of the pending trees gives exactly the unproduced output. Removing the next root emits its first label; replacing that tree by its children preserves the remainder of that [preorder traversal](../../../../../../preorder-traversal.md). Adding children at the front realizes an [explicit-stack depth-first tree traversal](../../../../../../explicit-stack-depth-first-tree-traversal.md); placing them at the end would give a different visiting order. The first states for the source example have roots `[1]`, `[2,5,6]`, `[3,4,5,6]`, `[4,5,6]`, `[5,6]`, `[6]`, `[7]`, `[]`.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
