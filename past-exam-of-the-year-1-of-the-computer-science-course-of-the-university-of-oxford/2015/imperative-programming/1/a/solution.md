<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In executable [Haskell](../../../../../haskell.md), the [algebraic data type](../../../../../algebraic-data-type.md) declaration uses `data`, rather than the printed `type`. A [leaf of a rooted tree](../../../../../leaf-of-a-rooted-tree.md) contributes `False`; a fork contributes `True` followed by its left and right [subtrees](../../../../../subtree.md) in that order.
```
data Tree = Leaf | Fork Tree Tree

preorder :: Tree -> [Bool]
preorder Leaf       = [False]
preorder (Fork l r) = True : (preorder l ++ preorder r)
```
This is a [preorder traversal](../../../../../preorder-traversal.md) of a [full binary tree](../../../../../full-binary-tree.md), including the [leaves](../../../../../leaf-of-a-rooted-tree.md). [Structural induction](../../../../../structural-induction.md) proves correctness: the [leaf of a rooted tree](../../../../../leaf-of-a-rooted-tree.md) case has precisely one output, and the fork case concatenates the correct [preorder traversals](../../../../../preorder-traversal.md) of its two [subtrees](../../../../../subtree.md) after its own marker.

An equivalent version avoids repeatedly copying the left [list](../../../../../list-abstract-data-type.md) through [list concatenation](../../../../../list-concatenation.md):
```
preorder t = walk t []
  where
    walk Leaf rest       = False : rest
    walk (Fork l r) rest = True : walk l (walk r rest)
```
Its strengthening is `walk t rest = preorder t ++ rest`. Each [vertex](../../../../../vertex-graph-theory.md) constructs one [list](../../../../../list-abstract-data-type.md) cell, so this version has linear [time complexity](../../../../../time-complexity.md). The concise result is

$$
\boxed{P(\mathrm{Leaf})=[\mathrm{False}],\quad P(\mathrm{Fork}(l,r))=[\mathrm{True}]\mathbin{+\!+}P(l)\mathbin{+\!+}P(r).}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
