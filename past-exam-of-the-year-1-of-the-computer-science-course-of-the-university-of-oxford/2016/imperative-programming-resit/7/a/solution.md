<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The **[Prototype pattern](../../../../../prototype-pattern.md) is a [creational pattern](../../../../../creational-pattern.md) that creates new [software objects](../../../../../software-object.md) by copying an existing configured object through a common cloning [object interface](../../../../../object-interface.md)**. A client keeps or selects a prototype and requests a copy, without naming the concrete [software class](../../../../../class-programming.md) or repeating its construction recipe.

It is useful when the concrete type is selected at runtime, when many objects share a configuration, or when reconstructing an initialized object is expensive. For example, a drawing application can duplicate a configured graphical object through the same interface for many shape classes. The contract must specify what is copied: nested mutable state may require a [deep copy](../../../../../deep-copy.md), whereas a shallow copy would retain [reference aliasing](../../../../../reference-aliasing.md). A copy should preserve the intended configuration while allowing independent changes where promised.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
