<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Throw an informative exception**, such as `NoSuchElementException`, and leave the set unchanged. This makes a violated nonempty [precondition](../../../../../precondition.md) visible at the point of misuse. Returning a distinguished [integer](../../../../../integer-split.md) would be ambiguous because every [integer](../../../../../integer-split.md) is a legitimate set member.

A different [object interface](../../../../../object-interface.md) could return an optional [integer](../../../../../integer-split.md), representing failure explicitly, but that changes the declared return type. For the supplied integer-returning operation, a checked failure is useful and consistent with the stated [precondition](../../../../../precondition.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
