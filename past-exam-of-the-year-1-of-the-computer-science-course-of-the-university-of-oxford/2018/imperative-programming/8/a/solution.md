<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the [Observer pattern](../../../../../observer-pattern.md), an observable subject maintains subscriptions and sends notifications through a common observer interface when a relevant change occurs. Observers can then react to the event or query the subject's coherent new state. Registration and removal allow multiple dependants to change independently of the subject's application logic.

It is useful when one [software object](../../../../../software-object.md) has several changing dependants, for example a document model with several views or a text field with an event handler. **It avoids hard-coding every concrete dependant into the subject**, reducing direct coupling and duplicated synchronization logic. Clients need not poll repeatedly to detect a change. This separation does not automatically prevent notification cycles, stale subscriptions, or inconsistent intermediate states: notification should occur after a coherent update, and observers should unregister when no longer needed. A [reentrant event handler](../../../../../reentrant-event-handler.md) can otherwise commit recursively while refreshing a display.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
