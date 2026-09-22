<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The return types suggest an **immutable [sequence](../../../../../sequence.md) implementation**: insertion and deletion return a new `Sequence[A]`, while the receiver can remain unchanged. A mutable implementation would more naturally return `Unit` for in-place edits, though it could return itself. Thus the signatures are evidence of an intended [immutable object](../../../../../immutable-object.md) implementation, not a logical guarantee. For the snapshot solution below, require that returned and retained `Sequence` values really are immutable. The owning `SlideSuite` can still have a mutable variable referring to its current immutable [sequence](../../../../../sequence.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
