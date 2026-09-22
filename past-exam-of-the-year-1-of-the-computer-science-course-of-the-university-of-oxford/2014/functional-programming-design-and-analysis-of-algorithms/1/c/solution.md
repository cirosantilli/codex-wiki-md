<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The base value can have any type `a`. The recursive result has that same type, so the step must accept and return `a`. Thus the most general [polymorphic](../../../../../programming-language-polymorphism.md) [type signature](../../../../../type-signature.md) of the [natural-number fold](../../../../../natural-number-fold.md) is

```
foldNat :: (a -> a) -> a -> Natural -> a
```

In mathematical type notation, $\boxed{(\alpha\to\alpha)\to\alpha\to\mathrm{Natural}\to\alpha}$. No equality, ordering or numeric constraint is needed: the [natural-number fold](../../../../../natural-number-fold.md) manipulates constructors, rather than performing arithmetic on the result.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
