<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A widget or model implementing `Publisher` is the subject. It calls `publish(event)` when an observable change occurs. An interested `Reactor` subscribes with `listenTo(subject)`, and adds a [partial function](../../../../../partial-function.md) to `reactions` that handles the event types it understands. `deafTo(subject)` ends that subscription when it is no longer needed.

The connection is therefore made through publisher and reactor interfaces rather than through a hard-coded [list](../../../../../list-abstract-data-type.md) of particular application classes. A reactor may observe several publishers and inspect an event's source to distinguish them. The implementation's registration machinery delivers published events to interested reactions; registering a reaction alone is not a substitute for subscribing to the source.[Official library README, event-system description; Reactor API entries listenTo, deafTo and reactions](../../../../../scala-swing-event-system-documentation.md)

For the converter, the three text fields are publishers and the frame is a reactor. Register the three fields once, then handle their edit-completion events to update the stored numeric state and refresh the appropriate displayed values.

## ↑ Ancestors (12)

1. [C](../c.md)
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
