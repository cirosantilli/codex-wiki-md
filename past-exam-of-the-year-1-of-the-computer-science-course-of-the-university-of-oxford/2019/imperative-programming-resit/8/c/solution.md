<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In [Scala Swing](../../../../../scala-swing.md), a `Publisher` is the observable subject and a `Reactor` supplies an observer's reactions. A reactor calls `listenTo(pounds, euros, rate)` to subscribe to the relevant publishing components. It adds a [partial function](../../../../../partial-function.md) from events to actions with `reactions += { case ... => ... }`; unmatched event types need no action. When a publisher calls `publish(e)`, subscribed reactions that handle that event are notified. Calling `deafTo` removes subscriptions that are no longer wanted.[README, About scala-swing: Publisher/Reactor, listenTo and reactions; archived Reactor API: deafTo](../../../../../scala-swing-event-system-documentation.md)

The publisher does not need to know the concrete frame or its currency-conversion code. A `TextField` supplies the relevant editing events, and the frame's reaction distinguishes the source field using `EditDone(source)`. **Both registration and a matching reaction are needed**: installing a case handler without subscribing does not establish the notification path. The observer logic should update the conversion model once and then refresh the other fields from that coherent state.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
