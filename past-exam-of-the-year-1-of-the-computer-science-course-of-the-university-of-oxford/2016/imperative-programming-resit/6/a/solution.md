<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The output is **`ABC`**, without a newline. The relevant [Scala trait linearization](../../../../../scala-trait-linearization.md) is `D,C,B,A`. Calling `d.m` starts with `C.m`, whose `super.m` continues to `B.m`, then to `A.m`. The latter prints `A`; returning through the two method bodies then prints `B` followed by `C`. The braces keep each final `print` inside that [object method](../../../../../object-method.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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
