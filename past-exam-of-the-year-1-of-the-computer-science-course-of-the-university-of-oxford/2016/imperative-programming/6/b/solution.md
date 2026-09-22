<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Programming language polymorphism](../../../../../programming-language-polymorphism.md) permits **one interface or piece of code to work with values of several types**, while providing the behavior appropriate to those values. For example a routine that calls `play` through a `Player` reference can use a `Regular`, `Optimistic`, or `House` object without knowing its concrete [software class](../../../../../class-programming.md).

Use [programming language polymorphism](../../../../../programming-language-polymorphism.md) when clients should depend on a common contract while concrete behavior varies, or when an [algorithm](../../../../../algorithm-split.md) is independent of the element type. It avoids duplicating client logic or repeatedly inspecting concrete [runtime types](../../../../../runtime-type.md), and supports extensions behind the same interface. A shared interface must still have meaningful behavioral guarantees: merely giving unrelated operations the same name does not establish that implementations can safely replace one another.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
