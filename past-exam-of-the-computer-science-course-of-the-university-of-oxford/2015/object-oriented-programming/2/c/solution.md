<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In [model-view-controller](../../../../../model-view-controller.md), the model owns application data and its rules: here it is the ordered `DataList` with its uniqueness condition on horizontal coordinates. A view renders those data, for example as a line plot or a bar plot. View-specific decisions such as whether to show axes need not change the model. A controller interprets actions such as entering a new sample or selecting a plot style, and requests the appropriate model or view operation.

This [separation of concerns](../../../../../separation-of-concerns.md) permits several views of the same data and allows model operations to be tested without drawing a window. When the model changes, affected views need a notification or another refresh mechanism. The [Observer pattern](../../../../../observer-pattern.md) in part (d) supplies one such mechanism, without making the model depend on every concrete view [software class](../../../../../class-programming.md). The division is

$$
\boxed{\text{model: state and rules; view: presentation; controller: input interpretation}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
