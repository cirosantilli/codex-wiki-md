<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The system uses the [observer pattern](../../../../../observer-pattern.md) with a pull-style update.** `Equipment` provides the subject interface and stores registered observers; `GymEquipment` is the concrete subject. `Functionality` is the observer interface, with `Performance` and `Prediction` as concrete observers. Their constructors subscribe them with `addFunctionality(this)`.

When `GymEquipment.updateUserMeasures` is called, it first updates both measurements through `super`, then calls `notifyFunctionalities`. Every subscribed observer receives `update()` and reads the new measurements from its stored equipment reference. `Performance` calculates the current score; `Prediction` calculates the score at time `time+5`, keeping the other quantities fixed. Since observers are prepended to a [list](../../../../../list-abstract-data-type.md), notification follows reverse registration order.

The source has two independent implementation defects. `deleteFunctionality(f)` computes `_functionalities diff List(f)` but does not assign it back, so it does not actually unsubscribe anything. The prediction message also contains a physical newline inside an ordinary quoted [Scala](../../../../../scala.md) string in the PDF; executable code must join that string, concatenate pieces, or use a multiline string. Neither issue changes the intended [observer pattern](../../../../../observer-pattern.md). The source's score is treated as the specified arithmetic expression, not as an independently validated physiological model.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
