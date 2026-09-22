<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Decorator pattern](../../../../../decorator-pattern.md) participants are:

- `CableTV`: the component [object interface](../../../../../object-interface.md), declaring the price and package description visible to clients.
- `BasicPlan`: the concrete component, supplying the initial £30 account and its description.
- `Packages`: the abstract [decorator object](../../../../../decorator-object.md), storing one component and forwarding its queries.
- `Movies` and `HDChannels`, and the extension `Sports`: concrete [decorator objects](../../../../../decorator-object.md), adding respectively £10, £7, and £5 and appending their labels.

The checking application is the client that chooses and nests these participants. **The common `CableTV` interface makes a decorated account usable wherever a basic account is usable**, while the nested [object composition](../../../../../object-composition.md) determines its accumulated behavior.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
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
