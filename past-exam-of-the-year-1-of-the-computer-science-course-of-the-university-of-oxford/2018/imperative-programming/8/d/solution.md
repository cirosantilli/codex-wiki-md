<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Model-view-controller](../../../../../model-view-controller.md) divides an interactive application into a model containing application state and domain rules, a view rendering that state, and a controller interpreting user actions and requesting model operations. In the converter, the numeric amounts and exchange relation belong to the model, the text fields and labels form the view, and the edit handler parses input and chooses which quantity to preserve. A playlist model similarly owns song order independently of the controls used to change it.

A user acts through the view, the controller interprets that input, the model validates and commits a change, and the view then renders the resulting state. The exact packaging varies: a widget can combine view and controller responsibilities while still separating domain logic. Keeping the model independent of particular controls supports [separation of concerns](../../../../../separation-of-concerns.md), [encapsulation](../../../../../encapsulation-computer-programming.md), reuse of the same model in several views, and [unit testing](../../../../../unit-testing.md) of domain behavior without a graphical interface.

The [Observer pattern](../../../../../observer-pattern.md) often supplies the model-to-view notification path: views subscribe to model changes, so the model need not directly know every concrete view. It can also carry view input events to a controller, as in [Scala Swing](../../../../../scala-swing.md). **[Model-view-controller](../../../../../model-view-controller.md) is an architectural separation of responsibilities; the [Observer pattern](../../../../../observer-pattern.md) is one mechanism for their communication.** They are related without being identical, and small applications can implement the separation with direct calls where event subscriptions add no benefit.

## ↑ Ancestors (12)

1. [D](../d.md)
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
