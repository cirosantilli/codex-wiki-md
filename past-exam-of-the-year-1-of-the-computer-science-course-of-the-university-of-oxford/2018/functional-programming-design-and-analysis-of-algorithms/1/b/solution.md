<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Count each [data constructor](../../../../../data-constructor.md) once, including each `Two`:

```
size :: Tree a -> Int
size (One _)   = 1
size (Two l r) = 1 + size l + size r
```

[Structural induction](../../../../../structural-induction.md) verifies the count: a leaf contributes one; an internal node contributes itself and the disjoint occurrences in its two [subtrees](../../../../../subtree.md). Fully evaluating the result takes [linear time](../../../../../linear-time.md) in the number of nodes. This [type signature](../../../../../type-signature.md) uses machine `Int` as usual in the examination; `Integer` avoids overflow for arbitrarily large inputs.

## ↑ Ancestors (12)

1. [B](../b.md)
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
