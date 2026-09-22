<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [function](../../../../../function-split.md) returning an [optional value](../../../../../optional-value.md) supplies the representation:
```
newtype List a = List (Int -> Maybe a)
```
For a finite represented [list](../../../../../list-abstract-data-type.md), require a length $m\geq0$ such that every index $0\leq i<m$ returns `Just` its element and every other index returns `Nothing`. Thus there are no holes: absence at a nonnegative index implies absence at every later index. The type alone does not enforce this [invariant](../../../../../invariant-mathematics.md), or [algorithm termination](../../../../../algorithm-termination.md) of a query. An infinite represented [sequence](../../../../../sequence.md) may instead have a present value at every nonnegative index; operations requiring its length will not terminate.

The implementations below return `Nothing` at negative indices. Finite lengths, requested counts and intermediate indices are assumed to fit `Int`; explicit guards on index shifts also prevent arithmetic wraparound from exposing an invalid element.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
