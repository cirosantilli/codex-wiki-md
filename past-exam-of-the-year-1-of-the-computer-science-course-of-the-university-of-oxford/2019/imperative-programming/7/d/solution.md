<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [object composition](../../../../../object-composition.md): a logging wrapper owns a private `ResizableFrame` and delegates dimension operations to it, rather than being its subclass. The wrapper takes the before/after area around each public operation. Its own `flip` calls the component's whole `flip` once, compares only the completed states, and therefore records no increase. The component must be exclusively owned or defensively copied, so clients cannot bypass the wrapper's accounting.

**The component's internal calls cannot dynamically dispatch into the separate wrapper.** This prevents the setter-based `flip` implementation change from creating false log entries and reduces dependence on undocumented superclass internals. The wrapper can also choose a smaller interface. Costs include forwarding code and the loss of automatic `ResizableFrame` subtyping: code requiring that concrete superclass cannot necessarily accept the wrapper. A shared abstract frame interface can recover substitutability while keeping implementation reuse based on composition. Composition improves this dependency boundary; it does not remove the need for a clear mutation and ownership contract.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
