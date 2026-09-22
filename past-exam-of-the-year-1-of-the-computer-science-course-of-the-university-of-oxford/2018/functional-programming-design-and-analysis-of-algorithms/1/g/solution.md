<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Include each child itself, followed by its proper [subtrees](../../../../../subtree.md), while excluding the current root:

```
proper :: Tree a -> [Tree a]
proper (One _)   = []
proper (Two l r) = (l : proper l) ++ (r : proper r)
```

Again, occurrences matter: a child with the same value as another child is not removed. The definition is a [structural recursion](../../../../../structural-recursion.md), but its right-hand side uses the original children as well as their recursively computed results.

## ↑ Ancestors (12)

1. [G](../g.md)
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
