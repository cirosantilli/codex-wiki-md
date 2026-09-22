<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[List concatenation](../../../../../list-concatenation.md) copies the spine of its first operand and shares the second:

```
(++) :: [a] -> [a] -> [a]
[]     ++ ys = ys
(x:xs) ++ ys = x : (xs ++ ys)
```

For finite first-operand length $m$, fully producing the copied spine costs **$\Theta(m+1)$**, independently of the second-operand length. With [lazy evaluation](../../../../../lazy-evaluation.md), requesting only the first few result constructors can cost less; the bound concerns the complete concatenation spine, without forcing its element values or traversing the already existing second operand.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
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
