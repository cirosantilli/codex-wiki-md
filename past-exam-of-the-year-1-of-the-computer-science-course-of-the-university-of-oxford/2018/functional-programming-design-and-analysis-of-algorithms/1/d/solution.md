<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Replace the leaf [data constructor](../../../../../data-constructor.md) by the constant one and the internal [data constructor](../../../../../data-constructor.md) by addition with one extra node:

```
size :: Tree a -> Int
size = fold (const 1) (\m n -> 1 + m + n)
```

The two defining equations of the [tree fold](../../../../../tree-fold.md) become exactly the two equations for the recursive node count.

## ↑ Ancestors (12)

1. [D](../d.md)
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
