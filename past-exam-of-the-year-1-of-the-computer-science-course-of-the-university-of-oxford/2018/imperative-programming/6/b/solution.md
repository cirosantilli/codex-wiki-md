<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Command pattern](../../../../../command-pattern.md) separates a request into a common command interface, concrete commands carrying arguments and execution behavior, a receiver doing the application work, an invoker requesting execution or retaining history, and a client assembling these [software objects](../../../../../software-object.md). A menu item, toolbar button or keyboard shortcut can invoke the same command without duplicating the playlist manipulation.

**`SongSuite` is the receiver.** The application/controller invokes its operations, and the returned `Change` [software objects](../../../../../software-object.md) hold the concrete inverse/forward behavior. A command wrapper can expose an initial `execute` that calls the appropriate `SongSuite` operation and then delegates later undo/redo to its returned record. `History` is the history-managing part of the invoker. Separating these roles avoids making a graphical control know how the playlist representation is edited; requests can be retained and reversed through a common [object interface](../../../../../object-interface.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
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
