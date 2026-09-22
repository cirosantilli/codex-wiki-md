<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The ordinary [list comprehension](../../../../../list-comprehension.md) exhausts the inner [list](../../../../../list-abstract-data-type.md) before advancing the outer one. Therefore it enumerates every argument pair when **`ys` is finite**, or when **`xs` has at most one element**. If `ys` is infinite and `xs` has two or more elements, it stays with the first outer element forever and misses every pair with a later outer occurrence. Applying a constant `f` might hide missing pairs as duplicate values; it does not make the enumeration fair.

An empty-result caveat remains when `ys = []` and `xs` is infinite: the literal comprehension traverses infinitely many empty rows and does not return a terminating empty [list](../../../../../list-abstract-data-type.md). Its occurrence requirement is vacuous, but its [productivity](../../../../../stream-productivity.md) as an empty-result computation fails. An explicit empty-input test avoids that particular failure.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
