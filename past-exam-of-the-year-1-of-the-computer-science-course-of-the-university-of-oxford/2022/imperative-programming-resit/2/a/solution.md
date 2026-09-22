<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an optional pair of [array indices](../../../../../array-index.md), so failure is distinct from every valid position:

```
def search(f: Array[Array[Int]], x: Int): Option[(Int, Int)]
```

**`Some((i,j))` denotes a match; `None` denotes absence.** The extra [array](../../../../../array-data-structure.md) argument makes the dependence on the searched data explicit; if `f` is already enclosed in the surrounding scope, it can instead be omitted. For all implementations below, assume `f` is non-null, its rows are non-null and rectangular, and it remains unchanged during the search. Empty dimensions are permitted.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
