<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [tree fold](../../../../../tree-fold.md) replaces `Empty` by a seed and `Node` by a combining [function](../../../../../function-split.md). The combining [function](../../../../../function-split.md) receives the already folded left subtree, the node's label and the already folded right subtree:

```
foldSTree :: (b -> a -> b -> b) -> b -> STree a -> b
foldSTree combine empty Empty = empty
foldSTree combine empty (Node left x right) =
  combine (foldSTree combine empty left)
          x
          (foldSTree combine empty right)
```

Its [polymorphic](../../../../../programming-language-polymorphism.md) [type signature](../../../../../type-signature.md) is

$$
\boxed{(\beta\to\alpha\to\beta\to\beta)\to\beta\to\mathrm{STree}\ \alpha\to\beta.}
$$

The result type need not be the label type: it may be a [list](../../../../../list-abstract-data-type.md), a number or another structure. No ordering constraint is needed because this [tree fold](../../../../../tree-fold.md) follows constructors without comparing labels.

## ↑ Ancestors (12)

1. [C](../c.md)
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
