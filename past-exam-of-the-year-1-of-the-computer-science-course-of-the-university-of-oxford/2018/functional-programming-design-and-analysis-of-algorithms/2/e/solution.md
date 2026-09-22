<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Addition and subtraction of [formal power series](../../../../../formal-power-series.md) are coefficientwise:

```
plus, minus :: Num a => [a] -> [a] -> [a]
plus  = zipWith (+)
minus = zipWith (-)
```

Here every valid input is an infinite coefficient [list](../../../../../list-abstract-data-type.md). If finite polynomial coefficient [lists](../../../../../list-abstract-data-type.md) were admitted, they would need zero-padding before these definitions: ordinary [list zip](../../../../../list-zip.md) otherwise truncates to the shorter length.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
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
