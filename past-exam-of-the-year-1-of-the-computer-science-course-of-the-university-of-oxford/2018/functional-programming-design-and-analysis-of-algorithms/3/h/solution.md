<h1 id="3/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Compose the three [functions](../../../../../function-split.md):

```
reverse :: [a] -> [a]
reverse = abs . rev . rep
```

The representation built by `rep` has $2n+1$ constructors. `rev` preserves that count, and `abs` traverses it once. Their three linear bounds add to **$\Theta(n+1)$ total time**, improving the direct quadratic reversal. The correctness equations for representation, reversal and abstraction compose to the required reversed [list](../../../../../list-abstract-data-type.md).

## ↑ Ancestors (12)

1. [H](../h.md)
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
