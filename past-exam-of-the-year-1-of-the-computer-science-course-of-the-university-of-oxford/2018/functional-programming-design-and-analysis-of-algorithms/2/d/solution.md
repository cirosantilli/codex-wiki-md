<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use infinite coefficient [lazy lists](../../../../../lazy-list.md):

```
zero, one :: Num a => [a]
zero = 0 : zero
one  = 1 : zero
```

For ordinary numeric coefficients such as `Rational`, **`zero == zero` does not terminate**, while **`zero == one` is `False`**. The former comparison never finds a differing coefficient or reaches two empty [lists](../../../../../list-abstract-data-type.md); the latter rejects the unequal first coefficients immediately. Equality of denoted [formal power series](../../../../../formal-power-series.md) is mathematical equality of all coefficients, whereas this executable [list](../../../../../list-abstract-data-type.md) comparison is a potentially nonterminating procedure.

## ↑ Ancestors (12)

1. [D](../d.md)
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
