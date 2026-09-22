<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [Observer pattern](../../../../../observer-pattern.md), a subject maintains subscriptions through a common observation interface. Interested observers register and unregister; when a relevant state change occurs, the subject sends a notification, and each observer runs its own reaction. Notifications can carry the new information directly or prompt the observer to query the subject's coherent updated state.

This fits an [event-driven programming](../../../../../event-driven-programming.md) interface in which one model can have several independently changing views: a displayed conversion, a chart or a status indicator can react to the same model change. It avoids hard-coding calls to every concrete view inside the subject, which would couple domain logic to presentation details and require editing the subject whenever another view is added. **The subject depends on the observer interface rather than every concrete observer class.**

The design still needs subscription cleanup and an update policy. Mutual notifications can create a feedback loop or a [reentrant event handler](../../../../../reentrant-event-handler.md), while an observer that reacts halfway through a state change can see inconsistent data. Publishing only coherent changes and controlling derived display updates address those problems; the pattern alone does not automatically solve them.

## ↑ Ancestors (12)

1. [B](../b.md)
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
