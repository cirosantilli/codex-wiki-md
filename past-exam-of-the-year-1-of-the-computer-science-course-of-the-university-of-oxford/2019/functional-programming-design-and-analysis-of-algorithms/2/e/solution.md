<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $n$ be the number of leaves; the total number of nodes is $2n-1$. [List concatenation](../../../../../list-concatenation.md) copies its left operand. For a [tree](../../../../../tree-graph-theory-split.md) whose left subtree contains $n-1$ leaves at each successive internal node, these copied lengths are $1,2,\ldots,n-1$. Their [sum](../../../../../sum.md) is $n(n-1)/2$, so the worst-case [running time](../../../../../running-time.md) is **$\Theta(n^2)$**.

A [difference list](../../../../../difference-list.md) representation avoids copying prefixes:

```
flattenFast :: Tree a -> [a]
flattenFast t = go t []
  where
    go (One x)   acc = x:acc
    go (Two l r) acc = go l (go r acc)
```

The [recursion invariant](../../../../../recursion-invariant.md) is `go t acc = flatten t ++ acc`. The leaf case is immediate; the internal-node case uses [associativity](../../../../../associative-property.md) of [list concatenation](../../../../../list-concatenation.md). Each node is visited once and each leaf contributes one output constructor, giving **$\Theta(n)$ [running time](../../../../../running-time.md)** when the result is fully consumed. This is [linear flattening of a binary tree](../../../../../linear-flattening-of-a-binary-tree.md) and does not assume balance.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
