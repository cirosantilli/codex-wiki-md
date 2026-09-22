<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [type synonym](../../../../../type-synonym.md) for names and an [algebraic data type](../../../../../algebraic-data-type.md) with the two teams and their goals in the given positional order:

```
type Team = String
data Match = Match Team Int Team Int
```

`Team` is a synonym, not a new runtime wrapper. `Match` on the left is the [type constructor](../../../../../type-constructor.md), while the same spelling on the right is a [data constructor](../../../../../data-constructor.md) in a different namespace. Its value-level [type signature](../../../../../type-signature.md) is `Match :: Team -> Int -> Team -> Int -> Match`.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
