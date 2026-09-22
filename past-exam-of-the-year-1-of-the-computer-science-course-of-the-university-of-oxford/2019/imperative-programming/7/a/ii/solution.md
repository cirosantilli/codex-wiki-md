<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Class inheritance](../../../../../../class-inheritance.md) defines a subclass by extending another class's behavior, often with [method overriding](../../../../../../method-overriding.md) and [subtyping](../../../../../../subtyping.md). An editor might have an abstract `Command` type with `execute`, and subclasses for insertion and deletion. The controller keeps commands through the common type and [dynamic dispatch](../../../../../../dynamic-dispatch.md) chooses each command's actual operation. Alternatively, a specialized document can extend a base document's documented behavior. **An inheritance relationship used for substitution must preserve the superclass contract**; borrowing its code alone does not justify exposing incompatible behavior. Commands exemplify the [Command pattern](../../../../../../command-pattern.md) without exposing document storage to the controller.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
