<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A base-class change can preserve its own set abstraction while breaking a subclass that intercepts internal calls. For example, suppose `IntegerSet.delete(x)` is reimplemented by collecting the elements to retain, calling `clear`, then calling `insert` for each retained element. Conceptually its body is

```
val retained = snapshotOfElements.filter(_ != x)
clear
retained.foreach(insert)
```

Here `snapshotOfElements` denotes the base implementer's own internal snapshot operation in this hypothetical revision, not an API supplied by the examination. The algorithm still removes exactly the requested value and preserves all other set members.

On an `IntegerSetWithCount`, however, these unqualified calls use [dynamic dispatch](../../../../../dynamic-dispatch.md). The internal `clear` resets the subclass counter and the internal insertions increase it. After client calls `insert(10)`, `insert(20)`, `insert(10)`, the correct count is three. Calling `delete(10)` with this revised base implementation leaves the right set, containing only the other value, but resets the counter and reinserts that value, leaving **count one instead of three**. The client made no further insertion attempt and requested no clear.

This is the [fragile base class problem](../../../../../fragile-base-class-problem.md): subclass correctness depends on the base implementation's internal call structure, beyond its public set [postconditions](../../../../../postcondition.md). A change need not alter the base API to expose that dependence.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
