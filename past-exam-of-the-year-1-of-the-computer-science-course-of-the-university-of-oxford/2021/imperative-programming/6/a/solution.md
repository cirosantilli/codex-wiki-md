<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A suitable relationship is a circle implementing a read-only shape [object interface](../../../../../object-interface.md) whose operations include area. Every circle satisfies that [object interface](../../../../../object-interface.md)'s behavioral contract, so clients using a shape can use a circle through [subtype polymorphism](../../../../../subtype-polymorphism.md); [dynamic dispatch](../../../../../dynamic-dispatch.md) selects its area implementation.

A car is not appropriately modeled as a subclass of an engine merely because it needs engine behavior. **Use [object composition](../../../../../object-composition.md)**: the car contains an engine and delegates engine-related work to it. An engine is a component of a car, not a category containing cars. The design can replace the component independently without making all engine operations part of the car's public [object interface](../../../../../object-interface.md). [Class inheritance](../../../../../class-inheritance.md) should reflect substitutability, rather than serve solely as a convenient way to obtain another [software class](../../../../../class-programming.md)'s code.

## ↑ Ancestors (12)

1. [A](../a.md)
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
