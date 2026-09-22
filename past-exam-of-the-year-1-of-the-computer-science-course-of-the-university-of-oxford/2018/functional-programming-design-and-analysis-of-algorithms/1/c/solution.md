<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The natural [tree fold](../../../../../tree-fold.md) replaces each [data constructor](../../../../../data-constructor.md) by the supplied operation:

```
fold :: (a -> b) -> (b -> b -> b) -> Tree a -> b
fold one two (One x)   = one x
fold one two (Two l r) = two (fold one two l) (fold one two r)
```

Its reconstruction identity is **`fold One Two = id`**. More generally a [function](../../../../../function-split.md) `h` equals `fold one two` on finite [trees](../../../../../tree-graph-theory-split.md) exactly when `h (One x) = one x` and `h (Two l r) = two (h l) (h r)`. These equations determine the result by [structural induction](../../../../../structural-induction.md), expressing why this is the natural [structural recursion](../../../../../structural-recursion.md) for this datatype.

## ↑ Ancestors (12)

1. [C](../c.md)
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
