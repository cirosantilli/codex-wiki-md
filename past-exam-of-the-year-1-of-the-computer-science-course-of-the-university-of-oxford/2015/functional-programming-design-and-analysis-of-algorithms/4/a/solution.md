<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Lazy evaluation](../../../../../lazy-evaluation.md) is evaluation by need: an expression is deferred until its value is demanded, and its computed value is shared for subsequent demands of the same suspended computation.

Its two key properties here are **avoiding evaluation of unused expressions** and **sharing demanded computations**. For example, the first component of `(3, undefined)` can be obtained without evaluating the second. A suspended expression is represented by a [thunk](../../../../../thunk.md); after evaluation its result can be reused. This supports productive infinite [lists](../../../../../list-abstract-data-type.md): `take 5 [0..]` demands only a finite prefix. It does not guarantee that a demanded computation terminates.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
