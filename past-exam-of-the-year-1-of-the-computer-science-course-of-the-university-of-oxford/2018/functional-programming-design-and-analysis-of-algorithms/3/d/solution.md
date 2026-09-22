<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

One simple right-associated representation is

```
rep :: [a] -> CatList a
rep []     = Nil
rep (x:xs) = Cat (One x) (rep xs)
```

It constructs two [data constructors](../../../../../data-constructor.md) per input element and one final `Nil`, so full construction takes **$\Theta(n+1)$ time** and produces $2n+1$ constructors. [Structural induction](../../../../../structural-induction.md) shows that its denotation is the original [list](../../../../../list-abstract-data-type.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
