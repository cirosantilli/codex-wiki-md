<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The three outcomes, in printed order, are **`ZagType 'A'`**, **`ZigType undefined`**, and **a static type error**.

In the first expression, [pattern matching](../../../../../pattern-matching.md) discovers that the first tail is nonempty, so the ignored first label, the [bottom value](../../../../../bottom-value.md) $\bot$, is never demanded. The singleton `Cans 'A' Nil` returns `ZagType 'A'`.

In the second expression the tail is `Nal`, so the result is `ZigType` applied to the [bottom value](../../../../../bottom-value.md). Under [lazy evaluation](../../../../../lazy-evaluation.md) this has a defined outer constructor and an undefined field: `case lastZig (Cins undefined Nal) of ZigType _ -> True` yields `True`, whereas extracting or fully printing the payload fails. Thus the result is $\operatorname{ZigType}(\bot)$, not a wholly undefined outer value.

The original PDF really prints `Nil` in the third expression. `Cins` requires a tail of type `Zag b a`, whereas `Nil` has type `Zig c d`. These distinct [type constructors](../../../../../type-constructor.md) cannot be unified. **There is no well-typed expression to evaluate**, regardless of the undefined first label; replacing `Nil` by `Nal` would change the question.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
