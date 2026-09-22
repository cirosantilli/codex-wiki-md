<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Observer pattern](../../../../../observer-pattern.md) lets interested observers subscribe through a common interface to a subject's events or state changes. The subject notifies registered observers, which perform their own reactions; subscriptions can later be removed. A document model can thereby update multiple editor views without containing explicit knowledge of each view class.

**It avoids tightly coupling the subject to every concrete consumer.** Adding another view does not require adding a new view-specific call inside core model logic. Notifications should expose a coherent updated state, and unused observers should unsubscribe. The pattern does not itself prevent feedback cycles: observers that update each other's sources can still cause repeated or reentrant notifications. The supplied buttons and containing frame use this subscription-and-reaction design through [Scala Swing](../../../../../scala-swing.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
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
