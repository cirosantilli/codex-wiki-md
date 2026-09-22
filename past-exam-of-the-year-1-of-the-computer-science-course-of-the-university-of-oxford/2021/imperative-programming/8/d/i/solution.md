<h1 id="8/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**[Garbage collection](../../../../../../garbage-collection.md) automatically reclaims allocated memory that is no longer reachable by the running program.** [Garbage collection roots](../../../../../../garbage-collection-root.md) such as active references and static storage lead through object-reference fields to reachable [software objects](../../../../../../software-object.md) in [heap memory](../../../../../../heap-memory.md). A [tracing garbage collection](../../../../../../tracing-garbage-collection.md) implementation preserves reachable [software objects](../../../../../../software-object.md) and can reclaim unreachable ones, including unreachable cycles.

An [software object](../../../../../../software-object.md) becoming unreachable is different from its state being old or its last [object method](../../../../../../object-method.md) call having finished. A retained reference can keep it live indefinitely. Collection timing is an implementation matter; automatic reclamation does not promise that an [software object](../../../../../../software-object.md) is reclaimed immediately when the final useful reference disappears.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [8](../../../8.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
