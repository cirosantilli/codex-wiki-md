<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [pattern matching](../../../../../pattern-matching.md) on the two [data constructors](../../../../../data-constructor.md), concatenating the left [subtree](../../../../../subtree.md)'s [inorder traversal](../../../../../inorder-traversal.md), the root label, and the right [subtree](../../../../../subtree.md)'s [inorder traversal](../../../../../inorder-traversal.md):
```
data Tree = Leaf | Fork Tree Int Tree

inorder :: Tree -> [Int]
inorder Leaf = []
inorder (Fork l x r) = inorder l ++ [x] ++ inorder r
```
Here `Leaf` represents the empty [binary tree](../../../../../binary-tree.md), rather than a labelled leaf. The printed declaration uses `type`; an executable [Haskell](../../../../../haskell.md) [algebraic data type](../../../../../algebraic-data-type.md) requires `data`, as above. By [structural induction](../../../../../structural-induction.md), the two equations return precisely the prescribed [inorder traversal](../../../../../inorder-traversal.md):

$$
\boxed{\operatorname{inorder}(\operatorname{Fork}(l,x,r))=\operatorname{inorder}(l)\mathbin{++}[x]\mathbin{++}\operatorname{inorder}(r).}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
