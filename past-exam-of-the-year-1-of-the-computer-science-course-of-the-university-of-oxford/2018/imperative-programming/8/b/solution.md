<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [Scala Swing](../../../../../scala-swing.md) `Publisher` is the subject-side event source. Calling `publish(e)` notifies its subscribed reactors. A `Reactor` is the observer-side participant: `listenTo(p1,p2)` registers it with the specified sources, `deafTo` ends those subscriptions, and `reactions` contains the event-handling cases.
```
listenTo(pounds, euros, rate)
reactions += {
  case EditDone(source) => handleCommittedEdit(source)
}
```
Here the containing frame supplies the reactor behavior, and each text field supplies publication. Defining `reactions` without `listenTo` is insufficient to establish the subscription. The pattern-matching cases can handle only events of interest while other events are ignored. This is the [Observer pattern](../../../../../observer-pattern.md) expressed through event publication rather than a separate hand-written `update` method for every subject.[Archived Reactor API: listenTo, deafTo and reactions; official library README: Publisher/Reactor event-system overview](../../../../../scala-swing-event-system-documentation.md)

## ↑ Ancestors (12)

1. [B](../b.md)
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
