<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Both versions preserve left-to-right leaf order:

```
flatten :: Tree a -> [a]
flatten (One x)   = [x]
flatten (Two l r) = flatten l ++ flatten r

flattenFold :: Tree a -> [a]
flattenFold = foldTree (\x -> [x]) (++)
```

The [tree fold](../../../../../tree-fold.md) replaces each leaf by a singleton [list](../../../../../list-abstract-data-type.md) and each internal node by [list concatenation](../../../../../list-concatenation.md). The defining equations of `flattenFold` are consequently those of `flatten`, proving their equality by [structural induction](../../../../../structural-induction.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
