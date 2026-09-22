<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [code smell](../../../../../code-smell.md) is an easily noticed feature that suggests a deeper design problem worth investigating. It is neither a proven bug nor an automatic instruction to rewrite the code. Context determines whether the symptom is troublesome.[9 February 2006: surface indication, investigation rather than automatic condemnation; long-method example](../../../../../code-smell-by-martin-fowler.md)

[Duplicate code](../../../../../duplicate-code.md) can indicate that the same knowledge has several maintenance sites: a correction made to one copy may be forgotten in the other. If the copies represent the same responsibility, extract that responsibility into one shared operation or component. Merely looking similar is insufficient; accidentally similar code with independent purposes should not necessarily be coupled.

[Feature envy](../../../../../feature-envy.md) occurs when an operation depends mainly on another object's data rather than the responsibilities of its own class. For example, an editor view might implement a text-policy decision by repeatedly inspecting document internals. Move that decision to the document, or extract and move the relevant part, so behavior sits with the data and responsibility it actually uses. **Duplication suggests consolidating repeated knowledge; feature envy suggests moving a responsibility between objects.** These are different design actions, and both can be [refactorings](../../../../../refactoring.md) that preserve observable behavior.[Move [Function](../../../../../function-split.md), called Move Method in the first edition: move behavior to a better-suited context](../../../../../move-function-in-the-refactoring-catalog.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
