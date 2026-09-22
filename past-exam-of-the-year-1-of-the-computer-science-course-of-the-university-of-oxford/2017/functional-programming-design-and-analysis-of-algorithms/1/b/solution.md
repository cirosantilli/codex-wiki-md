<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The completed identities are:

```
filter p . map f = map f . filter (p . f)

filter p . concat = concat . map (filter p)

zipWith f = (map (uncurry f) .) . zip
```

The first tests the [predicate](../../../../../predicate.md) after the mapped function; the second filters each inner [list](../../../../../list-abstract-data-type.md). In the third, `zip` is curried: after one argument it still returns a function of a second list. The [operator section](../../../../../operator-section.md) `(map (uncurry f) .)` composes with that returned function. Applying both sides to `xs` and `ys` gives `map (uncurry f) (zip xs ys)`. Omitting the section's extra composition level would not type-check.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
