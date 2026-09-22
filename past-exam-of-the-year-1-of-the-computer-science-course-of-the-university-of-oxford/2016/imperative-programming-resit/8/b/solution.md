<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**This is the [Observer pattern](../../../../../observer-pattern.md), a [behavioral pattern](../../../../../behavioral-pattern.md).** `Service` stores subscribers through the `Company` [object interface](../../../../../object-interface.md). `SomeService.updateValue` first changes the underlying value and then sends a notification to every registered company; each company's `meth()` queries the new value and computes its own response. This is a pull-style notification: the message announces the change, while the observer reads the data from its retained subject reference.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
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
