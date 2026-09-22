<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [decorator pattern](../../../../../decorator-pattern.md) participants are:

- **Component:** `CableTV` declares the common `cost` and `packages` queries, so clients can use both basic and decorated accounts through one [object interface](../../../../../object-interface.md).
- **Concrete component:** `BasicPlan` supplies the initial price and package description.
- **Decorator:** the abstract `Packages` class stores a component reference and forwards its operations, enabling recursive [object composition](../../../../../object-composition.md).
- **Concrete decorators:** `Movies` and `HDChannels` override the queries to add one responsibility while preserving the wrapped component's behavior.
- **Client:** an application chooses the nesting of components and observes the resulting account through `CableTV`.

Each wrapper contributes its price exactly once along the chain. The same structural arrangement handles a new optional package without changing the existing component interface.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
