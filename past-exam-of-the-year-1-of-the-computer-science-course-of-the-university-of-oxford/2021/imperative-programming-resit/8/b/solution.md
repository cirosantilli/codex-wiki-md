<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [observer pattern](../../../../../observer-pattern.md) connects one event-producing subject to a changing [set](../../../../../set-split.md) of interested consumers. Consumers register through an observation interface; when a relevant change occurs, the producer notifies them through that interface rather than naming every concrete consumer. Consumers can be added or removed without rewriting the producer's core behaviour.

This is useful for keeping displays, controls or other derived views synchronized with changing state. **The design avoids tight coupling from the producer to all concrete dependants**, which otherwise makes every new consumer require changes to the producer. Publishing after the producer's [representation invariant](../../../../../representation-invariant.md) has been restored also lets callbacks observe a coherent state. The pattern does not by itself prevent notification cycles or obsolete subscriptions; update policy and unregistration still matter.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
