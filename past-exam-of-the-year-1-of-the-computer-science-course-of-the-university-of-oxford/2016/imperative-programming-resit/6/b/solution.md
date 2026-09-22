<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The output becomes **`BCA`**, without a newline. Here each method body consists only of `super.m`; the semicolon ends that definition. The following `print("B")` or `print("C")` is a separate statement in the [trait](../../../../../trait.md) body, so it executes during construction.

Creating `new D` initializes the shared base and then the `B` and `C` [mixins](../../../../../mixin.md), printing `BC`. The subsequent `d.m` still forwards along `C,B,A`, but only `A.m` now prints anything, appending `A`. Thus it is the placement of the construction-time statements, not a changed [Scala trait linearization](../../../../../scala-trait-linearization.md), that changes the output. [Template Evaluation](../../../../../scala-2-11-classes-and-objects-specification.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
