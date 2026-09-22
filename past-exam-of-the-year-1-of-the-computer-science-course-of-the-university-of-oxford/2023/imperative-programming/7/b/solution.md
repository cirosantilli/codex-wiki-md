<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The design creates a separate concrete [class in object-oriented programming](../../../../../class-programming.md) for each selected platform combination. With $P$ independently selectable platforms, there are up to **$2^P$ combinations**. Adding a platform can therefore multiply the number of classes, even though each platform's send operation and per-message charge are simple independent behaviors.

Sending code and charges are duplicated across many classes; a changed charge must be updated consistently in every affected combination. A forgotten update can make billing and sending disagree. A customer's preferences are also tied to a concrete class, making recombination cumbersome. The repeated implementation has low modularity: it encodes a whole subset where a composition of independent capabilities would suffice. The [Decorator pattern](../../../../../decorator-pattern.md) addresses exactly that structure.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
