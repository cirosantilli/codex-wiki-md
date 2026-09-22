<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [observer pattern](../../../../../observer-pattern.md) has four main roles. The subject maintains subscriptions and offers attach, detach and notification operations. The observer interface specifies an update callback. A concrete subject owns the relevant state and triggers notification when that state changes. A concrete observer implements the callback and updates its dependent state.

In a pull-style arrangement, a concrete observer retains a reference to the concrete subject and reads its state when notified; in a push-style arrangement, notification carries the changed information. Either way, the subject's notification loop calls observers through their interface. The roles should specify how subscription changes during notification are handled, for example by iterating a snapshot of the current observer list.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
