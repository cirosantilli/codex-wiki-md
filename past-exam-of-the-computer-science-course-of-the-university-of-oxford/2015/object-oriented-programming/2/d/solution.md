<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the [Observer pattern](../../../../../observer-pattern.md), an observable subject keeps registered observers behind a shared [object interface](../../../../../object-interface.md). After a relevant update, the subject calls that [object interface](../../../../../object-interface.md) on each observer. Observers can register and unregister independently, and the subject needs no knowledge of their concrete [software classes](../../../../../class-programming.md).

For this [model-view-controller](../../../../../model-view-controller.md) application, `DataList` is the subject, while graph views are observers. After a successful insertion, a notification tells each registered view to redraw from the updated model. An invalid insertion leaves the model unchanged and needs no change notification. Calling observers only after restoring the [representation invariant](../../../../../representation-invariant.md) prevents views from seeing a half-completed insertion. Hence

$$
\boxed{\text{one coherent model change can refresh several independently registered views}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Object oriented programming](../../../object-oriented-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
