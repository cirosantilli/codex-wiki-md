<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Map over the optional payload, preserving failure:
```
mapMaybe :: (a -> b) -> Maybe a -> Maybe b
mapMaybe _ Nothing = Nothing
mapMaybe f (Just x) = Just (f x)
```
This is the optional-value mapping operation, equivalent to `fmap` for `Maybe`. The question's local name is distinct from the library function `Data.Maybe.mapMaybe`, which filters and maps an entire [list](../../../../../list-abstract-data-type.md). The [algebraic data type](../../../../../algebraic-data-type.md) keeps absence separate from every ordinary payload value.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
